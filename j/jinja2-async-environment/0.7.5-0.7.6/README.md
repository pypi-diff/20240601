# Comparing `tmp/jinja2_async_environment-0.7.5.tar.gz` & `tmp/jinja2_async_environment-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jinja2_async_environment-0.7.5.tar", last modified: Mon May 20 11:02:56 2024, max compression
+gzip compressed data, was "jinja2_async_environment-0.7.6.tar", last modified: Sat Jun  1 18:56:41 2024, max compression
```

## Comparing `jinja2_async_environment-0.7.5.tar` & `jinja2_async_environment-0.7.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1518 2023-04-29 16:12:44.541343 jinja2_async_environment-0.7.5/LICENSE
--rw-r--r--   0        0        0      256 2023-08-18 15:51:25.740188 jinja2_async_environment-0.7.5/README.md
--rw-r--r--   0        0        0      497 2023-06-08 14:36:19.764543 jinja2_async_environment-0.7.5/jinja2_async_environment/__init__.py
--rw-r--r--   0        0        0     1419 2024-03-03 12:44:33.505857 jinja2_async_environment-0.7.5/jinja2_async_environment/bccache.py
--rw-r--r--   0        0        0     4669 2024-03-03 08:37:52.586610 jinja2_async_environment-0.7.5/jinja2_async_environment/compiler.py
--rw-r--r--   0        0        0     3524 2024-03-03 13:52:16.395020 jinja2_async_environment-0.7.5/jinja2_async_environment/environment.py
--rw-r--r--   0        0        0     8520 2024-03-03 12:44:33.500636 jinja2_async_environment-0.7.5/jinja2_async_environment/loaders.py
--rw-r--r--   0        0        0     2087 2024-05-20 11:02:56.493043 jinja2_async_environment-0.7.5/pyproject.toml
--rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 jinja2_async_environment-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1518 2023-04-29 16:12:44.541343 jinja2_async_environment-0.7.6/LICENSE
+-rw-r--r--   0        0        0      256 2023-08-18 15:51:25.740188 jinja2_async_environment-0.7.6/README.md
+-rw-r--r--   0        0        0      426 2024-06-01 18:55:32.693249 jinja2_async_environment-0.7.6/jinja2_async_environment/__init__.py
+-rw-r--r--   0        0        0     1419 2024-03-03 12:44:33.505857 jinja2_async_environment-0.7.6/jinja2_async_environment/bccache.py
+-rw-r--r--   0        0        0     4615 2024-06-01 18:55:32.693404 jinja2_async_environment-0.7.6/jinja2_async_environment/compiler.py
+-rw-r--r--   0        0        0     3466 2024-06-01 18:55:32.693559 jinja2_async_environment-0.7.6/jinja2_async_environment/environment.py
+-rw-r--r--   0        0        0     8520 2024-03-03 12:44:33.500636 jinja2_async_environment-0.7.6/jinja2_async_environment/loaders.py
+-rw-r--r--   0        0        0     2317 2024-06-01 18:56:41.139410 jinja2_async_environment-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0      909 1970-01-01 00:00:00.000000 jinja2_async_environment-0.7.6/PKG-INFO
```

### Comparing `jinja2_async_environment-0.7.5/LICENSE` & `jinja2_async_environment-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.7.5/jinja2_async_environment/bccache.py` & `jinja2_async_environment-0.7.6/jinja2_async_environment/bccache.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.7.5/jinja2_async_environment/compiler.py` & `jinja2_async_environment-0.7.6/jinja2_async_environment/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 import typing as t
 
 from jinja2 import nodes
-from jinja2.compiler import CodeGenerator
-from jinja2.compiler import CompilerExit
-from jinja2.compiler import Frame
+from jinja2.compiler import CodeGenerator, CompilerExit, Frame
 
 
 class AsyncCodeGenerator(CodeGenerator):
     def visit_Block(self, node: nodes.Block, frame: Frame) -> None:
         level = 0
         if frame.toplevel:
             if self.has_known_extends:
```

### Comparing `jinja2_async_environment-0.7.5/jinja2_async_environment/environment.py` & `jinja2_async_environment-0.7.6/jinja2_async_environment/environment.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import typing as t
 from contextlib import suppress
 from weakref import ref
 
 from jinja2 import Environment
 from jinja2.environment import Template
-from jinja2.exceptions import TemplateNotFound
-from jinja2.exceptions import TemplatesNotFound
-from jinja2.exceptions import UndefinedError
+from jinja2.exceptions import TemplateNotFound, TemplatesNotFound, UndefinedError
 from jinja2.runtime import Undefined
 from jinja2.utils import internalcode
 from .compiler import AsyncCodeGenerator
 
 
 class AsyncEnvironment(Environment):
     code_generator_class: t.Any = AsyncCodeGenerator
```

### Comparing `jinja2_async_environment-0.7.5/jinja2_async_environment/loaders.py` & `jinja2_async_environment-0.7.6/jinja2_async_environment/loaders.py`

 * *Files identical despite different names*

### Comparing `jinja2_async_environment-0.7.5/pyproject.toml` & `jinja2_async_environment-0.7.6/pyproject.toml`

 * *Files 10% similar despite different names*

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
@@ -37,33 +56,33 @@
 
 [tool.creosote]
 paths = [
     "jinja2_async_environment",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
+    "pre-commit",
     "autotyping",
-    "pytest",
     "pdm",
-    "pre-commit",
     "pdm-bump",
+    "pytest",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "jinja2_async_environment",
 ]
 skips = [
-    "B603",
-    "B403",
     "B113",
+    "B603",
     "B404",
+    "B403",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "jinja2_async_environment",
 ]
@@ -84,15 +103,15 @@
 [tool.codespell]
 skip = "*/data/*"
 quiet-level = 3
 ignore-words-list = "crate,uptodate"
 
 [project]
 name = "jinja2-async-environment"
-version = "0.7.5"
+version = "0.7.6"
 description = ""
 dependencies = [
     "jinja2>=3.1.4",
     "redis>=5.0.4",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
```

### Comparing `jinja2_async_environment-0.7.5/PKG-INFO` & `jinja2_async_environment-0.7.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jinja2-async-environment
-Version: 0.7.5
+Version: 0.7.6
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Operating System :: OS Independent
 Classifier: Framework :: FastAPI
```

