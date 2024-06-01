# Comparing `tmp/anydi-0.26.1.tar.gz` & `tmp/anydi-0.27.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anydi-0.26.1.tar", max compression
+gzip compressed data, was "anydi-0.27.0a0.tar", max compression
```

## Comparing `anydi-0.26.1.tar` & `anydi-0.27.0a0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.26.1/LICENSE
--rw-r--r--   0        0        0     3414 2024-05-08 13:39:48.509983 anydi-0.26.1/README.md
--rw-r--r--   0        0        0      584 2024-05-06 12:48:30.095677 anydi-0.26.1/anydi/__init__.py
--rw-r--r--   0        0        0    29246 2024-05-28 08:33:14.693463 anydi-0.26.1/anydi/_container.py
--rw-r--r--   0        0        0    10815 2024-05-28 05:51:36.811241 anydi-0.26.1/anydi/_context.py
--rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.26.1/anydi/_logger.py
--rw-r--r--   0        0        0     3675 2024-05-20 08:55:10.775071 anydi-0.26.1/anydi/_module.py
--rw-r--r--   0        0        0     6667 2024-05-08 08:36:20.512668 anydi-0.26.1/anydi/_scanner.py
--rw-r--r--   0        0        0     3434 2024-05-08 08:36:20.512936 anydi-0.26.1/anydi/_types.py
--rw-r--r--   0        0        0     3871 2024-05-20 11:14:22.992185 anydi-0.26.1/anydi/_utils.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.26.1/anydi/ext/__init__.py
--rw-r--r--   0        0        0      223 2024-05-08 13:39:48.511489 anydi-0.26.1/anydi/ext/django/__init__.py
--rw-r--r--   0        0        0      418 2024-05-08 13:39:48.512186 anydi-0.26.1/anydi/ext/django/_container.py
--rw-r--r--   0        0        0      844 2024-05-09 08:27:16.715250 anydi-0.26.1/anydi/ext/django/_settings.py
--rw-r--r--   0        0        0     3673 2024-05-09 08:27:16.715602 anydi-0.26.1/anydi/ext/django/_utils.py
--rw-r--r--   0        0        0     2866 2024-05-09 08:27:16.715954 anydi-0.26.1/anydi/ext/django/apps.py
--rw-r--r--   0        0        0      823 2024-05-08 13:39:48.513463 anydi-0.26.1/anydi/ext/django/middleware.py
--rw-r--r--   0        0        0      546 2024-05-08 13:39:48.513678 anydi-0.26.1/anydi/ext/django/ninja/__init__.py
--rw-r--r--   0        0        0     2696 2024-05-08 13:39:48.513886 anydi-0.26.1/anydi/ext/django/ninja/_operation.py
--rw-r--r--   0        0        0     2207 2024-05-09 08:27:16.716393 anydi-0.26.1/anydi/ext/django/ninja/_signature.py
--rw-r--r--   0        0        0     5305 2024-05-08 08:36:20.513818 anydi-0.26.1/anydi/ext/fastapi.py
--rw-r--r--   0        0        0     4043 2024-05-20 11:14:22.992471 anydi-0.26.1/anydi/ext/pytest_plugin.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.26.1/anydi/ext/starlette/__init__.py
--rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.26.1/anydi/ext/starlette/middleware.py
--rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.26.1/anydi/py.typed
--rw-r--r--   0        0        0     3107 2024-05-28 08:33:25.456457 anydi-0.26.1/pyproject.toml
--rw-r--r--   0        0        0     5160 1970-01-01 00:00:00.000000 anydi-0.26.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-02-14 18:16:50.284355 anydi-0.27.0a0/LICENSE
+-rw-r--r--   0        0        0     3414 2024-05-08 13:39:48.509983 anydi-0.27.0a0/README.md
+-rw-r--r--   0        0        0      584 2024-05-06 12:48:30.095677 anydi-0.27.0a0/anydi/__init__.py
+-rw-r--r--   0        0        0    29246 2024-05-28 08:33:14.693463 anydi-0.27.0a0/anydi/_container.py
+-rw-r--r--   0        0        0    10815 2024-05-28 05:51:36.811241 anydi-0.27.0a0/anydi/_context.py
+-rw-r--r--   0        0        0       52 2024-02-28 07:17:37.316042 anydi-0.27.0a0/anydi/_logger.py
+-rw-r--r--   0        0        0     3675 2024-05-20 08:55:10.775071 anydi-0.27.0a0/anydi/_module.py
+-rw-r--r--   0        0        0     6667 2024-05-08 08:36:20.512668 anydi-0.27.0a0/anydi/_scanner.py
+-rw-r--r--   0        0        0     3434 2024-05-08 08:36:20.512936 anydi-0.27.0a0/anydi/_types.py
+-rw-r--r--   0        0        0     3871 2024-05-20 11:14:22.992185 anydi-0.27.0a0/anydi/_utils.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317316 anydi-0.27.0a0/anydi/ext/__init__.py
+-rw-r--r--   0        0        0     2691 2024-06-01 19:29:10.118885 anydi-0.27.0a0/anydi/ext/_utils.py
+-rw-r--r--   0        0        0      223 2024-05-08 13:39:48.511489 anydi-0.27.0a0/anydi/ext/django/__init__.py
+-rw-r--r--   0        0        0      418 2024-05-08 13:39:48.512186 anydi-0.27.0a0/anydi/ext/django/_container.py
+-rw-r--r--   0        0        0      844 2024-05-09 08:27:16.715250 anydi-0.27.0a0/anydi/ext/django/_settings.py
+-rw-r--r--   0        0        0     3673 2024-05-09 08:27:16.715602 anydi-0.27.0a0/anydi/ext/django/_utils.py
+-rw-r--r--   0        0        0     2866 2024-05-09 08:27:16.715954 anydi-0.27.0a0/anydi/ext/django/apps.py
+-rw-r--r--   0        0        0      823 2024-05-08 13:39:48.513463 anydi-0.27.0a0/anydi/ext/django/middleware.py
+-rw-r--r--   0        0        0      546 2024-05-08 13:39:48.513678 anydi-0.27.0a0/anydi/ext/django/ninja/__init__.py
+-rw-r--r--   0        0        0     2696 2024-05-08 13:39:48.513886 anydi-0.27.0a0/anydi/ext/django/ninja/_operation.py
+-rw-r--r--   0        0        0     2207 2024-05-09 08:27:16.716393 anydi-0.27.0a0/anydi/ext/django/ninja/_signature.py
+-rw-r--r--   0        0        0     2896 2024-06-01 19:29:10.116875 anydi-0.27.0a0/anydi/ext/fastapi.py
+-rw-r--r--   0        0        0     1617 2024-06-01 19:29:10.113661 anydi-0.27.0a0/anydi/ext/faststream.py
+-rw-r--r--   0        0        0     4043 2024-05-20 11:14:22.992471 anydi-0.27.0a0/anydi/ext/pytest_plugin.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.317749 anydi-0.27.0a0/anydi/ext/starlette/__init__.py
+-rw-r--r--   0        0        0     1139 2024-03-04 13:20:12.099383 anydi-0.27.0a0/anydi/ext/starlette/middleware.py
+-rw-r--r--   0        0        0        0 2024-02-28 07:17:37.318091 anydi-0.27.0a0/anydi/py.typed
+-rw-r--r--   0        0        0     3132 2024-06-01 19:30:58.714030 anydi-0.27.0a0/pyproject.toml
+-rw-r--r--   0        0        0     5162 1970-01-01 00:00:00.000000 anydi-0.27.0a0/PKG-INFO
```

### Comparing `anydi-0.26.1/LICENSE` & `anydi-0.27.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/README.md` & `anydi-0.27.0a0/README.md`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/anydi/__init__.py` & `anydi-0.27.0a0/anydi/__init__.py`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/anydi/_container.py` & `anydi-0.27.0a0/anydi/_container.py`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/anydi/_context.py` & `anydi-0.27.0a0/anydi/_context.py`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/anydi/_module.py` & `anydi-0.27.0a0/anydi/_module.py`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/anydi/_scanner.py` & `anydi-0.27.0a0/anydi/_scanner.py`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/anydi/_types.py` & `anydi-0.27.0a0/anydi/_types.py`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/anydi/_utils.py` & `anydi-0.27.0a0/anydi/_utils.py`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/anydi/ext/django/_settings.py` & `anydi-0.27.0a0/anydi/ext/django/_settings.py`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/anydi/ext/django/_utils.py` & `anydi-0.27.0a0/anydi/ext/django/_utils.py`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/anydi/ext/django/apps.py` & `anydi-0.27.0a0/anydi/ext/django/apps.py`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/anydi/ext/django/middleware.py` & `anydi-0.27.0a0/anydi/ext/django/middleware.py`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/anydi/ext/django/ninja/__init__.py` & `anydi-0.27.0a0/anydi/ext/django/ninja/__init__.py`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/anydi/ext/django/ninja/_operation.py` & `anydi-0.27.0a0/anydi/ext/django/ninja/_operation.py`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/anydi/ext/django/ninja/_signature.py` & `anydi-0.27.0a0/anydi/ext/django/ninja/_signature.py`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/anydi/ext/pytest_plugin.py` & `anydi-0.27.0a0/anydi/ext/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/anydi/ext/starlette/middleware.py` & `anydi-0.27.0a0/anydi/ext/starlette/middleware.py`

 * *Files identical despite different names*

