# Comparing `tmp/async_pymongo-0.1.4.tar.gz` & `tmp/async_pymongo-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_pymongo-0.1.4.tar", max compression
+gzip compressed data, was "async_pymongo-0.1.5.tar", max compression
```

## Comparing `async_pymongo-0.1.4.tar` & `async_pymongo-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-12-30 17:31:53.857264 async_pymongo-0.1.4/LICENSE
--rw-r--r--   0        0        0      545 2023-12-30 17:31:53.857264 async_pymongo-0.1.4/README.md
--rw-r--r--   0        0        0     1110 2023-12-30 17:31:53.857264 async_pymongo-0.1.4/async_pymongo/__init__.py
--rw-r--r--   0        0        0     1227 2023-12-30 17:31:53.857264 async_pymongo-0.1.4/async_pymongo/async_helper.py
--rw-r--r--   0        0        0     3383 2023-12-30 17:31:53.857264 async_pymongo-0.1.4/async_pymongo/base.py
--rw-r--r--   0        0        0     4419 2023-12-30 17:31:53.857264 async_pymongo-0.1.4/async_pymongo/change_stream.py
--rw-r--r--   0        0        0     8569 2023-12-30 17:31:53.857264 async_pymongo-0.1.4/async_pymongo/client.py
--rw-r--r--   0        0        0     6825 2023-12-30 17:31:53.857264 async_pymongo-0.1.4/async_pymongo/client_session.py
--rw-r--r--   0        0        0    17710 2023-12-30 17:31:53.857264 async_pymongo-0.1.4/async_pymongo/collection.py
--rw-r--r--   0        0        0     7482 2023-12-30 17:31:53.857264 async_pymongo-0.1.4/async_pymongo/command_cursor.py
--rw-r--r--   0        0        0     6533 2023-12-30 17:31:53.857264 async_pymongo-0.1.4/async_pymongo/cursor.py
--rw-r--r--   0        0        0     6977 2023-12-30 17:31:53.857264 async_pymongo-0.1.4/async_pymongo/cursor_base.py
--rw-r--r--   0        0        0     9347 2023-12-30 17:31:53.857264 async_pymongo-0.1.4/async_pymongo/db.py
--rw-r--r--   0        0        0      942 2023-12-30 17:31:53.857264 async_pymongo-0.1.4/async_pymongo/errors.py
--rw-r--r--   0        0        0     1338 2023-12-30 17:31:53.857264 async_pymongo-0.1.4/async_pymongo/typings.py
--rw-r--r--   0        0        0     1087 2023-12-30 17:35:19.582173 async_pymongo-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1523 1970-01-01 00:00:00.000000 async_pymongo-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-06-01 11:48:52.362574 async_pymongo-0.1.5/LICENSE
+-rw-r--r--   0        0        0      545 2024-06-01 11:48:52.362574 async_pymongo-0.1.5/README.md
+-rw-r--r--   0        0        0     1110 2024-06-01 11:48:52.362574 async_pymongo-0.1.5/async_pymongo/__init__.py
+-rw-r--r--   0        0        0     1227 2024-06-01 11:48:52.362574 async_pymongo-0.1.5/async_pymongo/async_helper.py
+-rw-r--r--   0        0        0     3383 2024-06-01 11:48:52.372574 async_pymongo-0.1.5/async_pymongo/base.py
+-rw-r--r--   0        0        0     4419 2024-06-01 11:48:52.372574 async_pymongo-0.1.5/async_pymongo/change_stream.py
+-rw-r--r--   0        0        0     8569 2024-06-01 11:48:52.372574 async_pymongo-0.1.5/async_pymongo/client.py
+-rw-r--r--   0        0        0     6825 2024-06-01 11:48:52.372574 async_pymongo-0.1.5/async_pymongo/client_session.py
+-rw-r--r--   0        0        0    17710 2024-06-01 11:48:52.372574 async_pymongo-0.1.5/async_pymongo/collection.py
+-rw-r--r--   0        0        0     7482 2024-06-01 11:48:52.372574 async_pymongo-0.1.5/async_pymongo/command_cursor.py
+-rw-r--r--   0        0        0     6533 2024-06-01 11:48:52.372574 async_pymongo-0.1.5/async_pymongo/cursor.py
+-rw-r--r--   0        0        0     6977 2024-06-01 11:48:52.372574 async_pymongo-0.1.5/async_pymongo/cursor_base.py
+-rw-r--r--   0        0        0     9347 2024-06-01 11:48:52.372574 async_pymongo-0.1.5/async_pymongo/db.py
+-rw-r--r--   0        0        0      942 2024-06-01 11:48:52.372574 async_pymongo-0.1.5/async_pymongo/errors.py
+-rw-r--r--   0        0        0     1338 2024-06-01 11:48:52.372574 async_pymongo-0.1.5/async_pymongo/typings.py
+-rw-r--r--   0        0        0     1095 2024-06-01 11:55:20.902515 async_pymongo-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1531 1970-01-01 00:00:00.000000 async_pymongo-0.1.5/PKG-INFO
```

### Comparing `async_pymongo-0.1.4/LICENSE` & `async_pymongo-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.4/README.md` & `async_pymongo-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.4/async_pymongo/__init__.py` & `async_pymongo-0.1.5/async_pymongo/__init__.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.4/async_pymongo/async_helper.py` & `async_pymongo-0.1.5/async_pymongo/async_helper.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.4/async_pymongo/base.py` & `async_pymongo-0.1.5/async_pymongo/base.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.4/async_pymongo/change_stream.py` & `async_pymongo-0.1.5/async_pymongo/change_stream.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.4/async_pymongo/client.py` & `async_pymongo-0.1.5/async_pymongo/client.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.4/async_pymongo/client_session.py` & `async_pymongo-0.1.5/async_pymongo/client_session.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.4/async_pymongo/collection.py` & `async_pymongo-0.1.5/async_pymongo/collection.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.4/async_pymongo/command_cursor.py` & `async_pymongo-0.1.5/async_pymongo/command_cursor.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.4/async_pymongo/cursor.py` & `async_pymongo-0.1.5/async_pymongo/cursor.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.4/async_pymongo/cursor_base.py` & `async_pymongo-0.1.5/async_pymongo/cursor_base.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.4/async_pymongo/db.py` & `async_pymongo-0.1.5/async_pymongo/db.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.4/async_pymongo/errors.py` & `async_pymongo-0.1.5/async_pymongo/errors.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.4/async_pymongo/typings.py` & `async_pymongo-0.1.5/async_pymongo/typings.py`

 * *Files identical despite different names*

### Comparing `async_pymongo-0.1.4/pyproject.toml` & `async_pymongo-0.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async-pymongo"
-version = "0.1.4"
+version = "0.1.5"
 description = "Asynchronous wrapper for pymongo"
 license = "GPL-3.0-or-later"
 authors = [
     "Adek Maulana <adekzmaulana@gmail.com>",
     "Gaung Ramadhan <hi@mrmiss.my.id>",
     "wulan17 <wulan17@nusantararom.org>"
 ]
@@ -25,13 +25,13 @@
     "Topic :: Database",
 ]
 
 packages = [{include = "async_pymongo"}]
 
 [tool.poetry.dependencies]
 python = "~=3.9"
-pymongo = ">=4.3.3"
+pymongo = ">=4.3.3 <=5.0.0"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `async_pymongo-0.1.4/PKG-INFO` & `async_pymongo-0.1.5/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-pymongo
-Version: 0.1.4
+Version: 0.1.5
 Summary: Asynchronous wrapper for pymongo
 Home-page: https://github.com/Mayuri-Chan/async_pymongo
 License: GPL-3.0-or-later
 Keywords: async,python,pymongo
 Author: Adek Maulana
 Author-email: adekzmaulana@gmail.com
 Requires-Python: >=3.9,<4.0
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Database
-Requires-Dist: pymongo (>=4.3.3)
+Requires-Dist: pymongo (>=4.3.3,<=5.0.0)
 Project-URL: Repository, https://github.com/Mayuri-Chan/async_pymongo
 Description-Content-Type: text/markdown
 
 ## async_pymongo
 Asynchronous wrapper for pymongo  
 [Comparison](https://github.com/Mayuri-Chan/async_pymongo/blob/staging/comparison.png)
```

