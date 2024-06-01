# Comparing `tmp/sigmacode-0.0.5.tar.gz` & `tmp/sigmacode-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmacode-0.0.5.tar", last modified: Sat Jun  1 11:14:28 2024, max compression
+gzip compressed data, was "sigmacode-0.0.6.tar", last modified: Sat Jun  1 11:17:09 2024, max compression
```

## Comparing `sigmacode-0.0.5.tar` & `sigmacode-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 11:14:28.606625 sigmacode-0.0.5/
--rw-rw-rw-   0        0        0     1092 2024-06-01 10:46:23.000000 sigmacode-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      871 2024-06-01 11:14:28.599543 sigmacode-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0       87 2024-06-01 10:47:51.000000 sigmacode-0.0.5/README.md
--rw-rw-rw-   0        0        0      963 2024-06-01 10:50:59.000000 sigmacode-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       16 2024-05-31 19:24:35.000000 sigmacode-0.0.5/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 11:14:28.607575 sigmacode-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-01 11:14:28.508625 sigmacode-0.0.5/sigmacode/
--rw-rw-rw-   0        0        0       63 2024-06-01 11:14:00.000000 sigmacode-0.0.5/sigmacode/__init__.py
--rw-rw-rw-   0        0        0      800 2024-06-01 11:13:56.000000 sigmacode-0.0.5/sigmacode/color.py
--rw-rw-rw-   0        0        0      574 2024-06-01 10:57:21.000000 sigmacode-0.0.5/sigmacode/terminal.py
-drwxrwxrwx   0        0        0        0 2024-06-01 11:14:28.595580 sigmacode-0.0.5/sigmacode.egg-info/
--rw-rw-rw-   0        0        0      871 2024-06-01 11:14:28.000000 sigmacode-0.0.5/sigmacode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2024-06-01 11:14:28.000000 sigmacode-0.0.5/sigmacode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 11:14:28.000000 sigmacode-0.0.5/sigmacode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-06-01 11:14:28.000000 sigmacode-0.0.5/sigmacode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-06-01 11:14:28.000000 sigmacode-0.0.5/sigmacode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 11:17:09.934399 sigmacode-0.0.6/
+-rw-rw-rw-   0        0        0     1092 2024-06-01 10:46:23.000000 sigmacode-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      871 2024-06-01 11:17:09.923398 sigmacode-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       87 2024-06-01 10:47:51.000000 sigmacode-0.0.6/README.md
+-rw-rw-rw-   0        0        0      963 2024-06-01 10:50:59.000000 sigmacode-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       16 2024-05-31 19:24:35.000000 sigmacode-0.0.6/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 11:17:09.936401 sigmacode-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-01 11:17:09.760426 sigmacode-0.0.6/sigmacode/
+-rw-rw-rw-   0        0        0       63 2024-06-01 11:16:38.000000 sigmacode-0.0.6/sigmacode/__init__.py
+-rw-rw-rw-   0        0        0      104 2024-06-01 11:16:34.000000 sigmacode-0.0.6/sigmacode/color.py
+-rw-rw-rw-   0        0        0      574 2024-06-01 10:57:21.000000 sigmacode-0.0.6/sigmacode/terminal.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:17:09.907401 sigmacode-0.0.6/sigmacode.egg-info/
+-rw-rw-rw-   0        0        0      871 2024-06-01 11:17:09.000000 sigmacode-0.0.6/sigmacode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2024-06-01 11:17:09.000000 sigmacode-0.0.6/sigmacode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 11:17:09.000000 sigmacode-0.0.6/sigmacode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-06-01 11:17:09.000000 sigmacode-0.0.6/sigmacode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-01 11:17:09.000000 sigmacode-0.0.6/sigmacode.egg-info/top_level.txt
```

### Comparing `sigmacode-0.0.5/LICENSE` & `sigmacode-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmacode-0.0.5/PKG-INFO` & `sigmacode-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmacode
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python Library for real sigmas!
 Author: codestantin
 License: MIT
 Project-URL: GitHub, https://github.com/codestantindev/sigmacode
 Keywords: swag,swaggy,nobitches,sigma,skibidi
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sigmacode-0.0.5/pyproject.toml` & `sigmacode-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sigmacode-0.0.5/sigmacode/terminal.py` & `sigmacode-0.0.6/sigmacode/terminal.py`

 * *Files identical despite different names*

### Comparing `sigmacode-0.0.5/sigmacode.egg-info/PKG-INFO` & `sigmacode-0.0.6/sigmacode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmacode
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Python Library for real sigmas!
 Author: codestantin
 License: MIT
 Project-URL: GitHub, https://github.com/codestantindev/sigmacode
 Keywords: swag,swaggy,nobitches,sigma,skibidi
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

