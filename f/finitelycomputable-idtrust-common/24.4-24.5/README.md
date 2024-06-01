# Comparing `tmp/finitelycomputable_idtrust_common-24.4.tar.gz` & `tmp/finitelycomputable_idtrust_common-24.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finitelycomputable_idtrust_common-24.4.tar", last modified: Tue Apr 30 04:47:12 2024, max compression
+gzip compressed data, was "finitelycomputable_idtrust_common-24.5.tar", last modified: Sat Jun  1 03:11:17 2024, max compression
```

## Comparing `finitelycomputable_idtrust_common-24.4.tar` & `finitelycomputable_idtrust_common-24.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:12.699825 finitelycomputable_idtrust_common-24.4/
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       59 2024-02-15 18:56:45.000000 finitelycomputable_idtrust_common-24.4/MANIFEST.in
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     1849 2024-04-30 04:47:12.699825 finitelycomputable_idtrust_common-24.4/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      313 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_common-24.4/README.rst
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:12.695825 finitelycomputable_idtrust_common-24.4/finitelycomputable/
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:12.695825 finitelycomputable_idtrust_common-24.4/finitelycomputable/idtrust_common/
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        0 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_common-24.4/finitelycomputable/idtrust_common/__init__.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1288 2024-04-14 05:27:48.000000 finitelycomputable_idtrust_common-24.4/finitelycomputable/idtrust_common/helpers_for_tests.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1002 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_common-24.4/finitelycomputable/idtrust_common/logic.py
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1899 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_common-24.4/finitelycomputable/idtrust_common/strategies.py
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:12.699825 finitelycomputable_idtrust_common-24.4/finitelycomputable/idtrust_common/templates/
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      499 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_common-24.4/finitelycomputable/idtrust_common/templates/exchange_form.html
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     2602 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_common-24.4/finitelycomputable/idtrust_common/templates/interaction.html
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1574 2023-09-12 03:23:48.000000 finitelycomputable_idtrust_common-24.4/finitelycomputable/idtrust_common/templates/interaction_begin.html
-drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-04-30 04:47:12.699825 finitelycomputable_idtrust_common-24.4/finitelycomputable_idtrust_common.egg-info/
--rw-r--r--   0 bellerophon (30000) bellerophon (30003)     1849 2024-04-30 04:47:12.000000 finitelycomputable_idtrust_common-24.4/finitelycomputable_idtrust_common.egg-info/PKG-INFO
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1044 2024-04-30 04:47:12.000000 finitelycomputable_idtrust_common-24.4/finitelycomputable_idtrust_common.egg-info/SOURCES.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-04-30 04:47:12.000000 finitelycomputable_idtrust_common-24.4/finitelycomputable_idtrust_common.egg-info/dependency_links.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       52 2024-04-30 04:47:12.000000 finitelycomputable_idtrust_common-24.4/finitelycomputable_idtrust_common.egg-info/requires.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-04-30 04:47:12.000000 finitelycomputable_idtrust_common-24.4/finitelycomputable_idtrust_common.egg-info/top_level.txt
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1449 2024-04-28 21:51:18.000000 finitelycomputable_idtrust_common-24.4/pyproject.toml
--rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-04-30 04:47:12.699825 finitelycomputable_idtrust_common-24.4/setup.cfg
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:17.347224 finitelycomputable_idtrust_common-24.5/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       59 2024-06-01 03:00:08.000000 finitelycomputable_idtrust_common-24.5/MANIFEST.in
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     1849 2024-06-01 03:11:17.343224 finitelycomputable_idtrust_common-24.5/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      313 2024-06-01 03:00:08.000000 finitelycomputable_idtrust_common-24.5/README.rst
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:17.343224 finitelycomputable_idtrust_common-24.5/finitelycomputable/
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:17.343224 finitelycomputable_idtrust_common-24.5/finitelycomputable/idtrust_common/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:00:08.000000 finitelycomputable_idtrust_common-24.5/finitelycomputable/idtrust_common/__init__.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1288 2024-06-01 03:00:08.000000 finitelycomputable_idtrust_common-24.5/finitelycomputable/idtrust_common/helpers_for_tests.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1002 2024-06-01 03:00:08.000000 finitelycomputable_idtrust_common-24.5/finitelycomputable/idtrust_common/logic.py
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1899 2024-06-01 03:00:08.000000 finitelycomputable_idtrust_common-24.5/finitelycomputable/idtrust_common/strategies.py
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:17.343224 finitelycomputable_idtrust_common-24.5/finitelycomputable/idtrust_common/templates/
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      499 2024-06-01 03:00:08.000000 finitelycomputable_idtrust_common-24.5/finitelycomputable/idtrust_common/templates/exchange_form.html
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     2602 2024-06-01 03:00:08.000000 finitelycomputable_idtrust_common-24.5/finitelycomputable/idtrust_common/templates/interaction.html
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1574 2024-06-01 03:00:08.000000 finitelycomputable_idtrust_common-24.5/finitelycomputable/idtrust_common/templates/interaction_begin.html
+drwxrwxr-x   0 bellerophon (30000) bellerophon (30003)        0 2024-06-01 03:11:17.343224 finitelycomputable_idtrust_common-24.5/finitelycomputable_idtrust_common.egg-info/
+-rw-r--r--   0 bellerophon (30000) bellerophon (30003)     1849 2024-06-01 03:11:17.000000 finitelycomputable_idtrust_common-24.5/finitelycomputable_idtrust_common.egg-info/PKG-INFO
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)      704 2024-06-01 03:11:17.000000 finitelycomputable_idtrust_common-24.5/finitelycomputable_idtrust_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)        1 2024-06-01 03:11:17.000000 finitelycomputable_idtrust_common-24.5/finitelycomputable_idtrust_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       52 2024-06-01 03:11:17.000000 finitelycomputable_idtrust_common-24.5/finitelycomputable_idtrust_common.egg-info/requires.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       19 2024-06-01 03:11:17.000000 finitelycomputable_idtrust_common-24.5/finitelycomputable_idtrust_common.egg-info/top_level.txt
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)     1449 2024-06-01 03:11:15.000000 finitelycomputable_idtrust_common-24.5/pyproject.toml
+-rw-rw-r--   0 bellerophon (30000) bellerophon (30003)       38 2024-06-01 03:11:17.347224 finitelycomputable_idtrust_common-24.5/setup.cfg
```

### Comparing `finitelycomputable_idtrust_common-24.4/PKG-INFO` & `finitelycomputable_idtrust_common-24.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-idtrust-common
-Version: 24.4
+Version: 24.5
 Summary: Shared files needed for the Identification of Trust microsite
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/identification_of_trust
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
```

### Comparing `finitelycomputable_idtrust_common-24.4/finitelycomputable/idtrust_common/helpers_for_tests.py` & `finitelycomputable_idtrust_common-24.5/finitelycomputable/idtrust_common/helpers_for_tests.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable_idtrust_common-24.4/finitelycomputable/idtrust_common/logic.py` & `finitelycomputable_idtrust_common-24.5/finitelycomputable/idtrust_common/logic.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable_idtrust_common-24.4/finitelycomputable/idtrust_common/strategies.py` & `finitelycomputable_idtrust_common-24.5/finitelycomputable/idtrust_common/strategies.py`

 * *Files identical despite different names*

### Comparing `finitelycomputable_idtrust_common-24.4/finitelycomputable/idtrust_common/templates/interaction.html` & `finitelycomputable_idtrust_common-24.5/finitelycomputable/idtrust_common/templates/interaction.html`

 * *Files identical despite different names*

### Comparing `finitelycomputable_idtrust_common-24.4/finitelycomputable/idtrust_common/templates/interaction_begin.html` & `finitelycomputable_idtrust_common-24.5/finitelycomputable/idtrust_common/templates/interaction_begin.html`

 * *Files identical despite different names*

### Comparing `finitelycomputable_idtrust_common-24.4/finitelycomputable_idtrust_common.egg-info/PKG-INFO` & `finitelycomputable_idtrust_common-24.5/finitelycomputable_idtrust_common.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finitelycomputable-idtrust-common
-Version: 24.4
+Version: 24.5
 Summary: Shared files needed for the Identification of Trust microsite
 Author-email: Samuel Newbold <sam@rwsh.org>
 License: AGPL-3.0-only
 Project-URL: Homepage, https://www.finitelycomputable.net/identification_of_trust
 Project-URL: Documentation, https://github.com/thrasymache/microsites
 Project-URL: Source, https://github.com/thrasymache/microsites
 Project-URL: Gitlab, https://gitlab.com/thrasymache/microsites
