# Comparing `tmp/pyjondb-1.1.tar.gz` & `tmp/pyjondb-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjondb-1.1.tar", last modified: Sat Jun  1 00:32:19 2024, max compression
+gzip compressed data, was "pyjondb-1.2.tar", last modified: Sat Jun  1 00:35:00 2024, max compression
```

## Comparing `pyjondb-1.1.tar` & `pyjondb-1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 00:32:19.248740 pyjondb-1.1/
--rw-rw-rw-   0        0        0     2732 2024-06-01 00:32:19.247740 pyjondb-1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-01 00:32:19.245473 pyjondb-1.1/PyJONDB.egg-info/
--rw-rw-rw-   0        0        0     2732 2024-06-01 00:32:19.000000 pyjondb-1.1/PyJONDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2024-06-01 00:32:19.000000 pyjondb-1.1/PyJONDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 00:32:19.000000 pyjondb-1.1/PyJONDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-06-01 00:32:19.000000 pyjondb-1.1/PyJONDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-06-01 00:32:19.000000 pyjondb-1.1/PyJONDB.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-01 00:32:19.244471 pyjondb-1.1/pyjondb/
--rw-rw-rw-   0        0        0    15374 2024-06-01 00:07:16.000000 pyjondb-1.1/pyjondb/__init__.py
--rw-rw-rw-   0        0        0       42 2024-06-01 00:32:19.248740 pyjondb-1.1/setup.cfg
--rw-rw-rw-   0        0        0     1669 2024-06-01 00:32:16.000000 pyjondb-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 00:35:00.389490 pyjondb-1.2/
+-rw-rw-rw-   0        0        0     2720 2024-06-01 00:35:00.388487 pyjondb-1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 00:35:00.387486 pyjondb-1.2/PyJONDB.egg-info/
+-rw-rw-rw-   0        0        0     2720 2024-06-01 00:35:00.000000 pyjondb-1.2/PyJONDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2024-06-01 00:35:00.000000 pyjondb-1.2/PyJONDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 00:35:00.000000 pyjondb-1.2/PyJONDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-06-01 00:35:00.000000 pyjondb-1.2/PyJONDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-06-01 00:35:00.000000 pyjondb-1.2/PyJONDB.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 00:35:00.385482 pyjondb-1.2/pyjondb/
+-rw-rw-rw-   0        0        0    15374 2024-06-01 00:07:16.000000 pyjondb-1.2/pyjondb/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 00:35:00.390487 pyjondb-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1654 2024-06-01 00:34:52.000000 pyjondb-1.2/setup.py
```

### Comparing `pyjondb-1.1/PKG-INFO` & `pyjondb-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: PyJONDB
-Version: 1.1
+Version: 1.2
 Summary: A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.
-Home-page: https://github.com/t-a-g-o/PyJONDB
+Home-page: https://tago.works/
 Author: t-a-g-o
 Author-email: santiago@tago.works
 Project-URL: Bug Reports, https://github.com/t-a-g-o/PyJONDB/issues
 Project-URL: Source, https://github.com/t-a-g-o/PyJONDB/
 Keywords: encryption database,encrypted database,json database,secure storage,lightweight database,document store,fernet encryption,cryptography,data security,data encryption,collections,document operations,aggregation,query,NoSQL,python database,uuid,file-based database,local database,secure json,nested data,tree structure,data management,data linkage,collection linking
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -53,9 +53,9 @@
 
 # Update a document in the collection
 document_id = results[0]['_id']
 db.update_document('mycollection', document_id, {'age': 31})
 
 # Delete a document from the collection
 db.delete_document('mycollection', document_id)
-
+```
 ### Learn more about it at the docs: https://github.com/t-a-g-o/PyJONDB/wiki
```

### Comparing `pyjondb-1.1/PyJONDB.egg-info/PKG-INFO` & `pyjondb-1.2/PyJONDB.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: PyJONDB
-Version: 1.1
+Version: 1.2
 Summary: A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.
-Home-page: https://github.com/t-a-g-o/PyJONDB
+Home-page: https://tago.works/
 Author: t-a-g-o
 Author-email: santiago@tago.works
 Project-URL: Bug Reports, https://github.com/t-a-g-o/PyJONDB/issues
 Project-URL: Source, https://github.com/t-a-g-o/PyJONDB/
 Keywords: encryption database,encrypted database,json database,secure storage,lightweight database,document store,fernet encryption,cryptography,data security,data encryption,collections,document operations,aggregation,query,NoSQL,python database,uuid,file-based database,local database,secure json,nested data,tree structure,data management,data linkage,collection linking
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -53,9 +53,9 @@
 
 # Update a document in the collection
 document_id = results[0]['_id']
 db.update_document('mycollection', document_id, {'age': 31})
 
 # Delete a document from the collection
 db.delete_document('mycollection', document_id)
-
+```
 ### Learn more about it at the docs: https://github.com/t-a-g-o/PyJONDB/wiki
```

### Comparing `pyjondb-1.1/pyjondb/__init__.py` & `pyjondb-1.2/pyjondb/__init__.py`

 * *Files identical despite different names*

### Comparing `pyjondb-1.1/setup.py` & `pyjondb-1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 import os
 
 desc = open('./database-viewer/pypi.readme').read()
 
 setup(
     name='PyJONDB',
-    version='1.1',
+    version='1.2',
     description='A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.',
     long_description=desc,
     long_description_content_type='text/markdown',
     author='t-a-g-o',
     author_email='santiago@tago.works',
-    url='https://github.com/t-a-g-o/PyJONDB',
+    url='https://tago.works/',
     packages=find_packages(),
     install_requires=[
         'cryptography',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

