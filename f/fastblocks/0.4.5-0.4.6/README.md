# Comparing `tmp/fastblocks-0.4.5.tar.gz` & `tmp/fastblocks-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastblocks-0.4.5.tar", last modified: Sat May 25 10:52:22 2024, max compression
+gzip compressed data, was "fastblocks-0.4.6.tar", last modified: Sat Jun  1 19:18:12 2024, max compression
```

## Comparing `fastblocks-0.4.5.tar` & `fastblocks-0.4.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 fastblocks-0.4.5/LICENSE
--rw-r--r--   0        0        0     1181 2024-05-20 05:59:48.364048 fastblocks-0.4.5/README.md
--rw-r--r--   0        0        0      256 2023-10-15 06:30:11.975198 fastblocks-0.4.5/fastblocks/Dockerfile
--rw-r--r--   0        0        0       80 2024-04-11 14:21:21.798764 fastblocks-0.4.5/fastblocks/__init__.py
--rw-r--r--   0        0        0      191 2024-01-19 13:43:05.790330 fastblocks-0.4.5/fastblocks/__main__.py
--rw-r--r--   0        0        0       61 2024-01-16 17:26:09.440085 fastblocks-0.4.5/fastblocks/actions/__init__.py
--rw-r--r--   0        0        0      407 2023-12-10 08:11:45.418815 fastblocks-0.4.5/fastblocks/actions/minify.py
--rw-r--r--   0        0        0        0 2024-02-08 21:10:42.403063 fastblocks-0.4.5/fastblocks/adapters/__init__.py
--rw-r--r--   0        0        0       62 2023-11-04 13:50:49.302945 fastblocks-0.4.5/fastblocks/adapters/admin/__init__.py
--rw-r--r--   0        0        0      211 2024-05-19 17:32:35.741801 fastblocks-0.4.5/fastblocks/adapters/admin/_base.py
--rw-r--r--   0        0        0     1286 2024-05-19 17:26:14.359108 fastblocks-0.4.5/fastblocks/adapters/admin/sqladmin.py
--rw-r--r--   0        0        0       60 2023-11-04 13:49:17.900293 fastblocks-0.4.5/fastblocks/adapters/app/__init__.py
--rw-r--r--   0        0        0      312 2024-02-24 10:37:18.246405 fastblocks-0.4.5/fastblocks/adapters/app/_base.py
--rw-r--r--   0        0        0     2778 2024-05-19 17:20:16.124648 fastblocks-0.4.5/fastblocks/adapters/app/main.py
--rw-r--r--   0        0        0       61 2024-01-24 11:58:07.288190 fastblocks-0.4.5/fastblocks/adapters/auth/__init__.py
--rw-r--r--   0        0        0     2021 2024-04-15 14:56:18.634894 fastblocks-0.4.5/fastblocks/adapters/auth/_base.py
--rw-r--r--   0        0        0        0 2024-01-24 11:37:07.550854 fastblocks-0.4.5/fastblocks/adapters/auth/basic.py
--rw-r--r--   0        0        0       62 2023-11-04 13:50:49.307356 fastblocks-0.4.5/fastblocks/adapters/fonts/__init__.py
--rw-r--r--   0        0        0      272 2024-04-15 14:56:18.661746 fastblocks-0.4.5/fastblocks/adapters/fonts/_base.py
--rw-r--r--   0        0        0     1230 2024-02-05 00:13:09.786522 fastblocks-0.4.5/fastblocks/adapters/fonts/google.py
--rw-r--r--   0        0        0       63 2024-02-07 11:18:36.653787 fastblocks-0.4.5/fastblocks/adapters/routes/__init__.py
--rw-r--r--   0        0        0      148 2024-02-07 21:14:30.088129 fastblocks-0.4.5/fastblocks/adapters/routes/_base.py
--rw-r--r--   0        0        0     3447 2024-05-19 17:32:35.905030 fastblocks-0.4.5/fastblocks/adapters/routes/default.py
--rw-r--r--   0        0        0        0 2023-09-24 01:35:41.606537 fastblocks-0.4.5/fastblocks/adapters/sitemap/__init__.py
--rw-r--r--   0        0        0      150 2024-04-15 14:56:18.653833 fastblocks-0.4.5/fastblocks/adapters/sitemap/_base.py
--rw-r--r--   0        0        0      883 2024-01-19 21:08:44.846106 fastblocks-0.4.5/fastblocks/adapters/sitemap/sitemap.py
--rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 fastblocks-0.4.5/fastblocks/adapters/style/__init__.py
--rw-r--r--   0        0        0     3812 2024-03-09 09:26:05.815486 fastblocks-0.4.5/fastblocks/adapters/style/_base.py
--rw-r--r--   0        0        0      118 2024-03-09 09:10:00.894074 fastblocks-0.4.5/fastblocks/adapters/style/bulma.py
--rw-r--r--   0        0        0       66 2023-11-04 13:50:49.311428 fastblocks-0.4.5/fastblocks/adapters/templates/__init__.py
--rw-r--r--   0        0        0      332 2024-03-03 09:36:13.663071 fastblocks-0.4.5/fastblocks/adapters/templates/_base.py
--rw-r--r--   0        0        0      758 2023-10-13 23:22:41.140320 fastblocks-0.4.5/fastblocks/adapters/templates/_filters.py
--rw-r--r--   0        0        0    14835 2024-05-25 09:45:13.843280 fastblocks-0.4.5/fastblocks/adapters/templates/jinja2.py
--rw-r--r--   0        0        0     3593 2024-04-11 14:20:14.047979 fastblocks-0.4.5/fastblocks/applications.py
--rw-r--r--   0        0        0     3056 2024-03-04 14:52:11.154976 fastblocks-0.4.5/fastblocks/middleware.py
--rw-r--r--   0        0        0      301 2024-03-11 12:41:28.420083 fastblocks-0.4.5/fastblocks/templates/admin/bootstrap/sqladmin/blocks/display_menu.html
--rw-r--r--   0        0        0     1127 2024-03-04 16:21:30.478801 fastblocks-0.4.5/fastblocks/templates/admin/bootstrap/sqladmin/blocks/menu_category.html
--rw-r--r--   0        0        0      422 2024-03-04 16:21:30.466542 fastblocks-0.4.5/fastblocks/templates/admin/bootstrap/sqladmin/blocks/menu_item.html
--rw-r--r--   0        0        0     1974 2024-05-25 10:44:19.709513 fastblocks-0.4.5/fastblocks/templates/admin/bootstrap/sqladmin/layout.html
--rw-r--r--   0        0        0     3052 2024-05-25 10:52:22.244897 fastblocks-0.4.5/pyproject.toml
--rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 fastblocks-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 fastblocks-0.4.6/LICENSE
+-rw-r--r--   0        0        0     1181 2024-05-20 05:59:48.364048 fastblocks-0.4.6/README.md
+-rw-r--r--   0        0        0      256 2023-10-15 06:30:11.975198 fastblocks-0.4.6/fastblocks/Dockerfile
+-rw-r--r--   0        0        0       80 2024-04-11 14:21:21.798764 fastblocks-0.4.6/fastblocks/__init__.py
+-rw-r--r--   0        0        0      191 2024-01-19 13:43:05.790330 fastblocks-0.4.6/fastblocks/__main__.py
+-rw-r--r--   0        0        0       61 2024-01-16 17:26:09.440085 fastblocks-0.4.6/fastblocks/actions/__init__.py
+-rw-r--r--   0        0        0      407 2023-12-10 08:11:45.418815 fastblocks-0.4.6/fastblocks/actions/minify.py
+-rw-r--r--   0        0        0        0 2024-02-08 21:10:42.403063 fastblocks-0.4.6/fastblocks/adapters/__init__.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:50:49.302945 fastblocks-0.4.6/fastblocks/adapters/admin/__init__.py
+-rw-r--r--   0        0        0      211 2024-05-19 17:32:35.741801 fastblocks-0.4.6/fastblocks/adapters/admin/_base.py
+-rw-r--r--   0        0        0     1277 2024-06-01 19:11:57.910642 fastblocks-0.4.6/fastblocks/adapters/admin/sqladmin.py
+-rw-r--r--   0        0        0       60 2023-11-04 13:49:17.900293 fastblocks-0.4.6/fastblocks/adapters/app/__init__.py
+-rw-r--r--   0        0        0      312 2024-06-01 19:11:57.909978 fastblocks-0.4.6/fastblocks/adapters/app/_base.py
+-rw-r--r--   0        0        0     2736 2024-06-01 19:11:57.912159 fastblocks-0.4.6/fastblocks/adapters/app/main.py
+-rw-r--r--   0        0        0       61 2024-01-24 11:58:07.288190 fastblocks-0.4.6/fastblocks/adapters/auth/__init__.py
+-rw-r--r--   0        0        0     1966 2024-06-01 19:11:57.910992 fastblocks-0.4.6/fastblocks/adapters/auth/_base.py
+-rw-r--r--   0        0        0        0 2024-01-24 11:37:07.550854 fastblocks-0.4.6/fastblocks/adapters/auth/basic.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:50:49.307356 fastblocks-0.4.6/fastblocks/adapters/fonts/__init__.py
+-rw-r--r--   0        0        0      272 2024-06-01 19:11:57.910733 fastblocks-0.4.6/fastblocks/adapters/fonts/_base.py
+-rw-r--r--   0        0        0     1211 2024-06-01 19:11:57.910790 fastblocks-0.4.6/fastblocks/adapters/fonts/google.py
+-rw-r--r--   0        0        0       63 2024-02-07 11:18:36.653787 fastblocks-0.4.6/fastblocks/adapters/routes/__init__.py
+-rw-r--r--   0        0        0      148 2024-06-01 19:11:57.909919 fastblocks-0.4.6/fastblocks/adapters/routes/_base.py
+-rw-r--r--   0        0        0     3271 2024-06-01 19:11:57.912016 fastblocks-0.4.6/fastblocks/adapters/routes/default.py
+-rw-r--r--   0        0        0        0 2023-09-24 01:35:41.606537 fastblocks-0.4.6/fastblocks/adapters/sitemap/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-15 14:56:18.653833 fastblocks-0.4.6/fastblocks/adapters/sitemap/_base.py
+-rw-r--r--   0        0        0      883 2024-01-19 21:08:44.846106 fastblocks-0.4.6/fastblocks/adapters/sitemap/sitemap.py
+-rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 fastblocks-0.4.6/fastblocks/adapters/style/__init__.py
+-rw-r--r--   0        0        0     3786 2024-06-01 19:11:57.910719 fastblocks-0.4.6/fastblocks/adapters/style/_base.py
+-rw-r--r--   0        0        0      118 2024-03-09 09:10:00.894074 fastblocks-0.4.6/fastblocks/adapters/style/bulma.py
+-rw-r--r--   0        0        0       66 2023-11-04 13:50:49.311428 fastblocks-0.4.6/fastblocks/adapters/templates/__init__.py
+-rw-r--r--   0        0        0      308 2024-06-01 19:11:57.911376 fastblocks-0.4.6/fastblocks/adapters/templates/_base.py
+-rw-r--r--   0        0        0      757 2024-06-01 19:11:57.911533 fastblocks-0.4.6/fastblocks/adapters/templates/_filters.py
+-rw-r--r--   0        0        0    14785 2024-06-01 19:14:38.200334 fastblocks-0.4.6/fastblocks/adapters/templates/jinja2.py
+-rw-r--r--   0        0        0     3478 2024-06-01 19:11:57.910636 fastblocks-0.4.6/fastblocks/applications.py
+-rw-r--r--   0        0        0     2974 2024-06-01 19:11:57.910733 fastblocks-0.4.6/fastblocks/middleware.py
+-rw-r--r--   0        0        0      301 2024-03-11 12:41:28.420083 fastblocks-0.4.6/fastblocks/templates/admin/bootstrap/sqladmin/blocks/display_menu.html
+-rw-r--r--   0        0        0     1127 2024-03-04 16:21:30.478801 fastblocks-0.4.6/fastblocks/templates/admin/bootstrap/sqladmin/blocks/menu_category.html
+-rw-r--r--   0        0        0      422 2024-03-04 16:21:30.466542 fastblocks-0.4.6/fastblocks/templates/admin/bootstrap/sqladmin/blocks/menu_item.html
+-rw-r--r--   0        0        0     1974 2024-05-25 10:44:19.709513 fastblocks-0.4.6/fastblocks/templates/admin/bootstrap/sqladmin/layout.html
+-rw-r--r--   0        0        0     3282 2024-06-01 19:18:12.523266 fastblocks-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0     2900 1970-01-01 00:00:00.000000 fastblocks-0.4.6/PKG-INFO
```

### Comparing `fastblocks-0.4.5/LICENSE` & `fastblocks-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.5/README.md` & `fastblocks-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.5/fastblocks/adapters/admin/sqladmin.py` & `fastblocks-0.4.6/fastblocks/adapters/admin/sqladmin.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import typing as t
 
 from acb.adapters import import_adapter
 from acb.depends import depends
