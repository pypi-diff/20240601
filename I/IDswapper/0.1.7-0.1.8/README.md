# Comparing `tmp/idswapper-0.1.7.tar.gz` & `tmp/idswapper-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idswapper-0.1.7.tar", last modified: Sat Jun  1 12:24:40 2024, max compression
+gzip compressed data, was "idswapper-0.1.8.tar", last modified: Sat Jun  1 12:37:38 2024, max compression
```

## Comparing `idswapper-0.1.7.tar` & `idswapper-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 12:24:40.744500 idswapper-0.1.7/
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 12:24:40.740500 idswapper-0.1.7/IDswapper/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-31 18:34:45.000000 idswapper-0.1.7/IDswapper/__init__.py
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)  5658381 2024-05-31 18:35:15.000000 idswapper-0.1.7/IDswapper/data_file.gz
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)      115 2024-05-31 18:35:15.000000 idswapper-0.1.7/IDswapper/db_config.json
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     8423 2024-06-01 12:22:28.000000 idswapper-0.1.7/IDswapper/fetchids.py
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 12:24:40.744500 idswapper-0.1.7/IDswapper.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2404 2024-06-01 12:24:40.000000 idswapper-0.1.7/IDswapper.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      310 2024-06-01 12:24:40.000000 idswapper-0.1.7/IDswapper.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 12:24:40.000000 idswapper-0.1.7/IDswapper.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       54 2024-06-01 12:24:40.000000 idswapper-0.1.7/IDswapper.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       43 2024-06-01 12:24:40.000000 idswapper-0.1.7/IDswapper.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-06-01 12:24:40.000000 idswapper-0.1.7/IDswapper.egg-info/top_level.txt
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2404 2024-06-01 12:24:40.744500 idswapper-0.1.7/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1845 2024-06-01 10:30:34.000000 idswapper-0.1.7/README.md
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 12:24:40.744500 idswapper-0.1.7/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      976 2024-06-01 12:19:32.000000 idswapper-0.1.7/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 12:37:38.286478 idswapper-0.1.8/
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 12:37:38.286478 idswapper-0.1.8/IDswapper/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)        0 2024-05-31 18:34:45.000000 idswapper-0.1.8/IDswapper/__init__.py
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)  5658381 2024-05-31 18:35:15.000000 idswapper-0.1.8/IDswapper/data_file.gz
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)      115 2024-05-31 18:35:15.000000 idswapper-0.1.8/IDswapper/db_config.json
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     8423 2024-06-01 12:22:28.000000 idswapper-0.1.8/IDswapper/fetchids.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 12:37:38.286478 idswapper-0.1.8/IDswapper.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2510 2024-06-01 12:37:38.000000 idswapper-0.1.8/IDswapper.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      310 2024-06-01 12:37:38.000000 idswapper-0.1.8/IDswapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 12:37:38.000000 idswapper-0.1.8/IDswapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       54 2024-06-01 12:37:38.000000 idswapper-0.1.8/IDswapper.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       43 2024-06-01 12:37:38.000000 idswapper-0.1.8/IDswapper.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-06-01 12:37:38.000000 idswapper-0.1.8/IDswapper.egg-info/top_level.txt
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2510 2024-06-01 12:37:38.286478 idswapper-0.1.8/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1951 2024-06-01 12:36:52.000000 idswapper-0.1.8/README.md
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 12:37:38.286478 idswapper-0.1.8/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      976 2024-06-01 12:28:01.000000 idswapper-0.1.8/setup.py
```

### Comparing `idswapper-0.1.7/IDswapper/data_file.gz` & `idswapper-0.1.8/IDswapper/data_file.gz`

 * *Files identical despite different names*

### Comparing `idswapper-0.1.7/IDswapper/fetchids.py` & `idswapper-0.1.8/IDswapper/fetchids.py`

 * *Files identical despite different names*

### Comparing `idswapper-0.1.7/IDswapper.egg-info/PKG-INFO` & `idswapper-0.1.8/IDswapper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IDswapper
-Version: 0.1.7
+Version: 0.1.8
 Summary: A tool for swapping IDs in a file by fetching various IDs from idswapper database
 Home-page: https://github.com/vkulaganathan/IDswapper/
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -72,12 +72,16 @@
 | ENSG00000146648 | P00533 | EGFR | 7p11.2 |
 | ENSG00000141510 | P04637 | TP53 | 17p13.1 |
 
 <br></br>
 
 **INSTALLATION**
 <br>`` $ pip install IDswapper ``</br>
-<br> Create the local database</br>
-``$ python setup_db.py``
 
+<br> Create the local idswapper database</br>
 <br> requires ``mysql`` up and running </br>
-<br> you can check using ``$ systemctl mysql status``</br>
+you can check using ``$ systemctl mysql status``
+<br>Next,</br> 
+<br>``$ python3 setup_db.py``<br>
+Make sure the entries match the mysql db configuration file``db_config.json`` 
+
+
```

### Comparing `idswapper-0.1.7/PKG-INFO` & `idswapper-0.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IDswapper
-Version: 0.1.7
+Version: 0.1.8
 Summary: A tool for swapping IDs in a file by fetching various IDs from idswapper database
 Home-page: https://github.com/vkulaganathan/IDswapper/
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -72,12 +72,16 @@
 | ENSG00000146648 | P00533 | EGFR | 7p11.2 |
 | ENSG00000141510 | P04637 | TP53 | 17p13.1 |
 
 <br></br>
 
 **INSTALLATION**
 <br>`` $ pip install IDswapper ``</br>
-<br> Create the local database</br>
-``$ python setup_db.py``
 
+<br> Create the local idswapper database</br>
 <br> requires ``mysql`` up and running </br>
-<br> you can check using ``$ systemctl mysql status``</br>
+you can check using ``$ systemctl mysql status``
+<br>Next,</br> 
+<br>``$ python3 setup_db.py``<br>
+Make sure the entries match the mysql db configuration file``db_config.json`` 
+
+
```

### Comparing `idswapper-0.1.7/README.md` & `idswapper-0.1.8/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -56,12 +56,16 @@
 | ENSG00000146648 | P00533 | EGFR | 7p11.2 |
 | ENSG00000141510 | P04637 | TP53 | 17p13.1 |
 
 <br></br>
 
 **INSTALLATION**
 <br>`` $ pip install IDswapper ``</br>
-<br> Create the local database</br>
-``$ python setup_db.py``
 
+<br> Create the local idswapper database</br>
 <br> requires ``mysql`` up and running </br>
-<br> you can check using ``$ systemctl mysql status``</br>
+you can check using ``$ systemctl mysql status``
+<br>Next,</br> 
+<br>``$ python3 setup_db.py``<br>
+Make sure the entries match the mysql db configuration file``db_config.json`` 
+
+
```

### Comparing `idswapper-0.1.7/setup.py` & `idswapper-0.1.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='IDswapper',
-    version='0.1.7',
+    version='0.1.8',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'IDswapper=IDswapper.fetchids:main'
         ]
     },
     install_requires=[
```

