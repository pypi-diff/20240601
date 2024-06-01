# Comparing `tmp/HakObserverLinuxpy-0.6.4.tar.gz` & `tmp/HakObserverLinuxpy-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HakObserverLinuxpy-0.6.4.tar", last modified: Wed May 29 08:52:47 2024, max compression
+gzip compressed data, was "HakObserverLinuxpy-0.6.5.tar", last modified: Sat Jun  1 07:27:41 2024, max compression
```

## Comparing `HakObserverLinuxpy-0.6.4.tar` & `HakObserverLinuxpy-0.6.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-29 08:52:47.143000 HakObserverLinuxpy-0.6.4/
-drwxrwxrwx   0        0        0        0 2024-05-29 08:52:47.111000 HakObserverLinuxpy-0.6.4/HakObserverLinuxpy.egg-info/
--rw-rw-rw-   0        0        0      743 2024-05-29 08:52:46.000000 HakObserverLinuxpy-0.6.4/HakObserverLinuxpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2024-05-29 08:52:46.000000 HakObserverLinuxpy-0.6.4/HakObserverLinuxpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-29 08:52:46.000000 HakObserverLinuxpy-0.6.4/HakObserverLinuxpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-05-29 08:52:46.000000 HakObserverLinuxpy-0.6.4/HakObserverLinuxpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-05-29 08:52:46.000000 HakObserverLinuxpy-0.6.4/HakObserverLinuxpy.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-29 08:52:47.131000 HakObserverLinuxpy-0.6.4/HakObserverpy/
--rw-rw-rw-   0        0        0     4276 2024-05-29 08:44:02.000000 HakObserverLinuxpy-0.6.4/HakObserverpy/HakObserverLinuxpy.py
--rw-rw-rw-   0        0        0      352 2024-05-29 08:43:41.000000 HakObserverLinuxpy-0.6.4/HakObserverpy/__init__.py
--rw-rw-rw-   0        0        0      743 2024-05-29 08:52:47.137000 HakObserverLinuxpy-0.6.4/PKG-INFO
--rw-rw-rw-   0        0        0      303 2024-05-29 08:41:59.000000 HakObserverLinuxpy-0.6.4/README.md
--rw-rw-rw-   0        0        0       42 2024-05-29 08:52:47.142000 HakObserverLinuxpy-0.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1059 2024-05-29 08:40:41.000000 HakObserverLinuxpy-0.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:27:41.327000 HakObserverLinuxpy-0.6.5/
+drwxrwxrwx   0        0        0        0 2024-06-01 07:27:41.294000 HakObserverLinuxpy-0.6.5/HakObserverLinuxpy.egg-info/
+-rw-rw-rw-   0        0        0      743 2024-06-01 07:27:41.000000 HakObserverLinuxpy-0.6.5/HakObserverLinuxpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      289 2024-06-01 07:27:41.000000 HakObserverLinuxpy-0.6.5/HakObserverLinuxpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 07:27:41.000000 HakObserverLinuxpy-0.6.5/HakObserverLinuxpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-06-01 07:27:41.000000 HakObserverLinuxpy-0.6.5/HakObserverLinuxpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-06-01 07:27:41.000000 HakObserverLinuxpy-0.6.5/HakObserverLinuxpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 07:27:41.315000 HakObserverLinuxpy-0.6.5/HakObserverpy/
+-rw-rw-rw-   0        0        0     4276 2024-05-29 08:44:02.000000 HakObserverLinuxpy-0.6.5/HakObserverpy/HakObserverLinuxpy.py
+-rw-rw-rw-   0        0        0      309 2024-06-01 07:26:46.000000 HakObserverLinuxpy-0.6.5/HakObserverpy/__init__.py
+-rw-rw-rw-   0        0        0      743 2024-06-01 07:27:41.322000 HakObserverLinuxpy-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0      303 2024-05-29 08:41:59.000000 HakObserverLinuxpy-0.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 07:27:41.326000 HakObserverLinuxpy-0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1059 2024-06-01 07:24:32.000000 HakObserverLinuxpy-0.6.5/setup.py
```

### Comparing `HakObserverLinuxpy-0.6.4/HakObserverLinuxpy.egg-info/PKG-INFO` & `HakObserverLinuxpy-0.6.5/HakObserverLinuxpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HakObserverLinuxpy
-Version: 0.6.4
+Version: 0.6.5
 Summary: A package connect endpoints to the Hakware Application for Linux
 Home-page: UNKNOWN
 Author: Jacob O'Brien
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `HakObserverLinuxpy-0.6.4/HakObserverpy/HakObserverLinuxpy.py` & `HakObserverLinuxpy-0.6.5/HakObserverpy/HakObserverLinuxpy.py`

 * *Files identical despite different names*

### Comparing `HakObserverLinuxpy-0.6.4/PKG-INFO` & `HakObserverLinuxpy-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HakObserverLinuxpy
-Version: 0.6.4
+Version: 0.6.5
 Summary: A package connect endpoints to the Hakware Application for Linux
 Home-page: UNKNOWN
 Author: Jacob O'Brien
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `HakObserverLinuxpy-0.6.4/setup.py` & `HakObserverLinuxpy-0.6.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import platform
 from setuptools import setup, find_packages
 
 setup(
     name='HakObserverLinuxpy',  # Your package name
-    version='0.6.4',  # Start with a version number
+    version='0.6.5',  # Start with a version number
     description='A package connect endpoints to the Hakware Application for Linux',  # Short description
     long_description=open('README.md').read(),  # Long description from README
     long_description_content_type='text/markdown',
     author='Jacob O\'Brien',  # Your name
     # author_email='your.email@example.com',  # Your email
     # url='https://github.com/your-username/XGRCPy',  # Your package's URL (if applicable)
     packages=find_packages(),  # Find all sub-packages
```

