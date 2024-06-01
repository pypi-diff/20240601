# Comparing `tmp/almax_common-0.9.5.tar.gz` & `tmp/almax_common-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-0.9.5.tar", last modified: Fri May 31 14:03:22 2024, max compression
+gzip compressed data, was "almax_common-0.9.6.tar", last modified: Sat Jun  1 13:49:42 2024, max compression
```

## Comparing `almax_common-0.9.5.tar` & `almax_common-0.9.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:03:22.778973 almax_common-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-31 14:03:22.778973 almax_common-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-31 14:02:58.000000 almax_common-0.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:03:22.778973 almax_common-0.9.5/Utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-05-31 14:02:58.000000 almax_common-0.9.5/Utils/FileSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-31 14:02:58.000000 almax_common-0.9.5/Utils/Generic.py
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-31 14:02:58.000000 almax_common-0.9.5/Utils/Time.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-31 14:02:58.000000 almax_common-0.9.5/Utils/Xml.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 14:02:58.000000 almax_common-0.9.5/Utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 14:03:22.778973 almax_common-0.9.5/almax_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-05-31 14:03:22.000000 almax_common-0.9.5/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-05-31 14:03:22.000000 almax_common-0.9.5/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 14:03:22.000000 almax_common-0.9.5/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-05-31 14:03:22.000000 almax_common-0.9.5/almax_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-31 14:03:22.000000 almax_common-0.9.5/almax_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 14:03:22.778973 almax_common-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-05-31 14:02:58.000000 almax_common-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:49:42.961400 almax_common-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-06-01 13:49:42.961400 almax_common-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-01 13:49:16.000000 almax_common-0.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:49:42.961400 almax_common-0.9.6/Utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 13:49:16.000000 almax_common-0.9.6/Utils/FileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-01 13:49:16.000000 almax_common-0.9.6/Utils/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 13:49:16.000000 almax_common-0.9.6/Utils/Time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-06-01 13:49:16.000000 almax_common-0.9.6/Utils/Xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-01 13:49:16.000000 almax_common-0.9.6/Utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:49:42.961400 almax_common-0.9.6/almax_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-06-01 13:49:42.000000 almax_common-0.9.6/almax_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-06-01 13:49:42.000000 almax_common-0.9.6/almax_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 13:49:42.000000 almax_common-0.9.6/almax_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-06-01 13:49:42.000000 almax_common-0.9.6/almax_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-01 13:49:42.000000 almax_common-0.9.6/almax_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 13:49:42.961400 almax_common-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-06-01 13:49:16.000000 almax_common-0.9.6/setup.py
```

### Comparing `almax_common-0.9.5/PKG-INFO` & `almax_common-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 0.9.5
+Version: 0.9.6
 Summary: A common library with some of my implementations
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: appnope==0.1.4
 Requires-Dist: asttokens==2.4.1
 Requires-Dist: attrs==23.2.0
```

### Comparing `almax_common-0.9.5/Utils/FileSystem.py` & `almax_common-0.9.6/Utils/FileSystem.py`

 * *Files identical despite different names*

### Comparing `almax_common-0.9.5/Utils/Generic.py` & `almax_common-0.9.6/Utils/Generic.py`

 * *Files identical despite different names*

### Comparing `almax_common-0.9.5/Utils/Time.py` & `almax_common-0.9.6/Utils/Time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 from datetime import datetime, timedelta;
 
 now = datetime.now();
 
 def CalculateTime(start: datetime):
     return datetime.now() - start;
```

### Comparing `almax_common-0.9.5/almax_common.egg-info/PKG-INFO` & `almax_common-0.9.6/almax_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 0.9.5
+Version: 0.9.6
 Summary: A common library with some of my implementations
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: appnope==0.1.4
 Requires-Dist: asttokens==2.4.1
 Requires-Dist: attrs==23.2.0
```

### Comparing `almax_common-0.9.5/almax_common.egg-info/requires.txt` & `almax_common-0.9.6/almax_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `almax_common-0.9.5/setup.py` & `almax_common-0.9.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     readMe = fh.read();
 
 with open("requirements.txt") as f:
     required = f.read().splitlines();
 
 setup(
     name='almax_common',
-    version='0.9.5',
+    version='0.9.6',
     description='A common library with some of my implementations',
     long_description=readMe,
     long_description_content_type='text/markdown',
     author='AlMax98',
     author_email='alihaider.maqsood@gmail.com',
     packages=find_packages(),
     package_dir={'': '.'},
```

