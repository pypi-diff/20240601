# Comparing `tmp/func_bk-1.5.3.tar.gz` & `tmp/func_bk-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_bk-1.5.3.tar", last modified: Sat Jun  1 13:06:25 2024, max compression
+gzip compressed data, was "func_bk-1.5.4.tar", last modified: Sat Jun  1 14:08:49 2024, max compression
```

## Comparing `func_bk-1.5.3.tar` & `func_bk-1.5.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 13:06:25.413606 func_bk-1.5.3/
--rw-rw-rw-   0        0        0     3482 2024-06-01 13:06:25.413606 func_bk-1.5.3/PKG-INFO
--rw-rw-rw-   0        0        0     3267 2024-06-01 12:58:41.000000 func_bk-1.5.3/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 13:06:25.406606 func_bk-1.5.3/func_bk/
--rw-rw-rw-   0        0        0     2574 2024-06-01 12:17:14.000000 func_bk-1.5.3/func_bk/__init__.py
--rw-rw-rw-   0        0        0     1719 2024-05-30 12:33:24.000000 func_bk-1.5.3/func_bk/django.py
--rw-rw-rw-   0        0        0     3637 2024-06-01 13:05:51.000000 func_bk-1.5.3/func_bk/fast_api.py
-drwxrwxrwx   0        0        0        0 2024-06-01 13:06:25.412607 func_bk-1.5.3/func_bk.egg-info/
--rw-rw-rw-   0        0        0     3482 2024-06-01 13:06:25.000000 func_bk-1.5.3/func_bk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-06-01 13:06:25.000000 func_bk-1.5.3/func_bk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 13:06:25.000000 func_bk-1.5.3/func_bk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-06-01 13:06:25.000000 func_bk-1.5.3/func_bk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2024-06-01 13:06:25.000000 func_bk-1.5.3/func_bk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2024-06-01 13:06:25.414605 func_bk-1.5.3/setup.cfg
--rw-rw-rw-   0        0        0      492 2024-06-01 12:17:34.000000 func_bk-1.5.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:08:49.255307 func_bk-1.5.4/
+-rw-rw-rw-   0        0        0     3482 2024-06-01 14:08:49.254306 func_bk-1.5.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3267 2024-06-01 12:58:41.000000 func_bk-1.5.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 14:08:49.248303 func_bk-1.5.4/func_bk/
+-rw-rw-rw-   0        0        0     2574 2024-06-01 12:17:14.000000 func_bk-1.5.4/func_bk/__init__.py
+-rw-rw-rw-   0        0        0     1719 2024-05-30 12:33:24.000000 func_bk-1.5.4/func_bk/django.py
+-rw-rw-rw-   0        0        0     3597 2024-06-01 14:08:41.000000 func_bk-1.5.4/func_bk/fast_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 14:08:49.254306 func_bk-1.5.4/func_bk.egg-info/
+-rw-rw-rw-   0        0        0     3482 2024-06-01 14:08:49.000000 func_bk-1.5.4/func_bk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-06-01 14:08:49.000000 func_bk-1.5.4/func_bk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 14:08:49.000000 func_bk-1.5.4/func_bk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-06-01 14:08:49.000000 func_bk-1.5.4/func_bk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-06-01 14:08:49.000000 func_bk-1.5.4/func_bk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2024-06-01 14:08:49.256304 func_bk-1.5.4/setup.cfg
+-rw-rw-rw-   0        0        0      492 2024-06-01 12:17:34.000000 func_bk-1.5.4/setup.py
```

### Comparing `func_bk-1.5.3/PKG-INFO` & `func_bk-1.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.5.3
+Version: 1.5.4
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
```

### Comparing `func_bk-1.5.3/README.md` & `func_bk-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `func_bk-1.5.3/func_bk/__init__.py` & `func_bk-1.5.4/func_bk/__init__.py`

 * *Files identical despite different names*

### Comparing `func_bk-1.5.3/func_bk/django.py` & `func_bk-1.5.4/func_bk/django.py`

 * *Files identical despite different names*

### Comparing `func_bk-1.5.3/func_bk/fast_api.py` & `func_bk-1.5.4/func_bk/fast_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,15 @@
 
 
 
 class BForm():
     def labels(self):
         a=[]
         for i in self.__dict__.items():
-            if i.__class__==Label:
-                a.append(i)
+            a.append(i)
         return a
 
     def as_p(self):
         a=''
         all=self.labels()
 
         for i in all:
```

### Comparing `func_bk-1.5.3/func_bk.egg-info/PKG-INFO` & `func_bk-1.5.4/func_bk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.5.3
+Version: 1.5.4
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
```

