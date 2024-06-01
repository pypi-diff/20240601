# Comparing `tmp/loadspinner-0.5.tar.gz` & `tmp/loadspinner-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loadspinner-0.5.tar", last modified: Sat May 18 04:56:41 2024, max compression
+gzip compressed data, was "loadspinner-0.6.tar", last modified: Sat Jun  1 10:26:39 2024, max compression
```

## Comparing `loadspinner-0.5.tar` & `loadspinner-0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-18 04:56:41.885583 loadspinner-0.5/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1061 2024-05-01 16:53:43.000000 loadspinner-0.5/LICENSE
--rw-r--r--   0 xyz       (1000) xyz       (1000)     2163 2024-05-18 04:56:41.885583 loadspinner-0.5/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1428 2024-05-18 04:53:05.000000 loadspinner-0.5/README.md
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-18 04:56:41.884584 loadspinner-0.5/loadspinner/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     3927 2024-05-18 04:34:14.000000 loadspinner-0.5/loadspinner/__init__.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)     5640 2024-05-12 08:59:13.000000 loadspinner-0.5/loadspinner/_spinners.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-18 04:56:41.885583 loadspinner-0.5/loadspinner/tools/
--rw-r--r--   0 xyz       (1000) xyz       (1000)      476 2024-04-29 18:02:17.000000 loadspinner-0.5/loadspinner/tools/demo.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      284 2024-05-08 23:02:02.000000 loadspinner-0.5/loadspinner/tools/preview.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-05-18 04:56:41.885583 loadspinner-0.5/loadspinner.egg-info/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     2163 2024-05-18 04:56:41.000000 loadspinner-0.5/loadspinner.egg-info/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      270 2024-05-18 04:56:41.000000 loadspinner-0.5/loadspinner.egg-info/SOURCES.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-05-18 04:56:41.000000 loadspinner-0.5/loadspinner.egg-info/dependency_links.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       12 2024-05-18 04:56:41.000000 loadspinner-0.5/loadspinner.egg-info/top_level.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-05-18 04:56:41.885583 loadspinner-0.5/setup.cfg
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1060 2024-05-01 07:28:17.000000 loadspinner-0.5/setup.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-01 10:26:39.128674 loadspinner-0.6/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1061 2024-05-01 16:53:43.000000 loadspinner-0.6/LICENSE
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     2163 2024-06-01 10:26:39.128674 loadspinner-0.6/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1428 2024-05-18 04:53:05.000000 loadspinner-0.6/README.md
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-01 10:26:39.125341 loadspinner-0.6/loadspinner/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     3927 2024-06-01 10:26:10.000000 loadspinner-0.6/loadspinner/__init__.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     5732 2024-06-01 10:23:47.000000 loadspinner-0.6/loadspinner/_spinners.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-01 10:26:39.125341 loadspinner-0.6/loadspinner/tools/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      476 2024-04-29 18:02:17.000000 loadspinner-0.6/loadspinner/tools/demo.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      284 2024-05-08 23:02:02.000000 loadspinner-0.6/loadspinner/tools/preview.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-01 10:26:39.128674 loadspinner-0.6/loadspinner.egg-info/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     2163 2024-06-01 10:26:39.000000 loadspinner-0.6/loadspinner.egg-info/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      270 2024-06-01 10:26:39.000000 loadspinner-0.6/loadspinner.egg-info/SOURCES.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-06-01 10:26:39.000000 loadspinner-0.6/loadspinner.egg-info/dependency_links.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       12 2024-06-01 10:26:39.000000 loadspinner-0.6/loadspinner.egg-info/top_level.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-06-01 10:26:39.128674 loadspinner-0.6/setup.cfg
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1060 2024-05-01 07:28:17.000000 loadspinner-0.6/setup.py
```

### Comparing `loadspinner-0.5/LICENSE` & `loadspinner-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `loadspinner-0.5/PKG-INFO` & `loadspinner-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadspinner
-Version: 0.5
+Version: 0.6
 Summary: a CLI based loading spinner.
 Home-page: https://github.com/xyzpw/loadspinner/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Keywords: loading,loader,progress,throbber,spinner
 Classifier: Programming Language :: Python :: 3
```

### Comparing `loadspinner-0.5/README.md` & `loadspinner-0.6/README.md`

 * *Files identical despite different names*

### Comparing `loadspinner-0.5/loadspinner/__init__.py` & `loadspinner-0.6/loadspinner/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 __all__ = [
     "Spinner",
     "functionSpinner",
     "makeSpinner",
 ]
 
-__version__ = "0.5"
+__version__ = "0.6"
 __description__ = "a CLI based loading spinner."
 __author__ = "xyzpw"
 __license__ = "MIT"
 
 class Spinner:
     def __init__(self, spinner_type: str = "classic"):
         self.spinner_type = spinner_type
```

### Comparing `loadspinner-0.5/loadspinner/_spinners.py` & `loadspinner-0.6/loadspinner/_spinners.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,14 +24,18 @@
         "frames": ["\u25CB", "\u25CF"],
         "interval": 0.5,
     },
     "blinkingSquare": {
         "frames": ["\u25A0", "\u25A1"],
         "interval": 0.5,
     },
+    "blinkingBenzene": {
+        "frames": ["\u232c", " "],
+        "interval": 0.5,
+    },
     "loadingCircle": {
         "frames": ["\u25D4", "\u25D1", "\u25D5", "\u25CF"],
         "interval": 1/3,
     },
     "spinningArrow": {
         "frames": [
             "\u2190",
```

### Comparing `loadspinner-0.5/loadspinner.egg-info/PKG-INFO` & `loadspinner-0.6/loadspinner.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loadspinner
-Version: 0.5
+Version: 0.6
 Summary: a CLI based loading spinner.
 Home-page: https://github.com/xyzpw/loadspinner/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Keywords: loading,loader,progress,throbber,spinner
 Classifier: Programming Language :: Python :: 3
```

### Comparing `loadspinner-0.5/setup.py` & `loadspinner-0.6/setup.py`

 * *Files identical despite different names*

