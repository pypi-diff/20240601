# Comparing `tmp/fdk_asgi-0.7.0.tar.gz` & `tmp/fdk_asgi-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fdk_asgi-0.7.0.tar", max compression
+gzip compressed data, was "fdk_asgi-0.7.1.tar", max compression
```

## Comparing `fdk_asgi-0.7.0.tar` & `fdk_asgi-0.7.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2024-05-30 12:27:13.304253 fdk_asgi-0.7.0/LICENSE
--rw-r--r--   0        0        0     7648 2024-05-30 12:27:13.304253 fdk_asgi-0.7.0/README.md
--rw-r--r--   0        0        0     2710 2024-05-30 12:27:13.304253 fdk_asgi-0.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 12:27:13.304253 fdk_asgi-0.7.0/src/fdk_asgi/__init__.py
--rw-r--r--   0        0        0     5547 2024-05-30 12:27:13.304253 fdk_asgi-0.7.0/src/fdk_asgi/app.py
--rw-r--r--   0        0        0     6099 2024-05-30 12:27:13.304253 fdk_asgi-0.7.0/src/fdk_asgi/cli.py
--rw-r--r--   0        0        0      880 2024-05-30 12:27:13.304253 fdk_asgi-0.7.0/src/fdk_asgi/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-30 12:27:13.304253 fdk_asgi-0.7.0/src/fdk_asgi/py.typed
--rw-r--r--   0        0        0      621 2024-05-30 12:27:13.308253 fdk_asgi-0.7.0/src/fdk_asgi/types.py
--rw-r--r--   0        0        0     2262 2024-05-30 12:27:13.308253 fdk_asgi-0.7.0/src/fdk_asgi/utils.py
--rw-r--r--   0        0        0     8554 1970-01-01 00:00:00.000000 fdk_asgi-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-06-01 13:47:26.459839 fdk_asgi-0.7.1/LICENSE
+-rw-r--r--   0        0        0     7648 2024-06-01 13:47:26.459839 fdk_asgi-0.7.1/README.md
+-rw-r--r--   0        0        0     2655 2024-06-01 13:47:26.459839 fdk_asgi-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-01 13:47:26.459839 fdk_asgi-0.7.1/src/fdk_asgi/__init__.py
+-rw-r--r--   0        0        0     5245 2024-06-01 13:47:26.459839 fdk_asgi-0.7.1/src/fdk_asgi/app.py
+-rw-r--r--   0        0        0     6099 2024-06-01 13:47:26.459839 fdk_asgi-0.7.1/src/fdk_asgi/cli.py
+-rw-r--r--   0        0        0      880 2024-06-01 13:47:26.459839 fdk_asgi-0.7.1/src/fdk_asgi/exceptions.py
+-rw-r--r--   0        0        0        0 2024-06-01 13:47:26.459839 fdk_asgi-0.7.1/src/fdk_asgi/py.typed
+-rw-r--r--   0        0        0      621 2024-06-01 13:47:26.459839 fdk_asgi-0.7.1/src/fdk_asgi/types.py
+-rw-r--r--   0        0        0     2131 2024-06-01 13:47:26.459839 fdk_asgi-0.7.1/src/fdk_asgi/utils.py
+-rw-r--r--   0        0        0     8554 1970-01-01 00:00:00.000000 fdk_asgi-0.7.1/PKG-INFO
```

### Comparing `fdk_asgi-0.7.0/LICENSE` & `fdk_asgi-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fdk_asgi-0.7.0/README.md` & `fdk_asgi-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `fdk_asgi-0.7.0/pyproject.toml` & `fdk_asgi-0.7.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "fdk-asgi"
 requires-python = ">=3.8"
 
 [tool.poetry]
 name = "fdk-asgi"
-version = "0.7.0"
+version = "0.7.1"
 description = "An alternative FDK to easily run any ASGI application on OCI Functions behind an API Gateway."
 authors = ["Björn Reetz <git@bjoern-reetz.de>"]
 readme = "README.md"
 packages = [{include = "fdk_asgi", from = "src"}]
 
 [tool.poetry.scripts]
 fdk-asgi-serve = 'fdk_asgi.cli:app'
@@ -105,17 +105,14 @@
     "TRY",
     # perflint
     "PERF",
     # Ruff-specific rules
     "RUF",
 ]
 
-[tool.ruff.lint.pyupgrade]
-keep-runtime-typing = true
-
 [tool.ruff.per-file-ignores]
 "tests/**/test_*.py" = ["S101"]
 "tests/utils.py" = ["S101"]
 "src/fdk_asgi/testing.py" = ["S101"]
 "src/fdk_asgi/cli.py" = ["FBT", "ERA001"]
 
 [tool.commitizen]
```

### Comparing `fdk_asgi-0.7.0/src/fdk_asgi/app.py` & `fdk_asgi-0.7.1/src/fdk_asgi/app.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,23 @@
 from __future__ import annotations
 
 import logging
 from http import HTTPStatus
 from importlib.metadata import version
 
-from asgiref.typing import (
-    ASGI3Application,
-    ASGIReceiveCallable,
-    ASGISendCallable,
-    ASGISendEvent,
-    HTTPResponseBodyEvent,
-    HTTPResponseStartEvent,
-    HTTPScope,
-    Scope,
-)
 from httptools import parse_url
 
 from fdk_asgi.exceptions import (
     FnMiddlewareError,
     MethodNotAllowedError,
     MissingMethodError,
     MissingUrlError,
     PathNotFoundError,
 )