-from fastblocks import FastBlocks
 from sqladmin import Admin as SqlAdmin
 from sqladmin.helpers import get_object_identifier
 from starlette.applications import Starlette
 from starlette_async_jinja import AsyncJinja2Templates
-from ._base import AdminBase
-from ._base import AdminBaseSettings
+from fastblocks import FastBlocks
+from ._base import AdminBase, AdminBaseSettings
 
 Templates = import_adapter()
 
 
 class AdminSettings(AdminBaseSettings): ...
 
 
@@ -23,15 +22,16 @@
     @depends.inject
     async def init(self) -> None:  # type: ignore
         ...
 
     @depends.inject
     @t.override
     def init_templating_engine(
-        self, templates: Templates = depends()  # type: ignore
+        self,
+        templates: Templates = depends(),  # type: ignore
     ) -> AsyncJinja2Templates:
         admin_templates = templates.admin
         admin_templates_env_globals = dict(
             min=min,
             zip=zip,
             admin=self,
             is_list=lambda x: isinstance(x, list),  # type: ignore
```

### Comparing `fastblocks-0.4.5/fastblocks/adapters/app/main.py` & `fastblocks-0.4.6/fastblocks/adapters/app/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import typing as t
 from contextlib import asynccontextmanager
 from time import perf_counter
 
-from acb.adapters import get_adapter
-from acb.adapters import import_adapter
+from acb.adapters import get_adapter, import_adapter
 from acb.config import Config
 from acb.depends import depends
 from fastblocks.applications import FastBlocks
-from ._base import AppBase
-from ._base import AppBaseSettings
+from ._base import AppBase, AppBaseSettings
 
 main_start = perf_counter()
 
 Logger = import_adapter()
 Cache = import_adapter()
 Auth = import_adapter()
 Models = import_adapter()
```

### Comparing `fastblocks-0.4.5/fastblocks/adapters/auth/_base.py` & `fastblocks-0.4.6/fastblocks/adapters/auth/_base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 import typing as t
-from abc import ABC
-from abc import abstractmethod
+from abc import ABC, abstractmethod
 from contextvars import ContextVar
 
 from acb.adapters import AdapterBase
 from acb.config import Settings
 from asgi_htmx import HtmxRequest
-from pydantic import EmailStr
-from pydantic import SecretStr
-from pydantic import UUID4
+from pydantic import UUID4, EmailStr, SecretStr
 from starlette.authentication import UnauthenticatedUser
 
 
 class AuthBaseSettings(Settings):
     token_id: t.Optional[str] = None
     session_cookie: t.Optional[str] = None
```

### Comparing `fastblocks-0.4.5/fastblocks/adapters/fonts/google.py` & `fastblocks-0.4.6/fastblocks/adapters/fonts/google.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 from acb.depends import depends
-
-from ._base import FontsBase
-from ._base import FontsBaseSettings
+from ._base import FontsBase, FontsBaseSettings
 
 
 class FontsSettings(FontsBaseSettings):
     primary: str = "Poppins"
     secondary: str = "Poppins"
     effects: dict[str, str] = {"primary": "3d-float"}
```

### Comparing `fastblocks-0.4.5/fastblocks/adapters/routes/default.py` & `fastblocks-0.4.6/fastblocks/adapters/routes/default.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,21 @@
 import typing as t
 from importlib import import_module
 
 from acb import base_path
-from acb.adapters import get_installed_adapters
-from acb.adapters import import_adapter
+from acb.adapters import get_installed_adapters, import_adapter
 from acb.debug import debug
 from acb.depends import depends
 from aiopath import AsyncPath
 from asgi_htmx import HtmxRequest
 from starlette.endpoints import HTTPEndpoint
-from starlette.responses import PlainTextResponse
-from starlette.responses import Response
-from starlette.routing import Host
-from starlette.routing import Mount
-from starlette.routing import Route
-from starlette.routing import Router
-from starlette.routing import WebSocketRoute
+from starlette.responses import PlainTextResponse, Response
+from starlette.routing import Host, Mount, Route, Router, WebSocketRoute
 from starlette_async_jinja import AsyncJinja2Templates
-from ._base import RoutesBase
-from ._base import RoutesBaseSettings
+from ._base import RoutesBase, RoutesBaseSettings
 
 Templates = import_adapter()
 
 base_routes_paths = [AsyncPath(base_path / "routes.py")]
 
 
 class RoutesSettings(RoutesBaseSettings): ...
@@ -31,15 +24,16 @@
 class Index(HTTPEndpoint):
     templates: Templates = depends()  # type: ignore
 
     async def get(self, request: HtmxRequest) -> Response:
         request.path_params["page"] = request.scope["path"].lstrip("/") or "home"
         debug(request.path_params.get("page"))
         return await self.templates.app.render_template(
-            request, "index.html"  # type: ignore
+            request,
+            "index.html",  # type: ignore
         )
 
 
 class Block(HTTPEndpoint):
     templates: Templates = depends()  # type: ignore
 
     async def get(self, request: HtmxRequest) -> Response:
```

### Comparing `fastblocks-0.4.5/fastblocks/adapters/sitemap/sitemap.py` & `fastblocks-0.4.6/fastblocks/adapters/sitemap/sitemap.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.5/fastblocks/adapters/style/_base.py` & `fastblocks-0.4.6/fastblocks/adapters/style/_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 from contextlib import closing
 from io import StringIO
 from string import hexdigits
 
-from acb.depends import depends
 from acb.actions.encode import load
-from acb.adapters import AdapterBase
-from acb.adapters import import_adapter
+from acb.adapters import AdapterBase, import_adapter
 from acb.config import Settings
 from acb.debug import debug
-from colour import web2hex  # type: ignore
-
+from acb.depends import depends
 from aiopath import AsyncPath
 from asgi_htmx import HtmxRequest
+from colour import web2hex  # type: ignore
 from fastblocks.actions.minify import minify
 
-
 Cache = import_adapter()
 Templates = import_adapter()
 
 
 class StyleBaseSettings(Settings): ...
```

### Comparing `fastblocks-0.4.5/fastblocks/adapters/templates/_filters.py` & `fastblocks-0.4.6/fastblocks/adapters/templates/_filters.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from urllib.parse import quote_plus
 
 from acb.config import Config
 from acb.depends import depends
-
 from fastblocks.actions import minify
 
 
 class Filters:
     templates = depends.get("templates")  # type: ignore
     config: Config = depends()  # type: ignore
```

### Comparing `fastblocks-0.4.5/fastblocks/adapters/templates/jinja2.py` & `fastblocks-0.4.6/fastblocks/adapters/templates/jinja2.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,31 +5,27 @@
 from importlib import import_module
 from importlib.util import find_spec
 from inspect import isclass
 from pathlib import Path
 from re import search
 
 from acb import base_path
-from acb.adapters import get_adapter
-from acb.adapters import import_adapter
+from acb.adapters import get_adapter, import_adapter
 from acb.config import Config
 from acb.debug import debug
 from acb.depends import depends
 from aiopath import AsyncPath
 from jinja2 import TemplateNotFound
+from jinja2.ext import Extension, i18n, loopcontrols
 from jinja2.ext import debug as jinja_debug
-from jinja2.ext import Extension
-from jinja2.ext import i18n
-from jinja2.ext import loopcontrols
 from jinja2_async_environment.bccache import AsyncRedisBytecodeCache
 from jinja2_async_environment.loaders import AsyncBaseLoader
 from pydantic import BaseModel
 from starlette_async_jinja import AsyncJinja2Templates
-from ._base import TemplatesBase
-from ._base import TemplatesBaseSettings
+from ._base import TemplatesBase, TemplatesBaseSettings
 
 Logger = import_adapter()
 Cache = import_adapter()
 Storage = import_adapter()
 Models = import_adapter()
 
 
@@ -292,15 +288,17 @@
         comment_start_string="[#",
         comment_end_string="#]",
     )
     globals: dict[str, t.Any] = {}
 
     @depends.inject
     def __init__(
-        self, models: Models = depends(), **data: t.Any  # type: ignore
+        self,
+        models: Models = depends(),  # type: ignore
+        **data: t.Any,  # type: ignore
     ) -> None:
         super().__init__(**data)
         self.globals["models"] = models
 
 
 class Templates(TemplatesBase):
     app: t.Optional[AsyncJinja2Templates] = None
