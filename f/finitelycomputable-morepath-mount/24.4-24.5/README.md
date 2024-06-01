# Comparing `tmp/finitelycomputable_morepath_mount-24.4.tar.gz` & `tmp/finitelycomputable_morepath_mount-24.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable_morepath_mount-24.4.tar", last modified: Tue Apr 30 04:45:01 2024, max compression
+gzip compressed data, was "finitelycomputable_morepath_mount-24.5.tar", last modified: Sat Jun  1 03:09:15 2024, max compression
```

## Comparing `finitelycomputable_morepath_mount-24.4.tar` & `finitelycomputable_morepath_mount-24.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:45:01.039219 finitelycomputable_morepath_mount-24.4/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2347 2024-04-30 04:45:01.039219 finitelycomputable_morepath_mount-24.4/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      193 2023-09-12 03:23:48.000000 finitelycomputable_morepath_mount-24.4/README.rst
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:45:01.035219 finitelycomputable_morepath_mount-24.4/finitelycomputable/
--rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)     1560 2023-11-30 06:01:53.000000 finitelycomputable_morepath_mount-24.4/finitelycomputable/morepath_mount.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:45:01.035219 finitelycomputable_morepath_mount-24.4/finitelycomputable/tests/
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      566 2024-04-30 03:37:13.000000 finitelycomputable_morepath_mount-24.4/finitelycomputable/tests/test_morepath_mount.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:45:01.039219 finitelycomputable_morepath_mount-24.4/finitelycomputable_morepath_mount.egg-info/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2347 2024-04-30 04:45:01.000000 finitelycomputable_morepath_mount-24.4/finitelycomputable_morepath_mount.egg-info/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      493 2024-04-30 04:45:01.000000 finitelycomputable_morepath_mount-24.4/finitelycomputable_morepath_mount.egg-info/SOURCES.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-30 04:45:01.000000 finitelycomputable_morepath_mount-24.4/finitelycomputable_morepath_mount.egg-info/dependency_links.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       92 2024-04-30 04:45:01.000000 finitelycomputable_morepath_mount-24.4/finitelycomputable_morepath_mount.egg-info/entry_points.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      254 2024-04-30 04:45:01.000000 finitelycomputable_morepath_mount-24.4/finitelycomputable_morepath_mount.egg-info/requires.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-30 04:45:01.000000 finitelycomputable_morepath_mount-24.4/finitelycomputable_morepath_mount.egg-info/top_level.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1861 2024-04-28 21:51:18.000000 finitelycomputable_morepath_mount-24.4/pyproject.toml
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-30 04:45:01.039219 finitelycomputable_morepath_mount-24.4/setup.cfg
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:09:15.202459 finitelycomputable_morepath_mount-24.5/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2347 2024-06-01 03:09:15.202459 finitelycomputable_morepath_mount-24.5/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      193 2024-06-01 03:00:08.000000 finitelycomputable_morepath_mount-24.5/README.rst
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:09:15.202459 finitelycomputable_morepath_mount-24.5/finitelycomputable/
+-rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)     1560 2024-06-01 03:00:08.000000 finitelycomputable_morepath_mount-24.5/finitelycomputable/morepath_mount.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:09:15.202459 finitelycomputable_morepath_mount-24.5/finitelycomputable/tests/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      566 2024-06-01 03:06:55.000000 finitelycomputable_morepath_mount-24.5/finitelycomputable/tests/test_morepath_mount.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:09:15.202459 finitelycomputable_morepath_mount-24.5/finitelycomputable_morepath_mount.egg-info/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2347 2024-06-01 03:09:15.000000 finitelycomputable_morepath_mount-24.5/finitelycomputable_morepath_mount.egg-info/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      454 2024-06-01 03:09:15.000000 finitelycomputable_morepath_mount-24.5/finitelycomputable_morepath_mount.egg-info/SOURCES.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-06-01 03:09:15.000000 finitelycomputable_morepath_mount-24.5/finitelycomputable_morepath_mount.egg-info/dependency_links.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       92 2024-06-01 03:09:15.000000 finitelycomputable_morepath_mount-24.5/finitelycomputable_morepath_mount.egg-info/entry_points.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      254 2024-06-01 03:09:15.000000 finitelycomputable_morepath_mount-24.5/finitelycomputable_morepath_mount.egg-info/requires.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-06-01 03:09:15.000000 finitelycomputable_morepath_mount-24.5/finitelycomputable_morepath_mount.egg-info/top_level.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1861 2024-06-01 03:09:13.000000 finitelycomputable_morepath_mount-24.5/pyproject.toml
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-06-01 03:09:15.202459 finitelycomputable_morepath_mount-24.5/setup.cfg
```

### Comparing `finitelycomputable_morepath_mount-24.4/PKG-INFO` & `finitelycomputable_morepath_mount-24.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-morepath-mount
-Version: 24.4
+Version: 24.5
 Summary: The Morepath-based wsgi app using Morepath.mount to combine the microsites of finitelycomputable.net
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/wsgi_info
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
```

### Comparing `finitelycomputable_morepath_mount-24.4/finitelycomputable/morepath_mount.py` & `finitelycomputable_morepath_mount-24.5/finitelycomputable/morepath_mount.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable_morepath_mount-24.4/finitelycomputable/tests/test_morepath_mount.py` & `finitelycomputable_morepath_mount-24.5/finitelycomputable/tests/test_morepath_mount.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable_morepath_mount-24.4/finitelycomputable_morepath_mount.egg-info/PKG-INFO` & `finitelycomputable_morepath_mount-24.5/finitelycomputable_morepath_mount.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-morepath-mount
-Version: 24.4
+Version: 24.5
 Summary: The Morepath-based wsgi app using Morepath.mount to combine the microsites of finitelycomputable.net
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/wsgi_info
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
```

### Comparing `finitelycomputable_morepath_mount-24.4/pyproject.toml` & `finitelycomputable_morepath_mount-24.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 authors = [{name = "Samuel Newbold", email = "sam@rwsh.org"}]
 license = {text = "AGPL-3.0-only"}
 readme = "README.rst"
-version = "24.4"
+version = "24.5"
 name = "finitelycomputable-morepath-mount"
 requires-python = ">=3.8"
 description = "The Morepath-based wsgi app using Morepath.mount to combine the microsites of finitelycomputable.net"
 dependencies = [
   "morepath~=0.19",
 ]
 classifiers = [
```