+from fdk_asgi.types import ASGIApp, Receive, Scope, Send
 from fdk_asgi.utils import get_client_addr, get_path_with_query_string
 
 FN_FDK_VERSION_HEADER = (
     b"fn-fdk-version",
     f"fdk-asgi/{version(__package__)}".encode(),
 )
 
@@ -44,51 +35,49 @@
 logger_access = logging.getLogger(f"{__package__}.access")
 
 
 class FnMiddleware:
     """A pure ASGI middleware, wrapping a regular ASGI application
     and translating Fn <-> REST."""
 
-    def __init__(self, app: ASGI3Application, prefix: str = ""):
+    def __init__(self, app: ASGIApp, prefix: str = "") -> None:
         self.app = app
         self.prefix = prefix
 
-    async def __call__(
-        self, scope: Scope, receive: ASGIReceiveCallable, send: ASGISendCallable
-    ) -> None:
+    async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         # leave all but HTTP connection scopes untouched
         # note that websockets are not supported by fn
         if scope["type"] != "http":
             return await self.app(scope, receive, send)
 
         try:
             mapped_scope = self._map_http_scope(scope)
         except FnMiddlewareError as exception:
             logger.critical(exception)
-            start_message: HTTPResponseStartEvent
-            start_message = {
-                "type": "http.response.start",
-                "status": exception.code,
-                "headers": [
-                    (b"content-type", b"text/plain"),
-                ],
-                "trailers": False,
-            }
-            await send(start_message)
-            body_message: HTTPResponseBodyEvent
-            body_message = {
-                "type": "http.response.body",
-                "body": str(exception).encode(),
-                "more_body": False,
-            }
-            await send(body_message)
+            await send(
+                {
+                    "type": "http.response.start",
+                    "status": exception.code,
+                    "headers": [
+                        (b"content-type", b"text/plain"),
+                    ],
+                    "trailers": False,
+                }
+            )
+            await send(
+                {
+                    "type": "http.response.body",
+                    "body": str(exception).encode(),
+                    "more_body": False,
+                }
+            )
             return
         await self.app(mapped_scope, receive, self._wrap_send(send, scope))
 
-    def _map_http_scope(self, scope: HTTPScope) -> HTTPScope:
+    def _map_http_scope(self, scope: Scope) -> Scope:
         """Transforms headers etc. sent by Fn/API Gateway
         so that ASGI apps can understand them."""
 
         # see https://asgi.readthedocs.io/en/latest/specs/www.html#http-connection-scope
 
         if scope["path"] != "/call":
             raise PathNotFoundError()
@@ -127,16 +116,16 @@
         # scope has precedence over environment variable
         scope["root_path"] = self.prefix
         scope["headers"] = http_headers
 
         return scope
 
     @staticmethod
-    def _wrap_send(send: ASGISendCallable, scope: HTTPScope) -> ASGISendCallable:
-        async def wrapped_send(message: ASGISendEvent) -> None:
+    def _wrap_send(send: Send, scope: Scope) -> Send:
+        async def wrapped_send(message: Scope) -> None:
             # only process messages of type=http.response.start,
             # leave message of other types untouched
             if message["type"] == "http.response.start":
                 new_headers = [
                     (key, value)
                     if key.lower() == b"content-type"
                     else (FN_HTTP_H_ + key, value)
```

### Comparing `fdk_asgi-0.7.0/src/fdk_asgi/cli.py` & `fdk_asgi-0.7.1/src/fdk_asgi/cli.py`

 * *Files identical despite different names*

### Comparing `fdk_asgi-0.7.0/src/fdk_asgi/exceptions.py` & `fdk_asgi-0.7.1/src/fdk_asgi/exceptions.py`

 * *Files identical despite different names*

### Comparing `fdk_asgi-0.7.0/src/fdk_asgi/types.py` & `fdk_asgi-0.7.1/src/fdk_asgi/types.py`

 * *Files identical despite different names*

### Comparing `fdk_asgi-0.7.0/src/fdk_asgi/utils.py` & `fdk_asgi-0.7.1/src/fdk_asgi/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import urllib.parse
 
-from asgiref.typing import WWWScope
+from fdk_asgi.types import Scope
 
 # Code taken from uvicorn.protocols.utils
 
 # Copyright © 2017-present, [Encode OSS Ltd](https://www.encode.io/).
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without
@@ -29,23 +29,21 @@
 # DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
 # SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
 # CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
 # OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 # OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 
-def get_client_addr(scope: WWWScope) -> str:
+def get_client_addr(scope: Scope) -> str:
     client = scope.get("client")
     if not client:
         return ""
-    # asgiref types scope["client"] as a Tuple[str, int],
-    # but the spec types it as an Iterable[Unicode string, int]
     return "{!s}:{:d}".format(*client)
 
 
-def get_path_with_query_string(scope: WWWScope) -> str:
+def get_path_with_query_string(scope: Scope) -> str:
     path_with_query_string = urllib.parse.quote(scope["path"])
     if scope["query_string"]:
         path_with_query_string = "{}?{}".format(
             path_with_query_string, scope["query_string"].decode("ascii")
         )
     return path_with_query_string
```

### Comparing `fdk_asgi-0.7.0/PKG-INFO` & `fdk_asgi-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fdk-asgi
-Version: 0.7.0
+Version: 0.7.1
 Summary: An alternative FDK to easily run any ASGI application on OCI Functions behind an API Gateway.
 Author: Björn Reetz
 Author-email: git@bjoern-reetz.de
 Requires-Python: >=3.8
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

