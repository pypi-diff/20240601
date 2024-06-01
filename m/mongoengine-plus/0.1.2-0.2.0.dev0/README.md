# Comparing `tmp/mongoengine-plus-0.1.2.tar.gz` & `tmp/mongoengine_plus-0.2.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongoengine-plus-0.1.2.tar", last modified: Thu Mar 21 17:05:40 2024, max compression
+gzip compressed data, was "mongoengine_plus-0.2.0.dev0.tar", last modified: Sat Jun  1 00:16:35 2024, max compression
```

## Comparing `mongoengine-plus-0.1.2.tar` & `mongoengine_plus-0.2.0.dev0.tar`

### file list

```diff
@@ -1,42 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:05:40.165457 mongoengine-plus-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-21 17:05:40.165457 mongoengine-plus-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:05:40.161457 mongoengine-plus-0.1.2/mongoengine_plus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/mongoengine_plus/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:05:40.161457 mongoengine-plus-0.1.2/mongoengine_plus/aio/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/mongoengine_plus/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/mongoengine_plus/aio/async_document.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/mongoengine_plus/aio/async_query_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/mongoengine_plus/aio/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:05:40.161457 mongoengine-plus-0.1.2/mongoengine_plus/models/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/mongoengine_plus/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/mongoengine_plus/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/mongoengine_plus/models/event_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/mongoengine_plus/models/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:05:40.161457 mongoengine-plus-0.1.2/mongoengine_plus/types/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/mongoengine_plus/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/mongoengine_plus/types/enum_field.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/mongoengine_plus/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:05:40.165457 mongoengine-plus-0.1.2/mongoengine_plus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-03-21 17:05:40.000000 mongoengine-plus-0.1.2/mongoengine_plus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-03-21 17:05:40.000000 mongoengine-plus-0.1.2/mongoengine_plus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 17:05:40.000000 mongoengine-plus-0.1.2/mongoengine_plus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-21 17:05:40.000000 mongoengine-plus-0.1.2/mongoengine_plus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-21 17:05:40.000000 mongoengine-plus-0.1.2/mongoengine_plus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-21 17:05:40.165457 mongoengine-plus-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:05:40.161457 mongoengine-plus-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:05:40.165457 mongoengine-plus-0.1.2/tests/aio/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/tests/aio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/tests/aio/cities.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/tests/aio/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/tests/aio/test_async_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/tests/aio/test_async_query_set.py
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 17:05:40.165457 mongoengine-plus-0.1.2/tests/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/tests/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/tests/models/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/tests/models/test_event_handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-03-21 17:05:27.000000 mongoengine-plus-0.1.2/tests/models/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:16:35.692026 mongoengine_plus-0.2.0.dev0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-06-01 00:16:35.692026 mongoengine_plus-0.2.0.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:16:35.684026 mongoengine_plus-0.2.0.dev0/mongoengine_plus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:16:35.688026 mongoengine_plus-0.2.0.dev0/mongoengine_plus/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus/aio/async_document.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus/aio/async_query_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus/aio/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:16:35.688026 mongoengine_plus-0.2.0.dev0/mongoengine_plus/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus/models/event_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3662 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus/models/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:16:35.688026 mongoengine_plus-0.2.0.dev0/mongoengine_plus/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus/types/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:16:35.688026 mongoengine_plus-0.2.0.dev0/mongoengine_plus/types/encrypted_string/
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus/types/encrypted_string/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus/types/encrypted_string/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus/types/encrypted_string/exc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus/types/encrypted_string/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus/types/enum_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:16:35.692026 mongoengine_plus-0.2.0.dev0/mongoengine_plus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-06-01 00:16:35.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-06-01 00:16:35.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:16:35.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-06-01 00:16:35.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-01 00:16:35.000000 mongoengine_plus-0.2.0.dev0/mongoengine_plus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-06-01 00:16:35.692026 mongoengine_plus-0.2.0.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:16:35.688026 mongoengine_plus-0.2.0.dev0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:16:35.688026 mongoengine_plus-0.2.0.dev0/tests/aio/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/tests/aio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/tests/aio/cities.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/tests/aio/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/tests/aio/test_async_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/tests/aio/test_async_query_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:16:35.692026 mongoengine_plus-0.2.0.dev0/tests/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/tests/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/tests/models/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/tests/models/test_event_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3331 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/tests/models/test_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:16:35.692026 mongoengine_plus-0.2.0.dev0/tests/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/tests/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4937 2024-06-01 00:16:28.000000 mongoengine_plus-0.2.0.dev0/tests/types/test_encrypted_string.py
```

### Comparing `mongoengine-plus-0.1.2/LICENSE` & `mongoengine_plus-0.2.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `mongoengine-plus-0.1.2/PKG-INFO` & `mongoengine_plus-0.2.0.dev0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: mongoengine-plus
-Version: 0.1.2
+Version: 0.2.0.dev0
 Summary: Extras for mongoengine
 Home-page: https://github.com/cuenca-mx/mongoengine-plus
 Author: Cuenca
 Author-email: dev@cuenca.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mongoengine>=0.20.0
 Requires-Dist: dnspython<2.2.0,>=2.0.0
+Requires-Dist: pymongo<4.0.0,>=3.11.0
+Requires-Dist: pymongocrypt<2.0.0,>=1.9.2
 
 # mongoengine-plus
 Extra types and helpers for mongoengine
```

