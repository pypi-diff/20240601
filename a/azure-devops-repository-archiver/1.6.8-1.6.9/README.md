# Comparing `tmp/azure-devops-repository-archiver-1.6.8.tar.gz` & `tmp/azure-devops-repository-archiver-1.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "azure-devops-repository-archiver-1.6.8.tar", last modified: Fri Mar  1 04:53:52 2024, max compression
+gzip compressed data, was "azure-devops-repository-archiver-1.6.9.tar", last modified: Mon Apr  1 07:23:29 2024, max compression
```

## Comparing `azure-devops-repository-archiver-1.6.8.tar` & `azure-devops-repository-archiver-1.6.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:53:52.503357 azure-devops-repository-archiver-1.6.8/
--rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-03-01 04:53:40.000000 azure-devops-repository-archiver-1.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-01 04:53:40.000000 azure-devops-repository-archiver-1.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-01 04:53:52.503357 azure-devops-repository-archiver-1.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-03-01 04:53:40.000000 azure-devops-repository-archiver-1.6.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-03-01 04:53:40.000000 azure-devops-repository-archiver-1.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-01 04:53:52.503357 azure-devops-repository-archiver-1.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-01 04:53:40.000000 azure-devops-repository-archiver-1.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:53:52.499357 azure-devops-repository-archiver-1.6.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:53:52.503357 azure-devops-repository-archiver-1.6.8/src/azure_devops_repository_archiver/
--rw-r--r--   0 runner    (1001) docker     (127)    17158 2024-03-01 04:53:40.000000 azure-devops-repository-archiver-1.6.8/src/azure_devops_repository_archiver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:53:52.503357 azure-devops-repository-archiver-1.6.8/src/azure_devops_repository_archiver/_jsii/
--rw-r--r--   0 runner    (1001) docker     (127)      444 2024-03-01 04:53:40.000000 azure-devops-repository-archiver-1.6.8/src/azure_devops_repository_archiver/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31527 2024-03-01 04:53:40.000000 azure-devops-repository-archiver-1.6.8/src/azure_devops_repository_archiver/_jsii/azure-devops-repository-archiver@1.6.8.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 04:53:40.000000 azure-devops-repository-archiver-1.6.8/src/azure_devops_repository_archiver/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-01 04:53:52.503357 azure-devops-repository-archiver-1.6.8/src/azure_devops_repository_archiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-03-01 04:53:52.000000 azure-devops-repository-archiver-1.6.8/src/azure_devops_repository_archiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-01 04:53:52.000000 azure-devops-repository-archiver-1.6.8/src/azure_devops_repository_archiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-01 04:53:52.000000 azure-devops-repository-archiver-1.6.8/src/azure_devops_repository_archiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-01 04:53:52.000000 azure-devops-repository-archiver-1.6.8/src/azure_devops_repository_archiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-01 04:53:52.000000 azure-devops-repository-archiver-1.6.8/src/azure_devops_repository_archiver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:23:29.889437 azure-devops-repository-archiver-1.6.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    11358 2024-04-01 07:23:14.000000 azure-devops-repository-archiver-1.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-01 07:23:14.000000 azure-devops-repository-archiver-1.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 07:23:29.889437 azure-devops-repository-archiver-1.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-01 07:23:14.000000 azure-devops-repository-archiver-1.6.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-01 07:23:14.000000 azure-devops-repository-archiver-1.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 07:23:29.889437 azure-devops-repository-archiver-1.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-04-01 07:23:14.000000 azure-devops-repository-archiver-1.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:23:29.885437 azure-devops-repository-archiver-1.6.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:23:29.885437 azure-devops-repository-archiver-1.6.9/src/azure_devops_repository_archiver/
+-rw-r--r--   0 runner    (1001) docker     (127)    17234 2024-04-01 07:23:14.000000 azure-devops-repository-archiver-1.6.9/src/azure_devops_repository_archiver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:23:29.889437 azure-devops-repository-archiver-1.6.9/src/azure_devops_repository_archiver/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-01 07:23:14.000000 azure-devops-repository-archiver-1.6.9/src/azure_devops_repository_archiver/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31528 2024-04-01 07:23:14.000000 azure-devops-repository-archiver-1.6.9/src/azure_devops_repository_archiver/_jsii/azure-devops-repository-archiver@1.6.9.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 07:23:14.000000 azure-devops-repository-archiver-1.6.9/src/azure_devops_repository_archiver/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 07:23:29.885437 azure-devops-repository-archiver-1.6.9/src/azure_devops_repository_archiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-01 07:23:29.000000 azure-devops-repository-archiver-1.6.9/src/azure_devops_repository_archiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-01 07:23:29.000000 azure-devops-repository-archiver-1.6.9/src/azure_devops_repository_archiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 07:23:29.000000 azure-devops-repository-archiver-1.6.9/src/azure_devops_repository_archiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 07:23:29.000000 azure-devops-repository-archiver-1.6.9/src/azure_devops_repository_archiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-01 07:23:29.000000 azure-devops-repository-archiver-1.6.9/src/azure_devops_repository_archiver.egg-info/top_level.txt
```

### Comparing `azure-devops-repository-archiver-1.6.8/LICENSE` & `azure-devops-repository-archiver-1.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `azure-devops-repository-archiver-1.6.8/PKG-INFO` & `azure-devops-repository-archiver-1.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-devops-repository-archiver
-Version: 1.6.8
+Version: 1.6.9
 Summary: Archive Azure DevOps git repositories to AWS S3
 Home-page: https://github.com/stefanfreitag/azure_s3_repository_archiver.git
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/azure_s3_repository_archiver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `azure-devops-repository-archiver-1.6.8/setup.py` & `azure-devops-repository-archiver-1.6.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "azure-devops-repository-archiver",
-    "version": "1.6.8",
+    "version": "1.6.9",
     "description": "Archive Azure DevOps git repositories to AWS S3",
     "license": "Apache-2.0",
     "url": "https://github.com/stefanfreitag/azure_s3_repository_archiver.git",
     "long_description_content_type": "text/markdown",
     "author": "Stefan Freitag<stefan.freitag@udo.edu>",
     "bdist_wheel": {
         "universal": true
@@ -22,25 +22,25 @@
     },
     "packages": [
         "azure_devops_repository_archiver",
         "azure_devops_repository_archiver._jsii"
     ],
     "package_data": {
         "azure_devops_repository_archiver._jsii": [
-            "azure-devops-repository-archiver@1.6.8.jsii.tgz"
+            "azure-devops-repository-archiver@1.6.9.jsii.tgz"
         ],
         "azure_devops_repository_archiver": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.8",
     "install_requires": [
         "aws-cdk-lib>=2.117.0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.94.0, <2.0.0",
+        "jsii>=1.96.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `azure-devops-repository-archiver-1.6.8/src/azure_devops_repository_archiver/__init__.py` & `azure-devops-repository-archiver-1.6.9/src/azure_devops_repository_archiver/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 
 The documentation is available [here](https://stefanfreitag.github.io/azure_s3_repository_archiver/).
 
 ## How to contribute
 
 * See [CONTRIBUTING.md](CONTRIBUTING.md) for how to contribute to this project.
 '''
+from pkgutil import extend_path
+__path__ = extend_path(__path__, __name__)
+
 import abc
 import builtins
 import datetime
 import enum
 import typing
 
 import jsii
```

### Comparing `azure-devops-repository-archiver-1.6.8/src/azure_devops_repository_archiver.egg-info/PKG-INFO` & `azure-devops-repository-archiver-1.6.9/src/azure_devops_repository_archiver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-devops-repository-archiver
-Version: 1.6.8
+Version: 1.6.9
 Summary: Archive Azure DevOps git repositories to AWS S3
 Home-page: https://github.com/stefanfreitag/azure_s3_repository_archiver.git
 Author: Stefan Freitag<stefan.freitag@udo.edu>
 License: Apache-2.0
 Project-URL: Source, https://github.com/stefanfreitag/azure_s3_repository_archiver.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `azure-devops-repository-archiver-1.6.8/src/azure_devops_repository_archiver.egg-info/SOURCES.txt` & `azure-devops-repository-archiver-1.6.9/src/azure_devops_repository_archiver.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/azure_devops_repository_archiver/py.typed
 src/azure_devops_repository_archiver.egg-info/PKG-INFO
 src/azure_devops_repository_archiver.egg-info/SOURCES.txt
 src/azure_devops_repository_archiver.egg-info/dependency_links.txt
 src/azure_devops_repository_archiver.egg-info/requires.txt
 src/azure_devops_repository_archiver.egg-info/top_level.txt
 src/azure_devops_repository_archiver/_jsii/__init__.py
-src/azure_devops_repository_archiver/_jsii/azure-devops-repository-archiver@1.6.8.jsii.tgz
+src/azure_devops_repository_archiver/_jsii/azure-devops-repository-archiver@1.6.9.jsii.tgz
```

