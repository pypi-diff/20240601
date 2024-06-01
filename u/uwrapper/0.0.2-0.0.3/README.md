# Comparing `tmp/uwrapper-0.0.2.tar.gz` & `tmp/uwrapper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uwrapper-0.0.2.tar", last modified: Sat Jun  1 15:06:50 2024, max compression
+gzip compressed data, was "uwrapper-0.0.3.tar", last modified: Sat Jun  1 15:09:53 2024, max compression
```

## Comparing `uwrapper-0.0.2.tar` & `uwrapper-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 15:06:50.736842 uwrapper-0.0.2/
--rw-rw-rw-   0        0        0      787 2024-06-01 15:06:50.732835 uwrapper-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-06-01 15:06:50.736842 uwrapper-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1039 2024-06-01 15:06:33.000000 uwrapper-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:06:50.732835 uwrapper-0.0.2/uwrapper.egg-info/
--rw-rw-rw-   0        0        0      787 2024-06-01 15:06:50.000000 uwrapper-0.0.2/uwrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      167 2024-06-01 15:06:50.000000 uwrapper-0.0.2/uwrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:06:50.000000 uwrapper-0.0.2/uwrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2024-06-01 15:06:50.000000 uwrapper-0.0.2/uwrapper.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:06:50.000000 uwrapper-0.0.2/uwrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 15:09:53.569793 uwrapper-0.0.3/
+-rw-rw-rw-   0        0        0      787 2024-06-01 15:09:53.565730 uwrapper-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:09:53.569793 uwrapper-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1039 2024-06-01 15:09:45.000000 uwrapper-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:09:53.561732 uwrapper-0.0.3/uwrapper.egg-info/
+-rw-rw-rw-   0        0        0      787 2024-06-01 15:09:53.000000 uwrapper-0.0.3/uwrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      167 2024-06-01 15:09:53.000000 uwrapper-0.0.3/uwrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:09:53.000000 uwrapper-0.0.3/uwrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2024-06-01 15:09:53.000000 uwrapper-0.0.3/uwrapper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:09:53.000000 uwrapper-0.0.3/uwrapper.egg-info/top_level.txt
```

### Comparing `uwrapper-0.0.2/PKG-INFO` & `uwrapper-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uwrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library for upstox APIs
 Home-page: https://github.com/azachbot/upstox_api_wrapper
 Author: Zachbot
 Author-email: zachbot006@gmail.com
 Keywords: upstox,nse,python,sdk,trading,stock markets,wrapper
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `uwrapper-0.0.2/setup.py` & `uwrapper-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = 'uwrapper',
     packages=setuptools.find_packages(),
-    version = '0.0.2',
+    version = '0.0.3',
     include_package_data=True,
     description = 'Python library for upstox APIs',
     long_description=long_description,
     long_description_content_type="text/markdown",  author = 'Zachbot',
     author_email = 'zachbot006@gmail.com',
     url = 'https://github.com/azachbot/upstox_api_wrapper',
     install_requires=['requests', 'pandas','upstox-python-sdk'],
```

### Comparing `uwrapper-0.0.2/uwrapper.egg-info/PKG-INFO` & `uwrapper-0.0.3/uwrapper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uwrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library for upstox APIs
 Home-page: https://github.com/azachbot/upstox_api_wrapper
 Author: Zachbot
 Author-email: zachbot006@gmail.com
 Keywords: upstox,nse,python,sdk,trading,stock markets,wrapper
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

