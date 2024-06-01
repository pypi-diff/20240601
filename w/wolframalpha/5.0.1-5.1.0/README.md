# Comparing `tmp/wolframalpha-5.0.1.tar.gz` & `tmp/wolframalpha-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wolframalpha-5.0.1.tar", last modified: Sat Jun  1 10:37:06 2024, max compression
+gzip compressed data, was "wolframalpha-5.1.0.tar", last modified: Sat Jun  1 11:08:39 2024, max compression
```

## Comparing `wolframalpha-5.0.1.tar` & `wolframalpha-5.1.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:37:06.547164 wolframalpha-5.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:37:06.543164 wolframalpha-5.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:37:06.543164 wolframalpha-5.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-06-01 10:37:06.547164 wolframalpha-5.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      325 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:37:06.543164 wolframalpha-5.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 10:37:06.547164 wolframalpha-5.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:37:06.543164 wolframalpha-5.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/tests/test_pmxbot.py
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:37:06.543164 wolframalpha-5.0.1/wolframalpha/
--rw-r--r--   0 runner    (1001) docker     (127)     7667 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/wolframalpha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-06-01 10:36:44.000000 wolframalpha-5.0.1/wolframalpha/pmxbot.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:37:06.543164 wolframalpha-5.0.1/wolframalpha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-06-01 10:37:06.000000 wolframalpha-5.0.1/wolframalpha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 10:37:06.000000 wolframalpha-5.0.1/wolframalpha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 10:37:06.000000 wolframalpha-5.0.1/wolframalpha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-01 10:37:06.000000 wolframalpha-5.0.1/wolframalpha.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-01 10:37:06.000000 wolframalpha-5.0.1/wolframalpha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-01 10:37:06.000000 wolframalpha-5.0.1/wolframalpha.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:08:39.002537 wolframalpha-5.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:08:38.994537 wolframalpha-5.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:08:38.994537 wolframalpha-5.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-06-01 11:08:39.002537 wolframalpha-5.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      325 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:08:38.998537 wolframalpha-5.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 11:08:39.002537 wolframalpha-5.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:08:38.998537 wolframalpha-5.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/tests/test_pmxbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:08:38.998537 wolframalpha-5.1.0/wolframalpha/
+-rw-r--r--   0 runner    (1001) docker     (127)     7741 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/wolframalpha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-06-01 11:08:18.000000 wolframalpha-5.1.0/wolframalpha/pmxbot.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:08:38.998537 wolframalpha-5.1.0/wolframalpha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-06-01 11:08:38.000000 wolframalpha-5.1.0/wolframalpha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 11:08:38.000000 wolframalpha-5.1.0/wolframalpha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 11:08:38.000000 wolframalpha-5.1.0/wolframalpha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-01 11:08:38.000000 wolframalpha-5.1.0/wolframalpha.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-06-01 11:08:38.000000 wolframalpha-5.1.0/wolframalpha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-01 11:08:38.000000 wolframalpha-5.1.0/wolframalpha.egg-info/top_level.txt
```

### Comparing `wolframalpha-5.0.1/.github/workflows/main.yml` & `wolframalpha-5.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.0.1/LICENSE` & `wolframalpha-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.0.1/NEWS.rst` & `wolframalpha-5.1.0/NEWS.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+v5.1.0
+======
+
+Features
+--------
+
+- Implement async support via client.aquery. (#30)
+
+
 v5.0.1
 ======
 
 Bugfixes
 --------
 
 - Now correctly resolve Warnings and Assumptions. (#29)
```

### Comparing `wolframalpha-5.0.1/PKG-INFO` & `wolframalpha-5.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: wolframalpha
-Version: 5.0.1
+Version: 5.1.0
 Summary: Wolfram|Alpha 2.0 API client
 Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
 Project-URL: Homepage, https://github.com/jaraco/wolframalpha
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: xmltodict
 Requires-Dist: more_itertools
 Requires-Dist: jaraco.context
+Requires-Dist: httpx
 Provides-Extra: test
 Requires-Dist: pytest!=8.1.*,>=6; extra == "test"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mypy; extra == "test"
 Requires-Dist: pytest-enabler>=2.2; extra == "test"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "test"
```

### Comparing `wolframalpha-5.0.1/README.rst` & `wolframalpha-5.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.0.1/docs/conf.py` & `wolframalpha-5.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.0.1/pyproject.toml` & `wolframalpha-5.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 	"Programming Language :: Python :: 3 :: Only",
 ]
 requires-python = ">=3.8"
 dependencies = [
 	"xmltodict",
 	"more_itertools",
 	"jaraco.context",
+	"httpx",
 ]
 dynamic = ["version"]
 
 [project.urls]
 Homepage = "https://github.com/jaraco/wolframalpha"
 
 [project.optional-dependencies]
```

### Comparing `wolframalpha-5.0.1/pytest.ini` & `wolframalpha-5.1.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.0.1/tests/test_client.py` & `wolframalpha-5.1.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.0.1/tox.ini` & `wolframalpha-5.1.0/tox.ini`

 * *Files identical despite different names*

### Comparing `wolframalpha-5.0.1/wolframalpha/__init__.py` & `wolframalpha-5.1.0/wolframalpha/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import itertools
 import json
 import getpass
 import os
-import urllib.parse
-import urllib.request
 import contextlib
 import collections
 from typing import Dict, Any, Callable, Tuple
 
+import httpx
 import xmltodict
 from jaraco.context import suppress
 from more_itertools import always_iterable
 
 
 def xml_bool(str_val):
     """
@@ -64,14 +63,16 @@
     All objects returned are dictionary subclasses, so to find out which attributes
     Wolfram|Alpha has supplied, simply invoke ``.keys()`` on the object.
     Attributes formed from XML attributes can be accessed with or without their
     "@" prefix (added by xmltodict).
 
     """
 
+    url = 'https://api.wolframalpha.com/v2/query'
+
     def __init__(self, app_id):
         self.app_id = app_id
 
     @classmethod
     def from_env(cls):
         """
         Create a client with a key discovered from the keyring
@@ -109,26 +110,27 @@
         ...     ('assumption', 'DateOrder_**Day.Month.Year--'),
         ... )
         >>> res = client.query(input='pi', params=params)
 
         For more details on Assumptions, see
         https://products.wolframalpha.com/api/documentation.html#6
         """
-        data = dict(
-            input=input,
-            appid=self.app_id,
-        )
-        data = itertools.chain(params, data.items(), kwargs.items())
-
-        query = urllib.parse.urlencode(tuple(data))
-        url = 'https://api.wolframalpha.com/v2/query?' + query
-        resp = urllib.request.urlopen(url)
-        assert resp.headers.get_content_type() == 'text/xml'
-        assert resp.headers.get_param('charset') == 'utf-8'
-        doc = xmltodict.parse(resp, postprocessor=Document.make)
+        resp = httpx.get(self.url, params=self.__params(input, **kwargs))
+        return self.__process(resp)
+
+    async def aquery(self, input, **kwargs):
+        resp = await httpx.aget(self.url, params=self.__params(input, **kwargs))
+        return self.__process(resp)
+
+    def __params(self, input, **kwargs):
+        return dict(appid=self.app_id, input=input) | kwargs
+
+    def __process(self, resp):
+        assert resp.headers['Content-Type'] == 'text/xml;charset=utf-8'
+        doc = xmltodict.parse(resp.content, postprocessor=Document.make)
         return doc['queryresult']
 
 
 class ErrorHandler:
     def __init__(self, *args, **kwargs):
         super(ErrorHandler, self).__init__(*args, **kwargs)
         self._handle_error()
```

### Comparing `wolframalpha-5.0.1/wolframalpha.egg-info/PKG-INFO` & `wolframalpha-5.1.0/wolframalpha.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: wolframalpha
-Version: 5.0.1
+Version: 5.1.0
 Summary: Wolfram|Alpha 2.0 API client
 Author-email: "Jason R. Coombs" <jaraco@jaraco.com>
 Project-URL: Homepage, https://github.com/jaraco/wolframalpha
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: xmltodict
 Requires-Dist: more_itertools
 Requires-Dist: jaraco.context
+Requires-Dist: httpx
 Provides-Extra: test
 Requires-Dist: pytest!=8.1.*,>=6; extra == "test"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: pytest-mypy; extra == "test"
 Requires-Dist: pytest-enabler>=2.2; extra == "test"
 Requires-Dist: pytest-ruff>=0.2.1; extra == "test"
```

### Comparing `wolframalpha-5.0.1/wolframalpha.egg-info/SOURCES.txt` & `wolframalpha-5.1.0/wolframalpha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