@@ -373,18 +371,18 @@
             logger.debug(f"{loader.__class__.__name__} initialized")
 
     @staticmethod
     def get_attr(html: str, attr: str) -> str | None:
         parser = HTMLParser()
         parser.feed(html)
         soup = parser.get_starttag_text()
-        attr = f"{attr}="
+        _attr = f"{attr}="
         for s in soup.split():
-            if search(attr, s):
-                attr_value = s.replace(attr, "").strip('"')
+            if search(_attr, s):
+                attr_value = s.replace(_attr, "").strip('"')
                 return attr_value
 
     def filter(self, name: t.Optional[str] = None):
         def decorator(f: t.Callable[..., t.Any]):
             self.app.env.filters[name or f.__name__] = f
             self.admin.env.filters[name or f.__name__] = f
             return f
```

### Comparing `fastblocks-0.4.5/fastblocks/applications.py` & `fastblocks-0.4.6/fastblocks/applications.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,23 @@
 import logging
 import typing as t
 from platform import system
 
-from acb.adapters import import_adapter
-from acb.adapters import register_adapters
+from acb.adapters import import_adapter, register_adapters
 from acb.adapters.logger.loguru import InterceptHandler
 from acb.config import Config
 from acb.depends import depends
 from asgi_htmx import HtmxRequest
