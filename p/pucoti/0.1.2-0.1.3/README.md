# Comparing `tmp/pucoti-0.1.2.tar.gz` & `tmp/pucoti-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pucoti-0.1.2.tar", max compression
+gzip compressed data, was "pucoti-0.1.3.tar", max compression
```

## Comparing `pucoti-0.1.2.tar` & `pucoti-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,7 @@
--rw-r--r--   0        0        0    35149 2024-06-01 02:27:24.918336 pucoti-0.1.2/COPYING
--rw-r--r--   0        0        0     1222 2024-06-01 02:40:08.335744 pucoti-0.1.2/README.md
--rw-r--r--   0        0        0   332160 2024-05-31 23:23:46.882152 pucoti-0.1.2/bell.mp3
--rwxr-xr-x   0        0        0    12849 2024-06-01 02:26:57.467326 pucoti-0.1.2/pucoti.py
--rw-r--r--   0        0        0      616 2024-06-01 02:47:47.675989 pucoti-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1836 1970-01-01 00:00:00.000000 pucoti-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-06-01 02:27:24.918336 pucoti-0.1.3/COPYING
+-rw-r--r--   0        0        0     1222 2024-06-01 02:40:08.335744 pucoti-0.1.3/README.md
+-rw-r--r--   0        0        0    52252 2024-05-31 22:06:43.242609 pucoti-0.1.3/Wellbutrin.ttf
+-rw-r--r--   0        0        0   332160 2024-05-31 23:23:46.882152 pucoti-0.1.3/bell.mp3
+-rwxr-xr-x   0        0        0    12849 2024-06-01 02:26:57.467326 pucoti-0.1.3/pucoti.py
+-rw-r--r--   0        0        0      641 2024-06-01 02:49:19.526031 pucoti-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1836 1970-01-01 00:00:00.000000 pucoti-0.1.3/PKG-INFO
```

### Comparing `pucoti-0.1.2/COPYING` & `pucoti-0.1.3/COPYING`

 * *Files identical despite different names*

### Comparing `pucoti-0.1.2/README.md` & `pucoti-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pucoti-0.1.2/bell.mp3` & `pucoti-0.1.3/bell.mp3`

 * *Files identical despite different names*

### Comparing `pucoti-0.1.2/pucoti.py` & `pucoti-0.1.3/pucoti.py`

 * *Files identical despite different names*

### Comparing `pucoti-0.1.2/pyproject.toml` & `pucoti-0.1.3/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 [tool.poetry]
 name = "pucoti"
-version = "0.1.2"
+version = "0.1.3"
 description = "A Purposeful Countdown Timer"
 authors = ["ddorn <diego.dorn@free.fr>"]
 readme = "README.md"
 license = "GPL-3.0"
 homepage = "https://github.com/ddorn/pucoti"
 repository = "https://github.com/ddorn/pucoti"
 keywords = ["timer", "countdown", "pygame"]
 include = [
-    "./bell.mp3"
+    "./bell.mp3",
+    "./Wellbutrin.ttf",
 ]
 
 [tool.poetry.scripts]
 pucoti = "pucoti:app"
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `pucoti-0.1.2/PKG-INFO` & `pucoti-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pucoti
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Purposeful Countdown Timer
 Home-page: https://github.com/ddorn/pucoti
 License: GPL-3.0
 Keywords: timer,countdown,pygame
 Author: ddorn
 Author-email: diego.dorn@free.fr
 Requires-Python: >=3.12,<4.0
```

