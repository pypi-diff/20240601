# Comparing `tmp/httpx_request-0.0.2.tar.gz` & `tmp/httpx_request-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpx_request-0.0.2.tar", max compression
+gzip compressed data, was "httpx_request-0.0.3.tar", max compression
```

## Comparing `httpx_request-0.0.2.tar` & `httpx_request-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 httpx_request-0.0.2/LICENSE
--rwxr-xr-x   0        0        0     5526 2024-05-16 04:04:15.691155 httpx_request-0.0.2/httpx_request/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 httpx_request-0.0.2/httpx_request/py.typed
--rw-r--r--   0        0        0     1184 2024-05-16 04:04:33.332737 httpx_request-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      217 2024-05-15 17:03:44.296772 httpx_request-0.0.2/readme.md
--rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 httpx_request-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 httpx_request-0.0.3/LICENSE
+-rwxr-xr-x   0        0        0     4785 2024-05-16 08:24:58.470025 httpx_request-0.0.3/httpx_request/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 httpx_request-0.0.3/httpx_request/py.typed
+-rw-r--r--   0        0        0     1184 2024-05-16 08:25:23.404061 httpx_request-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      217 2024-05-15 17:03:44.296772 httpx_request-0.0.3/readme.md
+-rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 httpx_request-0.0.3/PKG-INFO
```

### Comparing `httpx_request-0.0.2/LICENSE` & `httpx_request-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `httpx_request-0.0.2/httpx_request/__init__.py` & `httpx_request-0.0.3/httpx_request/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 2)
+__version__ = (0, 0, 3)
 __all__ = ["request"]
 
 from asyncio import get_running_loop, run, run_coroutine_threadsafe
 from collections.abc import Callable
 from json import loads
 
 from argtools import argcount
@@ -56,26 +56,15 @@
     session: None | Client = None, 
     auth: None | AuthTypes | UseClientDefault = USE_CLIENT_DEFAULT, 
     follow_redirects: bool | UseClientDefault = USE_CLIENT_DEFAULT, 
     stream: bool = True, 
     **request_kwargs, 
 ):
     if session is None:
-        with Client() as session:
-            return request_sync(
-                url, 
-                method, 
-                parse=parse, 
-                raise_for_status=raise_for_status, 
-                session=session, 
-                auth=auth, 
-                follow_redirects=follow_redirects, 
-                stream=stream, 
-                **request_kwargs, 
-            )
+        session = Client()
     request = session.build_request(
         method=method, 
         url=url, 
         **request_kwargs, 
     )
     resp = session.send(
         request=request,
@@ -115,26 +104,15 @@
     session: None | AsyncClient = None, 
     auth: None | AuthTypes | UseClientDefault = USE_CLIENT_DEFAULT, 
     follow_redirects: bool | UseClientDefault = USE_CLIENT_DEFAULT, 
     stream: bool = True, 
     **request_kwargs, 
 ):
     if session is None:
-        async with AsyncClient() as session:
-            return await request_async(
-                url, 
-                method, 
-                parse=parse, 
-                raise_for_status=raise_for_status, 
-                session=session, 
-                auth=auth, 
-                follow_redirects=follow_redirects, 
-                stream=stream, 
-                **request_kwargs, 
-            )
+        session = AsyncClient()
     request = session.build_request(
         method=method, 
         url=url, 
         **request_kwargs, 
     )
     resp = await session.send(
         request=request,
```

### Comparing `httpx_request-0.0.2/pyproject.toml` & `httpx_request-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "httpx_request"
-version = "0.0.2"
+version = "0.0.3"
 description = "httpx request extension."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/httpx_request"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/httpx_request"
 keywords = ["httpx", "request"]
```

### Comparing `httpx_request-0.0.2/PKG-INFO` & `httpx_request-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx_request
-Version: 0.0.2
+Version: 0.0.3
 Summary: httpx request extension.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/httpx_request
 License: MIT
 Keywords: httpx,request
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

