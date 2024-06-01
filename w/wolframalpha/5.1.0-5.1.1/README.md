# Comparing `tmp/wolframalpha-5.1.0.tar.gz` & `tmp/wolframalpha-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolframalpha-5.1.0.tar", last modified: Sat Jun  1 11:08:39 2024, max compression
+gzip compressed data, was "wolframalpha-5.1.1.tar", last modified: Sat Jun  1 16:24:08 2024, max compression
```

## Comparing `wolframalpha-5.1.0.tar` & `wolframalpha-5.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:08:39.002537 wolframalpha-5.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:08:38.994537 wolframalpha-5.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:08:38.994537 wolframalpha-5.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-06-01 11:08:39.002537 wolframalpha-5.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:08:38.998537 wolframalpha-5.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 11:08:39.002537 wolframalpha-5.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:08:38.998537 wolframalpha-5.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/tests/test_pmxbot.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:08:38.998537 wolframalpha-5.1.0/wolframalpha/
--rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/wolframalpha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/wolframalpha/pmxbot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:08:38.998537 wolframalpha-5.1.0/wolframalpha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-06-01 11:08:38.000000 wolframalpha-5.1.0/wolframalpha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 11:08:38.000000 wolframalpha-5.1.0/wolframalpha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 11:08:38.000000 wolframalpha-5.1.0/wolframalpha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-01 11:08:38.000000 wolframalpha-5.1.0/wolframalpha.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-06-01 11:08:38.000000 wolframalpha-5.1.0/wolframalpha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-01 11:08:38.000000 wolframalpha-5.1.0/wolframalpha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:24:08.127108 wolframalpha-5.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:24:08.123108 wolframalpha-5.1.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:24:08.123108 wolframalpha-5.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3135 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-06-01 16:24:08.127108 wolframalpha-5.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:24:08.123108 wolframalpha-5.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 16:24:08.127108 wolframalpha-5.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:24:08.123108 wolframalpha-5.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/tests/test_pmxbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:24:08.127108 wolframalpha-5.1.1/wolframalpha/
+-rw-r--r--   0 runner    (1001) docker     (127)     7625 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/wolframalpha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-06-01 16:23:47.000000 wolframalpha-5.1.1/wolframalpha/pmxbot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:24:08.127108 wolframalpha-5.1.1/wolframalpha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-06-01 16:24:08.000000 wolframalpha-5.1.1/wolframalpha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 16:24:08.000000 wolframalpha-5.1.1/wolframalpha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 16:24:08.000000 wolframalpha-5.1.1/wolframalpha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-01 16:24:08.000000 wolframalpha-5.1.1/wolframalpha.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-06-01 16:24:08.000000 wolframalpha-5.1.1/wolframalpha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-01 16:24:08.000000 wolframalpha-5.1.1/wolframalpha.egg-info/top_level.txt
```

### Comparing `wolframalpha-5.1.0/.github/workflows/main.yml` & `wolframalpha-5.1.1/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.1.0/LICENSE` & `wolframalpha-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.1.0/NEWS.rst` & `wolframalpha-5.1.1/NEWS.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v5.1.1
+======
+
+Bugfixes
+--------
+
+- Add test for async functionality and fixed issue with implementation.
+
+
 v5.1.0
 ======
 
 Features
 --------
 
 - Implement async support via client.aquery. (#30)
```

### Comparing `wolframalpha-5.1.0/PKG-INFO` & `wolframalpha-5.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolframalpha
-Version: 5.1.0
+Version: 5.1.1
 Summary: Wolfram|Alpha 2.0 API client
 Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
 Project-URL: Homepage, https://github.com/jaraco/wolframalpha
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wolframalpha-5.1.0/README.rst` & `wolframalpha-5.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.1.0/docs/conf.py` & `wolframalpha-5.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.1.0/pyproject.toml` & `wolframalpha-5.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.1.0/pytest.ini` & `wolframalpha-5.1.1/pytest.ini`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.1.0/tests/test_client.py` & `wolframalpha-5.1.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.1.0/tox.ini` & `wolframalpha-5.1.1/tox.ini`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.1.0/wolframalpha/__init__.py` & `wolframalpha-5.1.1/wolframalpha/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import asyncio
 import itertools
 import json
 import getpass
 import os
 import contextlib
 import collections
 from typing import Dict, Any, Callable, Tuple
@@ -110,25 +111,20 @@
         ...     ('assumption', 'DateOrder_**Day.Month.Year--'),
         ... )
         >>> res = client.query(input='pi', params=params)
 
         For more details on Assumptions, see
         https://products.wolframalpha.com/api/documentation.html#6
         """
-        resp = httpx.get(self.url, params=self.__params(input, **kwargs))
-        return self.__process(resp)
+        return asyncio.run(self.aquery(input, **kwargs))
 
     async def aquery(self, input, **kwargs):
-        resp = await httpx.aget(self.url, params=self.__params(input, **kwargs))
-        return self.__process(resp)
-
-    def __params(self, input, **kwargs):
-        return dict(appid=self.app_id, input=input) | kwargs
-
-    def __process(self, resp):
+        params = dict(appid=self.app_id, input=input) | kwargs
+        async with httpx.AsyncClient() as client:
+            resp = await client.get(self.url, params=params)
         assert resp.headers['Content-Type'] == 'text/xml;charset=utf-8'
         doc = xmltodict.parse(resp.content, postprocessor=Document.make)
         return doc['queryresult']
 
 
 class ErrorHandler:
     def __init__(self, *args, **kwargs):
```

### Comparing `wolframalpha-5.1.0/wolframalpha.egg-info/PKG-INFO` & `wolframalpha-5.1.1/wolframalpha.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wolframalpha
-Version: 5.1.0
+Version: 5.1.1
 Summary: Wolfram|Alpha 2.0 API client
 Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
 Project-URL: Homepage, https://github.com/jaraco/wolframalpha
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `wolframalpha-5.1.0/wolframalpha.egg-info/SOURCES.txt` & `wolframalpha-5.1.1/wolframalpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

