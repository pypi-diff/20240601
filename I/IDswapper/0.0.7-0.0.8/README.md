# Comparing `tmp/idswapper-0.0.7.tar.gz` & `tmp/idswapper-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idswapper-0.0.7.tar", last modified: Sat Jun  1 10:49:07 2024, max compression
+gzip compressed data, was "idswapper-0.0.8.tar", last modified: Sat Jun  1 10:57:36 2024, max compression
```

## Comparing `idswapper-0.0.7.tar` & `idswapper-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:49:07.217681 idswapper-0.0.7/
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:49:07.217681 idswapper-0.0.7/IDswapper.egg-info/
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2406 2024-06-01 10:49:07.000000 idswapper-0.0.7/IDswapper.egg-info/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      309 2024-06-01 10:49:07.000000 idswapper-0.0.7/IDswapper.egg-info/SOURCES.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 10:49:07.000000 idswapper-0.0.7/IDswapper.egg-info/dependency_links.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       59 2024-06-01 10:49:07.000000 idswapper-0.0.7/IDswapper.egg-info/entry_points.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       43 2024-06-01 10:49:07.000000 idswapper-0.0.7/IDswapper.egg-info/requires.txt
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-06-01 10:49:07.000000 idswapper-0.0.7/IDswapper.egg-info/top_level.txt
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2406 2024-06-01 10:49:07.217681 idswapper-0.0.7/PKG-INFO
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1845 2024-06-01 10:30:34.000000 idswapper-0.0.7/README.md
-drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:49:07.213681 idswapper-0.0.7/idswapper/
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:26:54.000000 idswapper-0.0.7/idswapper/__init__.py
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)      115 2024-05-31 18:35:15.000000 idswapper-0.0.7/idswapper/db_config.json
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     8399 2024-06-01 10:39:40.000000 idswapper-0.0.7/idswapper/fetchids.py
--rw-r--r--   0 ws2024    (1000) ws2024    (1000)     7616 2024-05-31 20:34:58.000000 idswapper-0.0.7/idswapper/setup_db.py
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 10:49:07.217681 idswapper-0.0.7/setup.cfg
--rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      967 2024-06-01 10:47:15.000000 idswapper-0.0.7/setup.py
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:57:36.202638 idswapper-0.0.8/
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:57:36.198638 idswapper-0.0.8/IDswapper.egg-info/
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2396 2024-06-01 10:57:36.000000 idswapper-0.0.8/IDswapper.egg-info/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      332 2024-06-01 10:57:36.000000 idswapper-0.0.8/IDswapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        1 2024-06-01 10:57:36.000000 idswapper-0.0.8/IDswapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       59 2024-06-01 10:57:36.000000 idswapper-0.0.8/IDswapper.egg-info/entry_points.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       43 2024-06-01 10:57:36.000000 idswapper-0.0.8/IDswapper.egg-info/requires.txt
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       10 2024-06-01 10:57:36.000000 idswapper-0.0.8/IDswapper.egg-info/top_level.txt
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     2396 2024-06-01 10:57:36.202638 idswapper-0.0.8/PKG-INFO
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)     1845 2024-06-01 10:30:34.000000 idswapper-0.0.8/README.md
+drwxrwxr-x   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:57:36.198638 idswapper-0.0.8/idswapper/
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)        0 2024-06-01 10:26:54.000000 idswapper-0.0.8/idswapper/__init__.py
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)  5658381 2024-05-31 18:35:15.000000 idswapper-0.0.8/idswapper/data_file.gz
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)      115 2024-05-31 18:35:15.000000 idswapper-0.0.8/idswapper/db_config.json
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     8399 2024-06-01 10:39:40.000000 idswapper-0.0.8/idswapper/fetchids.py
+-rw-r--r--   0 ws2024    (1000) ws2024    (1000)     7616 2024-05-31 20:34:58.000000 idswapper-0.0.8/idswapper/setup_db.py
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)       38 2024-06-01 10:57:36.202638 idswapper-0.0.8/setup.cfg
+-rw-rw-r--   0 ws2024    (1000) ws2024    (1000)      973 2024-06-01 10:57:22.000000 idswapper-0.0.8/setup.py
```

### Comparing `idswapper-0.0.7/IDswapper.egg-info/PKG-INFO` & `idswapper-0.0.8/IDswapper.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: IDswapper
-Version: 0.0.7
-Summary: A tool for swapping IDs in a file and fetching data from a idswapper MySQL database
+Version: 0.0.8
+Summary: A tool for swapping IDs in a file and fetching data from a MySQL database
 Home-page: https://github.com/vkulaganathan/IDswapper/
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `idswapper-0.0.7/PKG-INFO` & `idswapper-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: IDswapper
-Version: 0.0.7
-Summary: A tool for swapping IDs in a file and fetching data from a idswapper MySQL database
+Version: 0.0.8
+Summary: A tool for swapping IDs in a file and fetching data from a MySQL database
 Home-page: https://github.com/vkulaganathan/IDswapper/
 Author: Pr (France) Dr. rer. nat. Vijay K. ULAGANATHAN
 Author-email: 
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `idswapper-0.0.7/README.md` & `idswapper-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `idswapper-0.0.7/idswapper/fetchids.py` & `idswapper-0.0.8/idswapper/fetchids.py`

 * *Files identical despite different names*

### Comparing `idswapper-0.0.7/idswapper/setup_db.py` & `idswapper-0.0.8/idswapper/setup_db.py`

 * *Files identical despite different names*

