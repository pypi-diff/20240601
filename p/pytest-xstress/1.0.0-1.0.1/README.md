# Comparing `tmp/pytest_xstress-1.0.0.tar.gz` & `tmp/pytest_xstress-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_xstress-1.0.0.tar", max compression
+gzip compressed data, was "pytest_xstress-1.0.1.tar", max compression
```

## Comparing `pytest_xstress-1.0.0.tar` & `pytest_xstress-1.0.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2096 2024-05-27 23:36:39.392754 pytest_xstress-1.0.0/README.md
--rw-r--r--   0        0        0      727 2024-05-27 23:36:39.394081 pytest_xstress-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     7390 2024-05-27 23:36:39.394367 pytest_xstress-1.0.0/pytest_xstress.py
--rw-r--r--   0        0        0     2669 1970-01-01 00:00:00.000000 pytest_xstress-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     2096 2024-06-01 10:26:41.983527 pytest_xstress-1.0.1/README.md
+-rw-r--r--   0        0        0      727 2024-06-01 13:41:29.281993 pytest_xstress-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     8297 2024-06-01 13:41:23.311990 pytest_xstress-1.0.1/pytest_xstress.py
+-rw-r--r--   0        0        0     2669 1970-01-01 00:00:00.000000 pytest_xstress-1.0.1/PKG-INFO
```

### Comparing `pytest_xstress-1.0.0/README.md` & `pytest_xstress-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_xstress-1.0.0/pyproject.toml` & `pytest_xstress-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-xstress"
-version = "1.0.0"
+version = "1.0.1"
 description = ""
 authors = ["Yuvalino <yuvalino@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pytest = "^8.0.0"
```

### Comparing `pytest_xstress-1.0.0/pytest_xstress.py` & `pytest_xstress-1.0.1/pytest_xstress.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import functools
 from itertools import chain
 
 import pytest
 from xdist.remote import Producer
 from xdist.scheduler.loadgroup import LoadGroupScheduling
 from xdist.workermanage import WorkerController
 
@@ -33,20 +34,15 @@
         """Return the number of pending tests in a workload."""
         pending = sum(sum(scope.values()) for scope in workload.values())
         return pending
 
     def mark_test_complete(
         self, node: WorkerController, item_index: int, duration: float = 0
     ) -> None:
-        """Mark test item as completed by node.
-
-        Called by the hook:
-
-        - ``DSession.worker_testreport``.
-        """
+        """Add more tests to node if `pending_tests_in_node<MIN_TESTS_PER_NODE`"""
         nodeid = self.registered_collections[node][item_index]
         scope = self._split_scope(nodeid)
 
         if self.assigned_work[node][scope][nodeid]:
             self.assigned_work[node][scope][nodeid] -= 1
 
         # If the current scope has been finished, return it to the workqueue to be re-run
@@ -62,15 +58,15 @@
             and self.workqueue
         ):
             self._assign_work_unit(node)
         while self._pending_of(self.assigned_work[node]) < MIN_TESTS_PER_NODE:
             self._reassign_work_units(node)
 
     def _assign_work_unit(self, node: WorkerController) -> None:
-        """Assign a work unit to a node."""
+        """Assign a work unit from `self.workqueue` to a node."""
         assert self.workqueue
 
         # Grab a unit of work
         scope, work_unit = self.workqueue.popitem(last=False)
         for nodeid in work_unit.keys():
             work_unit[nodeid] = int(
                 not work_unit[nodeid]
@@ -90,14 +86,15 @@
                 ]
             )
         )
 
         node.send_runtest_some(nodeids_indexes)
 
     def _reassign_work_units(self, node: WorkerController):
+        """Ensure `pending_tests_in_node>=MIN_TESTS_PER_NODE` by reassigning more scopes"""
         for curr_scope in self.assigned_work[node]:
             if self._pending_of(self.assigned_work[node]) >= MIN_TESTS_PER_NODE:
                 break
 
             for curr_nodeid in self.assigned_work[node][curr_scope]:
                 self.assigned_work[node][curr_scope][curr_nodeid] += 1
 
@@ -182,22 +179,43 @@
         for node in self.nodes:
             while self._pending_of(self.assigned_work[node]) < MIN_TESTS_PER_NODE:
                 self._reassign_work_units(node)
 
 
 @pytest.hookimpl()
 def pytest_xdist_make_scheduler(config: pytest.Config, log):
+    """Switch to our cool scheduler if --xstress"""
     if not config.getvalue("xstress"):
         return None
     dist = config.getvalue("dist")
     if dist == "loadgroup":
         return LoadGroupStressScheduler(config, log)
     raise ValueError(f'xstress does not support "{dist}" distmode')
 
 
+@pytest.hookimpl
+def pytest_plugin_registered(plugin, manager: pytest.PytestPluginManager):
+    """Workaround until PR#1091 in pytest-xdist is merged"""
+    if type(plugin).__name__ == "WorkerInteractor":
+        # NOTE: Haven't found a better way to get config at this time
+        if not plugin.config.getvalue("xstress"):
+            return
+
+        # Switch `nextitem=item` to `nextitem=None` when calling `pytest_runtest_protocol`
+        func = plugin.config.hook.pytest_runtest_protocol
+
+        @functools.wraps(func)
+        def wrapper(item, nextitem, *args, **kwargs):
+            if item == nextitem:
+                nextitem = None
+            func(item=item, nextitem=nextitem, *args, **kwargs)
+
+        plugin.config.hook.pytest_runtest_protocol = wrapper
+
+
 @pytest.hookimpl()
 def pytest_addoption(parser: pytest.Parser):
     parser.addoption(
         "--xstress",
         action="store_true",
         default=False,
         dest="xstress",
```

### Comparing `pytest_xstress-1.0.0/PKG-INFO` & `pytest_xstress-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-xstress
-Version: 1.0.0
+Version: 1.0.1
 Summary: 
 Author: Yuvalino
 Author-email: yuvalino@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

