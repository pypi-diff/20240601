# Comparing `tmp/starlette_async_jinja-1.7.6.tar.gz` & `tmp/starlette_async_jinja-1.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_async_jinja-1.7.6.tar", last modified: Mon May 20 11:07:50 2024, max compression
+gzip compressed data, was "starlette_async_jinja-1.7.7.tar", last modified: Sat Jun  1 19:04:30 2024, max compression
```

## Comparing `starlette_async_jinja-1.7.6.tar` & `starlette_async_jinja-1.7.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 starlette_async_jinja-1.7.6/LICENSE
--rw-r--r--   0        0        0     1535 2024-02-26 07:33:43.485098 starlette_async_jinja-1.7.6/README.md
--rw-r--r--   0        0        0     2353 2024-05-20 11:07:50.729989 starlette_async_jinja-1.7.6/pyproject.toml
--rw-r--r--   0        0        0      211 2023-06-11 12:03:37.580220 starlette_async_jinja-1.7.6/starlette_async_jinja/__init__.py
--rw-r--r--   0        0        0     6344 2024-03-18 08:09:07.321729 starlette_async_jinja-1.7.6/starlette_async_jinja/responses.py
--rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 starlette_async_jinja-1.7.6/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 starlette_async_jinja-1.7.7/LICENSE
+-rw-r--r--   0        0        0     1535 2024-02-26 07:33:43.485098 starlette_async_jinja-1.7.7/README.md
+-rw-r--r--   0        0        0     2583 2024-06-01 19:04:30.879207 starlette_async_jinja-1.7.7/pyproject.toml
+-rw-r--r--   0        0        0      167 2024-06-01 19:04:03.152696 starlette_async_jinja-1.7.7/starlette_async_jinja/__init__.py
+-rw-r--r--   0        0        0     6223 2024-06-01 19:04:03.152779 starlette_async_jinja-1.7.7/starlette_async_jinja/responses.py
+-rw-r--r--   0        0        0     2466 1970-01-01 00:00:00.000000 starlette_async_jinja-1.7.7/PKG-INFO
```

### Comparing `starlette_async_jinja-1.7.6/LICENSE` & `starlette_async_jinja-1.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_async_jinja-1.7.6/README.md` & `starlette_async_jinja-1.7.7/README.md`

 * *Files identical despite different names*

### Comparing `starlette_async_jinja-1.7.6/pyproject.toml` & `starlette_async_jinja-1.7.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,34 +2,53 @@
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
@@ -37,34 +56,34 @@
 
 [tool.creosote]
 paths = [
     "starlette_async_jinja",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
+    "pdm",
     "pre-commit",
     "pytest",
     "pdm-bump",
-    "autotyping",
-    "pdm",
     "python-ulid",
+    "autotyping",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "starlette_async_jinja",
 ]
 skips = [
-    "B404",
+    "B603",
     "B113",
     "B403",
-    "B603",
+    "B404",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "starlette_async_jinja",
 ]
@@ -85,20 +104,20 @@
 [tool.codespell]
 skip = "*/data/*"
 quiet-level = 3
 ignore-words-list = "crate,uptodate"
 
 [project]
 name = "starlette-async-jinja"
-version = "1.7.6"
+version = "1.7.7"
 description = ""
 dependencies = [
     "starlette>=0.37.2",
     "jinja2>=3.1.4",
-    "jinja2-async-environment>=0.7.4",
+    "jinja2-async-environment>=0.7.6",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 classifiers = [
```

### Comparing `starlette_async_jinja-1.7.6/starlette_async_jinja/responses.py` & `starlette_async_jinja-1.7.7/starlette_async_jinja/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 import typing as t
 from functools import partial
 
 from aiopath import AsyncPath
 from jinja2.environment import Template
-from jinja2_async_environment import AsyncEnvironment
-from jinja2_async_environment import FileSystemLoader
+from jinja2_async_environment import AsyncEnvironment, FileSystemLoader
 from markupsafe import Markup
 from msgspec import json
 from starlette.background import BackgroundTask
 from starlette.datastructures import URL
-from starlette.responses import HTMLResponse
-from starlette.responses import JSONResponse
+from starlette.responses import HTMLResponse, JSONResponse
 from starlette.templating import pass_context
-from starlette.types import Receive
-from starlette.types import Scope
-from starlette.types import Send
+from starlette.types import Receive, Scope, Send
 
 
 class JsonResponse(JSONResponse):
     async def render(self, content: str) -> t.Any:  # type: ignore
         return json.encode(content)
```

### Comparing `starlette_async_jinja-1.7.6/PKG-INFO` & `starlette_async_jinja-1.7.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starlette-async-jinja
-Version: 1.7.6
+Version: 1.7.7
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: FastAPI
@@ -14,15 +14,15 @@
 Classifier: Development Status :: 4 - Beta
 Project-URL: Homepage, https://github.com/lesleslie/starlette-async-jinja
 Project-URL: Documentation, https://github.com/lesleslie/starlette-async-jinja
 Project-URL: Repository, https://github.com/lesleslie/starlette-async-jinja
 Requires-Python: >=3.12
 Requires-Dist: starlette>=0.37.2
 Requires-Dist: jinja2>=3.1.4
-Requires-Dist: jinja2-async-environment>=0.7.4
+Requires-Dist: jinja2-async-environment>=0.7.6
 Description-Content-Type: text/markdown
 
 # starlette-async-jinja
 
 [![Code style: crackerjack](https://img.shields.io/badge/code%20style-crackerjack-000042)](https://github.com/lesleslie/crackerjack)
 
 ### Jinja2 is_async template support for Starlette +
```

