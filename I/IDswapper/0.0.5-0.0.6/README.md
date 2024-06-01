# Comparing `tmp/idswapper-0.0.5.tar.gz` & `tmp/idswapper-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idswapper-0.0.5.tar", last modified: Sat Jun  1 10:32:39 2024, max compression
+gzip compressed data, was "idswapper-0.0.6.tar", last modified: Sat Jun  1 10:40:26 2024, max compression
```

## Comparing `idswapper-0.0.5.tar` & `idswapper-0.0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:32:39.913889 idswapper-0.0.5/
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:32:39.913889 idswapper-0.0.5/IDswapper.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2397 2024-06-01 10:32:39.000000 idswapper-0.0.5/IDswapper.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      309 2024-06-01 10:32:39.000000 idswapper-0.0.5/IDswapper.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 10:32:39.000000 idswapper-0.0.5/IDswapper.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       54 2024-06-01 10:32:39.000000 idswapper-0.0.5/IDswapper.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       43 2024-06-01 10:32:39.000000 idswapper-0.0.5/IDswapper.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-06-01 10:32:39.000000 idswapper-0.0.5/IDswapper.egg-info/top_level.txt
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2397 2024-06-01 10:32:39.913889 idswapper-0.0.5/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1845 2024-06-01 10:30:34.000000 idswapper-0.0.5/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:32:39.913889 idswapper-0.0.5/idswapper/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:26:54.000000 idswapper-0.0.5/idswapper/__init__.py
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)      115 2024-05-31 18:35:15.000000 idswapper-0.0.5/idswapper/db_config.json
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     8266 2024-06-01 09:22:54.000000 idswapper-0.0.5/idswapper/fetchids.py
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     7616 2024-05-31 20:34:58.000000 idswapper-0.0.5/idswapper/setup_db.py
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 10:32:39.913889 idswapper-0.0.5/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      990 2024-06-01 10:31:16.000000 idswapper-0.0.5/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:40:26.286302 idswapper-0.0.6/
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:40:26.286302 idswapper-0.0.6/IDswapper.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2397 2024-06-01 10:40:26.000000 idswapper-0.0.6/IDswapper.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      309 2024-06-01 10:40:26.000000 idswapper-0.0.6/IDswapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 10:40:26.000000 idswapper-0.0.6/IDswapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       54 2024-06-01 10:40:26.000000 idswapper-0.0.6/IDswapper.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       43 2024-06-01 10:40:26.000000 idswapper-0.0.6/IDswapper.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-06-01 10:40:26.000000 idswapper-0.0.6/IDswapper.egg-info/top_level.txt
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2397 2024-06-01 10:40:26.286302 idswapper-0.0.6/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1845 2024-06-01 10:30:34.000000 idswapper-0.0.6/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:40:26.286302 idswapper-0.0.6/idswapper/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:26:54.000000 idswapper-0.0.6/idswapper/__init__.py
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)      115 2024-05-31 18:35:15.000000 idswapper-0.0.6/idswapper/db_config.json
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     8399 2024-06-01 10:39:40.000000 idswapper-0.0.6/idswapper/fetchids.py
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     7616 2024-05-31 20:34:58.000000 idswapper-0.0.6/idswapper/setup_db.py
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 10:40:26.286302 idswapper-0.0.6/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      990 2024-06-01 10:39:38.000000 idswapper-0.0.6/setup.py
```

### Comparing `idswapper-0.0.5/IDswapper.egg-info/PKG-INFO` & `idswapper-0.0.6/IDswapper.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IDswapper
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool for swapping IDs in a file and fetching data from a MySQL database
 Home-page: https://github.com/vkulaganathan/IDswapper/
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email:  
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `idswapper-0.0.5/PKG-INFO` & `idswapper-0.0.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IDswapper
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool for swapping IDs in a file and fetching data from a MySQL database
 Home-page: https://github.com/vkulaganathan/IDswapper/
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email:  
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `idswapper-0.0.5/README.md` & `idswapper-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `idswapper-0.0.5/idswapper/fetchids.py` & `idswapper-0.0.6/idswapper/fetchids.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-#USAGE-- $ python fetchids.py --infile test.txt --id-column-index 0 --fetch "5" "10" "26" "20" "21" --outfile append_test.txt
-
 import argparse
 import pymysql
 import json
 import gzip
 from tqdm import tqdm
+import os  # Import os module for file path operations
+
+# Get the directory of the current script file
+script_dir = os.path.dirname(os.path.realpath(__file__))
+# Construct the path to the db_config.json file
+config_path = os.path.join(script_dir, 'db_config.json')
 
 # Load database configuration
-with open('db_config.json') as config_file:
+with open(config_path) as config_file:
     db_config = json.load(config_file)
 
 fetch_options = {
     "gene_stable_id": {"text": "Gene Stable ID", "number": 1},
     "transcript_stable_id": {"text": "Ensembl Transcript ID", "number": 2},
     "protein_stable_id": {"text": "Ensembl Protein ID", "number": 3},
     "hgnc_id": {"text": "HGNC ID", "number": 4},
```

### Comparing `idswapper-0.0.5/idswapper/setup_db.py` & `idswapper-0.0.6/idswapper/setup_db.py`

 * *Files identical despite different names*

### Comparing `idswapper-0.0.5/setup.py` & `idswapper-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='IDswapper',
-    version='0.0.5',
+    version='0.0.6',
     packages=find_packages(),  # Include all packages under the current directory
     entry_points={
         'console_scripts': [
             'IDswapper=idswapper.fetchids:main'
         ]
     },
     install_requires=[
```

