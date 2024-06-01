# Comparing `tmp/idswapper-0.0.4.tar.gz` & `tmp/idswapper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idswapper-0.0.4.tar", last modified: Sat Jun  1 10:13:23 2024, max compression
+gzip compressed data, was "idswapper-0.0.5.tar", last modified: Sat Jun  1 10:32:39 2024, max compression
```

## Comparing `idswapper-0.0.4.tar` & `idswapper-0.0.5.tar`

### file list

```diff
@@ -1,12 +1,17 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:13:23.379372 idswapper-0.0.4/
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:13:23.379372 idswapper-0.0.4/IDswapper.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2231 2024-06-01 10:13:23.000000 idswapper-0.0.4/IDswapper.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      218 2024-06-01 10:13:23.000000 idswapper-0.0.4/IDswapper.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 10:13:23.000000 idswapper-0.0.4/IDswapper.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       54 2024-06-01 10:13:23.000000 idswapper-0.0.4/IDswapper.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       43 2024-06-01 10:13:23.000000 idswapper-0.0.4/IDswapper.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 10:13:23.000000 idswapper-0.0.4/IDswapper.egg-info/top_level.txt
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2231 2024-06-01 10:13:23.379372 idswapper-0.0.4/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1679 2024-06-01 10:01:26.000000 idswapper-0.0.4/README.md
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 10:13:23.379372 idswapper-0.0.4/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      938 2024-06-01 10:13:14.000000 idswapper-0.0.4/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:32:39.913889 idswapper-0.0.5/
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:32:39.913889 idswapper-0.0.5/IDswapper.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2397 2024-06-01 10:32:39.000000 idswapper-0.0.5/IDswapper.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      309 2024-06-01 10:32:39.000000 idswapper-0.0.5/IDswapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 10:32:39.000000 idswapper-0.0.5/IDswapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       54 2024-06-01 10:32:39.000000 idswapper-0.0.5/IDswapper.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       43 2024-06-01 10:32:39.000000 idswapper-0.0.5/IDswapper.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-06-01 10:32:39.000000 idswapper-0.0.5/IDswapper.egg-info/top_level.txt
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2397 2024-06-01 10:32:39.913889 idswapper-0.0.5/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1845 2024-06-01 10:30:34.000000 idswapper-0.0.5/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:32:39.913889 idswapper-0.0.5/idswapper/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:26:54.000000 idswapper-0.0.5/idswapper/__init__.py
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)      115 2024-05-31 18:35:15.000000 idswapper-0.0.5/idswapper/db_config.json
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     8266 2024-06-01 09:22:54.000000 idswapper-0.0.5/idswapper/fetchids.py
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     7616 2024-05-31 20:34:58.000000 idswapper-0.0.5/idswapper/setup_db.py
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 10:32:39.913889 idswapper-0.0.5/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      990 2024-06-01 10:31:16.000000 idswapper-0.0.5/setup.py
```

### Comparing `idswapper-0.0.4/IDswapper.egg-info/PKG-INFO` & `idswapper-0.0.5/IDswapper.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: IDswapper
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool for swapping IDs in a file and fetching data from a MySQL database
 Home-page: https://github.com/vkulaganathan/IDswapper/
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email:  
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: tqdm
-Requires-Dist: pymysql
 Requires-Dist: pandas
 Requires-Dist: mysql-connector-python
+Requires-Dist: tqdm
+Requires-Dist: pymysql
 
 # IDswapper
 Convert given gene IDs to various other IDs. (under development, please come back later)
 
 **Usage**
 <br>``$ IDswapper --infile test.txt --id-column-index 0 --fetch "25" "5" "10" --outfile append_test.txt  ``</br>
 
@@ -72,7 +72,12 @@
 | ENSG00000146648 | P00533 | EGFR | 7p11.2 |
 | ENSG00000141510 | P04637 | TP53 | 17p13.1 |
 
 <br></br>
 
 **INSTALLATION**
 <br>`` $ pip install IDswapper ``</br>
+<br> Create the local database</br>
+``$ python setup_db.py``
+
+<br> requires ``mysql`` up and running </br>
+<br> you can check using ``$ systemctl mysql status``</br>
```

### Comparing `idswapper-0.0.4/PKG-INFO` & `idswapper-0.0.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: IDswapper
-Version: 0.0.4
+Version: 0.0.5
 Summary: A tool for swapping IDs in a file and fetching data from a MySQL database
 Home-page: https://github.com/vkulaganathan/IDswapper/
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email:  
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: tqdm
-Requires-Dist: pymysql
 Requires-Dist: pandas
 Requires-Dist: mysql-connector-python
+Requires-Dist: tqdm
+Requires-Dist: pymysql
 
 # IDswapper
 Convert given gene IDs to various other IDs. (under development, please come back later)
 
 **Usage**
 <br>``$ IDswapper --infile test.txt --id-column-index 0 --fetch "25" "5" "10" --outfile append_test.txt  ``</br>
 
@@ -72,7 +72,12 @@
 | ENSG00000146648 | P00533 | EGFR | 7p11.2 |
 | ENSG00000141510 | P04637 | TP53 | 17p13.1 |
 
 <br></br>
 
 **INSTALLATION**
 <br>`` $ pip install IDswapper ``</br>
+<br> Create the local database</br>
+``$ python setup_db.py``
+
+<br> requires ``mysql`` up and running </br>
+<br> you can check using ``$ systemctl mysql status``</br>
```

### Comparing `idswapper-0.0.4/README.md` & `idswapper-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -56,7 +56,12 @@
 | ENSG00000146648 | P00533 | EGFR | 7p11.2 |
 | ENSG00000141510 | P04637 | TP53 | 17p13.1 |
 
 <br></br>
 
 **INSTALLATION**
 <br>`` $ pip install IDswapper ``</br>
+<br> Create the local database</br>
+``$ python setup_db.py``
+
+<br> requires ``mysql`` up and running </br>
+<br> you can check using ``$ systemctl mysql status``</br>
```

### Comparing `idswapper-0.0.4/setup.py` & `idswapper-0.0.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup, find_packages
 
 setup(
     name='IDswapper',
-    version='0.0.4',
-    packages=find_packages(),
+    version='0.0.5',
+    packages=find_packages(),  # Include all packages under the current directory
     entry_points={
         'console_scripts': [
             'IDswapper=idswapper.fetchids:main'
         ]
     },
     install_requires=[
-        'tqdm',
-        'pymysql',
         'pandas',
         'mysql-connector-python',
+        'tqdm',
+        'pymysql',
     ],
     package_data={'idswapper': ['db_config.json']},
     include_package_data=True,
     author='Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN',
     author_email=' ',
     description='A tool for swapping IDs in a file and fetching data from a MySQL database',
     long_description=open('README.md').read(),
```

