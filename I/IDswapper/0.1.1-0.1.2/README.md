# Comparing `tmp/idswapper-0.1.1.tar.gz` & `tmp/idswapper-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idswapper-0.1.1.tar", last modified: Sat Jun  1 11:09:06 2024, max compression
+gzip compressed data, was "idswapper-0.1.2.tar", last modified: Sat Jun  1 11:34:06 2024, max compression
```

## Comparing `idswapper-0.1.1.tar` & `idswapper-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 11:09:06.061595 idswapper-0.1.1/
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 11:09:06.061595 idswapper-0.1.1/IDswapper.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2404 2024-06-01 11:09:06.000000 idswapper-0.1.1/IDswapper.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      332 2024-06-01 11:09:06.000000 idswapper-0.1.1/IDswapper.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 11:09:06.000000 idswapper-0.1.1/IDswapper.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       59 2024-06-01 11:09:06.000000 idswapper-0.1.1/IDswapper.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       43 2024-06-01 11:09:06.000000 idswapper-0.1.1/IDswapper.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-06-01 11:09:06.000000 idswapper-0.1.1/IDswapper.egg-info/top_level.txt
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2404 2024-06-01 11:09:06.061595 idswapper-0.1.1/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1845 2024-06-01 10:30:34.000000 idswapper-0.1.1/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 11:09:06.061595 idswapper-0.1.1/idswapper/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:26:54.000000 idswapper-0.1.1/idswapper/__init__.py
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)  5658381 2024-05-31 18:35:15.000000 idswapper-0.1.1/idswapper/data_file.gz
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)      115 2024-05-31 18:35:15.000000 idswapper-0.1.1/idswapper/db_config.json
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     8399 2024-06-01 10:39:40.000000 idswapper-0.1.1/idswapper/fetchids.py
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     7616 2024-05-31 20:34:58.000000 idswapper-0.1.1/idswapper/setup_db.py
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 11:09:06.061595 idswapper-0.1.1/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      981 2024-06-01 11:08:13.000000 idswapper-0.1.1/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 11:34:06.095809 idswapper-0.1.2/
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 11:34:06.095809 idswapper-0.1.2/IDswapper.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2404 2024-06-01 11:34:06.000000 idswapper-0.1.2/IDswapper.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      332 2024-06-01 11:34:06.000000 idswapper-0.1.2/IDswapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 11:34:06.000000 idswapper-0.1.2/IDswapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       59 2024-06-01 11:34:06.000000 idswapper-0.1.2/IDswapper.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       43 2024-06-01 11:34:06.000000 idswapper-0.1.2/IDswapper.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-06-01 11:34:06.000000 idswapper-0.1.2/IDswapper.egg-info/top_level.txt
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2404 2024-06-01 11:34:06.095809 idswapper-0.1.2/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1845 2024-06-01 10:30:34.000000 idswapper-0.1.2/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 11:34:06.095809 idswapper-0.1.2/idswapper/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-31 18:34:45.000000 idswapper-0.1.2/idswapper/__init__.py
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)  5658381 2024-05-31 18:35:15.000000 idswapper-0.1.2/idswapper/data_file.gz
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)      115 2024-05-31 18:35:15.000000 idswapper-0.1.2/idswapper/db_config.json
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     8399 2024-06-01 10:39:40.000000 idswapper-0.1.2/idswapper/fetchids.py
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     7616 2024-05-31 20:34:58.000000 idswapper-0.1.2/idswapper/setup_db.py
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 11:34:06.095809 idswapper-0.1.2/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      981 2024-06-01 11:25:21.000000 idswapper-0.1.2/setup.py
```

### Comparing `idswapper-0.1.1/IDswapper.egg-info/PKG-INFO` & `idswapper-0.1.2/IDswapper.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IDswapper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool for swapping IDs in a file by fetching various IDs from idswapper database
 Home-page: https://github.com/vkulaganathan/IDswapper/
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `idswapper-0.1.1/PKG-INFO` & `idswapper-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IDswapper
-Version: 0.1.1
+Version: 0.1.2
 Summary: A tool for swapping IDs in a file by fetching various IDs from idswapper database
 Home-page: https://github.com/vkulaganathan/IDswapper/
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `idswapper-0.1.1/README.md` & `idswapper-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `idswapper-0.1.1/idswapper/data_file.gz` & `idswapper-0.1.2/idswapper/data_file.gz`

 * *Files identical despite different names*

### Comparing `idswapper-0.1.1/idswapper/fetchids.py` & `idswapper-0.1.2/idswapper/fetchids.py`

 * *Files identical despite different names*

### Comparing `idswapper-0.1.1/idswapper/setup_db.py` & `idswapper-0.1.2/idswapper/setup_db.py`

 * *Files identical despite different names*

### Comparing `idswapper-0.1.1/setup.py` & `idswapper-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='IDswapper',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'IDswapper=idswapper.fetchids:fetch_ids'
         ]
     },
     install_requires=[
```
