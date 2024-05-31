# Comparing `tmp/display_colors-1.0.3.tar.gz` & `tmp/display_colors-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "display_colors-1.0.3.tar", max compression
+gzip compressed data, was "display_colors-1.0.4.tar", max compression
```

## Comparing `display_colors-1.0.3.tar` & `display_colors-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11356 2024-04-05 11:48:59.515054 display_colors-1.0.3/LICENSE
--rw-r--r--   0        0        0     8784 2024-05-28 21:37:05.940378 display_colors-1.0.3/README.md
--rw-r--r--   0        0        0     1052 2024-05-28 21:37:05.941680 display_colors-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-22 01:43:36.634637 display_colors-1.0.3/src/display_colors/__init__.py
--rw-r--r--   0        0        0    17745 2024-05-28 21:37:05.943169 display_colors-1.0.3/src/display_colors/__main__.py
--rw-r--r--   0        0        0     1014 2024-05-28 21:37:05.946111 display_colors-1.0.3/src/display_colors/cell.py
--rw-r--r--   0        0        0     1695 2024-05-28 21:37:05.949952 display_colors-1.0.3/src/display_colors/cmd/effects.py
--rw-r--r--   0        0        0     9431 2024-05-28 21:37:05.952168 display_colors-1.0.3/src/display_colors/cmd/eight_bit.py
--rw-r--r--   0        0        0     6171 2024-05-28 21:37:05.953274 display_colors-1.0.3/src/display_colors/cmd/four_bit.py
--rw-r--r--   0        0        0     1546 2024-05-28 21:37:05.953935 display_colors-1.0.3/src/display_colors/const.py
--rw-r--r--   0        0        0      389 2024-05-28 21:37:05.954644 display_colors-1.0.3/src/display_colors/gen.py
--rw-r--r--   0        0        0     3607 2024-05-28 21:37:05.955802 display_colors-1.0.3/src/display_colors/init.py
--rw-r--r--   0        0        0      221 2024-05-28 21:37:05.957990 display_colors-1.0.3/src/display_colors/math.py
--rw-r--r--   0        0        0     9795 1970-01-01 00:00:00.000000 display_colors-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-04-05 11:48:59.515054 display_colors-1.0.4/LICENSE
+-rw-r--r--   0        0        0     8786 2024-05-31 21:53:52.312137 display_colors-1.0.4/README.md
+-rw-r--r--   0        0        0     1052 2024-05-31 22:00:43.530384 display_colors-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-22 01:43:36.634637 display_colors-1.0.4/src/display_colors/__init__.py
+-rw-r--r--   0        0        0     1363 2024-05-31 21:55:40.742534 display_colors-1.0.4/src/display_colors/__main__.py
+-rw-r--r--   0        0        0     1014 2024-05-28 21:37:05.946111 display_colors-1.0.4/src/display_colors/cell.py
+-rw-r--r--   0        0        0     1695 2024-05-28 21:37:05.949952 display_colors-1.0.4/src/display_colors/cmd/effects.py
+-rw-r--r--   0        0        0     5133 2024-05-31 21:46:41.698045 display_colors-1.0.4/src/display_colors/cmd/eight_bit.py
+-rw-r--r--   0        0        0     6171 2024-05-28 21:37:05.953274 display_colors-1.0.4/src/display_colors/cmd/four_bit.py
+-rw-r--r--   0        0        0     1546 2024-05-28 21:37:05.953935 display_colors-1.0.4/src/display_colors/const.py
+-rw-r--r--   0        0        0      155 2024-05-31 21:47:46.520665 display_colors-1.0.4/src/display_colors/gen.py
+-rw-r--r--   0        0        0     3607 2024-05-28 21:37:05.955802 display_colors-1.0.4/src/display_colors/init.py
+-rw-r--r--   0        0        0      221 2024-05-28 21:37:05.957990 display_colors-1.0.4/src/display_colors/math.py
+-rw-r--r--   0        0        0     9797 1970-01-01 00:00:00.000000 display_colors-1.0.4/PKG-INFO
```

### Comparing `display_colors-1.0.3/LICENSE` & `display_colors-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `display_colors-1.0.3/README.md` & `display_colors-1.0.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 (.venv) python -m pip   install display-colors  // Install
 (.venv) python -m pip uninstall display-colors  // Uninstall
 ```
 
 ### Use
 
 ```
-(.venv) display-colors [--help|--version] COMMAND [OPTIONS]
+(.venv) display-colors [--help | --version] COMMAND [OPTIONS]
 ```
 
 COMMAND: 4-bit | 8-bit | effects
 
 OPTIONS vary depending on the command; do `display-colors COMMAND --help` to list them
 
 ## Features
```

### Comparing `display_colors-1.0.3/pyproject.toml` & `display_colors-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "display-colors"
-version = "1.0.3"
+version = "1.0.4"
 description = "Shows the 4-bit color and display effect capabilities of a terminal emulator"
 authors     = ["Joe Rodrigue <joe.rodrigue@gmail.com>"]
 maintainers = ["Joe Rodrigue <joe.rodrigue@gmail.com>"]
 repository  = "https://github.com/JoeRodrigue/display-colors"
 readme      = "README.md"
 classifiers = [
 	"License :: OSI Approved :: Apache Software License",
```

### Comparing `display_colors-1.0.3/src/display_colors/cell.py` & `display_colors-1.0.4/src/display_colors/cell.py`

 * *Files identical despite different names*

### Comparing `display_colors-1.0.3/src/display_colors/cmd/effects.py` & `display_colors-1.0.4/src/display_colors/cmd/effects.py`

 * *Files identical despite different names*

### Comparing `display_colors-1.0.3/src/display_colors/cmd/four_bit.py` & `display_colors-1.0.4/src/display_colors/cmd/four_bit.py`

 * *Files identical despite different names*

### Comparing `display_colors-1.0.3/src/display_colors/const.py` & `display_colors-1.0.4/src/display_colors/const.py`

 * *Files identical despite different names*

### Comparing `display_colors-1.0.3/src/display_colors/init.py` & `display_colors-1.0.4/src/display_colors/init.py`

 * *Files identical despite different names*

### Comparing `display_colors-1.0.3/PKG-INFO` & `display_colors-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: display-colors
-Version: 1.0.3
+Version: 1.0.4
 Summary: Shows the 4-bit color and display effect capabilities of a terminal emulator
 Home-page: https://github.com/JoeRodrigue/display-colors
 Keywords: color,terminal,emulator,SGR,ECMA-48
 Author: Joe Rodrigue
 Author-email: joe.rodrigue@gmail.com
 Maintainer: Joe Rodrigue
 Maintainer-email: joe.rodrigue@gmail.com
@@ -51,15 +51,15 @@
 (.venv) python -m pip   install display-colors  // Install
 (.venv) python -m pip uninstall display-colors  // Uninstall
 ```
 
 ### Use
 
 ```
-(.venv) display-colors [--help|--version] COMMAND [OPTIONS]
+(.venv) display-colors [--help | --version] COMMAND [OPTIONS]
 ```
 
 COMMAND: 4-bit | 8-bit | effects
 
 OPTIONS vary depending on the command; do `display-colors COMMAND --help` to list them
 
 ## Features
```

