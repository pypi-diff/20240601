# Comparing `tmp/idswapper-0.0.2.tar.gz` & `tmp/idswapper-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idswapper-0.0.2.tar", last modified: Sat Jun  1 10:05:33 2024, max compression
+gzip compressed data, was "idswapper-1.0.tar", last modified: Sat Jun  1 09:37:30 2024, max compression
```

## Comparing `idswapper-0.0.2.tar` & `idswapper-1.0.tar`

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
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 09:37:30.220493 idswapper-1.0/
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 09:37:30.220493 idswapper-1.0/IDswapper.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1465 2024-06-01 09:37:30.000000 idswapper-1.0/IDswapper.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      218 2024-06-01 09:37:30.000000 idswapper-1.0/IDswapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 09:37:30.000000 idswapper-1.0/IDswapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       54 2024-06-01 09:37:30.000000 idswapper-1.0/IDswapper.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       57 2024-06-01 09:37:30.000000 idswapper-1.0/IDswapper.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 09:37:30.000000 idswapper-1.0/IDswapper.egg-info/top_level.txt
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     1465 2024-06-01 09:37:30.220493 idswapper-1.0/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      931 2024-06-01 09:37:16.000000 idswapper-1.0/README.md
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 09:37:30.220493 idswapper-1.0/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      982 2024-06-01 09:33:39.000000 idswapper-1.0/setup.py
```

### Comparing `idswapper-0.0.2/setup.py` & `idswapper-1.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='IDswapper',
-    version='0.0.2',
+    version='1.0',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'IDswapper=idswapper.fetchids:main'
         ]
     },
     install_requires=[
         'pandas',
-        'mysql-connector-python',
-        'tqdm',
-        'gzip',
-        'json',
-        'pymysql',
-        'argparse',
+        'mysql-connector-python'
+        'tqdm'
+        'gzip'
+        'json'
+        'pymysql'
+        'argparse'
     ],
     package_data={'idswapper': ['db_config.json']},
     include_package_data=True,
     author='Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN',
     author_email=' ',
     description='A tool for swapping IDs in a file and fetching data from a MySQL database',
     long_description=open('README.md').read(),
```

