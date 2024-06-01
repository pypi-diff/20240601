# Comparing `tmp/sigmacode-0.0.1.tar.gz` & `tmp/sigmacode-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmacode-0.0.1.tar", last modified: Sat Jun  1 10:51:30 2024, max compression
+gzip compressed data, was "sigmacode-0.0.2.tar", last modified: Sat Jun  1 10:58:16 2024, max compression
```

## Comparing `sigmacode-0.0.1.tar` & `sigmacode-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 10:51:30.307667 sigmacode-0.0.1/
--rw-rw-rw-   0        0        0     1092 2024-06-01 10:46:23.000000 sigmacode-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      871 2024-06-01 10:51:30.288824 sigmacode-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       87 2024-06-01 10:47:51.000000 sigmacode-0.0.1/README.md
--rw-rw-rw-   0        0        0      963 2024-06-01 10:50:59.000000 sigmacode-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       16 2024-05-31 19:24:35.000000 sigmacode-0.0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 10:51:30.323643 sigmacode-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-01 10:51:30.105997 sigmacode-0.0.1/sigmacode/
--rw-rw-rw-   0        0        0       58 2024-06-01 10:50:02.000000 sigmacode-0.0.1/sigmacode/__init__.py
--rw-rw-rw-   0        0        0      438 2024-06-01 10:49:47.000000 sigmacode-0.0.1/sigmacode/terminal.py
-drwxrwxrwx   0        0        0        0 2024-06-01 10:51:30.282829 sigmacode-0.0.1/sigmacode.egg-info/
--rw-rw-rw-   0        0        0      871 2024-06-01 10:51:29.000000 sigmacode-0.0.1/sigmacode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-06-01 10:51:29.000000 sigmacode-0.0.1/sigmacode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 10:51:29.000000 sigmacode-0.0.1/sigmacode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-06-01 10:51:29.000000 sigmacode-0.0.1/sigmacode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-06-01 10:51:29.000000 sigmacode-0.0.1/sigmacode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 10:58:16.564261 sigmacode-0.0.2/
+-rw-rw-rw-   0        0        0     1092 2024-06-01 10:46:23.000000 sigmacode-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      871 2024-06-01 10:58:16.535265 sigmacode-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       87 2024-06-01 10:47:51.000000 sigmacode-0.0.2/README.md
+-rw-rw-rw-   0        0        0      963 2024-06-01 10:50:59.000000 sigmacode-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       16 2024-05-31 19:24:35.000000 sigmacode-0.0.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 10:58:16.565232 sigmacode-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-01 10:58:16.250235 sigmacode-0.0.2/sigmacode/
+-rw-rw-rw-   0        0        0      107 2024-06-01 10:57:24.000000 sigmacode-0.0.2/sigmacode/__init__.py
+-rw-rw-rw-   0        0        0      852 2024-06-01 10:57:05.000000 sigmacode-0.0.2/sigmacode/color.py
+-rw-rw-rw-   0        0        0      574 2024-06-01 10:57:21.000000 sigmacode-0.0.2/sigmacode/terminal.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:58:16.527459 sigmacode-0.0.2/sigmacode.egg-info/
+-rw-rw-rw-   0        0        0      871 2024-06-01 10:58:15.000000 sigmacode-0.0.2/sigmacode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2024-06-01 10:58:15.000000 sigmacode-0.0.2/sigmacode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 10:58:15.000000 sigmacode-0.0.2/sigmacode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-06-01 10:58:15.000000 sigmacode-0.0.2/sigmacode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-01 10:58:15.000000 sigmacode-0.0.2/sigmacode.egg-info/top_level.txt
```

### Comparing `sigmacode-0.0.1/LICENSE` & `sigmacode-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmacode-0.0.1/PKG-INFO` & `sigmacode-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmacode
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python Library for real sigmas!
 Author: codestantin
 License: MIT
 Project-URL: GitHub, https://github.com/codestantindev/sigmacode
 Keywords: swag,swaggy,nobitches,sigma,skibidi
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sigmacode-0.0.1/pyproject.toml` & `sigmacode-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sigmacode-0.0.1/sigmacode.egg-info/PKG-INFO` & `sigmacode-0.0.2/sigmacode.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmacode
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python Library for real sigmas!
 Author: codestantin
 License: MIT
 Project-URL: GitHub, https://github.com/codestantindev/sigmacode
 Keywords: swag,swaggy,nobitches,sigma,skibidi
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

