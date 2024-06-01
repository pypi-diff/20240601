# Comparing `tmp/wolframalpha-5.1.1.tar.gz` & `tmp/wolframalpha-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolframalpha-5.1.1.tar", last modified: Sat Jun  1 16:24:08 2024, max compression
+gzip compressed data, was "wolframalpha-5.1.2.tar", last modified: Sat Jun  1 16:46:45 2024, max compression
```

## Comparing `wolframalpha-5.1.1.tar` & `wolframalpha-5.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:24:08.127108 wolframalpha-5.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:24:08.123108 wolframalpha-5.1.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:24:08.123108 wolframalpha-5.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-06-01 16:24:08.127108 wolframalpha-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:24:08.123108 wolframalpha-5.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 16:24:08.127108 wolframalpha-5.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:24:08.123108 wolframalpha-5.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/tests/test_pmxbot.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:24:08.127108 wolframalpha-5.1.1/wolframalpha/
--rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/wolframalpha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/wolframalpha/pmxbot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:24:08.127108 wolframalpha-5.1.1/wolframalpha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-06-01 16:24:08.000000 wolframalpha-5.1.1/wolframalpha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 16:24:08.000000 wolframalpha-5.1.1/wolframalpha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 16:24:08.000000 wolframalpha-5.1.1/wolframalpha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-01 16:24:08.000000 wolframalpha-5.1.1/wolframalpha.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-06-01 16:24:08.000000 wolframalpha-5.1.1/wolframalpha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-01 16:24:08.000000 wolframalpha-5.1.1/wolframalpha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:46:45.706260 wolframalpha-5.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:46:45.702260 wolframalpha-5.1.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:46:45.702260 wolframalpha-5.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-06-01 16:46:45.706260 wolframalpha-5.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:46:45.702260 wolframalpha-5.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 16:46:45.706260 wolframalpha-5.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:46:45.702260 wolframalpha-5.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/tests/test_pmxbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:46:45.702260 wolframalpha-5.1.2/wolframalpha/
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/wolframalpha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-06-01 16:46:26.000000 wolframalpha-5.1.2/wolframalpha/pmxbot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:46:45.706260 wolframalpha-5.1.2/wolframalpha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2373 2024-06-01 16:46:45.000000 wolframalpha-5.1.2/wolframalpha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 16:46:45.000000 wolframalpha-5.1.2/wolframalpha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 16:46:45.000000 wolframalpha-5.1.2/wolframalpha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-01 16:46:45.000000 wolframalpha-5.1.2/wolframalpha.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      255 2024-06-01 16:46:45.000000 wolframalpha-5.1.2/wolframalpha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-01 16:46:45.000000 wolframalpha-5.1.2/wolframalpha.egg-info/top_level.txt
```

### Comparing `wolframalpha-5.1.1/.github/workflows/main.yml` & `wolframalpha-5.1.2/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.1.1/LICENSE` & `wolframalpha-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.1.1/NEWS.rst` & `wolframalpha-5.1.2/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v5.1.2
+======
+
+Bugfixes
+--------
+
+- Restore support for query params.
+
+
 v5.1.1
 ======
 
 Bugfixes
 --------
 
 - Add test for async functionality and fixed issue with implementation.
```

### Comparing `wolframalpha-5.1.1/PKG-INFO` & `wolframalpha-5.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolframalpha
-Version: 5.1.1
+Version: 5.1.2
 Summary: Wolfram|Alpha 2.0 API client
 Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
 Project-URL: Homepage, https://github.com/jaraco/wolframalpha
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: xmltodict
 Requires-Dist: more_itertools
 Requires-Dist: jaraco.context
 Requires-Dist: httpx
+Requires-Dist: multidict
 Provides-Extra: test
 Requires-Dist: pytest!=8.1.*,>=6; extra == "test"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mypy; extra == "test"
 Requires-Dist: pytest-enabler>=2.2; extra == "test"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "test"
```

### Comparing `wolframalpha-5.1.1/README.rst` & `wolframalpha-5.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.1.1/docs/conf.py` & `wolframalpha-5.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.1.1/pyproject.toml` & `wolframalpha-5.1.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 ]
 requires-python = ">=3.8"
 dependencies = [
 	"xmltodict",
 	"more_itertools",
 	"jaraco.context",
 	"httpx",
+	"multidict",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/jaraco/wolframalpha"
 
 [project.optional-dependencies]
```

### Comparing `wolframalpha-5.1.1/pytest.ini` & `wolframalpha-5.1.2/pytest.ini`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.1.1/tests/test_client.py` & `wolframalpha-5.1.2/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.1.1/tox.ini` & `wolframalpha-5.1.2/tox.ini`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.1.1/wolframalpha/__init__.py` & `wolframalpha-5.1.2/wolframalpha/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import getpass
 import os
 import contextlib
 import collections
 from typing import Dict, Any, Callable, Tuple
 
 import httpx
+import multidict
 import xmltodict
 from jaraco.context import suppress
 from more_itertools import always_iterable
 
 
 def xml_bool(str_val):
     """
@@ -111,20 +112,24 @@
         ...     ('assumption', 'DateOrder_**Day.Month.Year--'),
         ... )
         >>> res = client.query(input='pi', params=params)
 
         For more details on Assumptions, see
         https://products.wolframalpha.com/api/documentation.html#6
         """
-        return asyncio.run(self.aquery(input, **kwargs))
+        return asyncio.run(self.aquery(input, params, **kwargs))
 
-    async def aquery(self, input, **kwargs):
-        params = dict(appid=self.app_id, input=input) | kwargs
+    async def aquery(self, input, params=(), **kwargs):
         async with httpx.AsyncClient() as client:
-            resp = await client.get(self.url, params=params)
+            resp = await client.get(
+                self.url,
+                params=multidict.MultiDict(
+                    params, appid=self.app_id, input=input, **kwargs
+                ),
+            )
         assert resp.headers['Content-Type'] == 'text/xml;charset=utf-8'
         doc = xmltodict.parse(resp.content, postprocessor=Document.make)
         return doc['queryresult']
 
 
 class ErrorHandler:
     def __init__(self, *args, **kwargs):
```

### Comparing `wolframalpha-5.1.1/wolframalpha.egg-info/PKG-INFO` & `wolframalpha-5.1.2/wolframalpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolframalpha
-Version: 5.1.1
+Version: 5.1.2
 Summary: Wolfram|Alpha 2.0 API client
 Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
 Project-URL: Homepage, https://github.com/jaraco/wolframalpha
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,14 +12,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: xmltodict
 Requires-Dist: more_itertools
 Requires-Dist: jaraco.context
 Requires-Dist: httpx
+Requires-Dist: multidict
 Provides-Extra: test
 Requires-Dist: pytest!=8.1.*,>=6; extra == "test"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mypy; extra == "test"
 Requires-Dist: pytest-enabler>=2.2; extra == "test"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "test"
```

### Comparing `wolframalpha-5.1.1/wolframalpha.egg-info/SOURCES.txt` & `wolframalpha-5.1.2/wolframalpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

