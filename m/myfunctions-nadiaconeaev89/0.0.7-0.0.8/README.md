# Comparing `tmp/myfunctions_nadiaconeaev89-0.0.7.tar.gz` & `tmp/myfunctions_nadiaconeaev89-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/nadiaconeaev89/python-class/evolvecyber/Class5/dist/tmpm1ym64me/myfunctions_nadiaconeaev89-0.0.7.tar", last modified: Thu May 30 01:36:17 2024, max compression
+gzip compressed data, was "/mnt/nadiaconeaev89/python-class/evolvecyber/Class5/dist/tmp71gxd4pt/myfunctions_nadiaconeaev89-0.0.8.tar", last modified: Fri May 31 22:10:21 2024, max compression
```

## Comparing `myfunctions_nadiaconeaev89-0.0.7.tar` & `myfunctions_nadiaconeaev89-0.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:36:17.000000 myfunctions_nadiaconeaev89-0.0.7/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      651 2024-05-30 01:36:06.000000 myfunctions_nadiaconeaev89-0.0.7/setup.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2398 2024-05-30 01:18:52.000000 myfunctions_nadiaconeaev89-0.0.7/README.md
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:36:17.000000 myfunctions_nadiaconeaev89-0.0.7/myfunctions_nadiaconeaev89/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      438 2024-05-30 01:31:04.000000 myfunctions_nadiaconeaev89-0.0.7/myfunctions_nadiaconeaev89/math.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:48:55.000000 myfunctions_nadiaconeaev89-0.0.7/myfunctions_nadiaconeaev89/__init__.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-30 01:36:17.000000 myfunctions_nadiaconeaev89-0.0.7/PKG-INFO
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 01:36:17.000000 myfunctions_nadiaconeaev89-0.0.7/myfunctions_nadiaconeaev89.egg-info/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       27 2024-05-30 01:36:17.000000 myfunctions_nadiaconeaev89-0.0.7/myfunctions_nadiaconeaev89.egg-info/top_level.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      292 2024-05-30 01:36:17.000000 myfunctions_nadiaconeaev89-0.0.7/myfunctions_nadiaconeaev89.egg-info/SOURCES.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        1 2024-05-30 01:36:17.000000 myfunctions_nadiaconeaev89-0.0.7/myfunctions_nadiaconeaev89.egg-info/dependency_links.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-30 01:36:17.000000 myfunctions_nadiaconeaev89-0.0.7/myfunctions_nadiaconeaev89.egg-info/PKG-INFO
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       38 2024-05-30 01:36:17.000000 myfunctions_nadiaconeaev89-0.0.7/setup.cfg
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      651 2024-05-31 22:10:03.000000 myfunctions_nadiaconeaev89-0.0.8/setup.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2398 2024-05-30 01:18:52.000000 myfunctions_nadiaconeaev89-0.0.8/README.md
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      577 2024-05-31 22:07:00.000000 myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89/math.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:48:55.000000 myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89/__init__.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/PKG-INFO
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89.egg-info/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       27 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89.egg-info/top_level.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      292 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89.egg-info/SOURCES.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        1 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89.egg-info/dependency_links.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89.egg-info/PKG-INFO
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       38 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/setup.cfg
```

### Comparing `myfunctions_nadiaconeaev89-0.0.7/setup.py` & `myfunctions_nadiaconeaev89-0.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_nadiaconeaev89',
-    version='0.0.7',
+    version='0.0.8',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/nadiaconeaev89/',
     license='MIT',
     author='Nadejda Coneaev',
     author_email='nadejda.savin@gmail.com',
     description='A description of your package',
```

### Comparing `myfunctions_nadiaconeaev89-0.0.7/README.md` & `myfunctions_nadiaconeaev89-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_nadiaconeaev89-0.0.7/PKG-INFO` & `myfunctions_nadiaconeaev89-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_nadiaconeaev89
-Version: 0.0.7
+Version: 0.0.8
 Summary: A description of your package
 Home-page: https://github.com/nadiaconeaev89/
 Author: Nadejda Coneaev
 Author-email: nadejda.savin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_nadiaconeaev89-0.0.7/myfunctions_nadiaconeaev89.egg-info/PKG-INFO` & `myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-nadiaconeaev89
-Version: 0.0.7
+Version: 0.0.8
 Summary: A description of your package
 Home-page: https://github.com/nadiaconeaev89/
 Author: Nadejda Coneaev
 Author-email: nadejda.savin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

