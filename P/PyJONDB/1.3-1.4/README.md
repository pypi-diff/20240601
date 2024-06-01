# Comparing `tmp/pyjondb-1.3.tar.gz` & `tmp/pyjondb-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjondb-1.3.tar", last modified: Sat Jun  1 00:50:57 2024, max compression
+gzip compressed data, was "pyjondb-1.4.tar", last modified: Sat Jun  1 00:52:32 2024, max compression
```

## Comparing `pyjondb-1.3.tar` & `pyjondb-1.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 00:50:57.930015 pyjondb-1.3/
--rw-rw-rw-   0        0        0     2720 2024-06-01 00:50:57.929016 pyjondb-1.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-01 00:50:57.926980 pyjondb-1.3/PyJONDB.egg-info/
--rw-rw-rw-   0        0        0     2720 2024-06-01 00:50:57.000000 pyjondb-1.3/PyJONDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2024-06-01 00:50:57.000000 pyjondb-1.3/PyJONDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 00:50:57.000000 pyjondb-1.3/PyJONDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-06-01 00:50:57.000000 pyjondb-1.3/PyJONDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-06-01 00:50:57.000000 pyjondb-1.3/PyJONDB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-01 00:50:57.925427 pyjondb-1.3/pyjondb/
--rw-rw-rw-   0        0        0    15374 2024-06-01 00:07:16.000000 pyjondb-1.3/pyjondb/__init__.py
--rw-rw-rw-   0        0        0       42 2024-06-01 00:50:57.930015 pyjondb-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1713 2024-06-01 00:50:33.000000 pyjondb-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:52:32.318663 pyjondb-1.4/
+-rw-rw-rw-   0        0        0     2720 2024-06-01 00:52:32.316206 pyjondb-1.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 00:52:32.315198 pyjondb-1.4/PyJONDB.egg-info/
+-rw-rw-rw-   0        0        0     2720 2024-06-01 00:52:32.000000 pyjondb-1.4/PyJONDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2024-06-01 00:52:32.000000 pyjondb-1.4/PyJONDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 00:52:32.000000 pyjondb-1.4/PyJONDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-06-01 00:52:32.000000 pyjondb-1.4/PyJONDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-01 00:52:32.000000 pyjondb-1.4/PyJONDB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 00:52:32.313119 pyjondb-1.4/pyjondb/
+-rw-rw-rw-   0        0        0    15374 2024-06-01 00:07:16.000000 pyjondb-1.4/pyjondb/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 00:52:32.318802 pyjondb-1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1744 2024-06-01 00:52:25.000000 pyjondb-1.4/setup.py
```

### Comparing `pyjondb-1.3/PKG-INFO` & `pyjondb-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJONDB
-Version: 1.3
+Version: 1.4
 Summary: A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.
 Home-page: https://tago.works/
 Author: t-a-g-o
 Author-email: santiago@tago.works
 Project-URL: Bug Reports, https://github.com/t-a-g-o/PyJONDB/issues
 Project-URL: Source, https://github.com/t-a-g-o/PyJONDB/
 Keywords: encryption database,encrypted database,json database,secure storage,lightweight database,document store,fernet encryption,cryptography,data security,data encryption,collections,document operations,aggregation,query,NoSQL,python database,uuid,file-based database,local database,secure json,nested data,tree structure,data management,data linkage,collection linking
```

### Comparing `pyjondb-1.3/PyJONDB.egg-info/PKG-INFO` & `pyjondb-1.4/PyJONDB.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJONDB
-Version: 1.3
+Version: 1.4
 Summary: A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.
 Home-page: https://tago.works/
 Author: t-a-g-o
 Author-email: santiago@tago.works
 Project-URL: Bug Reports, https://github.com/t-a-g-o/PyJONDB/issues
 Project-URL: Source, https://github.com/t-a-g-o/PyJONDB/
 Keywords: encryption database,encrypted database,json database,secure storage,lightweight database,document store,fernet encryption,cryptography,data security,data encryption,collections,document operations,aggregation,query,NoSQL,python database,uuid,file-based database,local database,secure json,nested data,tree structure,data management,data linkage,collection linking
```

### Comparing `pyjondb-1.3/pyjondb/__init__.py` & `pyjondb-1.4/pyjondb/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjondb-1.3/setup.py` & `pyjondb-1.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 import os
 
 with open(os.path.join(os.path.dirname(__file__), 'pypi.readme'), encoding='utf-8') as f:
     desc = f.read()
 
 setup(
     name='PyJONDB',
-    version='1.3',
+    version='1.4',
     description='A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.',
     long_description=desc,
     long_description_content_type='text/markdown',
     author='t-a-g-o',
+    data_files="pypi.readme",
     author_email='santiago@tago.works',
     url='https://tago.works/',
     packages=find_packages(),
     install_requires=[
         'cryptography',
     ],
     classifiers=[
```

