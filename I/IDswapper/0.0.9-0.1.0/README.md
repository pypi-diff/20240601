# Comparing `tmp/idswapper-0.0.9.tar.gz` & `tmp/idswapper-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idswapper-0.0.9.tar", last modified: Sat Jun  1 10:59:40 2024, max compression
+gzip compressed data, was "idswapper-0.1.0.tar", last modified: Sat Jun  1 11:06:37 2024, max compression
```

## Comparing `idswapper-0.0.9.tar` & `idswapper-0.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:59:40.738044 idswapper-0.0.9/
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:59:40.738044 idswapper-0.0.9/IDswapper.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2396 2024-06-01 10:59:40.000000 idswapper-0.0.9/IDswapper.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      332 2024-06-01 10:59:40.000000 idswapper-0.0.9/IDswapper.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 10:59:40.000000 idswapper-0.0.9/IDswapper.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       54 2024-06-01 10:59:40.000000 idswapper-0.0.9/IDswapper.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       43 2024-06-01 10:59:40.000000 idswapper-0.0.9/IDswapper.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-06-01 10:59:40.000000 idswapper-0.0.9/IDswapper.egg-info/top_level.txt
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2396 2024-06-01 10:59:40.738044 idswapper-0.0.9/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1845 2024-06-01 10:30:34.000000 idswapper-0.0.9/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:59:40.738044 idswapper-0.0.9/idswapper/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:26:54.000000 idswapper-0.0.9/idswapper/__init__.py
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)  5658381 2024-05-31 18:35:15.000000 idswapper-0.0.9/idswapper/data_file.gz
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)      115 2024-05-31 18:35:15.000000 idswapper-0.0.9/idswapper/db_config.json
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     8399 2024-06-01 10:39:40.000000 idswapper-0.0.9/idswapper/fetchids.py
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     7616 2024-05-31 20:34:58.000000 idswapper-0.0.9/idswapper/setup_db.py
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 10:59:40.738044 idswapper-0.0.9/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      968 2024-06-01 10:59:26.000000 idswapper-0.0.9/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 11:06:37.914997 idswapper-0.1.0/
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 11:06:37.914997 idswapper-0.1.0/IDswapper.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2404 2024-06-01 11:06:37.000000 idswapper-0.1.0/IDswapper.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      332 2024-06-01 11:06:37.000000 idswapper-0.1.0/IDswapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 11:06:37.000000 idswapper-0.1.0/IDswapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       59 2024-06-01 11:06:37.000000 idswapper-0.1.0/IDswapper.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       43 2024-06-01 11:06:37.000000 idswapper-0.1.0/IDswapper.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-06-01 11:06:37.000000 idswapper-0.1.0/IDswapper.egg-info/top_level.txt
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2404 2024-06-01 11:06:37.914997 idswapper-0.1.0/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1845 2024-06-01 10:30:34.000000 idswapper-0.1.0/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 11:06:37.914997 idswapper-0.1.0/idswapper/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:26:54.000000 idswapper-0.1.0/idswapper/__init__.py
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)  5658381 2024-05-31 18:35:15.000000 idswapper-0.1.0/idswapper/data_file.gz
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)      115 2024-05-31 18:35:15.000000 idswapper-0.1.0/idswapper/db_config.json
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     8399 2024-06-01 10:39:40.000000 idswapper-0.1.0/idswapper/fetchids.py
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     7616 2024-05-31 20:34:58.000000 idswapper-0.1.0/idswapper/setup_db.py
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 11:06:37.914997 idswapper-0.1.0/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      965 2024-06-01 11:06:08.000000 idswapper-0.1.0/setup.py
```

### Comparing `idswapper-0.0.9/IDswapper.egg-info/PKG-INFO` & `idswapper-0.1.0/IDswapper.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: IDswapper
-Version: 0.0.9
-Summary: A tool for swapping IDs in a file and fetching data from a MySQL database
+Version: 0.1.0
+Summary: A tool for swapping IDs in a file by fetching various IDs from idswapper database
 Home-page: https://github.com/vkulaganathan/IDswapper/
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `idswapper-0.0.9/PKG-INFO` & `idswapper-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: IDswapper
-Version: 0.0.9
-Summary: A tool for swapping IDs in a file and fetching data from a MySQL database
+Version: 0.1.0
+Summary: A tool for swapping IDs in a file by fetching various IDs from idswapper database
 Home-page: https://github.com/vkulaganathan/IDswapper/
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `idswapper-0.0.9/README.md` & `idswapper-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `idswapper-0.0.9/idswapper/data_file.gz` & `idswapper-0.1.0/idswapper/data_file.gz`

 * *Files identical despite different names*

### Comparing `idswapper-0.0.9/idswapper/fetchids.py` & `idswapper-0.1.0/idswapper/fetchids.py`

 * *Files identical despite different names*

### Comparing `idswapper-0.0.9/idswapper/setup_db.py` & `idswapper-0.1.0/idswapper/setup_db.py`

 * *Files identical despite different names*

