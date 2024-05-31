# Comparing `tmp/fiftyone_db-1.1.3rc1.tar.gz` & `tmp/fiftyone_db-1.1.3rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fiftyone_db-1.1.3rc1.tar", last modified: Tue May 28 23:16:47 2024, max compression
+gzip compressed data, was "fiftyone_db-1.1.3rc2.tar", last modified: Fri May 31 22:06:02 2024, max compression
```

## Comparing `fiftyone_db-1.1.3rc1.tar` & `fiftyone_db-1.1.3rc2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:16:47.238535 fiftyone_db-1.1.3rc1/
--rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-28 23:16:39.000000 fiftyone_db-1.1.3rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-28 23:16:47.238535 fiftyone_db-1.1.3rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-28 23:16:42.000000 fiftyone_db-1.1.3rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:16:47.238535 fiftyone_db-1.1.3rc1/fiftyone_db.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-28 23:16:47.000000 fiftyone_db-1.1.3rc1/fiftyone_db.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-28 23:16:47.000000 fiftyone_db-1.1.3rc1/fiftyone_db.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 23:16:47.000000 fiftyone_db-1.1.3rc1/fiftyone_db.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-28 23:16:47.000000 fiftyone_db-1.1.3rc1/fiftyone_db.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-28 23:16:42.000000 fiftyone_db-1.1.3rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 23:16:47.238535 fiftyone_db-1.1.3rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)    10610 2024-05-28 23:16:42.000000 fiftyone_db-1.1.3rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:16:47.238535 fiftyone_db-1.1.3rc1/src/
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-28 23:16:42.000000 fiftyone_db-1.1.3rc1/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 23:16:47.238535 fiftyone_db-1.1.3rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-28 23:16:42.000000 fiftyone_db-1.1.3rc1/tests/test_db.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:06:02.294437 fiftyone_db-1.1.3rc2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11349 2024-05-31 22:05:54.000000 fiftyone_db-1.1.3rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-31 22:06:02.294437 fiftyone_db-1.1.3rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-31 22:05:57.000000 fiftyone_db-1.1.3rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:06:02.290437 fiftyone_db-1.1.3rc2/fiftyone_db.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-31 22:06:02.000000 fiftyone_db-1.1.3rc2/fiftyone_db.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      214 2024-05-31 22:06:02.000000 fiftyone_db-1.1.3rc2/fiftyone_db.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:06:02.000000 fiftyone_db-1.1.3rc2/fiftyone_db.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 22:06:02.000000 fiftyone_db-1.1.3rc2/fiftyone_db.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-05-31 22:05:57.000000 fiftyone_db-1.1.3rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 22:06:02.294437 fiftyone_db-1.1.3rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)    10610 2024-05-31 22:05:57.000000 fiftyone_db-1.1.3rc2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:06:02.290437 fiftyone_db-1.1.3rc2/src/
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-31 22:05:57.000000 fiftyone_db-1.1.3rc2/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:06:02.290437 fiftyone_db-1.1.3rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-05-31 22:05:57.000000 fiftyone_db-1.1.3rc2/tests/test_db.py
```

### Comparing `fiftyone_db-1.1.3rc1/LICENSE` & `fiftyone_db-1.1.3rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `fiftyone_db-1.1.3rc1/PKG-INFO` & `fiftyone_db-1.1.3rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone_db
-Version: 1.1.3rc1
+Version: 1.1.3rc2
 Summary: FiftyOne DB
 Home-page: https://github.com/voxel51/fiftyone
 Author: Voxel51, Inc.
 Author-email: info@voxel51.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `fiftyone_db-1.1.3rc1/fiftyone_db.egg-info/PKG-INFO` & `fiftyone_db-1.1.3rc2/fiftyone_db.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fiftyone_db
-Version: 1.1.3rc1
+Version: 1.1.3rc2
 Summary: FiftyOne DB
 Home-page: https://github.com/voxel51/fiftyone
 Author: Voxel51, Inc.
 Author-email: info@voxel51.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `fiftyone_db-1.1.3rc1/setup.py` & `fiftyone_db-1.1.3rc2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 """
 Installs the ``fiftyone-db`` package.
 
-| Copyright 2017-2023, Voxel51, Inc.
+| Copyright 2017-2024, Voxel51, Inc.
 | `voxel51.com <https://voxel51.com/>`_
 |
 """
 import csv
 import os
 import pathlib
 import platform
```

