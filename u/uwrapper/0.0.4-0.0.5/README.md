# Comparing `tmp/uwrapper-0.0.4.tar.gz` & `tmp/uwrapper-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uwrapper-0.0.4.tar", last modified: Sat Jun  1 15:21:25 2024, max compression
+gzip compressed data, was "uwrapper-0.0.5.tar", last modified: Sat Jun  1 15:24:44 2024, max compression
```

## Comparing `uwrapper-0.0.4.tar` & `uwrapper-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 15:21:25.207007 uwrapper-0.0.4/
--rw-rw-rw-   0        0        0      787 2024-06-01 15:21:25.203000 uwrapper-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-06-01 15:21:25.207007 uwrapper-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1039 2024-06-01 15:20:15.000000 uwrapper-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:21:25.070728 uwrapper-0.0.4/uwrapper/
--rw-rw-rw-   0        0        0       45 2024-06-01 15:20:04.000000 uwrapper-0.0.4/uwrapper/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:21:25.167000 uwrapper-0.0.4/uwrapper/config/
--rw-rw-rw-   0        0        0       60 2024-06-01 13:44:37.000000 uwrapper-0.0.4/uwrapper/config/__init__.py
--rw-rw-rw-   0        0        0      557 2024-06-01 11:27:07.000000 uwrapper-0.0.4/uwrapper/config/config.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:21:25.174993 uwrapper-0.0.4/uwrapper/scripts/
--rw-rw-rw-   0        0        0       85 2024-06-01 13:45:05.000000 uwrapper-0.0.4/uwrapper/scripts/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:21:25.186996 uwrapper-0.0.4/uwrapper/scripts/services/
--rw-rw-rw-   0        0        0       20 2024-06-01 13:45:23.000000 uwrapper-0.0.4/uwrapper/scripts/services/__init__.py
--rw-rw-rw-   0        0        0      921 2024-06-01 12:10:08.000000 uwrapper-0.0.4/uwrapper/scripts/services/login.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:21:25.191020 uwrapper-0.0.4/uwrapper/scripts/src/
--rw-rw-rw-   0        0        0        0 2024-06-01 13:45:51.000000 uwrapper-0.0.4/uwrapper/scripts/src/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:21:25.199012 uwrapper-0.0.4/uwrapper.egg-info/
--rw-rw-rw-   0        0        0      787 2024-06-01 15:21:24.000000 uwrapper-0.0.4/uwrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      377 2024-06-01 15:21:24.000000 uwrapper-0.0.4/uwrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:21:24.000000 uwrapper-0.0.4/uwrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-06-01 15:21:24.000000 uwrapper-0.0.4/uwrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-06-01 15:21:24.000000 uwrapper-0.0.4/uwrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 15:24:44.352744 uwrapper-0.0.5/
+-rw-rw-rw-   0        0        0      787 2024-06-01 15:24:44.348746 uwrapper-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:24:44.352744 uwrapper-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1039 2024-06-01 15:24:39.000000 uwrapper-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:24:44.276744 uwrapper-0.0.5/uwrapper/
+-rw-rw-rw-   0        0        0       45 2024-06-01 15:20:04.000000 uwrapper-0.0.5/uwrapper/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:24:44.328744 uwrapper-0.0.5/uwrapper/config/
+-rw-rw-rw-   0        0        0       60 2024-06-01 13:44:37.000000 uwrapper-0.0.5/uwrapper/config/__init__.py
+-rw-rw-rw-   0        0        0      532 2024-06-01 15:23:32.000000 uwrapper-0.0.5/uwrapper/config/config.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:24:44.328744 uwrapper-0.0.5/uwrapper/scripts/
+-rw-rw-rw-   0        0        0       85 2024-06-01 13:45:05.000000 uwrapper-0.0.5/uwrapper/scripts/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:24:44.336746 uwrapper-0.0.5/uwrapper/scripts/services/
+-rw-rw-rw-   0        0        0       20 2024-06-01 13:45:23.000000 uwrapper-0.0.5/uwrapper/scripts/services/__init__.py
+-rw-rw-rw-   0        0        0      921 2024-06-01 12:10:08.000000 uwrapper-0.0.5/uwrapper/scripts/services/login.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:24:44.340745 uwrapper-0.0.5/uwrapper/scripts/src/
+-rw-rw-rw-   0        0        0        0 2024-06-01 13:45:51.000000 uwrapper-0.0.5/uwrapper/scripts/src/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:24:44.344746 uwrapper-0.0.5/uwrapper.egg-info/
+-rw-rw-rw-   0        0        0      787 2024-06-01 15:24:43.000000 uwrapper-0.0.5/uwrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      377 2024-06-01 15:24:44.000000 uwrapper-0.0.5/uwrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:24:43.000000 uwrapper-0.0.5/uwrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-06-01 15:24:43.000000 uwrapper-0.0.5/uwrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-06-01 15:24:44.000000 uwrapper-0.0.5/uwrapper.egg-info/top_level.txt
```

### Comparing `uwrapper-0.0.4/PKG-INFO` & `uwrapper-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uwrapper
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python library for upstox APIs
 Home-page: https://github.com/azachbot/upstox_api_wrapper
 Author: Zachbot
 Author-email: zachbot006@gmail.com
 Keywords: upstox,nse,python,sdk,trading,stock markets,wrapper
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `uwrapper-0.0.4/setup.py` & `uwrapper-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = 'uwrapper',
     packages=setuptools.find_packages(),
-    version = '0.0.4',
+    version = '0.0.5',
     include_package_data=True,
     description = 'Python library for upstox APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",  author = 'Zachbot',
     author_email = 'zachbot006@gmail.com',
     url = 'https://github.com/azachbot/upstox_api_wrapper',
     install_requires=['requests', 'pandas','upstox-python-sdk'],
```

### Comparing `uwrapper-0.0.4/uwrapper/scripts/services/login.py` & `uwrapper-0.0.5/uwrapper/scripts/services/login.py`

 * *Files identical despite different names*

### Comparing `uwrapper-0.0.4/uwrapper.egg-info/PKG-INFO` & `uwrapper-0.0.5/uwrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uwrapper
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python library for upstox APIs
 Home-page: https://github.com/azachbot/upstox_api_wrapper
 Author: Zachbot
 Author-email: zachbot006@gmail.com
 Keywords: upstox,nse,python,sdk,trading,stock markets,wrapper
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

