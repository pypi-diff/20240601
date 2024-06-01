# Comparing `tmp/nautc-1.1.1.tar.gz` & `tmp/nautc-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nautc-1.1.1.tar", last modified: Thu Apr  4 03:41:37 2024, max compression
+gzip compressed data, was "nautc-1.1.2.tar", last modified: Sat Jun  1 14:05:56 2024, max compression
```

## Comparing `nautc-1.1.1.tar` & `nautc-1.1.2.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0    18353 2024-04-04 03:40:38.913356 nautc-1.1.1/README.md
--rw-r--r--   0        0        0     3198 2024-04-04 03:41:37.074261 nautc-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     9884 2020-03-07 18:12:55.000000 nautc-1.1.1/txt.gz
--rw-r--r--   0        0        0    18669 1970-01-01 00:00:00.000000 nautc-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    18353 2024-04-04 03:40:38.913356 nautc-1.1.2/README.md
+-rw-r--r--   0        0        0     2858 2024-04-04 03:38:54.809701 nautc-1.1.2/nautc.py
+-rw-r--r--   0        0        0     3210 2024-06-01 14:05:56.604664 nautc-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     9884 2020-03-07 18:12:55.000000 nautc-1.1.2/txt.gz
+-rw-r--r--   0        0        0    18669 1970-01-01 00:00:00.000000 nautc-1.1.2/PKG-INFO
```

### Comparing `nautc-1.1.1/README.md` & `nautc-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nautc-1.1.1/pyproject.toml` & `nautc-1.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [tool.pdm.build]
 includes = [
     "txt.gz",
+    "*.py",
 ]
 
 [tool.mypy]
 mypy_path = "./typings"
 exclude = [
     "__pypackages__/",
     "./typings",
@@ -183,15 +184,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "nautc"
-version = "1.1.1"
+version = "1.1.2"
 description = "Convert plain text (letters, sometimes numbers, sometimes punctuation) to obscure but cool characters."
 authors = [
     { name = "Nasy", email = "nasyxx+python@gmail.com" },
 ]
 dependencies = [
     "tyro>=0.7.3",
 ]
```

### Comparing `nautc-1.1.1/txt.gz` & `nautc-1.1.2/txt.gz`

 * *Files identical despite different names*

### Comparing `nautc-1.1.1/PKG-INFO` & `nautc-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nautc
-Version: 1.1.1
+Version: 1.1.2
 Summary: Convert plain text (letters, sometimes numbers, sometimes punctuation) to obscure but cool characters.
 Author-Email: Nasy <nasyxx+python@gmail.com>
 License: MIT
 Requires-Python: <4.0,>=3.10
 Requires-Dist: tyro>=0.7.3
 Description-Content-Type: text/markdown
```

