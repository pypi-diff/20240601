# Comparing `tmp/httpx_request-0.0.3.tar.gz` & `tmp/httpx_request-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpx_request-0.0.3.tar", max compression
+gzip compressed data, was "httpx_request-0.0.4.tar", max compression
```

## Comparing `httpx_request-0.0.3.tar` & `httpx_request-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 httpx_request-0.0.3/LICENSE
--rwxr-xr-x   0        0        0     4785 2024-05-16 08:24:58.470025 httpx_request-0.0.3/httpx_request/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 httpx_request-0.0.3/httpx_request/py.typed
--rw-r--r--   0        0        0     1184 2024-05-16 08:25:23.404061 httpx_request-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      217 2024-05-15 17:03:44.296772 httpx_request-0.0.3/readme.md
--rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 httpx_request-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 httpx_request-0.0.4/LICENSE
+-rwxr-xr-x   0        0        0     6077 2024-06-01 14:35:31.330850 httpx_request-0.0.4/httpx_request/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 httpx_request-0.0.4/httpx_request/py.typed
+-rw-r--r--   0        0        0     1184 2024-06-01 14:43:57.725273 httpx_request-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      217 2024-05-15 17:03:44.296772 httpx_request-0.0.4/readme.md
+-rw-r--r--   0        0        0     1395 1970-01-01 00:00:00.000000 httpx_request-0.0.4/PKG-INFO
```

### Comparing `httpx_request-0.0.3/LICENSE` & `httpx_request-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `httpx_request-0.0.3/httpx_request/__init__.py` & `httpx_request-0.0.4/httpx_request/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 #!/usr/bin/env python3
 # coding: utf-8
 
 __author__ = "ChenyangGao <https://chenyanggao.github.io>"
-__version__ = (0, 0, 3)
+__version__ = (0, 0, 4)
 __all__ = ["request"]
 
 from asyncio import get_running_loop, run, run_coroutine_threadsafe
-from collections.abc import Callable
+from collections.abc import Awaitable, Callable
 from json import loads
+from typing import cast, overload, Any, Literal, TypeVar
 
 from argtools import argcount
+from httpx import ConnectTimeout, ReadTimeout
 from httpx._types import AuthTypes, SyncByteStream, URLTypes
 from httpx._client import AsyncClient, Client, Response, UseClientDefault, USE_CLIENT_DEFAULT
 
+
 if "__del__" not in Client.__dict__:
     setattr(Client, "__del__", Client.close)
 
 if "__del__" not in AsyncClient.__dict__:
     def __del__(self, /):
         try:
             try:
@@ -57,25 +60,33 @@
     auth: None | AuthTypes | UseClientDefault = USE_CLIENT_DEFAULT, 
     follow_redirects: bool | UseClientDefault = USE_CLIENT_DEFAULT, 
     stream: bool = True, 
     **request_kwargs, 
 ):
     if session is None:
         session = Client()
+    method = method.upper()
     request = session.build_request(
         method=method, 
         url=url, 
         **request_kwargs, 
     )
-    resp = session.send(
-        request=request,
-        auth=auth,
-        follow_redirects=follow_redirects,
-        stream=stream,
-    )
+    for _ in range(5):
+        try:
+            resp = session.send(
+                request=request,
+                auth=auth,
+                follow_redirects=follow_redirects,
+                stream=stream,
+            )
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
         return resp.read()
     elif parse is True:
@@ -110,20 +121,27 @@
     if session is None:
         session = AsyncClient()
     request = session.build_request(
         method=method, 
         url=url, 
         **request_kwargs, 
     )
-    resp = await session.send(
-        request=request,
-        auth=auth,
-        follow_redirects=follow_redirects,
-        stream=stream,
-    )
+    for _ in range(5):
+        try:
+            resp = await session.send(
+                request=request,
+                auth=auth,
+                follow_redirects=follow_redirects,
+                stream=stream,
+            )
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
         return await resp.aread()
     elif parse is True:
@@ -140,28 +158,57 @@
         ac = argcount(parse)
         if ac == 1:
             return parse(resp)
         else:
             return parse(resp, await resp.aread())
 
 
+@overload
+def request(
+    url: URLTypes, 
+    method: str = "GET", 
+    parse: None | bool | Callable = None, 
+    raise_for_status: bool = False, 
+    session: None | Client | AsyncClient = None, 
+    async_: Literal[False] = False, 
+    **request_kwargs, 
+) -> Any:
+    ...
+@overload
+def request(
+    url: URLTypes, 
+    method: str, 
+    parse: None | bool | Callable, 
+    raise_for_status: bool, 
+    session: None | AsyncClient, 
+    async_: Literal[True], 
+    **request_kwargs, 
+) -> Awaitable[Any]:
+    ...
 def request(
     url: URLTypes, 
     method: str = "GET", 
     parse: None | bool | Callable = None, 
     raise_for_status: bool = False, 
     session: None | Client | AsyncClient = None, 
-    async_: bool = False, 
+    async_: Literal[False, True] = False, 
     **request_kwargs, 
 ):
-    if session is not None:
-        async_ = isinstance(session, AsyncClient)
-    request = request_async if async_ else request_sync
-    return request( # type: ignore
-        url, 
-        method, 
-        parse=parse, 
-        raise_for_status=raise_for_status, 
-        session=session, 
-        **request_kwargs, 
-    )
+    if async_:
+        return request_async(
+            url, 
+            method=method, 
+            parse=parse, 
+            raise_for_status=raise_for_status, 
+            session=cast(None | AsyncClient, session), 
+            **request_kwargs, 
+        )
+    else:
+        return request_sync(
+            url, 
+            method=method, 
+            parse=parse, 
+            raise_for_status=raise_for_status, 
+            session=cast(None | Client, session), 
+            **request_kwargs, 
+        )
```

### Comparing `httpx_request-0.0.3/pyproject.toml` & `httpx_request-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "httpx_request"
-version = "0.0.3"
+version = "0.0.4"
 description = "httpx request extension."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/httpx_request"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/httpx_request"
 keywords = ["httpx", "request"]
```

### Comparing `httpx_request-0.0.3/PKG-INFO` & `httpx_request-0.0.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpx_request
-Version: 0.0.3
+Version: 0.0.4
 Summary: httpx request extension.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/httpx_request
 License: MIT
 Keywords: httpx,request
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