### Comparing `mongoengine-plus-0.1.2/mongoengine_plus/aio/async_document.py` & `mongoengine_plus-0.2.0.dev0/mongoengine_plus/aio/async_document.py`

 * *Files identical despite different names*

### Comparing `mongoengine-plus-0.1.2/mongoengine_plus/aio/async_query_set.py` & `mongoengine_plus-0.2.0.dev0/mongoengine_plus/aio/async_query_set.py`

 * *Files identical despite different names*

### Comparing `mongoengine-plus-0.1.2/mongoengine_plus/models/base.py` & `mongoengine_plus-0.2.0.dev0/mongoengine_plus/models/base.py`

 * *Files identical despite different names*

### Comparing `mongoengine-plus-0.1.2/mongoengine_plus/models/event_handlers.py` & `mongoengine_plus-0.2.0.dev0/mongoengine_plus/models/event_handlers.py`

 * *Files identical despite different names*

### Comparing `mongoengine-plus-0.1.2/mongoengine_plus/models/helpers.py` & `mongoengine_plus-0.2.0.dev0/mongoengine_plus/models/helpers.py`

 * *Files identical despite different names*

### Comparing `mongoengine-plus-0.1.2/mongoengine_plus/types/enum_field.py` & `mongoengine_plus-0.2.0.dev0/mongoengine_plus/types/enum_field.py`

 * *Files identical despite different names*

### Comparing `mongoengine-plus-0.1.2/mongoengine_plus.egg-info/PKG-INFO` & `mongoengine_plus-0.2.0.dev0/mongoengine_plus.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: mongoengine-plus
-Version: 0.1.2
+Version: 0.2.0.dev0
 Summary: Extras for mongoengine
 Home-page: https://github.com/cuenca-mx/mongoengine-plus
 Author: Cuenca
 Author-email: dev@cuenca.com
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: mongoengine>=0.20.0
 Requires-Dist: dnspython<2.2.0,>=2.0.0
+Requires-Dist: pymongo<4.0.0,>=3.11.0
+Requires-Dist: pymongocrypt<2.0.0,>=1.9.2
 
 # mongoengine-plus
 Extra types and helpers for mongoengine
```

### Comparing `mongoengine-plus-0.1.2/mongoengine_plus.egg-info/SOURCES.txt` & `mongoengine_plus-0.2.0.dev0/mongoengine_plus.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -15,18 +15,24 @@
 mongoengine_plus/aio/utils.py
 mongoengine_plus/models/__init__.py
 mongoengine_plus/models/base.py
 mongoengine_plus/models/event_handlers.py
 mongoengine_plus/models/helpers.py
 mongoengine_plus/types/__init__.py
 mongoengine_plus/types/enum_field.py
+mongoengine_plus/types/encrypted_string/__init__.py
+mongoengine_plus/types/encrypted_string/base.py
+mongoengine_plus/types/encrypted_string/exc.py
+mongoengine_plus/types/encrypted_string/fields.py
 tests/__init__.py
 tests/conftest.py
 tests/aio/__init__.py
 tests/aio/cities.py
 tests/aio/conftest.py
 tests/aio/test_async_model.py
 tests/aio/test_async_query_set.py
 tests/models/__init__.py
 tests/models/test_base.py
 tests/models/test_event_handlers.py
-tests/models/test_helpers.py
+tests/models/test_helpers.py
+tests/types/__init__.py
+tests/types/test_encrypted_string.py
```

### Comparing `mongoengine-plus-0.1.2/setup.py` & `mongoengine_plus-0.2.0.dev0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     packages=find_packages(),
     include_package_data=True,
     package_data=dict(mongoengine_plus=['py.typed']),
     python_requires='>=3.8',
     install_requires=[
         'mongoengine>=0.20.0',
         'dnspython>=2.0.0,<2.2.0',
+        'pymongo>=3.11.0,<4.0.0',
+        'pymongocrypt>=1.9.2,<2.0.0',
     ],
     classifiers=[
         'Programming Language :: Python :: 3.8',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
 )
```

### Comparing `mongoengine-plus-0.1.2/tests/aio/conftest.py` & `mongoengine_plus-0.2.0.dev0/tests/aio/conftest.py`

 * *Files identical despite different names*

### Comparing `mongoengine-plus-0.1.2/tests/aio/test_async_model.py` & `mongoengine_plus-0.2.0.dev0/tests/aio/test_async_model.py`

 * *Files identical despite different names*

### Comparing `mongoengine-plus-0.1.2/tests/aio/test_async_query_set.py` & `mongoengine_plus-0.2.0.dev0/tests/aio/test_async_query_set.py`

 * *Files identical despite different names*

### Comparing `mongoengine-plus-0.1.2/tests/models/test_helpers.py` & `mongoengine_plus-0.2.0.dev0/tests/models/test_helpers.py`

 * *Files identical despite different names*

