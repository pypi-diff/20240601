# Comparing `tmp/func_bk-1.3.7.tar.gz` & `tmp/func_bk-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_bk-1.3.7.tar", last modified: Sat Jun  1 11:48:31 2024, max compression
+gzip compressed data, was "func_bk-1.5.0.tar", last modified: Sat Jun  1 12:17:42 2024, max compression
```

## Comparing `func_bk-1.3.7.tar` & `func_bk-1.5.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 11:48:31.891839 func_bk-1.3.7/
--rw-rw-rw-   0        0        0     2994 2024-06-01 11:48:31.891839 func_bk-1.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     2777 2024-05-30 12:32:20.000000 func_bk-1.3.7/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 11:48:31.884839 func_bk-1.3.7/func_bk/
--rw-rw-rw-   0        0        0     2491 2024-05-30 10:23:47.000000 func_bk-1.3.7/func_bk/__init__.py
--rw-rw-rw-   0        0        0     1719 2024-05-30 12:33:24.000000 func_bk-1.3.7/func_bk/django.py
--rw-rw-rw-   0        0        0     2713 2024-06-01 11:48:02.000000 func_bk-1.3.7/func_bk/fast_api.py
-drwxrwxrwx   0        0        0        0 2024-06-01 11:48:31.890839 func_bk-1.3.7/func_bk.egg-info/
--rw-rw-rw-   0        0        0     2994 2024-06-01 11:48:31.000000 func_bk-1.3.7/func_bk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-06-01 11:48:31.000000 func_bk-1.3.7/func_bk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 11:48:31.000000 func_bk-1.3.7/func_bk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-06-01 11:48:31.000000 func_bk-1.3.7/func_bk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2024-06-01 11:48:31.000000 func_bk-1.3.7/func_bk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2024-06-01 11:48:31.892839 func_bk-1.3.7/setup.cfg
--rw-rw-rw-   0        0        0      492 2024-05-30 12:34:31.000000 func_bk-1.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:17:42.024962 func_bk-1.5.0/
+-rw-rw-rw-   0        0        0     2994 2024-06-01 12:17:42.023963 func_bk-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2777 2024-05-30 12:32:20.000000 func_bk-1.5.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 12:17:42.017962 func_bk-1.5.0/func_bk/
+-rw-rw-rw-   0        0        0     2574 2024-06-01 12:17:14.000000 func_bk-1.5.0/func_bk/__init__.py
+-rw-rw-rw-   0        0        0     1719 2024-05-30 12:33:24.000000 func_bk-1.5.0/func_bk/django.py
+-rw-rw-rw-   0        0        0     2682 2024-06-01 11:58:16.000000 func_bk-1.5.0/func_bk/fast_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:17:42.023963 func_bk-1.5.0/func_bk.egg-info/
+-rw-rw-rw-   0        0        0     2994 2024-06-01 12:17:41.000000 func_bk-1.5.0/func_bk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-06-01 12:17:41.000000 func_bk-1.5.0/func_bk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 12:17:41.000000 func_bk-1.5.0/func_bk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-06-01 12:17:41.000000 func_bk-1.5.0/func_bk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-06-01 12:17:41.000000 func_bk-1.5.0/func_bk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2024-06-01 12:17:42.025962 func_bk-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0      492 2024-06-01 12:17:34.000000 func_bk-1.5.0/setup.py
```

### Comparing `func_bk-1.3.7/PKG-INFO` & `func_bk-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.3.7
+Version: 1.5.0
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
```

### Comparing `func_bk-1.3.7/README.md` & `func_bk-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `func_bk-1.3.7/func_bk/__init__.py` & `func_bk-1.5.0/func_bk/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+import sys
+import os
+sys.path.append(os.path.join(os.path.dirname(__file__)))
+
 import random
 from colour import Color
 import inspect
 import django
 import fast_api
 
 def listrand(min,max,kol):
```

### Comparing `func_bk-1.3.7/func_bk/django.py` & `func_bk-1.5.0/func_bk/django.py`

 * *Files identical despite different names*

### Comparing `func_bk-1.3.7/func_bk/fast_api.py` & `func_bk-1.5.0/func_bk/fast_api.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,30 +28,30 @@
         include_in_schema: bool = True,
         response_class: type[Response] = JSONResponse,
         name: str = None,
         callbacks = None,
         openapi_extra = None,
         generate_unique_id_function = generate_unique_id
     ):
-    type_lower = type.lower()
+    type = type.lower()
     route_function = None
-    if type_lower == "get":
+    if type == "get":
         route_function = app.get
-    elif type_lower == "post":
+    elif type == "post":
         route_function = app.post
-    elif type_lower == "put":
+    elif type == "put":
         route_function = app.put
-    elif type_lower == "delete":
+    elif type == "delete":
         route_function = app.delete
-    elif type_lower == "patch":
+    elif type == "patch":
         route_function = app.patch
 
     if route_function:
         route_function(
-            path,
+            path=path,
             response_model=response_model,
             status_code=status_code,
             tags=tags,
             dependencies=dependencies,
             summary=summary,
             description=description,
             response_description=response_description,
```

### Comparing `func_bk-1.3.7/func_bk.egg-info/PKG-INFO` & `func_bk-1.5.0/func_bk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.3.7
+Version: 1.5.0
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
```

