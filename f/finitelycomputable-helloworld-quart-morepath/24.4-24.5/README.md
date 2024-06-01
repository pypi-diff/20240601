# Comparing `tmp/finitelycomputable_helloworld_quart_morepath-24.4.tar.gz` & `tmp/finitelycomputable_helloworld_quart_morepath-24.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable_helloworld_quart_morepath-24.4.tar", last modified: Tue Apr 30 04:47:08 2024, max compression
+gzip compressed data, was "finitelycomputable_helloworld_quart_morepath-24.5.tar", last modified: Sat Jun  1 03:11:13 2024, max compression
```

## Comparing `finitelycomputable_helloworld_quart_morepath-24.4.tar` & `finitelycomputable_helloworld_quart_morepath-24.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:08.015804 finitelycomputable_helloworld_quart_morepath-24.4/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     1864 2024-04-30 04:47:08.015804 finitelycomputable_helloworld_quart_morepath-24.4/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      260 2024-01-21 18:31:00.000000 finitelycomputable_helloworld_quart_morepath-24.4/README.rst
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:08.015804 finitelycomputable_helloworld_quart_morepath-24.4/finitelycomputable/
--rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)      997 2024-03-02 07:07:32.000000 finitelycomputable_helloworld_quart_morepath-24.4/finitelycomputable/helloworld_quart.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:08.015804 finitelycomputable_helloworld_quart_morepath-24.4/finitelycomputable/tests/
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      783 2024-04-30 03:36:52.000000 finitelycomputable_helloworld_quart_morepath-24.4/finitelycomputable/tests/test_helloworld_quart.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:08.015804 finitelycomputable_helloworld_quart_morepath-24.4/finitelycomputable_helloworld_quart_morepath.egg-info/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     1864 2024-04-30 04:47:08.000000 finitelycomputable_helloworld_quart_morepath-24.4/finitelycomputable_helloworld_quart_morepath.egg-info/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      565 2024-04-30 04:47:08.000000 finitelycomputable_helloworld_quart_morepath-24.4/finitelycomputable_helloworld_quart_morepath.egg-info/SOURCES.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-30 04:47:08.000000 finitelycomputable_helloworld_quart_morepath-24.4/finitelycomputable_helloworld_quart_morepath.egg-info/dependency_links.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       96 2024-04-30 04:47:08.000000 finitelycomputable_helloworld_quart_morepath-24.4/finitelycomputable_helloworld_quart_morepath.egg-info/entry_points.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       79 2024-04-30 04:47:08.000000 finitelycomputable_helloworld_quart_morepath-24.4/finitelycomputable_helloworld_quart_morepath.egg-info/requires.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-30 04:47:08.000000 finitelycomputable_helloworld_quart_morepath-24.4/finitelycomputable_helloworld_quart_morepath.egg-info/top_level.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1597 2024-04-28 21:51:18.000000 finitelycomputable_helloworld_quart_morepath-24.4/pyproject.toml
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-30 04:47:08.015804 finitelycomputable_helloworld_quart_morepath-24.4/setup.cfg
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:13.031197 finitelycomputable_helloworld_quart_morepath-24.5/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     1864 2024-06-01 03:11:13.027197 finitelycomputable_helloworld_quart_morepath-24.5/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      260 2024-06-01 03:00:08.000000 finitelycomputable_helloworld_quart_morepath-24.5/README.rst
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:13.027197 finitelycomputable_helloworld_quart_morepath-24.5/finitelycomputable/
+-rwxrwxr-x   0 bellerophon (30000) bellerophon (30003)      997 2024-06-01 03:00:08.000000 finitelycomputable_helloworld_quart_morepath-24.5/finitelycomputable/helloworld_quart.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:13.027197 finitelycomputable_helloworld_quart_morepath-24.5/finitelycomputable/tests/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      783 2024-06-01 03:00:08.000000 finitelycomputable_helloworld_quart_morepath-24.5/finitelycomputable/tests/test_helloworld_quart.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:13.027197 finitelycomputable_helloworld_quart_morepath-24.5/finitelycomputable_helloworld_quart_morepath.egg-info/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     1864 2024-06-01 03:11:13.000000 finitelycomputable_helloworld_quart_morepath-24.5/finitelycomputable_helloworld_quart_morepath.egg-info/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      524 2024-06-01 03:11:13.000000 finitelycomputable_helloworld_quart_morepath-24.5/finitelycomputable_helloworld_quart_morepath.egg-info/SOURCES.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-06-01 03:11:13.000000 finitelycomputable_helloworld_quart_morepath-24.5/finitelycomputable_helloworld_quart_morepath.egg-info/dependency_links.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       96 2024-06-01 03:11:13.000000 finitelycomputable_helloworld_quart_morepath-24.5/finitelycomputable_helloworld_quart_morepath.egg-info/entry_points.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       79 2024-06-01 03:11:13.000000 finitelycomputable_helloworld_quart_morepath-24.5/finitelycomputable_helloworld_quart_morepath.egg-info/requires.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-06-01 03:11:13.000000 finitelycomputable_helloworld_quart_morepath-24.5/finitelycomputable_helloworld_quart_morepath.egg-info/top_level.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1597 2024-06-01 03:11:11.000000 finitelycomputable_helloworld_quart_morepath-24.5/pyproject.toml
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-06-01 03:11:13.031197 finitelycomputable_helloworld_quart_morepath-24.5/setup.cfg
```

### Comparing `finitelycomputable_helloworld_quart_morepath-24.4/PKG-INFO` & `finitelycomputable_helloworld_quart_morepath-24.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-helloworld-quart-morepath
-Version: 24.4
+Version: 24.5
 Summary: hello_world in Quart from an implementation in Morepath
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/hello_world
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
```

### Comparing `finitelycomputable_helloworld_quart_morepath-24.4/finitelycomputable/helloworld_quart.py` & `finitelycomputable_helloworld_quart_morepath-24.5/finitelycomputable/helloworld_quart.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable_helloworld_quart_morepath-24.4/finitelycomputable/tests/test_helloworld_quart.py` & `finitelycomputable_helloworld_quart_morepath-24.5/finitelycomputable/tests/test_helloworld_quart.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable_helloworld_quart_morepath-24.4/finitelycomputable_helloworld_quart_morepath.egg-info/PKG-INFO` & `finitelycomputable_helloworld_quart_morepath-24.5/finitelycomputable_helloworld_quart_morepath.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-helloworld-quart-morepath
-Version: 24.4
+Version: 24.5
 Summary: hello_world in Quart from an implementation in Morepath
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/hello_world
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
```

### Comparing `finitelycomputable_helloworld_quart_morepath-24.4/finitelycomputable_helloworld_quart_morepath.egg-info/SOURCES.txt` & `finitelycomputable_helloworld_quart_morepath-24.5/finitelycomputable_helloworld_quart_morepath.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 README.rst
 pyproject.toml
-./finitelycomputable/helloworld_quart.py
 finitelycomputable/helloworld_quart.py
 finitelycomputable/tests/test_helloworld_quart.py
 finitelycomputable_helloworld_quart_morepath.egg-info/PKG-INFO
 finitelycomputable_helloworld_quart_morepath.egg-info/SOURCES.txt
 finitelycomputable_helloworld_quart_morepath.egg-info/dependency_links.txt
 finitelycomputable_helloworld_quart_morepath.egg-info/entry_points.txt
 finitelycomputable_helloworld_quart_morepath.egg-info/requires.txt
```

### Comparing `finitelycomputable_helloworld_quart_morepath-24.4/pyproject.toml` & `finitelycomputable_helloworld_quart_morepath-24.5/pyproject.toml`

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
 name = "finitelycomputable-helloworld-quart-morepath"
 requires-python = ">=3.8"
 description = "hello_world in Quart from an implementation in Morepath"
 dependencies = [
   "Quart~=0.19",
 ]
 classifiers = [
```

