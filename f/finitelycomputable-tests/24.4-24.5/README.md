# Comparing `tmp/finitelycomputable_tests-24.4.tar.gz` & `tmp/finitelycomputable_tests-24.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable_tests-24.4.tar", last modified: Tue Apr 30 04:45:05 2024, max compression
+gzip compressed data, was "finitelycomputable_tests-24.5.tar", last modified: Sat Jun  1 03:09:19 2024, max compression
```

## Comparing `finitelycomputable_tests-24.4.tar` & `finitelycomputable_tests-24.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:45:05.595240 finitelycomputable_tests-24.4/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2118 2024-04-30 04:45:05.595240 finitelycomputable_tests-24.4/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      585 2024-04-25 05:27:23.000000 finitelycomputable_tests-24.4/README.rst
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:45:05.591240 finitelycomputable_tests-24.4/finitelycomputable/
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:45:05.591240 finitelycomputable_tests-24.4/finitelycomputable/tests/
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:45:05.591240 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        0 2024-04-19 05:07:58.000000 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/__init__.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       97 2024-04-30 03:04:04.000000 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/test_cherrypy_mount.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       89 2024-03-29 09:17:45.000000 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/test_django_apps.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       97 2024-04-16 06:37:18.000000 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/test_falcon_addroute.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       99 2024-04-30 03:31:26.000000 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/test_flask_blueprints.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       99 2024-04-30 03:31:51.000000 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/test_flask_dispatcher.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      102 2024-04-30 03:32:15.000000 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/test_helloworld_cherrypy.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       95 2024-03-29 09:18:53.000000 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/test_helloworld_django.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      100 2024-04-30 03:32:42.000000 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/test_helloworld_falcon.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       99 2024-04-30 03:32:55.000000 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/test_helloworld_flask.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      102 2024-04-30 03:33:18.000000 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/test_helloworld_morepath.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       99 2024-04-30 03:33:36.000000 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/test_helloworld_quart.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       92 2024-03-29 09:19:06.000000 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/test_idtrust_django.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       97 2024-04-30 03:34:48.000000 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/test_idtrust_falcon.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       96 2024-04-30 03:35:01.000000 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/test_idtrust_flask.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       97 2024-04-30 03:35:17.000000 finitelycomputable_tests-24.4/finitelycomputable/tests/tests_with_import_guards/test_morepath_mount.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:45:05.591240 finitelycomputable_tests-24.4/finitelycomputable_tests.egg-info/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2118 2024-04-30 04:45:05.000000 finitelycomputable_tests-24.4/finitelycomputable_tests.egg-info/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1493 2024-04-30 04:45:05.000000 finitelycomputable_tests-24.4/finitelycomputable_tests.egg-info/SOURCES.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-30 04:45:05.000000 finitelycomputable_tests-24.4/finitelycomputable_tests.egg-info/dependency_links.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       57 2024-04-30 04:45:05.000000 finitelycomputable_tests-24.4/finitelycomputable_tests.egg-info/entry_points.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       52 2024-04-30 04:45:05.000000 finitelycomputable_tests-24.4/finitelycomputable_tests.egg-info/requires.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-30 04:45:05.000000 finitelycomputable_tests-24.4/finitelycomputable_tests.egg-info/top_level.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1506 2024-04-28 21:51:18.000000 finitelycomputable_tests-24.4/pyproject.toml
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-30 04:45:05.595240 finitelycomputable_tests-24.4/setup.cfg
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:09:19.518486 finitelycomputable_tests-24.5/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2118 2024-06-01 03:09:19.518486 finitelycomputable_tests-24.5/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      585 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/README.rst
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:09:19.514486 finitelycomputable_tests-24.5/finitelycomputable/
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:09:19.514486 finitelycomputable_tests-24.5/finitelycomputable/tests/
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:09:19.518486 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/__init__.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       97 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/test_cherrypy_mount.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       89 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/test_django_apps.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       97 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/test_falcon_addroute.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       99 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/test_flask_blueprints.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       99 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/test_flask_dispatcher.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      102 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/test_helloworld_cherrypy.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       95 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/test_helloworld_django.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      100 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/test_helloworld_falcon.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       99 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/test_helloworld_flask.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      102 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/test_helloworld_morepath.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       99 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/test_helloworld_quart.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       92 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/test_idtrust_django.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       97 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/test_idtrust_falcon.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       96 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/test_idtrust_flask.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       97 2024-06-01 03:00:08.000000 finitelycomputable_tests-24.5/finitelycomputable/tests/tests_with_import_guards/test_morepath_mount.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:09:19.518486 finitelycomputable_tests-24.5/finitelycomputable_tests.egg-info/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     2118 2024-06-01 03:09:19.000000 finitelycomputable_tests-24.5/finitelycomputable_tests.egg-info/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1493 2024-06-01 03:09:19.000000 finitelycomputable_tests-24.5/finitelycomputable_tests.egg-info/SOURCES.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-06-01 03:09:19.000000 finitelycomputable_tests-24.5/finitelycomputable_tests.egg-info/dependency_links.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       57 2024-06-01 03:09:19.000000 finitelycomputable_tests-24.5/finitelycomputable_tests.egg-info/entry_points.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       52 2024-06-01 03:09:19.000000 finitelycomputable_tests-24.5/finitelycomputable_tests.egg-info/requires.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-06-01 03:09:19.000000 finitelycomputable_tests-24.5/finitelycomputable_tests.egg-info/top_level.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1506 2024-06-01 03:09:17.000000 finitelycomputable_tests-24.5/pyproject.toml
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-06-01 03:09:19.518486 finitelycomputable_tests-24.5/setup.cfg
```

### Comparing `finitelycomputable_tests-24.4/PKG-INFO` & `finitelycomputable_tests-24.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-tests
-Version: 24.4
+Version: 24.5
 Summary: Imports for all the test modules for the apps in the microsites of finitelycomputable.net.
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
```

### Comparing `finitelycomputable_tests-24.4/README.rst` & `finitelycomputable_tests-24.5/README.rst`

 * *Files identical despite different names*

### Comparing `finitelycomputable_tests-24.4/finitelycomputable_tests.egg-info/PKG-INFO` & `finitelycomputable_tests-24.5/finitelycomputable_tests.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-tests
-Version: 24.4
+Version: 24.5
 Summary: Imports for all the test modules for the apps in the microsites of finitelycomputable.net.
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
```

### Comparing `finitelycomputable_tests-24.4/finitelycomputable_tests.egg-info/SOURCES.txt` & `finitelycomputable_tests-24.5/finitelycomputable_tests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `finitelycomputable_tests-24.4/pyproject.toml` & `finitelycomputable_tests-24.5/pyproject.toml`

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
 name = "finitelycomputable-tests"
 requires-python = ">=3.8"
 description = "Imports for all the test modules for the apps in the microsites of finitelycomputable.net."
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
```

