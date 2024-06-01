# Comparing `tmp/ptipython_metapackage-1.2.1.tar.gz` & `tmp/ptipython_metapackage-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptipython_metapackage-1.2.1.tar", last modified: Tue May 28 01:33:13 2024, max compression
+gzip compressed data, was "ptipython_metapackage-1.3.0.tar", last modified: Sat Jun  1 01:38:56 2024, max compression
```

## Comparing `ptipython_metapackage-1.2.1.tar` & `ptipython_metapackage-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:33:13.033721 ptipython_metapackage-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-28 01:33:05.000000 ptipython_metapackage-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-28 01:33:13.033721 ptipython_metapackage-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-28 01:33:05.000000 ptipython_metapackage-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:33:13.033721 ptipython_metapackage-1.2.1/ptipython_metapackage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-05-28 01:33:13.000000 ptipython_metapackage-1.2.1/ptipython_metapackage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-05-28 01:33:13.000000 ptipython_metapackage-1.2.1/ptipython_metapackage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:33:13.000000 ptipython_metapackage-1.2.1/ptipython_metapackage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-28 01:33:13.000000 ptipython_metapackage-1.2.1/ptipython_metapackage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-28 01:33:13.000000 ptipython_metapackage-1.2.1/ptipython_metapackage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-28 01:33:13.000000 ptipython_metapackage-1.2.1/ptipython_metapackage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-05-28 01:33:05.000000 ptipython_metapackage-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-28 01:33:13.033721 ptipython_metapackage-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-28 01:33:13.033721 ptipython_metapackage-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-28 01:33:05.000000 ptipython_metapackage-1.2.1/tests/test_bump_metapackage_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-28 01:33:05.000000 ptipython_metapackage-1.2.1/tests/test_compare_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:38:56.067712 ptipython_metapackage-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-06-01 01:38:48.000000 ptipython_metapackage-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-06-01 01:38:56.067712 ptipython_metapackage-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-06-01 01:38:48.000000 ptipython_metapackage-1.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:38:56.067712 ptipython_metapackage-1.3.0/ptipython_metapackage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-06-01 01:38:56.000000 ptipython_metapackage-1.3.0/ptipython_metapackage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-06-01 01:38:56.000000 ptipython_metapackage-1.3.0/ptipython_metapackage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:38:56.000000 ptipython_metapackage-1.3.0/ptipython_metapackage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-01 01:38:56.000000 ptipython_metapackage-1.3.0/ptipython_metapackage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 01:38:56.000000 ptipython_metapackage-1.3.0/ptipython_metapackage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:38:56.000000 ptipython_metapackage-1.3.0/ptipython_metapackage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-06-01 01:38:48.000000 ptipython_metapackage-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:38:56.067712 ptipython_metapackage-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:38:56.067712 ptipython_metapackage-1.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-06-01 01:38:48.000000 ptipython_metapackage-1.3.0/tests/test_bump_metapackage_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-06-01 01:38:48.000000 ptipython_metapackage-1.3.0/tests/test_compare_versions.py
```

### Comparing `ptipython_metapackage-1.2.1/LICENSE` & `ptipython_metapackage-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ptipython_metapackage-1.2.1/PKG-INFO` & `ptipython_metapackage-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptipython-metapackage
-Version: 1.2.1
+Version: 1.3.0
 Summary: ptipython metapackage
 Author-email: Dmitry Meyer <me@undef.im>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/un-def/ptipython-metapackage
 Project-URL: Repository, https://github.com/un-def/ptipython-metapackage.git
 Project-URL: Changelog, https://github.com/un-def/ptipython-metapackage/releases
 Project-URL: Issues, https://github.com/un-def/ptipython-metapackage/issues
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ptpython==3.0.27
-Requires-Dist: ipython==8.24.0
+Requires-Dist: ipython==8.25.0
 
 # ptipython metapackage
 
 ptpython + ipython = ptipython
 
 ## Description
```

### Comparing `ptipython_metapackage-1.2.1/README.md` & `ptipython_metapackage-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ptipython_metapackage-1.2.1/ptipython_metapackage.egg-info/PKG-INFO` & `ptipython_metapackage-1.3.0/ptipython_metapackage.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ptipython-metapackage
-Version: 1.2.1
+Version: 1.3.0
 Summary: ptipython metapackage
 Author-email: Dmitry Meyer <me@undef.im>
 License: BSD-3-Clause
 Project-URL: Homepage, https://github.com/un-def/ptipython-metapackage
 Project-URL: Repository, https://github.com/un-def/ptipython-metapackage.git
 Project-URL: Changelog, https://github.com/un-def/ptipython-metapackage/releases
 Project-URL: Issues, https://github.com/un-def/ptipython-metapackage/issues
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: ptpython==3.0.27
-Requires-Dist: ipython==8.24.0
+Requires-Dist: ipython==8.25.0
 
 # ptipython metapackage
 
 ptpython + ipython = ptipython
 
 ## Description
```

### Comparing `ptipython_metapackage-1.2.1/pyproject.toml` & `ptipython_metapackage-1.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ptipython-metapackage"
-version = "1.2.1"
+version = "1.3.0"
 description = "ptipython metapackage"
 readme = "README.md"
 license = {text = "BSD-3-Clause"}
 authors = [
     {name = "Dmitry Meyer", email = "me@undef.im"},
 ]
 classifiers = [
@@ -17,15 +17,15 @@
     "License :: OSI Approved :: BSD License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
 ]
 keywords = ["ptipython", "ptpython", "ipython"]
 requires-python = ">= 3.10"
-dependencies = ["ptpython == 3.0.27", "ipython == 8.24.0"]
+dependencies = ["ptpython == 3.0.27", "ipython == 8.25.0"]
 
 [project.scripts]
 ptipython = "ptpython.entry_points.run_ptipython:run"
 ptpython = "ptpython.entry_points.run_ptpython:run"
 ipython = "IPython:start_ipython"
 
 [project.urls]
```

### Comparing `ptipython_metapackage-1.2.1/tests/test_compare_versions.py` & `ptipython_metapackage-1.3.0/tests/test_compare_versions.py`

 * *Files identical despite different names*

