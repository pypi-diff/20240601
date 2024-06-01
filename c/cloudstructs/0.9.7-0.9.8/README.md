# Comparing `tmp/cloudstructs-0.9.7.tar.gz` & `tmp/cloudstructs-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudstructs-0.9.7.tar", last modified: Sat May 25 13:35:16 2024, max compression
+gzip compressed data, was "cloudstructs-0.9.8.tar", last modified: Sat Jun  1 11:18:43 2024, max compression
```

## Comparing `cloudstructs-0.9.7.tar` & `cloudstructs-0.9.8.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:35:16.264942 cloudstructs-0.9.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-05-25 13:35:06.000000 cloudstructs-0.9.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-25 13:35:06.000000 cloudstructs-0.9.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-25 13:35:16.264942 cloudstructs-0.9.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-25 13:35:06.000000 cloudstructs-0.9.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-05-25 13:35:06.000000 cloudstructs-0.9.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-25 13:35:16.264942 cloudstructs-0.9.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-05-25 13:35:06.000000 cloudstructs-0.9.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:35:16.256942 cloudstructs-0.9.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:35:16.260942 cloudstructs-0.9.7/src/cloudstructs/
--rw-r--r--   0 runner    (1001) docker     (127)   184196 2024-05-25 13:35:06.000000 cloudstructs-0.9.7/src/cloudstructs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:35:16.260942 cloudstructs-0.9.7/src/cloudstructs/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-25 13:35:06.000000 cloudstructs-0.9.7/src/cloudstructs/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)  3338536 2024-05-25 13:35:06.000000 cloudstructs-0.9.7/src/cloudstructs/_jsii/cloudstructs@0.9.7.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 13:35:06.000000 cloudstructs-0.9.7/src/cloudstructs/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-25 13:35:16.260942 cloudstructs-0.9.7/src/cloudstructs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-05-25 13:35:16.000000 cloudstructs-0.9.7/src/cloudstructs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-25 13:35:16.000000 cloudstructs-0.9.7/src/cloudstructs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-25 13:35:16.000000 cloudstructs-0.9.7/src/cloudstructs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-25 13:35:16.000000 cloudstructs-0.9.7/src/cloudstructs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-25 13:35:16.000000 cloudstructs-0.9.7/src/cloudstructs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:18:43.147482 cloudstructs-0.9.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-06-01 11:18:29.000000 cloudstructs-0.9.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-01 11:18:29.000000 cloudstructs-0.9.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-06-01 11:18:43.147482 cloudstructs-0.9.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-06-01 11:18:29.000000 cloudstructs-0.9.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-06-01 11:18:29.000000 cloudstructs-0.9.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 11:18:43.147482 cloudstructs-0.9.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1733 2024-06-01 11:18:29.000000 cloudstructs-0.9.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:18:43.139482 cloudstructs-0.9.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:18:43.139482 cloudstructs-0.9.8/src/cloudstructs/
+-rw-r--r--   0 runner    (1001) docker     (127)   184196 2024-06-01 11:18:29.000000 cloudstructs-0.9.8/src/cloudstructs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:18:43.139482 cloudstructs-0.9.8/src/cloudstructs/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-06-01 11:18:29.000000 cloudstructs-0.9.8/src/cloudstructs/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)  3393397 2024-06-01 11:18:29.000000 cloudstructs-0.9.8/src/cloudstructs/_jsii/cloudstructs@0.9.8.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 11:18:29.000000 cloudstructs-0.9.8/src/cloudstructs/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 11:18:43.139482 cloudstructs-0.9.8/src/cloudstructs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2409 2024-06-01 11:18:43.000000 cloudstructs-0.9.8/src/cloudstructs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-06-01 11:18:43.000000 cloudstructs-0.9.8/src/cloudstructs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 11:18:43.000000 cloudstructs-0.9.8/src/cloudstructs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-06-01 11:18:43.000000 cloudstructs-0.9.8/src/cloudstructs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-01 11:18:43.000000 cloudstructs-0.9.8/src/cloudstructs.egg-info/top_level.txt
```

### Comparing `cloudstructs-0.9.7/LICENSE` & `cloudstructs-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudstructs-0.9.7/PKG-INFO` & `cloudstructs-0.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudstructs
-Version: 0.9.7
+Version: 0.9.8
 Summary: High-level constructs for AWS CDK
 Home-page: https://github.com/jogold/cloudstructs.git
 Author: Jonathan Goldwasser<jonathan.goldwasser@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/jogold/cloudstructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cloudstructs-0.9.7/README.md` & `cloudstructs-0.9.8/README.md`

 * *Files identical despite different names*

### Comparing `cloudstructs-0.9.7/setup.py` & `cloudstructs-0.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cloudstructs",
-    "version": "0.9.7",
+    "version": "0.9.8",
     "description": "High-level constructs for AWS CDK",
     "license": "Apache-2.0",
     "url": "https://github.com/jogold/cloudstructs.git",
     "long_description_content_type": "text/markdown",
     "author": "Jonathan Goldwasser<jonathan.goldwasser@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cloudstructs",
         "cloudstructs._jsii"
     ],
     "package_data": {
         "cloudstructs._jsii": [
-            "cloudstructs@0.9.7.jsii.tgz"
+            "cloudstructs@0.9.8.jsii.tgz"
         ],
         "cloudstructs": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
```

### Comparing `cloudstructs-0.9.7/src/cloudstructs/__init__.py` & `cloudstructs-0.9.8/src/cloudstructs/__init__.py`

 * *Files identical despite different names*

### Comparing `cloudstructs-0.9.7/src/cloudstructs.egg-info/PKG-INFO` & `cloudstructs-0.9.8/src/cloudstructs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudstructs
-Version: 0.9.7
+Version: 0.9.8
 Summary: High-level constructs for AWS CDK
 Home-page: https://github.com/jogold/cloudstructs.git
 Author: Jonathan Goldwasser<jonathan.goldwasser@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/jogold/cloudstructs.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