-from starception import add_link_template
-from starception import install_error_handler
-from starception import set_editor
+from starception import add_link_template, install_error_handler, set_editor
 from starlette.applications import Starlette
 from starlette.middleware import Middleware
 from starlette.middleware.errors import ServerErrorMiddleware
 from starlette.middleware.exceptions import ExceptionMiddleware
 from starlette.responses import Response
-from starlette.types import ASGIApp
-from starlette.types import ExceptionHandler
-from starlette.types import Lifespan
+from starlette.types import ASGIApp, ExceptionHandler, Lifespan
 from .middleware import middlewares
 
 register_adapters()
 
 Logger = import_adapter()
 
 AppType = t.TypeVar("AppType", bound="FastBlocks")
@@ -64,15 +59,16 @@
         for _logger in ("uvicorn", "uvicorn.access"):
             _logger = logging.getLogger(_logger)
             _logger.handlers.clear()
             _logger.handlers = [InterceptHandler()]
 
     @depends.inject
     def build_middleware_stack(
-        self, logger: Logger = depends()  # type: ignore
+        self,
+        logger: Logger = depends(),  # type: ignore
     ) -> ASGIApp:
         error_handler = None
         exception_handlers: dict[
             t.Any, t.Callable[[HtmxRequest, Exception], Response]
         ] = {}
         for key, value in self.exception_handlers.items():
             if key in (500, Exception):
