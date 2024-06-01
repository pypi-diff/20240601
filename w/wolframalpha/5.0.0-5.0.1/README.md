# Comparing `tmp/wolframalpha-5.0.0.tar.gz` & `tmp/wolframalpha-5.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolframalpha-5.0.0.tar", last modified: Mon Feb 15 01:43:40 2021, max compression
+gzip compressed data, was "wolframalpha-5.0.1.tar", last modified: Sat Jun  1 10:37:06 2024, max compression
```

## Comparing `wolframalpha-5.0.0.tar` & `wolframalpha-5.0.1.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 01:43:40.215556 wolframalpha-5.0.0/
--rw-r--r--   0 runner    (1001) docker     (121)       50 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      136 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 01:43:40.211555 wolframalpha-5.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 01:43:40.211555 wolframalpha-5.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      497 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/.github/workflows/automerge.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1111 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)       79 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2848 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2021-02-15 01:43:40.215556 wolframalpha-5.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      939 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      325 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 01:43:40.215556 wolframalpha-5.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      756 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)       81 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (121)      296 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       37 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (121)      367 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      333 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2021-02-15 01:43:40.215556 wolframalpha-5.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       92 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    10139 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/skeleton.md
--rw-r--r--   0 runner    (1001) docker     (121)      751 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 01:43:40.215556 wolframalpha-5.0.0/wolframalpha/
--rw-r--r--   0 runner    (1001) docker     (121)     7517 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/wolframalpha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      391 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/wolframalpha/pmxbot.py
--rw-r--r--   0 runner    (1001) docker     (121)     2435 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/wolframalpha/test_client.py
--rw-r--r--   0 runner    (1001) docker     (121)      336 2021-02-15 01:43:18.000000 wolframalpha-5.0.0/wolframalpha/test_pmxbot.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 01:43:40.215556 wolframalpha-5.0.0/wolframalpha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2021-02-15 01:43:40.000000 wolframalpha-5.0.0/wolframalpha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      603 2021-02-15 01:43:40.000000 wolframalpha-5.0.0/wolframalpha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-15 01:43:40.000000 wolframalpha-5.0.0/wolframalpha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2021-02-15 01:43:40.000000 wolframalpha-5.0.0/wolframalpha.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      287 2021-02-15 01:43:40.000000 wolframalpha-5.0.0/wolframalpha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-02-15 01:43:40.000000 wolframalpha-5.0.0/wolframalpha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:37:06.547164 wolframalpha-5.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:37:06.543164 wolframalpha-5.0.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:37:06.543164 wolframalpha-5.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-06-01 10:37:06.547164 wolframalpha-5.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:37:06.543164 wolframalpha-5.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 10:37:06.547164 wolframalpha-5.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:37:06.543164 wolframalpha-5.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/tests/test_pmxbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:37:06.543164 wolframalpha-5.0.1/wolframalpha/
+-rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/wolframalpha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/wolframalpha/pmxbot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:37:06.543164 wolframalpha-5.0.1/wolframalpha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-06-01 10:37:06.000000 wolframalpha-5.0.1/wolframalpha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 10:37:06.000000 wolframalpha-5.0.1/wolframalpha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 10:37:06.000000 wolframalpha-5.0.1/wolframalpha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-01 10:37:06.000000 wolframalpha-5.0.1/wolframalpha.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-01 10:37:06.000000 wolframalpha-5.0.1/wolframalpha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-01 10:37:06.000000 wolframalpha-5.0.1/wolframalpha.egg-info/top_level.txt
```

### Comparing `wolframalpha-5.0.0/CHANGES.rst` & `wolframalpha-5.0.1/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v5.0.1
+======
+
+Bugfixes
+--------
+
+- Now correctly resolve Warnings and Assumptions. (#29)
+
+
 v5.0.0
 ======
 
 * Rewrote object model to load objects more automatically.
   API is mostly compatible, but there may be some rare
   uses that may need some adjustment. In particular,
   access to 'children' properties ('pods', 'subpods',
```

### Comparing `wolframalpha-5.0.0/LICENSE` & `wolframalpha-5.0.1/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-Copyright Jason R. Coombs
-
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to
 deal in the Software without restriction, including without limitation the
 rights to use, copy, modify, merge, publish, distribute, sublicense, and/or
 sell copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `wolframalpha-5.0.0/docs/conf.py` & `wolframalpha-5.0.1/docs/conf.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,42 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-
-extensions = ['sphinx.ext.autodoc', 'jaraco.packaging.sphinx', 'rst.linker']
+extensions = [
+    'sphinx.ext.autodoc',
+    'jaraco.packaging.sphinx',
+]
 
 master_doc = "index"
+html_theme = "furo"
 
+# Link dates and other references in the changelog
+extensions += ['rst.linker']
 link_files = {
-    '../CHANGES.rst': dict(
+    '../NEWS.rst': dict(
         using=dict(GH='https://github.com'),
         replace=[
             dict(
                 pattern=r'(Issue #|\B#)(?P<issue>\d+)',
                 url='{package_url}/issues/{issue}',
             ),
             dict(
                 pattern=r'(?m:^((?P<scm_version>v?\d+(\.\d+){1,2}))\n[-=]+\n)',
                 with_scm='{text}\n{rev[timestamp]:%d %b %Y}\n',
             ),
             dict(
                 pattern=r'PEP[- ](?P<pep_number>\d+)',
-                url='https://www.python.org/dev/peps/pep-{pep_number:0>4}/',
+                url='https://peps.python.org/pep-{pep_number:0>4}/',
             ),
         ],
     )
 }
+
+# Be strict about any broken references
+nitpicky = True
+
+# Include Python intersphinx mapping to prevent failures
+# jaraco/skeleton#51
+extensions += ['sphinx.ext.intersphinx']
+intersphinx_mapping = {
+    'python': ('https://docs.python.org/3', None),
+}
+
+# Preserve authored syntax for defaults
+autodoc_preserve_defaults = True
```

### Comparing `wolframalpha-5.0.0/wolframalpha/__init__.py` & `wolframalpha-5.0.1/wolframalpha/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -185,20 +185,22 @@
         except KeyError:
             raise AttributeError(name)
         return val
 
     def _get_children(self, name):
         if name not in self.__class__.children:
             return
+
+        # some objects, like Assumptions and Warnings
+        # are found in a container with the plural name;
+        # others like Pods and Subpods appear directly in
+        # the parent (self).
+        container = self.get(name, self)
         singular = name.rstrip('s')
-        try:
-            val = self._get_attr(singular)
-        except AttributeError:
-            val = None
-        return always_iterable(val, base_type=dict)
+        return always_iterable(container.get(singular), base_type=dict)
 
 
 class Assumption(Document):
     @property
     def text(self):
         text = self.template.replace('${desc1}', self.description)
         with contextlib.suppress(Exception):
```

### Comparing `wolframalpha-5.0.0/wolframalpha/test_client.py` & `wolframalpha-5.0.1/tests/test_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,14 +40,21 @@
     assumptions = list(res.assumptions)
     assert all(isinstance(item, wolframalpha.Assumption) for item in assumptions)
     pods = list(res.pods)
     assert all(isinstance(item, wolframalpha.Pod) for item in pods)
     assert len(info) == len(pods) + len(warnings) + len(assumptions)
 
 
+def test_assumptions(client):
+    res = client.query('pi')
+    (assumption,) = res.assumptions
+    assert assumption.word == 'pi'
+    assert assumption.type == 'Clash'
+
+
 def test_pod_attributes(temp_result):
     pod = next(temp_result.pods)
     assert isinstance(pod.position, float)
     assert isinstance(pod.id, str)
     img = next(iter(pod.subpods)).img
     assert isinstance(img.height, int)
```

