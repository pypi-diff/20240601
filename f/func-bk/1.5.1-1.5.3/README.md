# Comparing `tmp/func_bk-1.5.1.tar.gz` & `tmp/func_bk-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_bk-1.5.1.tar", last modified: Sat Jun  1 12:58:51 2024, max compression
+gzip compressed data, was "func_bk-1.5.3.tar", last modified: Sat Jun  1 13:06:25 2024, max compression
```

## Comparing `func_bk-1.5.1.tar` & `func_bk-1.5.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 12:58:51.881334 func_bk-1.5.1/
--rw-rw-rw-   0        0        0     3482 2024-06-01 12:58:51.881334 func_bk-1.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     3267 2024-06-01 12:58:41.000000 func_bk-1.5.1/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 12:58:51.875334 func_bk-1.5.1/func_bk/
--rw-rw-rw-   0        0        0     2574 2024-06-01 12:17:14.000000 func_bk-1.5.1/func_bk/__init__.py
--rw-rw-rw-   0        0        0     1719 2024-05-30 12:33:24.000000 func_bk-1.5.1/func_bk/django.py
--rw-rw-rw-   0        0        0     3425 2024-06-01 12:54:03.000000 func_bk-1.5.1/func_bk/fast_api.py
-drwxrwxrwx   0        0        0        0 2024-06-01 12:58:51.880334 func_bk-1.5.1/func_bk.egg-info/
--rw-rw-rw-   0        0        0     3482 2024-06-01 12:58:51.000000 func_bk-1.5.1/func_bk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-06-01 12:58:51.000000 func_bk-1.5.1/func_bk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 12:58:51.000000 func_bk-1.5.1/func_bk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-06-01 12:58:51.000000 func_bk-1.5.1/func_bk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2024-06-01 12:58:51.000000 func_bk-1.5.1/func_bk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2024-06-01 12:58:51.882337 func_bk-1.5.1/setup.cfg
--rw-rw-rw-   0        0        0      492 2024-06-01 12:17:34.000000 func_bk-1.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:06:25.413606 func_bk-1.5.3/
+-rw-rw-rw-   0        0        0     3482 2024-06-01 13:06:25.413606 func_bk-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2024-06-01 12:58:41.000000 func_bk-1.5.3/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 13:06:25.406606 func_bk-1.5.3/func_bk/
+-rw-rw-rw-   0        0        0     2574 2024-06-01 12:17:14.000000 func_bk-1.5.3/func_bk/__init__.py
+-rw-rw-rw-   0        0        0     1719 2024-05-30 12:33:24.000000 func_bk-1.5.3/func_bk/django.py
+-rw-rw-rw-   0        0        0     3637 2024-06-01 13:05:51.000000 func_bk-1.5.3/func_bk/fast_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:06:25.412607 func_bk-1.5.3/func_bk.egg-info/
+-rw-rw-rw-   0        0        0     3482 2024-06-01 13:06:25.000000 func_bk-1.5.3/func_bk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-06-01 13:06:25.000000 func_bk-1.5.3/func_bk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 13:06:25.000000 func_bk-1.5.3/func_bk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-06-01 13:06:25.000000 func_bk-1.5.3/func_bk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-06-01 13:06:25.000000 func_bk-1.5.3/func_bk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2024-06-01 13:06:25.414605 func_bk-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      492 2024-06-01 12:17:34.000000 func_bk-1.5.3/setup.py
```

### Comparing `func_bk-1.5.1/PKG-INFO` & `func_bk-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.5.1
+Version: 1.5.3
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
```

### Comparing `func_bk-1.5.1/README.md` & `func_bk-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `func_bk-1.5.1/func_bk/__init__.py` & `func_bk-1.5.3/func_bk/__init__.py`

 * *Files identical despite different names*

### Comparing `func_bk-1.5.1/func_bk/django.py` & `func_bk-1.5.3/func_bk/django.py`

 * *Files identical despite different names*

### Comparing `func_bk-1.5.1/func_bk/fast_api.py` & `func_bk-1.5.3/func_bk/fast_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,20 @@
 
 class Label():
     type: str
     id: str
     placeholder: str
     help_text: str
     style_input:str
+    def __init__(self,atype,aid,place = None,help = None,style = None):
+        self.type=atype
+        self.id=aid
+        self.placeholder=place
+        self.help_text=help
+        self.style_input=style
 
 
 
 class BForm():
     def labels(self):
         a=[]
         for i in self.__dict__.items():
```

### Comparing `func_bk-1.5.1/func_bk.egg-info/PKG-INFO` & `func_bk-1.5.3/func_bk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.5.1
+Version: 1.5.3
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
```

