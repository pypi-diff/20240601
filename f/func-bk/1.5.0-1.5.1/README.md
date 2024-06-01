# Comparing `tmp/func_bk-1.5.0.tar.gz` & `tmp/func_bk-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_bk-1.5.0.tar", last modified: Sat Jun  1 12:17:42 2024, max compression
+gzip compressed data, was "func_bk-1.5.1.tar", last modified: Sat Jun  1 12:58:51 2024, max compression
```

## Comparing `func_bk-1.5.0.tar` & `func_bk-1.5.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 12:17:42.024962 func_bk-1.5.0/
--rw-rw-rw-   0        0        0     2994 2024-06-01 12:17:42.023963 func_bk-1.5.0/PKG-INFO
--rw-rw-rw-   0        0        0     2777 2024-05-30 12:32:20.000000 func_bk-1.5.0/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 12:17:42.017962 func_bk-1.5.0/func_bk/
--rw-rw-rw-   0        0        0     2574 2024-06-01 12:17:14.000000 func_bk-1.5.0/func_bk/__init__.py
--rw-rw-rw-   0        0        0     1719 2024-05-30 12:33:24.000000 func_bk-1.5.0/func_bk/django.py
--rw-rw-rw-   0        0        0     2682 2024-06-01 11:58:16.000000 func_bk-1.5.0/func_bk/fast_api.py
-drwxrwxrwx   0        0        0        0 2024-06-01 12:17:42.023963 func_bk-1.5.0/func_bk.egg-info/
--rw-rw-rw-   0        0        0     2994 2024-06-01 12:17:41.000000 func_bk-1.5.0/func_bk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-06-01 12:17:41.000000 func_bk-1.5.0/func_bk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 12:17:41.000000 func_bk-1.5.0/func_bk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-06-01 12:17:41.000000 func_bk-1.5.0/func_bk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2024-06-01 12:17:41.000000 func_bk-1.5.0/func_bk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2024-06-01 12:17:42.025962 func_bk-1.5.0/setup.cfg
--rw-rw-rw-   0        0        0      492 2024-06-01 12:17:34.000000 func_bk-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:58:51.881334 func_bk-1.5.1/
+-rw-rw-rw-   0        0        0     3482 2024-06-01 12:58:51.881334 func_bk-1.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2024-06-01 12:58:41.000000 func_bk-1.5.1/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 12:58:51.875334 func_bk-1.5.1/func_bk/
+-rw-rw-rw-   0        0        0     2574 2024-06-01 12:17:14.000000 func_bk-1.5.1/func_bk/__init__.py
+-rw-rw-rw-   0        0        0     1719 2024-05-30 12:33:24.000000 func_bk-1.5.1/func_bk/django.py
+-rw-rw-rw-   0        0        0     3425 2024-06-01 12:54:03.000000 func_bk-1.5.1/func_bk/fast_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:58:51.880334 func_bk-1.5.1/func_bk.egg-info/
+-rw-rw-rw-   0        0        0     3482 2024-06-01 12:58:51.000000 func_bk-1.5.1/func_bk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-06-01 12:58:51.000000 func_bk-1.5.1/func_bk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 12:58:51.000000 func_bk-1.5.1/func_bk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-06-01 12:58:51.000000 func_bk-1.5.1/func_bk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-06-01 12:58:51.000000 func_bk-1.5.1/func_bk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2024-06-01 12:58:51.882337 func_bk-1.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      492 2024-06-01 12:17:34.000000 func_bk-1.5.1/setup.py
```

### Comparing `func_bk-1.5.0/PKG-INFO` & `func_bk-1.5.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.5.0
+Version: 1.5.1
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
@@ -108,7 +108,33 @@
 
 FAST_API:
 
 path(): this is django path for fast api, He have args from FastAPI.get() or FastAPI.post etc, new arguments=
         app:your app FastAPI
         func:function from your FastAPI
         type:str, type:'get','post','put','delete','patch'(register is not important)
+example:
+    urls.py:
+        from func_bk.fast_api import path
+        from fastapi import FastAPI
+        import main
+
+
+        def initi(app: FastAPI):
+            path(app,main.hello,'post','/')
+    main.py:
+        from fastapi import FastAPI, Request
+        from urls import initi
+        app=FastAPI()
+
+        def hello():
+            return 'hello world'
+        
+        initi(app)
+
+
+
+urls.py
+
+BForm: class for inheritance form
+
+Label: label for form
```

### Comparing `func_bk-1.5.0/README.md` & `func_bk-1.5.1/func_bk.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: func_bk
+Version: 1.5.1
+Summary: add function for normal python and add class(for inheritance) for django
+Author-email: lilo.pio147@mail.ru
+Description-Content-Type: text/markdown
+
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
 
 
 adder - dict,**kwargs 
 add to dict all arguments kwargs
@@ -100,8 +107,34 @@
 
 
 FAST_API:
 
 path(): this is django path for fast api, He have args from FastAPI.get() or FastAPI.post etc, new arguments=
         app:your app FastAPI
         func:function from your FastAPI
-        type:str, type:'get','post','put','delete','patch'(register is not important)
+        type:str, type:'get','post','put','delete','patch'(register is not important)
+example:
+    urls.py:
+        from func_bk.fast_api import path
+        from fastapi import FastAPI
+        import main
+
+
+        def initi(app: FastAPI):
+            path(app,main.hello,'post','/')
+    main.py:
+        from fastapi import FastAPI, Request
+        from urls import initi
+        app=FastAPI()
+
+        def hello():
+            return 'hello world'
+        
+        initi(app)
+
+
+
+urls.py
+
+BForm: class for inheritance form
+
+Label: label for form
```

### Comparing `func_bk-1.5.0/func_bk/__init__.py` & `func_bk-1.5.1/func_bk/__init__.py`

 * *Files identical despite different names*

### Comparing `func_bk-1.5.0/func_bk/django.py` & `func_bk-1.5.1/func_bk/django.py`

 * *Files identical despite different names*

### Comparing `func_bk-1.5.0/func_bk.egg-info/PKG-INFO` & `func_bk-1.5.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: func_bk
-Version: 1.5.0
-Summary: add function for normal python and add class(for inheritance) for django
-Author-email: lilo.pio147@mail.ru
-Description-Content-Type: text/markdown
-
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
 
 
 adder - dict,**kwargs 
 add to dict all arguments kwargs
@@ -108,7 +101,33 @@
 
 FAST_API:
 
 path(): this is django path for fast api, He have args from FastAPI.get() or FastAPI.post etc, new arguments=
         app:your app FastAPI
         func:function from your FastAPI
         type:str, type:'get','post','put','delete','patch'(register is not important)
+example:
+    urls.py:
+        from func_bk.fast_api import path
+        from fastapi import FastAPI
+        import main
+
+
+        def initi(app: FastAPI):
+            path(app,main.hello,'post','/')
+    main.py:
+        from fastapi import FastAPI, Request
+        from urls import initi
+        app=FastAPI()
+
+        def hello():
+            return 'hello world'
+        
+        initi(app)
+
+
+
+urls.py
+
+BForm: class for inheritance form
+
+Label: label for form
```

