# Comparing `tmp/lexset-4.2.8.tar.gz` & `tmp/lexset-4.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lexset-4.2.8.tar", last modified: Tue Apr 23 21:57:59 2024, max compression
+gzip compressed data, was "lexset-4.2.9.tar", last modified: Fri May 31 23:00:06 2024, max compression
```

## Comparing `lexset-4.2.8.tar` & `lexset-4.2.9.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:57:59.898743 lexset-4.2.8/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-23 21:57:59.898743 lexset-4.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-23 21:57:49.000000 lexset-4.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:57:59.898743 lexset-4.2.8/lexset/
--rw-r--r--   0 runner    (1001) docker     (127)    28521 2024-04-23 21:57:49.000000 lexset-4.2.8/lexset/LexsetManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-23 21:57:49.000000 lexset-4.2.8/lexset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-04-23 21:57:49.000000 lexset-4.2.8/lexset/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-04-23 21:57:49.000000 lexset-4.2.8/lexset/medtronic_Debug.py
--rw-r--r--   0 runner    (1001) docker     (127)    22730 2024-04-23 21:57:49.000000 lexset-4.2.8/lexset/review.py
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-23 21:57:49.000000 lexset-4.2.8/lexset/test_ssim.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 21:57:59.898743 lexset-4.2.8/lexset.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-23 21:57:59.000000 lexset-4.2.8/lexset.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-23 21:57:59.000000 lexset-4.2.8/lexset.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 21:57:59.000000 lexset-4.2.8/lexset.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-23 21:57:59.000000 lexset-4.2.8/lexset.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-23 21:57:59.000000 lexset-4.2.8/lexset.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 21:57:59.898743 lexset-4.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-23 21:57:49.000000 lexset-4.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:00:06.803243 lexset-4.2.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-31 23:00:06.803243 lexset-4.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-31 22:59:57.000000 lexset-4.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:00:06.803243 lexset-4.2.9/lexset/
+-rw-r--r--   0 runner    (1001) docker     (127)    28521 2024-05-31 22:59:57.000000 lexset-4.2.9/lexset/LexsetManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-31 22:59:57.000000 lexset-4.2.9/lexset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-31 22:59:57.000000 lexset-4.2.9/lexset/compression_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-31 22:59:57.000000 lexset-4.2.9/lexset/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-31 22:59:57.000000 lexset-4.2.9/lexset/medtronic_Debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22730 2024-05-31 22:59:57.000000 lexset-4.2.9/lexset/review.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-31 22:59:57.000000 lexset-4.2.9/lexset/test_ssim.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:00:06.803243 lexset-4.2.9/lexset.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-05-31 23:00:06.000000 lexset-4.2.9/lexset.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-31 23:00:06.000000 lexset-4.2.9/lexset.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 23:00:06.000000 lexset-4.2.9/lexset.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-31 23:00:06.000000 lexset-4.2.9/lexset.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-31 23:00:06.000000 lexset-4.2.9/lexset.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 23:00:06.803243 lexset-4.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-31 22:59:57.000000 lexset-4.2.9/setup.py
```

### Comparing `lexset-4.2.8/lexset/LexsetManager.py` & `lexset-4.2.9/lexset/LexsetManager.py`

 * *Files identical despite different names*

### Comparing `lexset-4.2.8/lexset/credentials.py` & `lexset-4.2.9/lexset/credentials.py`

 * *Files identical despite different names*

### Comparing `lexset-4.2.8/lexset/medtronic_Debug.py` & `lexset-4.2.9/lexset/medtronic_Debug.py`

 * *Files identical despite different names*

### Comparing `lexset-4.2.8/lexset/review.py` & `lexset-4.2.9/lexset/review.py`

 * *Files identical despite different names*

### Comparing `lexset-4.2.8/lexset/test_ssim.py` & `lexset-4.2.9/lexset/test_ssim.py`

 * *Files identical despite different names*

### Comparing `lexset-4.2.8/setup.py` & `lexset-4.2.9/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 
 setup(name='lexset',
-      version='4.2.8',
+      version='4.2.9',
       author='F. Bitonti',
       author_email='Francis@lexset.ai',
       license='Apache 2.0',
       classifiers=[
           'Development Status :: 4 - Beta',
           'Programming Language :: Python :: 3'
       ],
```

