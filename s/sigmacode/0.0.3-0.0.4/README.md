# Comparing `tmp/sigmacode-0.0.3.tar.gz` & `tmp/sigmacode-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sigmacode-0.0.3.tar", last modified: Sat Jun  1 11:08:34 2024, max compression
+gzip compressed data, was "sigmacode-0.0.4.tar", last modified: Sat Jun  1 11:11:13 2024, max compression
```

## Comparing `sigmacode-0.0.3.tar` & `sigmacode-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 11:08:34.936514 sigmacode-0.0.3/
--rw-rw-rw-   0        0        0     1092 2024-06-01 10:46:23.000000 sigmacode-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      871 2024-06-01 11:08:34.891844 sigmacode-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       87 2024-06-01 10:47:51.000000 sigmacode-0.0.3/README.md
--rw-rw-rw-   0        0        0      963 2024-06-01 10:50:59.000000 sigmacode-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       16 2024-05-31 19:24:35.000000 sigmacode-0.0.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 11:08:34.937516 sigmacode-0.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-01 11:08:33.648476 sigmacode-0.0.3/sigmacode/
--rw-rw-rw-   0        0        0       58 2024-06-01 11:08:07.000000 sigmacode-0.0.3/sigmacode/__init__.py
--rw-rw-rw-   0        0        0      852 2024-06-01 11:05:58.000000 sigmacode-0.0.3/sigmacode/color.py
--rw-rw-rw-   0        0        0      574 2024-06-01 10:57:21.000000 sigmacode-0.0.3/sigmacode/terminal.py
-drwxrwxrwx   0        0        0        0 2024-06-01 11:08:34.886514 sigmacode-0.0.3/sigmacode.egg-info/
--rw-rw-rw-   0        0        0      871 2024-06-01 11:08:33.000000 sigmacode-0.0.3/sigmacode.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      295 2024-06-01 11:08:33.000000 sigmacode-0.0.3/sigmacode.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 11:08:33.000000 sigmacode-0.0.3/sigmacode.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-06-01 11:08:33.000000 sigmacode-0.0.3/sigmacode.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-06-01 11:08:33.000000 sigmacode-0.0.3/sigmacode.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 11:11:13.673196 sigmacode-0.0.4/
+-rw-rw-rw-   0        0        0     1092 2024-06-01 10:46:23.000000 sigmacode-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      871 2024-06-01 11:11:13.570317 sigmacode-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       87 2024-06-01 10:47:51.000000 sigmacode-0.0.4/README.md
+-rw-rw-rw-   0        0        0      963 2024-06-01 10:50:59.000000 sigmacode-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       16 2024-05-31 19:24:35.000000 sigmacode-0.0.4/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 11:11:13.674200 sigmacode-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-01 11:11:13.112201 sigmacode-0.0.4/sigmacode/
+-rw-rw-rw-   0        0        0       63 2024-06-01 11:10:42.000000 sigmacode-0.0.4/sigmacode/__init__.py
+-rw-rw-rw-   0        0        0      852 2024-06-01 11:05:58.000000 sigmacode-0.0.4/sigmacode/color.py
+-rw-rw-rw-   0        0        0      574 2024-06-01 10:57:21.000000 sigmacode-0.0.4/sigmacode/terminal.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:11:13.563290 sigmacode-0.0.4/sigmacode.egg-info/
+-rw-rw-rw-   0        0        0      871 2024-06-01 11:11:12.000000 sigmacode-0.0.4/sigmacode.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      295 2024-06-01 11:11:12.000000 sigmacode-0.0.4/sigmacode.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 11:11:12.000000 sigmacode-0.0.4/sigmacode.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-06-01 11:11:12.000000 sigmacode-0.0.4/sigmacode.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-06-01 11:11:12.000000 sigmacode-0.0.4/sigmacode.egg-info/top_level.txt
```

### Comparing `sigmacode-0.0.3/LICENSE` & `sigmacode-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sigmacode-0.0.3/PKG-INFO` & `sigmacode-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmacode
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Library for real sigmas!
 Author: codestantin
 License: MIT
 Project-URL: GitHub, https://github.com/codestantindev/sigmacode
 Keywords: swag,swaggy,nobitches,sigma,skibidi
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sigmacode-0.0.3/pyproject.toml` & `sigmacode-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sigmacode-0.0.3/sigmacode/color.py` & `sigmacode-0.0.4/sigmacode/color.py`

 * *Files identical despite different names*

### Comparing `sigmacode-0.0.3/sigmacode/terminal.py` & `sigmacode-0.0.4/sigmacode/terminal.py`

 * *Files identical despite different names*

### Comparing `sigmacode-0.0.3/sigmacode.egg-info/PKG-INFO` & `sigmacode-0.0.4/sigmacode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sigmacode
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python Library for real sigmas!
 Author: codestantin
 License: MIT
 Project-URL: GitHub, https://github.com/codestantindev/sigmacode
 Keywords: swag,swaggy,nobitches,sigma,skibidi
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
```

