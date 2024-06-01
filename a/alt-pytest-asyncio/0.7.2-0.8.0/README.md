# Comparing `tmp/alt_pytest_asyncio-0.7.2.tar.gz` & `tmp/alt_pytest_asyncio-0.8.0.tar.gz`

## Comparing `alt_pytest_asyncio-0.7.2.tar` & `alt_pytest_asyncio-0.8.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      994 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.2/alt_pytest_asyncio/__init__.py
--rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.2/alt_pytest_asyncio/async_converters.py
--rw-r--r--   0        0        0     8724 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.2/alt_pytest_asyncio/plugin.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.2/alt_pytest_asyncio/version.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.2/.gitignore
--rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.2/LICENSE
--rw-r--r--   0        0        0     6972 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.2/README.rst
--rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     7597 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/alt_pytest_asyncio/__init__.py
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/alt_pytest_asyncio/async_converters.py
+-rw-r--r--   0        0        0     9299 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/alt_pytest_asyncio/plugin.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/alt_pytest_asyncio/version.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/LICENSE
+-rw-r--r--   0        0        0     7154 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/README.rst
+-rw-r--r--   0        0        0     1150 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 alt_pytest_asyncio-0.8.0/PKG-INFO
```

### Comparing `alt_pytest_asyncio-0.7.2/alt_pytest_asyncio/__init__.py` & `alt_pytest_asyncio-0.8.0/alt_pytest_asyncio/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """pytest-cov: avoid already-imported warning: PYTEST_DONT_REWRITE."""
+
 import pytest
 
 from alt_pytest_asyncio.version import VERSION
 
 
 @pytest.hookimpl
 def pytest_addoption(parser):
