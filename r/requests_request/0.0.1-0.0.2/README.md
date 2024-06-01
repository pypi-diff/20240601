# Comparing `tmp/requests_request-0.0.1.tar.gz` & `tmp/requests_request-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "requests_request-0.0.1.tar", max compression
+gzip compressed data, was "requests_request-0.0.2.tar", max compression
```

## Comparing `requests_request-0.0.1.tar` & `requests_request-0.0.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 requests_request-0.0.1/LICENSE
--rw-r--r--   0        0        0     1205 2024-05-16 03:52:48.629947 requests_request-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      229 2024-05-16 03:53:04.645244 requests_request-0.0.1/readme.md
--rwxr-xr-x   0        0        0     1837 2024-05-16 04:05:44.313594 requests_request-0.0.1/requests_request/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 requests_request-0.0.1/requests_request/py.typed
--rw-r--r--   0        0        0     1425 1970-01-01 00:00:00.000000 requests_request-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 requests_request-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1205 2024-06-01 14:46:01.270161 requests_request-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      229 2024-05-16 03:53:04.645244 requests_request-0.0.2/readme.md
+-rwxr-xr-x   0        0        0     2092 2024-06-01 14:43:21.208227 requests_request-0.0.2/requests_request/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 requests_request-0.0.2/requests_request/py.typed
+-rw-r--r--   0        0        0     1425 1970-01-01 00:00:00.000000 requests_request-0.0.2/PKG-INFO
```

### Comparing `requests_request-0.0.1/LICENSE` & `requests_request-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `requests_request-0.0.1/pyproject.toml` & `requests_request-0.0.2/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "requests_request"
-version = "0.0.1"
+version = "0.0.2"
 description = "requests request extension."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/requests_request"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/requests_request"
 keywords = ["requests", "request"]
```

### Comparing `requests_request-0.0.1/requests_request/__init__.py` & `requests_request-0.0.2/requests_request/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 1)
+__version__ = (0, 0, 2)
 __all__ = ["request"]
 
 from collections.abc import Callable
 from json import loads
 
 from argtools import argcount
+from requests.exceptions import ConnectTimeout, ReadTimeout
 from requests.models import Response
 from requests.sessions import Session
 
 if "__del__" not in Response.__dict__:
     setattr(Response, "__del__", Response.close)
 
 if "__del__" not in Session.__dict__:
@@ -33,16 +34,24 @@
                 url, 
                 method, 
                 parse=parse, 
                 raise_for_status=raise_for_status, 
                 session=session, 
                 **request_kwargs, 
             )
+    method = method.upper()
     request_kwargs.setdefault("stream", True)
-    resp = session.request(method, url, **request_kwargs)
+    while True:
+        try:
+            resp = session.request(method, url, **request_kwargs)
+        except ConnectTimeout:
+            pass
+        except ReadTimeout:
+            if method != "GET":
+                raise
     if raise_for_status:
         resp.raise_for_status()
     if parse is None:
         return resp
     elif parse is False:
         return resp.content
     elif parse is True:
```

### Comparing `requests_request-0.0.1/PKG-INFO` & `requests_request-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: requests_request
-Version: 0.0.1
+Version: 0.0.2
 Summary: requests request extension.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/requests_request
 License: MIT
 Keywords: requests,request
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

