# Comparing `tmp/pyjondb-1.7.tar.gz` & `tmp/pyjondb-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjondb-1.7.tar", last modified: Sat Jun  1 06:30:33 2024, max compression
+gzip compressed data, was "pyjondb-1.8.tar", last modified: Sat Jun  1 15:58:05 2024, max compression
```

## Comparing `pyjondb-1.7.tar` & `pyjondb-1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 06:30:33.936293 pyjondb-1.7/
--rw-rw-rw-   0        0        0     1085 2024-06-01 01:14:36.000000 pyjondb-1.7/LICENSE
--rw-rw-rw-   0        0        0     2707 2024-06-01 06:30:33.934788 pyjondb-1.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-01 06:30:33.933787 pyjondb-1.7/PyJONDB.egg-info/
--rw-rw-rw-   0        0        0     2707 2024-06-01 06:30:33.000000 pyjondb-1.7/PyJONDB.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      192 2024-06-01 06:30:33.000000 pyjondb-1.7/PyJONDB.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 06:30:33.000000 pyjondb-1.7/PyJONDB.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-06-01 06:30:33.000000 pyjondb-1.7/PyJONDB.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 06:30:33.000000 pyjondb-1.7/PyJONDB.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3008 2024-06-01 06:00:21.000000 pyjondb-1.7/README.md
--rw-rw-rw-   0        0        0     1628 2024-06-01 06:02:25.000000 pyjondb-1.7/pypi.readme
--rw-rw-rw-   0        0        0       42 2024-06-01 06:30:33.936293 pyjondb-1.7/setup.cfg
--rw-rw-rw-   0        0        0     1754 2024-06-01 06:30:21.000000 pyjondb-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:58:05.721443 pyjondb-1.8/
+-rw-rw-rw-   0        0        0     1085 2024-06-01 01:14:36.000000 pyjondb-1.8/LICENSE
+-rw-rw-rw-   0        0        0     2707 2024-06-01 15:58:05.720437 pyjondb-1.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-06-01 15:58:05.717929 pyjondb-1.8/PyJONDB.egg-info/
+-rw-rw-rw-   0        0        0     2707 2024-06-01 15:58:05.000000 pyjondb-1.8/PyJONDB.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      192 2024-06-01 15:58:05.000000 pyjondb-1.8/PyJONDB.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:58:05.000000 pyjondb-1.8/PyJONDB.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-06-01 15:58:05.000000 pyjondb-1.8/PyJONDB.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:58:05.000000 pyjondb-1.8/PyJONDB.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3008 2024-06-01 06:00:21.000000 pyjondb-1.8/README.md
+-rw-rw-rw-   0        0        0     1628 2024-06-01 06:02:25.000000 pyjondb-1.8/pypi.readme
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:58:05.721443 pyjondb-1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1812 2024-06-01 15:58:03.000000 pyjondb-1.8/setup.py
```

### Comparing `pyjondb-1.7/LICENSE` & `pyjondb-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyjondb-1.7/PKG-INFO` & `pyjondb-1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJONDB
-Version: 1.7
+Version: 1.8
 Summary: A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.
 Home-page: https://tago.works/
 Author: t-a-g-o
 Author-email: santiago@tago.works
 Project-URL: Bug Reports, https://github.com/t-a-g-o/PyJONDB/issues
 Project-URL: Source, https://github.com/t-a-g-o/PyJONDB/
 Keywords: encryption database,encrypted database,json database,secure storage,lightweight database,document store,fernet encryption,cryptography,data security,data encryption,collections,document operations,aggregation,query,NoSQL,python database,uuid,file-based database,local database,secure json,nested data,tree structure,data management,data linkage,collection linking
```

### Comparing `pyjondb-1.7/PyJONDB.egg-info/PKG-INFO` & `pyjondb-1.8/PyJONDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyJONDB
-Version: 1.7
+Version: 1.8
 Summary: A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.
 Home-page: https://tago.works/
 Author: t-a-g-o
 Author-email: santiago@tago.works
 Project-URL: Bug Reports, https://github.com/t-a-g-o/PyJONDB/issues
 Project-URL: Source, https://github.com/t-a-g-o/PyJONDB/
 Keywords: encryption database,encrypted database,json database,secure storage,lightweight database,document store,fernet encryption,cryptography,data security,data encryption,collections,document operations,aggregation,query,NoSQL,python database,uuid,file-based database,local database,secure json,nested data,tree structure,data management,data linkage,collection linking
```

### Comparing `pyjondb-1.7/README.md` & `pyjondb-1.8/README.md`

 * *Files identical despite different names*

### Comparing `pyjondb-1.7/pypi.readme` & `pyjondb-1.8/pypi.readme`

 * *Files identical despite different names*

### Comparing `pyjondb-1.7/setup.py` & `pyjondb-1.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 import os
 
 with open(os.path.join(os.path.dirname(__file__), 'pypi.readme'), encoding='utf-8') as f:
     desc = f.read()
 
 setup(
     name='PyJONDB',
-    version='1.7',
+    version='1.8',
     description='A lightweight, encrypted JSON-based database with support for collections, document operations, and aggregation.',
     long_description=desc,
     long_description_content_type='text/markdown',
     author='t-a-g-o',
     author_email='santiago@tago.works',
     url='https://tago.works/',
-    packages=find_packages(),
+    packages=find_packages(include=['pyjondb', 'pyjondb.session', 'pyjondb.database']),
     install_requires=[
         'cryptography',
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Libraries',
```