```

### Comparing `alt_pytest_asyncio-0.7.2/alt_pytest_asyncio/async_converters.py` & `alt_pytest_asyncio-0.8.0/alt_pytest_asyncio/async_converters.py`

 * *Files 21% similar despite different names*

```diff
@@ -4,46 +4,106 @@
 convert_fixtures and converted_async_test are used by the Plugin
 to convert async fixtures and async tests.
 
 We try our best to make sure error reporting is short and useful by doing some
 hacks with capturing errors inside run_until_complete rather than outside so
 that you don't get asyncio internals in the errors.
 """
+
 import asyncio
 import inspect
 import sys
 from functools import wraps
 
 
-def convert_fixtures(fixturedef, request, node):
+def convert_fixtures(ctx, fixturedef, request, node):
     """Used to replace async fixtures"""
     if not hasattr(fixturedef, "func"):
         return
 
+    if hasattr(fixturedef.func, "__alt_asyncio_pytest_converted__"):
+        return
+
     if inspect.iscoroutinefunction(fixturedef.func):
-        convert_async_coroutine_fixture(fixturedef, request, node)
+        convert_async_coroutine_fixture(ctx, fixturedef, request, node)
+        fixturedef.func.__alt_asyncio_pytest_converted__ = True
 
     elif inspect.isasyncgenfunction(fixturedef.func):
-        convert_async_gen_fixture(fixturedef, request, node)
+        convert_async_gen_fixture(ctx, fixturedef, request, node)
+        fixturedef.func.__alt_asyncio_pytest_converted__ = True
+
+    elif inspect.isgeneratorfunction(fixturedef.func):
+        convert_sync_gen_fixture(ctx, fixturedef)
+        fixturedef.func.__alt_asyncio_pytest_converted__ = True
+
+    else:
+        convert_sync_fixture(ctx, fixturedef)
+        fixturedef.func.__alt_asyncio_pytest_converted__ = True
+
+
+def convert_sync_fixture(ctx, fixturedef):
+    """
+    Used to make sure a non-async fixture is run in our
+    asyncio contextvars
+    """
+    original = fixturedef.func
+
+    @wraps(original)
+    def run_fixture(*args, **kwargs):
+        try:
+            ctx.run(lambda: None)
+            run = lambda func, *a, **kw: ctx.run(func, *a, **kw)
+        except RuntimeError:
+            run = lambda func, *a, **kw: func(*a, **kw)
+
+        return run(original, *args, **kwargs)
 
+    fixturedef.func = run_fixture
 
-def converted_async_test(test_tasks, func, timeout, *args, **kwargs):
+
+def convert_sync_gen_fixture(ctx, fixturedef):
+    """
+    Used to make sure a non-async generator fixture is run in our
+    asyncio contextvars
+    """
+    original = fixturedef.func
+
+    @wraps(original)
+    def run_fixture(*args, **kwargs):
+        try:
+            ctx.run(lambda: None)
+            run = lambda func, *a, **kw: ctx.run(func, *a, **kw)
+        except RuntimeError:
+            run = lambda func, *a, **kw: func(*a, **kw)
+
+        cm = original(*args, **kwargs)
+        value = run(cm.__next__)
+        try:
+            yield value
+            run(cm.__next__)
+        except StopIteration:
+            pass
+
+    fixturedef.func = run_fixture
+
+
+def converted_async_test(ctx, test_tasks, func, timeout, *args, **kwargs):
     """Used to replace async tests"""
     __tracebackhide__ = True
 
     info = {}
     loop = asyncio.get_event_loop_policy().get_event_loop()
 
     def look_at_task(t):
         test_tasks[loop].append(t)
 
     info["func"] = func
 
     return _run_and_raise(
-        loop, info, func, async_runner(func, timeout, info, args, kwargs), look_at_task
+        ctx, loop, info, func, async_runner(func, timeout, info, args, kwargs), look_at_task
     )
 
 
 def _find_async_timeout(func, node):
     timeout = float(
         node.config.getoption("default_async_timeout", None)
         or node.config.getini("default_async_timeout")
@@ -79,23 +139,23 @@
 
     if info.get("e"):
         # Use a separate function so when --tb=short is not set we don't get
         # this entire function in the output
         raise_error()
 
 
-def _run_and_raise(loop, info, func, coro, look_at_task=None):
+def _run_and_raise(ctx, loop, info, func, coro, look_at_task=None):
     __tracebackhide__ = True
 
     def silent_done_task(res):
         if res.cancelled():
             pass
         res.exception()
 
-    task = loop.create_task(coro)
+    task = loop.create_task(coro, context=ctx)
     task.add_done_callback(silent_done_task)
 
     if look_at_task:
         look_at_task(task)
 
     res = loop.run_until_complete(task)
     _raise_maybe(func, info)
@@ -144,33 +204,35 @@
         return override(got, *args, **kwargs)
 
     wrapper.__original__ = func
 
     return wrapper
 
 
-def convert_async_coroutine_fixture(fixturedef, request, node):
+def convert_async_coroutine_fixture(ctx, fixturedef, request, node):
     """
     Run our async fixture in our event loop and capture the error from
     inside the loop.
     """
     func = fixturedef.func
     timeout = _find_async_timeout(func, node)
 
     def override(extra, *args, **kwargs):
         __tracebackhide__ = True
 
         info = {"func": func}
         loop = asyncio.get_event_loop_policy().get_event_loop()
-        return _run_and_raise(loop, info, func, async_runner(func, timeout, info, args, kwargs))
+        return _run_and_raise(
+            ctx, loop, info, func, async_runner(func, timeout, info, args, kwargs)
+        )
 
     fixturedef.func = _wrap(fixturedef, [], override, func)
 
 
-def convert_async_gen_fixture(fixturedef, request, node):
+def convert_async_gen_fixture(ctx, fixturedef, request, node):
     """
     Return the yield'd value from the generator and ensure the generator is
     finished.
     """
     generator = fixturedef.func
 
     def override(extra, *args, **kwargs):
@@ -200,19 +262,20 @@
                 await async_runner(gen_obj.__anext__, timeout, info, (), {})
                 if "e" in info:
                     if isinstance(info["e"], StopAsyncIteration):
                         del info["e"]
                 else:
                     info["e"] = ValueError("Async generator fixture should only yield once")
 
-            _run_and_raise(loop, info, generator, async_finalizer())
+            _run_and_raise(ctx, loop, info, generator, async_finalizer())
 
         request.addfinalizer(finalizer)
 
         return _run_and_raise(
+            ctx,
             loop,
             info,
             generator,
             async_runner(gen_obj.__anext__, timeout, info, (), {}),
         )
 
     fixturedef.func = _wrap(fixturedef, ["request"], override, generator)
```

### Comparing `alt_pytest_asyncio-0.7.2/alt_pytest_asyncio/plugin.py` & `alt_pytest_asyncio-0.8.0/alt_pytest_asyncio/plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import contextvars
 import inspect
 import sys
 from collections import defaultdict
 from functools import partial, wraps
 
 import pytest
 from _pytest._code.code import ExceptionInfo
@@ -15,15 +16,17 @@
         self.own_loop = False
         self.test_tasks = defaultdict(list)
 
         if loop is None:
             self.own_loop = True
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
+
         self.loop = loop
+        self.ctx = contextvars.copy_context()
 
     def pytest_configure(self, config):
         """Register our timeout marker which is used to signify async timeouts"""
         config.addinivalue_line(
             "markers", "async_timeout(length): mark async test to have a timeout"
         )
 
@@ -53,15 +56,15 @@
                     cancel_all_tasks(self.loop)
                 finally:
                     self.loop.close()
 
     @pytest.hookimpl(tryfirst=True, hookwrapper=True)
     def pytest_fixture_setup(self, fixturedef, request):
         """Convert async fixtures to sync fixtures"""
-        convert_fixtures(fixturedef, request, request.node)
+        convert_fixtures(self.ctx, fixturedef, request, request.node)
         yield
 
     @pytest.hookimpl(tryfirst=True, hookwrapper=True)
     def pytest_pyfunc_call(self, pyfuncitem):
         """Convert async tests to sync tests"""
         if inspect.iscoroutinefunction(pyfuncitem.obj):
             timeout = pyfuncitem.get_closest_marker("async_timeout")
@@ -71,15 +74,33 @@
             else:
                 timeout = float(
                     pyfuncitem.config.getoption("default_async_timeout", None)
                     or pyfuncitem.config.getini("default_async_timeout")
                 )
 
             o = pyfuncitem.obj
-            pyfuncitem.obj = wraps(o)(partial(converted_async_test, self.test_tasks, o, timeout))
+            pyfuncitem.obj = wraps(o)(
+                partial(converted_async_test, self.ctx, self.test_tasks, o, timeout)
+            )
+        else:
+
+            original = pyfuncitem.obj
+
+            @wraps(original)
+            def run_obj(*args, **kwargs):
+                try:
+                    self.ctx.run(lambda: None)
+                    run = lambda func, *a, **kw: self.ctx.run(func, *a, **kw)
+                except RuntimeError:
+                    run = lambda func, *a, **kw: func(*a, **kw)
+
+                run(original, *args, **kwargs)
+
+            pyfuncitem.obj = run_obj
+
         yield
 
 
 def cancel_all_tasks(loop, ignore_errors_from_tasks=None):
     if hasattr(asyncio.tasks, "all_tasks"):
         to_cancel = asyncio.tasks.all_tasks(loop)
     else:
```

### Comparing `alt_pytest_asyncio-0.7.2/LICENSE` & `alt_pytest_asyncio-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `alt_pytest_asyncio-0.7.2/README.rst` & `alt_pytest_asyncio-0.8.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 
 Like pytest-asyncio it supports async tests, coroutine fixtures and async
 generator fixtures.
 
 Changelog
 ---------
 
+0.8.0 - 1 June 2024
+    * Provide simple support for tests being aware of asyncio.Context
+    * Remove support for python less than 3.11
+    * Added support for asyncio ContextVars
+
 0.7.2 - 1 October 2023
     * Timeouts don't take affect if the debugger is active
 
 0.7.1 - 23 June 2023
     * No functional changes, only fixing how hatchling understands the
       license field in the pyproject.toml with thanks to @piotrm-nvidia
```

### Comparing `alt_pytest_asyncio-0.7.2/pyproject.toml` & `alt_pytest_asyncio-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 
 [project]
 name = "alt-pytest-asyncio"
 dynamic = ["version"]
 description = "Alternative pytest plugin to pytest-asyncio"
 readme = "README.rst"
 license = { text = "MIT" }
-requires-python = ">= 3.7"
+requires-python = ">= 3.11"
 authors = [
     { name = "Stephen Moore", email = "delfick755@gmail.com" },
 ]
 classifiers = [
     "Framework :: Pytest",
     "Topic :: Software Development :: Testing",
 ]
 dependencies = [
-    "pytest >= 7.0.0",
+    "pytest >= 8.0.0",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "nest-asyncio==1.0.0",
-    "noseOfYeti[black]==2.4.1",
-    "pytest==7.3.0",
+    "nest-asyncio==1.6.0",
+    "noseOfYeti[black]==2.4.9",
+    "pytest==8.2.1",
+    "pytest-order==1.2.1"
 ]
 
 [project.entry-points.pytest11]
 alt_pytest_asyncio = "alt_pytest_asyncio"
 
 [project.urls]
 Homepage = "https://github.com/delfick/alt-pytest-asyncio"
```

### Comparing `alt_pytest_asyncio-0.7.2/PKG-INFO` & `alt_pytest_asyncio-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: alt-pytest-asyncio
-Version: 0.7.2
+Version: 0.8.0
 Summary: Alternative pytest plugin to pytest-asyncio
 Project-URL: Homepage, https://github.com/delfick/alt-pytest-asyncio
 Author-email: Stephen Moore <delfick755@gmail.com>
 License: MIT
 License-File: LICENSE
 Classifier: Framework :: Pytest
 Classifier: Topic :: Software Development :: Testing
-Requires-Python: >=3.7
-Requires-Dist: pytest>=7.0.0
+Requires-Python: >=3.11
+Requires-Dist: pytest>=8.0.0
 Provides-Extra: tests
-Requires-Dist: nest-asyncio==1.0.0; extra == 'tests'
-Requires-Dist: noseofyeti[black]==2.4.1; extra == 'tests'
-Requires-Dist: pytest==7.3.0; extra == 'tests'
+Requires-Dist: nest-asyncio==1.6.0; extra == 'tests'
+Requires-Dist: noseofyeti[black]==2.4.9; extra == 'tests'
+Requires-Dist: pytest-order==1.2.1; extra == 'tests'
+Requires-Dist: pytest==8.2.1; extra == 'tests'
 Description-Content-Type: text/x-rst
 
 Alternative Pytest Asyncio
 ==========================
 
 This plugin allows you to have async pytest fixtures and tests.
 
@@ -35,14 +36,19 @@
 
 Like pytest-asyncio it supports async tests, coroutine fixtures and async
 generator fixtures.
 
 Changelog
 ---------
 
+0.8.0 - 1 June 2024
+    * Provide simple support for tests being aware of asyncio.Context
+    * Remove support for python less than 3.11
+    * Added support for asyncio ContextVars
+
 0.7.2 - 1 October 2023
     * Timeouts don't take affect if the debugger is active
 
 0.7.1 - 23 June 2023
     * No functional changes, only fixing how hatchling understands the
       license field in the pyproject.toml with thanks to @piotrm-nvidia
```