```

### Comparing `fastblocks-0.4.5/fastblocks/middleware.py` & `fastblocks-0.4.6/fastblocks/middleware.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 from time import perf_counter
 
 from acb.adapters import import_adapter
 from acb.config import Config
 from acb.depends import depends
-
 from asgi_htmx import HtmxMiddleware
 from brotli_asgi import BrotliMiddleware
 from secure import Secure
 from starlette.applications import Starlette
 from starlette.datastructures import MutableHeaders
 from starlette.middleware import Middleware
 from starlette.middleware.sessions import SessionMiddleware
-from starlette.types import Message
-from starlette.types import Receive
-from starlette.types import Scope
-from starlette.types import Send
+from starlette.types import Message, Receive, Scope, Send
 from starlette_csrf.middleware import CSRFMiddleware
 
 Logger = import_adapter()
 
 secure_headers = Secure()
```

### Comparing `fastblocks-0.4.5/fastblocks/templates/admin/bootstrap/sqladmin/blocks/menu_category.html` & `fastblocks-0.4.6/fastblocks/templates/admin/bootstrap/sqladmin/blocks/menu_category.html`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.5/fastblocks/templates/admin/bootstrap/sqladmin/layout.html` & `fastblocks-0.4.6/fastblocks/templates/admin/bootstrap/sqladmin/layout.html`

 * *Files identical despite different names*

