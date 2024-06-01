# Comparing `tmp/eventum_cli-1.0.3.tar.gz` & `tmp/eventum_cli-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventum_cli-1.0.3.tar", max compression
+gzip compressed data, was "eventum_cli-1.0.4.tar", max compression
```

## Comparing `eventum_cli-1.0.3.tar` & `eventum_cli-1.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    11357 2024-05-27 16:38:37.957612 eventum_cli-1.0.3/LICENSE
--rw-r--r--   0        0        0       48 2024-05-27 16:38:37.957612 eventum_cli-1.0.3/README.md
--rw-r--r--   0        0        0        0 2024-05-27 16:42:27.537551 eventum_cli-1.0.3/eventum_cli/__init__.py
--rw-r--r--   0        0        0     5069 2024-05-31 18:13:28.547724 eventum_cli-1.0.3/eventum_cli/__main__.py
--rw-r--r--   0        0        0     3645 2024-05-29 10:18:47.654317 eventum_cli-1.0.3/eventum_cli/config_finalizer.py
--rw-r--r--   0        0        0     2044 2024-05-30 17:25:52.683877 eventum_cli-1.0.3/eventum_cli/logging_config.py
--rw-r--r--   0        0        0        0 2024-05-27 19:10:59.623431 eventum_cli-1.0.3/eventum_cli/py.typed
--rw-r--r--   0        0        0      747 2024-05-28 19:57:23.878268 eventum_cli-1.0.3/eventum_cli/validation_prettier.py
--rw-r--r--   0        0        0     1333 2024-05-31 19:34:41.947830 eventum_cli-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1404 1970-01-01 00:00:00.000000 eventum_cli-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-27 16:38:37.957612 eventum_cli-1.0.4/LICENSE
+-rw-r--r--   0        0        0       48 2024-05-27 16:38:37.957612 eventum_cli-1.0.4/README.md
+-rw-r--r--   0        0        0        0 2024-05-27 16:42:27.537551 eventum_cli-1.0.4/eventum_cli/__init__.py
+-rw-r--r--   0        0        0     5069 2024-05-31 18:13:28.547724 eventum_cli-1.0.4/eventum_cli/__main__.py
+-rw-r--r--   0        0        0     3645 2024-05-29 10:18:47.654317 eventum_cli-1.0.4/eventum_cli/config_finalizer.py
+-rw-r--r--   0        0        0     2044 2024-05-30 17:25:52.683877 eventum_cli-1.0.4/eventum_cli/logging_config.py
+-rw-r--r--   0        0        0        0 2024-05-27 19:10:59.623431 eventum_cli-1.0.4/eventum_cli/py.typed
+-rw-r--r--   0        0        0      747 2024-05-28 19:57:23.878268 eventum_cli-1.0.4/eventum_cli/validation_prettier.py
+-rw-r--r--   0        0        0     1333 2024-05-31 20:03:45.937420 eventum_cli-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1404 1970-01-01 00:00:00.000000 eventum_cli-1.0.4/PKG-INFO
```

### Comparing `eventum_cli-1.0.3/LICENSE` & `eventum_cli-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eventum_cli-1.0.3/eventum_cli/__main__.py` & `eventum_cli-1.0.4/eventum_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `eventum_cli-1.0.3/eventum_cli/config_finalizer.py` & `eventum_cli-1.0.4/eventum_cli/config_finalizer.py`

 * *Files identical despite different names*

### Comparing `eventum_cli-1.0.3/eventum_cli/logging_config.py` & `eventum_cli-1.0.4/eventum_cli/logging_config.py`

 * *Files identical despite different names*

### Comparing `eventum_cli-1.0.3/eventum_cli/validation_prettier.py` & `eventum_cli-1.0.4/eventum_cli/validation_prettier.py`

 * *Files identical despite different names*

### Comparing `eventum_cli-1.0.3/pyproject.toml` & `eventum_cli-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventum-cli"
-version = "1.0.3"
+version = "1.0.4"
 description = "Command line interface for Eventum"
 license = "Apache-2.0"
 authors = ["Nikita Reznikov <nikita.reznikov.public@mail.ru>"]
 readme = "README.md"
 repository = "https://github.com/Eventum-Generatives/EventumCLI"
 documentation = "https://eventum-generatives.github.io/Website/"
 keywords = ["generator", "testing", "data", "cli"]
```

### Comparing `eventum_cli-1.0.3/PKG-INFO` & `eventum_cli-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventum-cli
-Version: 1.0.3
+Version: 1.0.4
 Summary: Command line interface for Eventum
 Home-page: https://github.com/Eventum-Generatives/EventumCLI
 License: Apache-2.0
 Keywords: generator,testing,data,cli
 Author: Nikita Reznikov
 Author-email: nikita.reznikov.public@mail.ru
 Requires-Python: >=3.11,<4.0
```

