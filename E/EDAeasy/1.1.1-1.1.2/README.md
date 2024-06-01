# Comparing `tmp/edaeasy-1.1.1.tar.gz` & `tmp/edaeasy-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edaeasy-1.1.1.tar", max compression
+gzip compressed data, was "edaeasy-1.1.2.tar", max compression
```

## Comparing `edaeasy-1.1.1.tar` & `edaeasy-1.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1093 2023-08-30 17:58:18.245963 edaeasy-1.1.1/LICENSE
--rw-r--r--   0        0        0     1835 2023-07-28 01:32:55.456083 edaeasy-1.1.1/README.md
--rw-r--r--   0        0        0      588 2024-05-31 06:13:37.248317 edaeasy-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      124 2024-05-31 06:12:58.866248 edaeasy-1.1.1/src/edaeasy/__init__.py
--rw-r--r--   0        0        0        0 2023-07-27 19:33:18.234490 edaeasy-1.1.1/src/edaeasy/config.toml
--rw-r--r--   0        0        0     4406 2024-05-31 06:13:08.070851 edaeasy-1.1.1/src/edaeasy/functions.py
--rw-r--r--   0        0        0     2559 1970-01-01 00:00:00.000000 edaeasy-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-08-30 17:58:18.245963 edaeasy-1.1.2/LICENSE
+-rw-r--r--   0        0        0     1835 2023-07-28 01:32:55.456083 edaeasy-1.1.2/README.md
+-rw-r--r--   0        0        0      588 2024-06-01 18:16:31.956376 edaeasy-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      124 2024-05-31 06:12:58.866248 edaeasy-1.1.2/src/edaeasy/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-27 19:33:18.234490 edaeasy-1.1.2/src/edaeasy/config.toml
+-rw-r--r--   0        0        0     4406 2024-05-31 06:13:08.070851 edaeasy-1.1.2/src/edaeasy/functions.py
+-rw-r--r--   0        0        0     2559 1970-01-01 00:00:00.000000 edaeasy-1.1.2/PKG-INFO
```

### Comparing `edaeasy-1.1.1/LICENSE` & `edaeasy-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `edaeasy-1.1.1/README.md` & `edaeasy-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `edaeasy-1.1.1/pyproject.toml` & `edaeasy-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "EDAeasy"
-version = "1.1.1"
+version = "1.1.2"
 description = "Functions and tools for making Exploratory Data Analysis easy!"
 authors = ["Francisco Jesus Ocazionez Cardozo <pach812@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["Exploratory Analysis","EDA"]
 
 [tool.poetry.dependencies]
```

### Comparing `edaeasy-1.1.1/src/edaeasy/functions.py` & `edaeasy-1.1.2/src/edaeasy/functions.py`

 * *Files identical despite different names*

### Comparing `edaeasy-1.1.1/PKG-INFO` & `edaeasy-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: EDAeasy
-Version: 1.1.1
+Version: 1.1.2
 Summary: Functions and tools for making Exploratory Data Analysis easy!
 License: MIT
 Keywords: Exploratory Analysis,EDA
 Author: Francisco Jesus Ocazionez Cardozo
 Author-email: pach812@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