### Comparing `fastblocks-0.4.5/pyproject.toml` & `fastblocks-0.4.6/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fastblocks"
-version = "0.4.5"
+version = "0.4.6"
 description = "Starlette based app for the rapid delivery HTMX/Jinja template blocks"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
@@ -36,25 +36,25 @@
 ]
 readme = "README.md"
 dependencies = [
     "asgi-htmx>=0.1.0",
     "brotli-asgi>=1.4.0",
     "starlette-csrf>=3.0.0",
     "starception>=1.2.1",
-    "pydantic>=2.7.1",
+    "pydantic>=2.7.2",
     "pyfiglet>=1.0.2",
     "starlette>=0.37.2",
-    "uvicorn>=0.29.0",
+    "uvicorn>=0.30.0",
     "htmlmin>=0.1.12",
     "jsmin>=3.0.1",
     "libsass>=0.23.0",
     "aiohttp>=3.9.5",
-    "starlette-async-jinja>=1.7.5",
+    "starlette-async-jinja>=1.7.7",
     "secure>=0.3.0",
-    "acb[cache,requests,secret,storage]>=0.6.1",
+    "acb[cache,requests,secret,storage]>=0.6.3",
 ]
 
 [project.optional-dependencies]
 sitemap = [
     "asgi-sitemaps>=1.0.0",
 ]
 style = [
@@ -72,34 +72,53 @@
 config = [
     "python.use_venv",
     "true",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "crackerjack>=0.7.34",
+    "crackerjack>=0.8.3",
 ]
 
 [tool.ruff]
 line-length = 88
 target-version = "py312"
 fix = true
 show-fixes = true
 output-format = "full"
 
+[tool.ruff.format]
+docstring-code-format = true
+
 [tool.ruff.lint]
 ignore = [
     "F821",
+    "D100",
+    "D101",
+    "D102",
+    "D103",
+    "D104",
+    "D105",
+    "D106",
+    "D107",
+]
+extend-select = [
+    "I",
+    "C901",
+    "D",
 ]
 
 [tool.ruff.lint.isort]
-force-single-line = true
+no-lines-before = [
+    "first-party",
+    "local-folder",
+]
 
 [tool.ruff.lint.mccabe]
-max-complexity = 10
+max-complexity = 11
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
 
 [tool.black]
 target-version = [
     "py312",
@@ -107,37 +126,37 @@
 
 [tool.creosote]
 paths = [
     "fastblocks",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
-    "pytest",
-    "autotyping",
-    "libsass",
-    "pdm",
     "pdm-bump",
-    "phonenumbers",
-    "pre-commit",
     "pyfiglet",
+    "pdm",
+    "libsass",
+    "autotyping",
+    "pytest",
     "aiohttp",
+    "phonenumbers",
+    "pre-commit",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "fastblocks",
 ]
 skips = [
+    "B403",
+    "B603",
     "B113",
     "B404",
-    "B603",
-    "B403",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "fastblocks",
 ]
```

### Comparing `fastblocks-0.4.5/PKG-INFO` & `fastblocks-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastblocks
-Version: 0.4.5
+Version: 0.4.6
 Summary: Starlette based app for the rapid delivery HTMX/Jinja template blocks
 Keywords: starlette,htmx,jinja,httpx,fastapi,sqladmin,sqlmodel,pydantic,sqlalchemy,redis
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
@@ -18,25 +18,25 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Development Status :: 3 - Alpha
 Requires-Python: >=3.12
 Requires-Dist: asgi-htmx>=0.1.0
 Requires-Dist: brotli-asgi>=1.4.0
 Requires-Dist: starlette-csrf>=3.0.0
 Requires-Dist: starception>=1.2.1
-Requires-Dist: pydantic>=2.7.1
+Requires-Dist: pydantic>=2.7.2
 Requires-Dist: pyfiglet>=1.0.2
 Requires-Dist: starlette>=0.37.2
-Requires-Dist: uvicorn>=0.29.0
+Requires-Dist: uvicorn>=0.30.0
 Requires-Dist: htmlmin>=0.1.12
 Requires-Dist: jsmin>=3.0.1
 Requires-Dist: libsass>=0.23.0
 Requires-Dist: aiohttp>=3.9.5
-Requires-Dist: starlette-async-jinja>=1.7.5
+Requires-Dist: starlette-async-jinja>=1.7.7
 Requires-Dist: secure>=0.3.0
-Requires-Dist: acb[cache,requests,secret,storage]>=0.6.1
+Requires-Dist: acb[cache,requests,secret,storage]>=0.6.3
 Requires-Dist: asgi-sitemaps>=1.0.0; extra == "sitemap"
 Requires-Dist: beautifulsoup4>=4.12.3; extra == "style"
 Requires-Dist: tinycss2>=1.3.0; extra == "style"
 Requires-Dist: sqladmin>=0.17.0; extra == "admin"
 Provides-Extra: sitemap
 Provides-Extra: style
 Provides-Extra: admin
```

#### html2text {}

```diff
@@ -1,27 +1,27 @@
-Metadata-Version: 2.1 Name: fastblocks Version: 0.4.5 Summary: Starlette based
+Metadata-Version: 2.1 Name: fastblocks Version: 0.4.6 Summary: Starlette based
 app for the rapid delivery HTMX/Jinja template blocks Keywords:
 starlette,htmx,jinja,httpx,fastapi,sqladmin,sqlmodel,pydantic,sqlalchemy,redis
 Author-Email: lesleslie
 wedgwoodwebworks.com> Maintainer-Email: lesleslie
 wedgwoodwebworks.com> License: BSD-3-Clause Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3.12 Classifier: Topic ::
 Internet :: WWW/HTTP :: Dynamic Content Classifier: Topic :: Software
 Development :: Libraries :: Application Frameworks Classifier: Operating System
 :: OS Independent Classifier: Framework :: Pydantic Classifier: Framework ::
 Pydantic :: 2 Classifier: Framework :: AsyncIO Classifier: Typing :: Typed
 Classifier: License :: OSI Approved :: BSD License Classifier: Development
 Status :: 3 - Alpha Requires-Python: >=3.12 Requires-Dist: asgi-htmx>=0.1.0
 Requires-Dist: brotli-asgi>=1.4.0 Requires-Dist: starlette-csrf>=3.0.0
-Requires-Dist: starception>=1.2.1 Requires-Dist: pydantic>=2.7.1 Requires-Dist:
-pyfiglet>=1.0.2 Requires-Dist: starlette>=0.37.2 Requires-Dist: uvicorn>=0.29.0
+Requires-Dist: starception>=1.2.1 Requires-Dist: pydantic>=2.7.2 Requires-Dist:
+pyfiglet>=1.0.2 Requires-Dist: starlette>=0.37.2 Requires-Dist: uvicorn>=0.30.0
 Requires-Dist: htmlmin>=0.1.12 Requires-Dist: jsmin>=3.0.1 Requires-Dist:
 libsass>=0.23.0 Requires-Dist: aiohttp>=3.9.5 Requires-Dist: starlette-async-
-jinja>=1.7.5 Requires-Dist: secure>=0.3.0 Requires-Dist: acb
-[cache,requests,secret,storage]>=0.6.1 Requires-Dist: asgi-sitemaps>=1.0.0;
+jinja>=1.7.7 Requires-Dist: secure>=0.3.0 Requires-Dist: acb
+[cache,requests,secret,storage]>=0.6.3 Requires-Dist: asgi-sitemaps>=1.0.0;
 extra == "sitemap" Requires-Dist: beautifulsoup4>=4.12.3; extra == "style"
 Requires-Dist: tinycss2>=1.3.0; extra == "style" Requires-Dist:
 sqladmin>=0.17.0; extra == "admin" Provides-Extra: sitemap Provides-Extra:
 style Provides-Extra: admin Description-Content-Type: text/markdown
       [https://drive.google.com/uc?id=1pMUqyvgMkhGYoLz3jBibZDl3J63HEcCC]
 # FastBlocks [![Code style: crackerjack](https://img.shields.io/badge/
 code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
```

