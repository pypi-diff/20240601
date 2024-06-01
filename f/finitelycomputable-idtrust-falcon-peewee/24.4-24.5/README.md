# Comparing `tmp/finitelycomputable_idtrust_falcon_peewee-24.4.tar.gz` & `tmp/finitelycomputable_idtrust_falcon_peewee-24.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable_idtrust_falcon_peewee-24.4.tar", last modified: Tue Apr 30 04:47:31 2024, max compression
+gzip compressed data, was "finitelycomputable_idtrust_falcon_peewee-24.5.tar", last modified: Sat Jun  1 03:11:34 2024, max compression
```

## Comparing `finitelycomputable_idtrust_falcon_peewee-24.4.tar` & `finitelycomputable_idtrust_falcon_peewee-24.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:31.127909 finitelycomputable_idtrust_falcon_peewee-24.4/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2433 2024-04-30 04:47:31.127909 finitelycomputable_idtrust_falcon_peewee-24.4/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      330 2024-03-18 03:42:34.000000 finitelycomputable_idtrust_falcon_peewee-24.4/README.rst
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:31.127909 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable/
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:31.127909 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable/idtrust_falcon/
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       55 2024-03-18 04:20:08.000000 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable/idtrust_falcon/__init__.py
--rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)      119 2024-03-18 04:22:15.000000 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable/idtrust_falcon/peewee.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:31.127909 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable_idtrust_falcon_peewee.egg-info/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2433 2024-04-30 04:47:31.000000 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable_idtrust_falcon_peewee.egg-info/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      501 2024-04-30 04:47:31.000000 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable_idtrust_falcon_peewee.egg-info/SOURCES.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-30 04:47:31.000000 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable_idtrust_falcon_peewee.egg-info/dependency_links.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      103 2024-04-30 04:47:31.000000 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable_idtrust_falcon_peewee.egg-info/entry_points.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      265 2024-04-30 04:47:31.000000 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable_idtrust_falcon_peewee.egg-info/requires.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-30 04:47:31.000000 finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable_idtrust_falcon_peewee.egg-info/top_level.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1877 2024-04-28 21:51:18.000000 finitelycomputable_idtrust_falcon_peewee-24.4/pyproject.toml
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-30 04:47:31.127909 finitelycomputable_idtrust_falcon_peewee-24.4/setup.cfg
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:34.627332 finitelycomputable_idtrust_falcon_peewee-24.5/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2433 2024-06-01 03:11:34.627332 finitelycomputable_idtrust_falcon_peewee-24.5/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      330 2024-06-01 03:00:08.000000 finitelycomputable_idtrust_falcon_peewee-24.5/README.rst
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:34.623331 finitelycomputable_idtrust_falcon_peewee-24.5/finitelycomputable/
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:34.623331 finitelycomputable_idtrust_falcon_peewee-24.5/finitelycomputable/idtrust_falcon/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       55 2024-06-01 03:00:08.000000 finitelycomputable_idtrust_falcon_peewee-24.5/finitelycomputable/idtrust_falcon/__init__.py
+-rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)      119 2024-06-01 03:00:08.000000 finitelycomputable_idtrust_falcon_peewee-24.5/finitelycomputable/idtrust_falcon/peewee.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:34.623331 finitelycomputable_idtrust_falcon_peewee-24.5/finitelycomputable_idtrust_falcon_peewee.egg-info/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2433 2024-06-01 03:11:34.000000 finitelycomputable_idtrust_falcon_peewee-24.5/finitelycomputable_idtrust_falcon_peewee.egg-info/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      501 2024-06-01 03:11:34.000000 finitelycomputable_idtrust_falcon_peewee-24.5/finitelycomputable_idtrust_falcon_peewee.egg-info/SOURCES.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-06-01 03:11:34.000000 finitelycomputable_idtrust_falcon_peewee-24.5/finitelycomputable_idtrust_falcon_peewee.egg-info/dependency_links.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      103 2024-06-01 03:11:34.000000 finitelycomputable_idtrust_falcon_peewee-24.5/finitelycomputable_idtrust_falcon_peewee.egg-info/entry_points.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      265 2024-06-01 03:11:34.000000 finitelycomputable_idtrust_falcon_peewee-24.5/finitelycomputable_idtrust_falcon_peewee.egg-info/requires.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-06-01 03:11:34.000000 finitelycomputable_idtrust_falcon_peewee-24.5/finitelycomputable_idtrust_falcon_peewee.egg-info/top_level.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1877 2024-06-01 03:11:32.000000 finitelycomputable_idtrust_falcon_peewee-24.5/pyproject.toml
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-06-01 03:11:34.627332 finitelycomputable_idtrust_falcon_peewee-24.5/setup.cfg
```

### Comparing `finitelycomputable_idtrust_falcon_peewee-24.4/PKG-INFO` & `finitelycomputable_idtrust_falcon_peewee-24.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-idtrust-falcon-peewee
-Version: 24.4
+Version: 24.5
 Summary: A Falcon+peewee microsite to explore identifying game-theory strategies
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/identification_of_trust
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
```

### Comparing `finitelycomputable_idtrust_falcon_peewee-24.4/finitelycomputable_idtrust_falcon_peewee.egg-info/PKG-INFO` & `finitelycomputable_idtrust_falcon_peewee-24.5/finitelycomputable_idtrust_falcon_peewee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-idtrust-falcon-peewee
-Version: 24.4
+Version: 24.5
 Summary: A Falcon+peewee microsite to explore identifying game-theory strategies
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/identification_of_trust
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
```

### Comparing `finitelycomputable_idtrust_falcon_peewee-24.4/pyproject.toml` & `finitelycomputable_idtrust_falcon_peewee-24.5/pyproject.toml`

 * *Files 0% similar despite different names*

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
 name = "finitelycomputable-idtrust-falcon-peewee"
 requires-python = ">=3.8"
 description = "A Falcon+peewee microsite to explore identifying game-theory strategies"
 dependencies = [
   "finitelycomputable-idtrust-app-falcon",
   "finitelycomputable-idtrust-db-peewee",
   "falcon~=3.1",
```

