# Comparing `tmp/func_bk-1.3.6.tar.gz` & `tmp/func_bk-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "func_bk-1.3.6.tar", last modified: Thu May 30 14:56:44 2024, max compression
+gzip compressed data, was "func_bk-1.3.7.tar", last modified: Sat Jun  1 11:48:31 2024, max compression
```

## Comparing `func_bk-1.3.6.tar` & `func_bk-1.3.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-30 14:56:44.713737 func_bk-1.3.6/
--rw-rw-rw-   0        0        0     2994 2024-05-30 14:56:44.712736 func_bk-1.3.6/PKG-INFO
--rw-rw-rw-   0        0        0     2777 2024-05-30 12:32:20.000000 func_bk-1.3.6/README.md
-drwxrwxrwx   0        0        0        0 2024-05-30 14:56:44.706736 func_bk-1.3.6/func_bk/
--rw-rw-rw-   0        0        0     2491 2024-05-30 10:23:47.000000 func_bk-1.3.6/func_bk/__init__.py
--rw-rw-rw-   0        0        0     1719 2024-05-30 12:33:24.000000 func_bk-1.3.6/func_bk/django.py
--rw-rw-rw-   0        0        0     7029 2024-05-30 14:56:36.000000 func_bk-1.3.6/func_bk/fast_api.py
-drwxrwxrwx   0        0        0        0 2024-05-30 14:56:44.711739 func_bk-1.3.6/func_bk.egg-info/
--rw-rw-rw-   0        0        0     2994 2024-05-30 14:56:44.000000 func_bk-1.3.6/func_bk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2024-05-30 14:56:44.000000 func_bk-1.3.6/func_bk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-30 14:56:44.000000 func_bk-1.3.6/func_bk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-05-30 14:56:44.000000 func_bk-1.3.6/func_bk.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2024-05-30 14:56:44.000000 func_bk-1.3.6/func_bk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2024-05-30 14:56:44.713737 func_bk-1.3.6/setup.cfg
--rw-rw-rw-   0        0        0      492 2024-05-30 12:34:31.000000 func_bk-1.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:48:31.891839 func_bk-1.3.7/
+-rw-rw-rw-   0        0        0     2994 2024-06-01 11:48:31.891839 func_bk-1.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2777 2024-05-30 12:32:20.000000 func_bk-1.3.7/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 11:48:31.884839 func_bk-1.3.7/func_bk/
+-rw-rw-rw-   0        0        0     2491 2024-05-30 10:23:47.000000 func_bk-1.3.7/func_bk/__init__.py
+-rw-rw-rw-   0        0        0     1719 2024-05-30 12:33:24.000000 func_bk-1.3.7/func_bk/django.py
+-rw-rw-rw-   0        0        0     2713 2024-06-01 11:48:02.000000 func_bk-1.3.7/func_bk/fast_api.py
+drwxrwxrwx   0        0        0        0 2024-06-01 11:48:31.890839 func_bk-1.3.7/func_bk.egg-info/
+-rw-rw-rw-   0        0        0     2994 2024-06-01 11:48:31.000000 func_bk-1.3.7/func_bk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      240 2024-06-01 11:48:31.000000 func_bk-1.3.7/func_bk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 11:48:31.000000 func_bk-1.3.7/func_bk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-06-01 11:48:31.000000 func_bk-1.3.7/func_bk.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2024-06-01 11:48:31.000000 func_bk-1.3.7/func_bk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2024-06-01 11:48:31.892839 func_bk-1.3.7/setup.cfg
+-rw-rw-rw-   0        0        0      492 2024-05-30 12:34:31.000000 func_bk-1.3.7/setup.py
```

### Comparing `func_bk-1.3.6/PKG-INFO` & `func_bk-1.3.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.3.6
+Version: 1.3.7
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
```

### Comparing `func_bk-1.3.6/README.md` & `func_bk-1.3.7/README.md`

 * *Files identical despite different names*

### Comparing `func_bk-1.3.6/func_bk/__init__.py` & `func_bk-1.3.7/func_bk/__init__.py`

 * *Files identical despite different names*

### Comparing `func_bk-1.3.6/func_bk/django.py` & `func_bk-1.3.7/func_bk/django.py`

 * *Files identical despite different names*

### Comparing `func_bk-1.3.6/func_bk.egg-info/PKG-INFO` & `func_bk-1.3.7/func_bk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: func_bk
-Version: 1.3.6
+Version: 1.3.7
 Summary: add function for normal python and add class(for inheritance) for django
 Author-email: lilo.pio147@mail.ru
 Description-Content-Type: text/markdown
 
 add function 
 
 sejango - 3 arguments form(django),key(in form cleaned data),var(return if key is not find)
```

