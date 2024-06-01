# Comparing `tmp/idswapper-0.0.2.tar.gz` & `tmp/idswapper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idswapper-0.0.2.tar", last modified: Sat Jun  1 10:05:33 2024, max compression
+gzip compressed data, was "idswapper-0.0.3.tar", last modified: Sat Jun  1 10:11:25 2024, max compression
```

## Comparing `idswapper-0.0.2.tar` & `idswapper-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:05:33.168260 idswapper-0.0.2/
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:05:33.168260 idswapper-0.0.2/IDswapper.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2295 2024-06-01 10:05:33.000000 idswapper-0.0.2/IDswapper.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      218 2024-06-01 10:05:33.000000 idswapper-0.0.2/IDswapper.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 10:05:33.000000 idswapper-0.0.2/IDswapper.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       54 2024-06-01 10:05:33.000000 idswapper-0.0.2/IDswapper.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       62 2024-06-01 10:05:33.000000 idswapper-0.0.2/IDswapper.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 10:05:33.000000 idswapper-0.0.2/IDswapper.egg-info/top_level.txt
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2295 2024-06-01 10:05:33.168260 idswapper-0.0.2/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1679 2024-06-01 10:01:26.000000 idswapper-0.0.2/README.md
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 10:05:33.168260 idswapper-0.0.2/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      990 2024-06-01 09:52:21.000000 idswapper-0.0.2/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:11:25.181628 idswapper-0.0.3/
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:11:25.177628 idswapper-0.0.3/IDswapper.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2171 2024-06-01 10:11:25.000000 idswapper-0.0.3/IDswapper.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      218 2024-06-01 10:11:25.000000 idswapper-0.0.3/IDswapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 10:11:25.000000 idswapper-0.0.3/IDswapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       54 2024-06-01 10:11:25.000000 idswapper-0.0.3/IDswapper.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       13 2024-06-01 10:11:25.000000 idswapper-0.0.3/IDswapper.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 10:11:25.000000 idswapper-0.0.3/IDswapper.egg-info/top_level.txt
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2171 2024-06-01 10:11:25.177628 idswapper-0.0.3/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1679 2024-06-01 10:01:26.000000 idswapper-0.0.3/README.md
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 10:11:25.181628 idswapper-0.0.3/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      886 2024-06-01 10:10:44.000000 idswapper-0.0.3/setup.py
```

### Comparing `idswapper-0.0.2/IDswapper.egg-info/PKG-INFO` & `idswapper-0.0.3/IDswapper.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 Metadata-Version: 2.1
 Name: IDswapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool for swapping IDs in a file and fetching data from a MySQL database
 Home-page: https://github.com/vkulaganathan/IDswapper/
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email:  
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: pandas
-Requires-Dist: mysql-connector-python
 Requires-Dist: tqdm
-Requires-Dist: gzip
-Requires-Dist: json
 Requires-Dist: pymysql
-Requires-Dist: argparse
 
 # IDswapper
 Convert given gene IDs to various other IDs. (under development, please come back later)
 
 **Usage**
 <br>``$ IDswapper --infile test.txt --id-column-index 0 --fetch "25" "5" "10" --outfile append_test.txt  ``</br>
```

### Comparing `idswapper-0.0.2/PKG-INFO` & `idswapper-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 Metadata-Version: 2.1
 Name: IDswapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: A tool for swapping IDs in a file and fetching data from a MySQL database
 Home-page: https://github.com/vkulaganathan/IDswapper/
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email:  
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: pandas
-Requires-Dist: mysql-connector-python
 Requires-Dist: tqdm
-Requires-Dist: gzip
-Requires-Dist: json
 Requires-Dist: pymysql
-Requires-Dist: argparse
 
 # IDswapper
 Convert given gene IDs to various other IDs. (under development, please come back later)
 
 **Usage**
 <br>``$ IDswapper --infile test.txt --id-column-index 0 --fetch "25" "5" "10" --outfile append_test.txt  ``</br>
```

### Comparing `idswapper-0.0.2/README.md` & `idswapper-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `idswapper-0.0.2/setup.py` & `idswapper-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
     name='IDswapper',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'IDswapper=idswapper.fetchids:main'
         ]
     },
     install_requires=[
-        'pandas',
-        'mysql-connector-python',
         'tqdm',
-        'gzip',
-        'json',
         'pymysql',
-        'argparse',
     ],
     package_data={'idswapper': ['db_config.json']},
     include_package_data=True,
     author='Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN',
     author_email=' ',
     description='A tool for swapping IDs in a file and fetching data from a MySQL database',
     long_description=open('README.md').read(),
```