```

### Comparing `finitelycomputable_idtrust_common-24.4/finitelycomputable_idtrust_common.egg-info/SOURCES.txt` & `finitelycomputable_idtrust_common-24.5/finitelycomputable_idtrust_common.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,10 @@
 MANIFEST.in
 README.rst
 pyproject.toml
-./finitelycomputable/idtrust_common/__init__.py
-./finitelycomputable/idtrust_common/logic.py
-./finitelycomputable/idtrust_common/strategies.py
-./finitelycomputable/idtrust_common/templates/exchange_form.html
-./finitelycomputable/idtrust_common/templates/interaction.html
-./finitelycomputable/idtrust_common/templates/interaction_begin.html
 finitelycomputable/idtrust_common/__init__.py
 finitelycomputable/idtrust_common/helpers_for_tests.py
 finitelycomputable/idtrust_common/logic.py
 finitelycomputable/idtrust_common/strategies.py
 finitelycomputable/idtrust_common/templates/exchange_form.html
 finitelycomputable/idtrust_common/templates/interaction.html
 finitelycomputable/idtrust_common/templates/interaction_begin.html
```

### Comparing `finitelycomputable_idtrust_common-24.4/pyproject.toml` & `finitelycomputable_idtrust_common-24.5/pyproject.toml`

 * *Files 8% similar despite different names*

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
 name = "finitelycomputable-idtrust-common"
 requires-python = ">=3.8"
 description = "Shared files needed for the Identification of Trust microsite"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Environment :: Web Environment",
   "Intended Audience :: Developers",
```

