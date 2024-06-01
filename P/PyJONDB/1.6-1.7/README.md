# Comparing `tmp/pyjondb-1.6.tar.gz` & `tmp/pyjondb-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjondb-1.6.tar", last modified: Sat Jun  1 06:03:14 2024, max compression
+gzip compressed data, was "pyjondb-1.7.tar", last modified: Sat Jun  1 06:30:33 2024, max compression
```

## Comparing `pyjondb-1.6.tar` & `pyjondb-1.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 06:03:14.102083 pyjondb-1.6/
--rw-rw-rw-   0        0        0     1085 2024-06-01 01:14:36.000000 pyjondb-1.6/LICENSE
--rw-rw-rw-   0        0        0     2707 2024-06-01 06:03:14.100081 pyjondb-1.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-01 06:03:14.099081 pyjondb-1.6/PyJONDB.egg-info/
--rw-rw-rw-   0        0        0     2707 2024-06-01 06:03:14.000000 pyjondb-1.6/PyJONDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-06-01 06:03:14.000000 pyjondb-1.6/PyJONDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 06:03:14.000000 pyjondb-1.6/PyJONDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-06-01 06:03:14.000000 pyjondb-1.6/PyJONDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 06:03:14.000000 pyjondb-1.6/PyJONDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3008 2024-06-01 06:00:21.000000 pyjondb-1.6/README.md
--rw-rw-rw-   0        0        0     1628 2024-06-01 06:02:25.000000 pyjondb-1.6/pypi.readme
--rw-rw-rw-   0        0        0       42 2024-06-01 06:03:14.102083 pyjondb-1.6/setup.cfg
--rw-rw-rw-   0        0        0     1754 2024-06-01 06:01:33.000000 pyjondb-1.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 06:30:33.936293 pyjondb-1.7/
+-rw-rw-rw-   0        0        0     1085 2024-06-01 01:14:36.000000 pyjondb-1.7/LICENSE
+-rw-rw-rw-   0        0        0     2707 2024-06-01 06:30:33.934788 pyjondb-1.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 06:30:33.933787 pyjondb-1.7/PyJONDB.egg-info/
+-rw-rw-rw-   0        0        0     2707 2024-06-01 06:30:33.000000 pyjondb-1.7/PyJONDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-06-01 06:30:33.000000 pyjondb-1.7/PyJONDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 06:30:33.000000 pyjondb-1.7/PyJONDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-06-01 06:30:33.000000 pyjondb-1.7/PyJONDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 06:30:33.000000 pyjondb-1.7/PyJONDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3008 2024-06-01 06:00:21.000000 pyjondb-1.7/README.md
+-rw-rw-rw-   0        0        0     1628 2024-06-01 06:02:25.000000 pyjondb-1.7/pypi.readme
+-rw-rw-rw-   0        0        0       42 2024-06-01 06:30:33.936293 pyjondb-1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1754 2024-06-01 06:30:21.000000 pyjondb-1.7/setup.py
```

### Comparing `pyjondb-1.6/LICENSE` & `pyjondb-1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjondb-1.6/PKG-INFO` & `pyjondb-1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJONDB
-Version: 1.6
+Version: 1.7
 Summary: A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.
 Home-page: https://tago.works/
 Author: t-a-g-o
 Author-email: santiago@tago.works
 Project-URL: Bug Reports, https://github.com/t-a-g-o/PyJONDB/issues
 Project-URL: Source, https://github.com/t-a-g-o/PyJONDB/
 Keywords: encryption database,encrypted database,json database,secure storage,lightweight database,document store,fernet encryption,cryptography,data security,data encryption,collections,document operations,aggregation,query,NoSQL,python database,uuid,file-based database,local database,secure json,nested data,tree structure,data management,data linkage,collection linking
```

### Comparing `pyjondb-1.6/PyJONDB.egg-info/PKG-INFO` & `pyjondb-1.7/PyJONDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJONDB
-Version: 1.6
+Version: 1.7
 Summary: A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.
 Home-page: https://tago.works/
 Author: t-a-g-o
 Author-email: santiago@tago.works
 Project-URL: Bug Reports, https://github.com/t-a-g-o/PyJONDB/issues
 Project-URL: Source, https://github.com/t-a-g-o/PyJONDB/
 Keywords: encryption database,encrypted database,json database,secure storage,lightweight database,document store,fernet encryption,cryptography,data security,data encryption,collections,document operations,aggregation,query,NoSQL,python database,uuid,file-based database,local database,secure json,nested data,tree structure,data management,data linkage,collection linking
```

### Comparing `pyjondb-1.6/README.md` & `pyjondb-1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyjondb-1.6/pypi.readme` & `pyjondb-1.7/pypi.readme`

 * *Files identical despite different names*

### Comparing `pyjondb-1.6/setup.py` & `pyjondb-1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 with open(os.path.join(os.path.dirname(__file__), 'pypi.readme'), encoding='utf-8') as f:
     desc = f.read()
 
 setup(
     name='PyJONDB',
-    version='1.6',
+    version='1.7',
     description='A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.',
     long_description=desc,
     long_description_content_type='text/markdown',
     author='t-a-g-o',
     author_email='santiago@tago.works',
     url='https://tago.works/',
     packages=find_packages(),
```

