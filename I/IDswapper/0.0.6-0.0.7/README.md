# Comparing `tmp/idswapper-0.0.6.tar.gz` & `tmp/idswapper-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idswapper-0.0.6.tar", last modified: Sat Jun  1 10:40:26 2024, max compression
+gzip compressed data, was "idswapper-0.0.7.tar", last modified: Sat Jun  1 10:49:07 2024, max compression
```

## Comparing `idswapper-0.0.6.tar` & `idswapper-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:40:26.286302 idswapper-0.0.6/
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:40:26.286302 idswapper-0.0.6/IDswapper.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2397 2024-06-01 10:40:26.000000 idswapper-0.0.6/IDswapper.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      309 2024-06-01 10:40:26.000000 idswapper-0.0.6/IDswapper.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 10:40:26.000000 idswapper-0.0.6/IDswapper.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       54 2024-06-01 10:40:26.000000 idswapper-0.0.6/IDswapper.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       43 2024-06-01 10:40:26.000000 idswapper-0.0.6/IDswapper.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-06-01 10:40:26.000000 idswapper-0.0.6/IDswapper.egg-info/top_level.txt
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2397 2024-06-01 10:40:26.286302 idswapper-0.0.6/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1845 2024-06-01 10:30:34.000000 idswapper-0.0.6/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:40:26.286302 idswapper-0.0.6/idswapper/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:26:54.000000 idswapper-0.0.6/idswapper/__init__.py
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)      115 2024-05-31 18:35:15.000000 idswapper-0.0.6/idswapper/db_config.json
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     8399 2024-06-01 10:39:40.000000 idswapper-0.0.6/idswapper/fetchids.py
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     7616 2024-05-31 20:34:58.000000 idswapper-0.0.6/idswapper/setup_db.py
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 10:40:26.286302 idswapper-0.0.6/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      990 2024-06-01 10:39:38.000000 idswapper-0.0.6/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:49:07.217681 idswapper-0.0.7/
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:49:07.217681 idswapper-0.0.7/IDswapper.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2406 2024-06-01 10:49:07.000000 idswapper-0.0.7/IDswapper.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      309 2024-06-01 10:49:07.000000 idswapper-0.0.7/IDswapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 10:49:07.000000 idswapper-0.0.7/IDswapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       59 2024-06-01 10:49:07.000000 idswapper-0.0.7/IDswapper.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       43 2024-06-01 10:49:07.000000 idswapper-0.0.7/IDswapper.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-06-01 10:49:07.000000 idswapper-0.0.7/IDswapper.egg-info/top_level.txt
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2406 2024-06-01 10:49:07.217681 idswapper-0.0.7/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1845 2024-06-01 10:30:34.000000 idswapper-0.0.7/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:49:07.213681 idswapper-0.0.7/idswapper/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:26:54.000000 idswapper-0.0.7/idswapper/__init__.py
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)      115 2024-05-31 18:35:15.000000 idswapper-0.0.7/idswapper/db_config.json
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     8399 2024-06-01 10:39:40.000000 idswapper-0.0.7/idswapper/fetchids.py
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     7616 2024-05-31 20:34:58.000000 idswapper-0.0.7/idswapper/setup_db.py
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 10:49:07.217681 idswapper-0.0.7/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      967 2024-06-01 10:47:15.000000 idswapper-0.0.7/setup.py
```

### Comparing `idswapper-0.0.6/IDswapper.egg-info/PKG-INFO` & `idswapper-0.0.7/IDswapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: IDswapper
-Version: 0.0.6
-Summary: A tool for swapping IDs in a file and fetching data from a MySQL database
+Version: 0.0.7
+Summary: A tool for swapping IDs in a file and fetching data from a idswapper MySQL database
 Home-page: https://github.com/vkulaganathan/IDswapper/
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
-Author-email:  
+Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: mysql-connector-python
 Requires-Dist: tqdm
```

### Comparing `idswapper-0.0.6/PKG-INFO` & `idswapper-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: IDswapper
-Version: 0.0.6
-Summary: A tool for swapping IDs in a file and fetching data from a MySQL database
+Version: 0.0.7
+Summary: A tool for swapping IDs in a file and fetching data from a idswapper MySQL database
 Home-page: https://github.com/vkulaganathan/IDswapper/
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
-Author-email:  
+Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Requires-Dist: pandas
 Requires-Dist: mysql-connector-python
 Requires-Dist: tqdm
```

### Comparing `idswapper-0.0.6/README.md` & `idswapper-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `idswapper-0.0.6/idswapper/fetchids.py` & `idswapper-0.0.7/idswapper/fetchids.py`

 * *Files identical despite different names*

### Comparing `idswapper-0.0.6/idswapper/setup_db.py` & `idswapper-0.0.7/idswapper/setup_db.py`

 * *Files identical despite different names*

### Comparing `idswapper-0.0.6/setup.py` & `idswapper-0.0.7/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from setuptools import setup, find_packages
 
 setup(
     name='IDswapper',
-    version='0.0.6',
-    packages=find_packages(),  # Include all packages under the current directory
+    version='0.0.7',
+    packages=find_packages(),
     entry_points={
         'console_scripts': [
-            'IDswapper=idswapper.fetchids:main'
+            'IDswapper=idswapper.fetchids:fetch_ids'
         ]
     },
     install_requires=[
         'pandas',
         'mysql-connector-python',
         'tqdm',
         'pymysql',
     ],
-    package_data={'idswapper': ['db_config.json']},
+    package_data={'idswapper': ['fetchids.py', 'db_config.json']},
     include_package_data=True,
     author='Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN',
-    author_email=' ',
-    description='A tool for swapping IDs in a file and fetching data from a MySQL database',
+    author_email='',
+    description='A tool for swapping IDs in a file and fetching data from a idswapper MySQL database',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/vkulaganathan/IDswapper/',
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
```

