# Comparing `tmp/eventu-0.1.0.tar.gz` & `tmp/eventu-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventu-0.1.0.tar", max compression
+gzip compressed data, was "eventu-0.1.1.tar", max compression
```

## Comparing `eventu-0.1.0.tar` & `eventu-0.1.1.tar`

### file list

```diff
@@ -1,3 +1,4 @@
--rw-r--r--   0        0        0    13412 2024-06-01 12:02:29.672336 eventu-0.1.0/eventu/eventu.py
--rw-r--r--   0        0        0      531 2024-06-01 12:02:57.331710 eventu-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 eventu-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    13412 2024-06-01 12:02:29.672336 eventu-0.1.1/eventu/eventu.py
+-rw-r--r--   0        0        0        0 2024-06-01 14:02:32.595614 eventu-0.1.1/eventu/py.typed
+-rw-r--r--   0        0        0      531 2024-06-01 14:03:12.855685 eventu-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 eventu-0.1.1/PKG-INFO
```

### Comparing `eventu-0.1.0/eventu/eventu.py` & `eventu-0.1.1/eventu/eventu.py`

 * *Files identical despite different names*

### Comparing `eventu-0.1.0/pyproject.toml` & `eventu-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eventu"
-version = "0.1.0"
+version = "0.1.1"
 description = "Transactional outbox and idempotent consumer"
 authors = ["Yuriy Kehter <yuriy.kehter@gmail.com>"]
 packages = [
     { include = "eventu" },
 ]
 
 [tool.poetry.dependencies]
```

### Comparing `eventu-0.1.0/PKG-INFO` & `eventu-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventu
-Version: 0.1.0
+Version: 0.1.1
 Summary: Transactional outbox and idempotent consumer
 Author: Yuriy Kehter
 Author-email: yuriy.kehter@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

