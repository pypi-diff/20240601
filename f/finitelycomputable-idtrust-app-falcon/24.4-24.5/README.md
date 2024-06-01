# Comparing `tmp/finitelycomputable_idtrust_app_falcon-24.4.tar.gz` & `tmp/finitelycomputable_idtrust_app_falcon-24.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable_idtrust_app_falcon-24.4.tar", last modified: Tue Apr 30 04:47:26 2024, max compression
+gzip compressed data, was "finitelycomputable_idtrust_app_falcon-24.5.tar", last modified: Sat Jun  1 03:11:30 2024, max compression
```

## Comparing `finitelycomputable_idtrust_app_falcon-24.4.tar` & `finitelycomputable_idtrust_app_falcon-24.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:26.531888 finitelycomputable_idtrust_app_falcon-24.4/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2258 2024-04-30 04:47:26.531888 finitelycomputable_idtrust_app_falcon-24.4/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      198 2024-03-16 18:32:50.000000 finitelycomputable_idtrust_app_falcon-24.4/README.rst
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:26.531888 finitelycomputable_idtrust_app_falcon-24.4/finitelycomputable/
--rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)     6897 2024-04-25 20:05:48.000000 finitelycomputable_idtrust_app_falcon-24.4/finitelycomputable/idtrust_app_falcon.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:26.531888 finitelycomputable_idtrust_app_falcon-24.4/finitelycomputable/tests/
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     9011 2024-04-30 04:36:59.000000 finitelycomputable_idtrust_app_falcon-24.4/finitelycomputable/tests/test_idtrust_falcon.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:26.531888 finitelycomputable_idtrust_app_falcon-24.4/finitelycomputable_idtrust_app_falcon.egg-info/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2258 2024-04-30 04:47:26.000000 finitelycomputable_idtrust_app_falcon-24.4/finitelycomputable_idtrust_app_falcon.egg-info/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      482 2024-04-30 04:47:26.000000 finitelycomputable_idtrust_app_falcon-24.4/finitelycomputable_idtrust_app_falcon.egg-info/SOURCES.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-30 04:47:26.000000 finitelycomputable_idtrust_app_falcon-24.4/finitelycomputable_idtrust_app_falcon.egg-info/dependency_links.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      100 2024-04-30 04:47:26.000000 finitelycomputable_idtrust_app_falcon-24.4/finitelycomputable_idtrust_app_falcon.egg-info/entry_points.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      224 2024-04-30 04:47:26.000000 finitelycomputable_idtrust_app_falcon-24.4/finitelycomputable_idtrust_app_falcon.egg-info/requires.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-30 04:47:26.000000 finitelycomputable_idtrust_app_falcon-24.4/finitelycomputable_idtrust_app_falcon.egg-info/top_level.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1841 2024-04-28 21:51:18.000000 finitelycomputable_idtrust_app_falcon-24.4/pyproject.toml
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-30 04:47:26.531888 finitelycomputable_idtrust_app_falcon-24.4/setup.cfg
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:30.235304 finitelycomputable_idtrust_app_falcon-24.5/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2258 2024-06-01 03:11:30.235304 finitelycomputable_idtrust_app_falcon-24.5/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      198 2024-06-01 03:00:08.000000 finitelycomputable_idtrust_app_falcon-24.5/README.rst
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:30.231304 finitelycomputable_idtrust_app_falcon-24.5/finitelycomputable/
+-rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)     6897 2024-06-01 03:00:08.000000 finitelycomputable_idtrust_app_falcon-24.5/finitelycomputable/idtrust_app_falcon.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:30.231304 finitelycomputable_idtrust_app_falcon-24.5/finitelycomputable/tests/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     9011 2024-06-01 03:00:08.000000 finitelycomputable_idtrust_app_falcon-24.5/finitelycomputable/tests/test_idtrust_falcon.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:30.231304 finitelycomputable_idtrust_app_falcon-24.5/finitelycomputable_idtrust_app_falcon.egg-info/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2258 2024-06-01 03:11:30.000000 finitelycomputable_idtrust_app_falcon-24.5/finitelycomputable_idtrust_app_falcon.egg-info/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      482 2024-06-01 03:11:30.000000 finitelycomputable_idtrust_app_falcon-24.5/finitelycomputable_idtrust_app_falcon.egg-info/SOURCES.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-06-01 03:11:30.000000 finitelycomputable_idtrust_app_falcon-24.5/finitelycomputable_idtrust_app_falcon.egg-info/dependency_links.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      100 2024-06-01 03:11:30.000000 finitelycomputable_idtrust_app_falcon-24.5/finitelycomputable_idtrust_app_falcon.egg-info/entry_points.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      224 2024-06-01 03:11:30.000000 finitelycomputable_idtrust_app_falcon-24.5/finitelycomputable_idtrust_app_falcon.egg-info/requires.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-06-01 03:11:30.000000 finitelycomputable_idtrust_app_falcon-24.5/finitelycomputable_idtrust_app_falcon.egg-info/top_level.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1841 2024-06-01 03:11:28.000000 finitelycomputable_idtrust_app_falcon-24.5/pyproject.toml
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-06-01 03:11:30.235304 finitelycomputable_idtrust_app_falcon-24.5/setup.cfg
```

### Comparing `finitelycomputable_idtrust_app_falcon-24.4/PKG-INFO` & `finitelycomputable_idtrust_app_falcon-24.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-idtrust-app-falcon
-Version: 24.4
+Version: 24.5
 Summary: The Falcon-dependent code for a microsite to explore identifying game-theory strategies
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/identification_of_trust
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
```

### Comparing `finitelycomputable_idtrust_app_falcon-24.4/finitelycomputable/idtrust_app_falcon.py` & `finitelycomputable_idtrust_app_falcon-24.5/finitelycomputable/idtrust_app_falcon.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable_idtrust_app_falcon-24.4/finitelycomputable/tests/test_idtrust_falcon.py` & `finitelycomputable_idtrust_app_falcon-24.5/finitelycomputable/tests/test_idtrust_falcon.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable_idtrust_app_falcon-24.4/finitelycomputable_idtrust_app_falcon.egg-info/PKG-INFO` & `finitelycomputable_idtrust_app_falcon-24.5/finitelycomputable_idtrust_app_falcon.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-idtrust-app-falcon
-Version: 24.4
+Version: 24.5
 Summary: The Falcon-dependent code for a microsite to explore identifying game-theory strategies
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/identification_of_trust
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
```

### Comparing `finitelycomputable_idtrust_app_falcon-24.4/pyproject.toml` & `finitelycomputable_idtrust_app_falcon-24.5/pyproject.toml`

 * *Files 5% similar despite different names*

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
 name = "finitelycomputable-idtrust-app-falcon"
 requires-python = ">=3.8"
 description = "The Falcon-dependent code for a microsite to explore identifying game-theory strategies"
 dependencies = [
   "finitelycomputable-idtrust-common",
   "falcon~=3.1",
 ]
```

