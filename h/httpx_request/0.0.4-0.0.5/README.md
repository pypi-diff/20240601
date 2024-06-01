# Comparing `tmp/httpx_request-0.0.4.tar.gz` & `tmp/httpx_request-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpx_request-0.0.4.tar", max compression
+gzip compressed data, was "httpx_request-0.0.5.tar", max compression
```

## Comparing `httpx_request-0.0.4.tar` & `httpx_request-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 httpx_request-0.0.4/LICENSE
--rwxr-xr-x   0        0        0     6077 2024-06-01 14:35:31.330850 httpx_request-0.0.4/httpx_request/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 httpx_request-0.0.4/httpx_request/py.typed
--rw-r--r--   0        0        0     1184 2024-06-01 14:43:57.725273 httpx_request-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      217 2024-05-15 17:03:44.296772 httpx_request-0.0.4/readme.md
--rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 httpx_request-0.0.4/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 httpx_request-0.0.5/LICENSE
+-rwxr-xr-x   0        0        0     6120 2024-06-01 14:48:42.933610 httpx_request-0.0.5/httpx_request/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 httpx_request-0.0.5/httpx_request/py.typed
+-rw-r--r--   0        0        0     1184 2024-06-01 15:24:21.428595 httpx_request-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      217 2024-05-15 17:03:44.296772 httpx_request-0.0.5/readme.md
+-rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 httpx_request-0.0.5/PKG-INFO
```

### Comparing `httpx_request-0.0.4/LICENSE` & `httpx_request-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `httpx_request-0.0.4/httpx_request/__init__.py` & `httpx_request-0.0.5/httpx_request/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from asyncio import get_running_loop, run, run_coroutine_threadsafe
 from collections.abc import Awaitable, Callable
 from json import loads
 from typing import cast, overload, Any, Literal, TypeVar
 
 from argtools import argcount
-from httpx import ConnectTimeout, ReadTimeout
+from httpx import ConnectTimeout, PoolTimeout, ReadTimeout
 from httpx._types import AuthTypes, SyncByteStream, URLTypes
 from httpx._client import AsyncClient, Client, Response, UseClientDefault, USE_CLIENT_DEFAULT
 
 
 if "__del__" not in Client.__dict__:
     setattr(Client, "__del__", Client.close)
 
@@ -74,15 +74,15 @@
         try:
             resp = session.send(
                 request=request,
                 auth=auth,
                 follow_redirects=follow_redirects,
                 stream=stream,
             )
-        except ConnectTimeout:
+        except (ConnectTimeout, PoolTimeout):
             pass
         except ReadTimeout:
             if method != "GET":
                 raise
     if raise_for_status:
         resp.raise_for_status()
     if parse is None:
@@ -129,15 +129,15 @@
         try:
             resp = await session.send(
                 request=request,
                 auth=auth,
                 follow_redirects=follow_redirects,
                 stream=stream,
             )
-        except ConnectTimeout:
+        except (ConnectTimeout, PoolTimeout):
             pass
         except ReadTimeout:
             if method != "GET":
                 raise
     if raise_for_status:
         resp.raise_for_status()
     if parse is None:
```

### Comparing `httpx_request-0.0.4/pyproject.toml` & `httpx_request-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "httpx_request"
-version = "0.0.4"
+version = "0.0.5"
 description = "httpx request extension."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/httpx_request"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/httpx_request"
 keywords = ["httpx", "request"]
```

### Comparing `httpx_request-0.0.4/PKG-INFO` & `httpx_request-0.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx_request
-Version: 0.0.4
+Version: 0.0.5
 Summary: httpx request extension.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/httpx_request
 License: MIT
 Keywords: httpx,request
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