### Comparing `anydi-0.26.1/pyproject.toml` & `anydi-0.27.0a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anydi"
-version = "0.26.1"
+version = "0.27.0a0"
 description = "Dependency Injection library"
 authors = ["Anton Ruhlov <antonruhlov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/antonrh/anydi"
 keywords = ["dependency injection", "dependencies", "di", "async", "asyncio", "application"]
 classifiers = [
@@ -51,14 +51,15 @@
 pytest = "^8.1.0"
 pytest-cov = "^5.0.0"
 fastapi = "^0.100.0"
 httpx = "^0.26.0"
 django = "^4.2"
 django-ninja = "^1.1.0"
 pytest-django = "^4.8.0"
+faststream = "^0.5.10"
 
 [tool.poetry.plugins.pytest11]
 anydi = "anydi.ext.pytest_plugin"
 
 [tool.ruff]
 line-length = 88
```

### Comparing `anydi-0.26.1/PKG-INFO` & `anydi-0.27.0a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anydi
-Version: 0.26.1
+Version: 0.27.0a0
 Summary: Dependency Injection library
 Home-page: https://github.com/antonrh/anydi
 License: MIT
 Keywords: dependency injection,dependencies,di,async,asyncio,application
 Author: Anton Ruhlov
 Author-email: antonruhlov@gmail.com
 Requires-Python: >=3.8,<4.0
```

