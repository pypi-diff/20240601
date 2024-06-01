# Comparing `tmp/schwab-client-0.0.1.tar.gz` & `tmp/schwab-client-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schwab-client-0.0.1.tar", last modified: Sat Jun  1 02:49:27 2024, max compression
+gzip compressed data, was "schwab-client-0.0.2.tar", last modified: Sat Jun  1 02:58:44 2024, max compression
```

## Comparing `schwab-client-0.0.1.tar` & `schwab-client-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-06-01 02:49:27.716266 schwab-client-0.0.1/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      576 2024-06-01 02:49:27.716266 schwab-client-0.0.1/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3042 2024-05-30 21:36:54.000000 schwab-client-0.0.1/README.md
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-06-01 02:49:27.716266 schwab-client-0.0.1/schwab-client/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       23 2024-06-01 02:14:41.000000 schwab-client-0.0.1/schwab-client/__init__.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    21826 2024-06-01 01:21:57.000000 schwab-client-0.0.1/schwab-client/api.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)    11717 2024-06-01 01:21:57.000000 schwab-client-0.0.1/schwab-client/stream.py
--rw-rw-r--   0 tyler     (1000) tyler     (1000)     3624 2024-05-30 21:36:54.000000 schwab-client-0.0.1/schwab-client/terminal.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-06-01 02:49:27.716266 schwab-client-0.0.1/schwab_client.egg-info/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      576 2024-06-01 02:49:27.000000 schwab-client-0.0.1/schwab_client.egg-info/PKG-INFO
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      318 2024-06-01 02:49:27.000000 schwab-client-0.0.1/schwab_client.egg-info/SOURCES.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-06-01 02:49:27.000000 schwab-client-0.0.1/schwab_client.egg-info/dependency_links.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       20 2024-06-01 02:49:27.000000 schwab-client-0.0.1/schwab_client.egg-info/requires.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       14 2024-06-01 02:49:27.000000 schwab-client-0.0.1/schwab_client.egg-info/top_level.txt
--rw-rw-r--   0 tyler     (1000) tyler     (1000)       38 2024-06-01 02:49:27.716266 schwab-client-0.0.1/setup.cfg
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      893 2024-06-01 02:49:23.000000 schwab-client-0.0.1/setup.py
-drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-06-01 02:49:27.716266 schwab-client-0.0.1/tests/
--rw-rw-r--   0 tyler     (1000) tyler     (1000)      186 2024-06-01 02:46:57.000000 schwab-client-0.0.1/tests/test_main.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-06-01 02:58:44.900231 schwab-client-0.0.2/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      576 2024-06-01 02:58:44.900231 schwab-client-0.0.2/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3042 2024-05-30 21:36:54.000000 schwab-client-0.0.2/README.md
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-06-01 02:58:44.900231 schwab-client-0.0.2/pyschwab/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       23 2024-06-01 02:14:41.000000 schwab-client-0.0.2/pyschwab/__init__.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    21826 2024-06-01 01:21:57.000000 schwab-client-0.0.2/pyschwab/api.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)    11717 2024-06-01 01:21:57.000000 schwab-client-0.0.2/pyschwab/stream.py
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)     3624 2024-05-30 21:36:54.000000 schwab-client-0.0.2/pyschwab/terminal.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-06-01 02:58:44.900231 schwab-client-0.0.2/schwab_client.egg-info/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      576 2024-06-01 02:58:44.000000 schwab-client-0.0.2/schwab_client.egg-info/PKG-INFO
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      298 2024-06-01 02:58:44.000000 schwab-client-0.0.2/schwab_client.egg-info/SOURCES.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        1 2024-06-01 02:58:44.000000 schwab-client-0.0.2/schwab_client.egg-info/dependency_links.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       20 2024-06-01 02:58:44.000000 schwab-client-0.0.2/schwab_client.egg-info/requires.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)        9 2024-06-01 02:58:44.000000 schwab-client-0.0.2/schwab_client.egg-info/top_level.txt
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)       38 2024-06-01 02:58:44.900231 schwab-client-0.0.2/setup.cfg
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      893 2024-06-01 02:58:39.000000 schwab-client-0.0.2/setup.py
+drwxrwxr-x   0 tyler     (1000) tyler     (1000)        0 2024-06-01 02:58:44.900231 schwab-client-0.0.2/tests/
+-rw-rw-r--   0 tyler     (1000) tyler     (1000)      186 2024-06-01 02:46:57.000000 schwab-client-0.0.2/tests/test_main.py
```

### Comparing `schwab-client-0.0.1/PKG-INFO` & `schwab-client-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: Schwab API Python Client (unofficial)
 Author: Tyler Bowers
 Author-email: tylerebowers@gmail.com
 Keywords: python,schwab,api,client
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schwab-client-0.0.1/README.md` & `schwab-client-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `schwab-client-0.0.1/schwab-client/api.py` & `schwab-client-0.0.2/pyschwab/api.py`

 * *Files identical despite different names*

### Comparing `schwab-client-0.0.1/schwab-client/stream.py` & `schwab-client-0.0.2/pyschwab/stream.py`

 * *Files identical despite different names*

### Comparing `schwab-client-0.0.1/schwab-client/terminal.py` & `schwab-client-0.0.2/pyschwab/terminal.py`

 * *Files identical despite different names*

### Comparing `schwab-client-0.0.1/schwab_client.egg-info/PKG-INFO` & `schwab-client-0.0.2/schwab_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schwab-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: Schwab API Python Client (unofficial)
 Author: Tyler Bowers
 Author-email: tylerebowers@gmail.com
 Keywords: python,schwab,api,client
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schwab-client-0.0.1/setup.py` & `schwab-client-0.0.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Schwab API Python Client (unofficial)'
 LONG_DESCRIPTION = 'This is an unofficial python program to access the Schwab api.'
 
 setup(
     name='schwab-client',
     version=VERSION,
     author='Tyler Bowers',
```

