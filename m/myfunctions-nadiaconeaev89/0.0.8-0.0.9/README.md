# Comparing `tmp/myfunctions_nadiaconeaev89-0.0.8.tar.gz` & `tmp/myfunctions_nadiaconeaev89-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/nadiaconeaev89/python-class/evolvecyber/Class5/dist/tmp71gxd4pt/myfunctions_nadiaconeaev89-0.0.8.tar", last modified: Fri May 31 22:10:21 2024, max compression
+gzip compressed data, was "/mnt/nadiaconeaev89/python-class/evolvecyber/Class5/dist/tmpf6h42t6e/myfunctions_nadiaconeaev89-0.0.9.tar", last modified: Fri May 31 22:15:55 2024, max compression
```

## Comparing `myfunctions_nadiaconeaev89-0.0.8.tar` & `myfunctions_nadiaconeaev89-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      651 2024-05-31 22:10:03.000000 myfunctions_nadiaconeaev89-0.0.8/setup.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2398 2024-05-30 01:18:52.000000 myfunctions_nadiaconeaev89-0.0.8/README.md
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      577 2024-05-31 22:07:00.000000 myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89/math.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:48:55.000000 myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89/__init__.py
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/PKG-INFO
-drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89.egg-info/
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       27 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89.egg-info/top_level.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      292 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89.egg-info/SOURCES.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        1 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89.egg-info/dependency_links.txt
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89.egg-info/PKG-INFO
--rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       38 2024-05-31 22:10:21.000000 myfunctions_nadiaconeaev89-0.0.8/setup.cfg
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-31 22:15:55.000000 myfunctions_nadiaconeaev89-0.0.9/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      651 2024-05-31 22:15:43.000000 myfunctions_nadiaconeaev89-0.0.9/setup.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2398 2024-05-30 01:18:52.000000 myfunctions_nadiaconeaev89-0.0.9/README.md
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-31 22:15:55.000000 myfunctions_nadiaconeaev89-0.0.9/myfunctions_nadiaconeaev89/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      723 2024-05-31 22:15:25.000000 myfunctions_nadiaconeaev89-0.0.9/myfunctions_nadiaconeaev89/math.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-30 00:48:55.000000 myfunctions_nadiaconeaev89-0.0.9/myfunctions_nadiaconeaev89/__init__.py
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-31 22:15:55.000000 myfunctions_nadiaconeaev89-0.0.9/PKG-INFO
+drwxrwxr-x   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        0 2024-05-31 22:15:55.000000 myfunctions_nadiaconeaev89-0.0.9/myfunctions_nadiaconeaev89.egg-info/
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       27 2024-05-31 22:15:55.000000 myfunctions_nadiaconeaev89-0.0.9/myfunctions_nadiaconeaev89.egg-info/top_level.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)      292 2024-05-31 22:15:55.000000 myfunctions_nadiaconeaev89-0.0.9/myfunctions_nadiaconeaev89.egg-info/SOURCES.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)        1 2024-05-31 22:15:55.000000 myfunctions_nadiaconeaev89-0.0.9/myfunctions_nadiaconeaev89.egg-info/dependency_links.txt
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)     2858 2024-05-31 22:15:55.000000 myfunctions_nadiaconeaev89-0.0.9/myfunctions_nadiaconeaev89.egg-info/PKG-INFO
+-rw-rw-r--   0 nadiaconeaev89  (1699) nadiaconeaev89  (1700)       38 2024-05-31 22:15:55.000000 myfunctions_nadiaconeaev89-0.0.9/setup.cfg
```

### Comparing `myfunctions_nadiaconeaev89-0.0.8/setup.py` & `myfunctions_nadiaconeaev89-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_nadiaconeaev89',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/nadiaconeaev89/',
     license='MIT',
     author='Nadejda Coneaev',
     author_email='nadejda.savin@gmail.com',
     description='A description of your package',
```

### Comparing `myfunctions_nadiaconeaev89-0.0.8/README.md` & `myfunctions_nadiaconeaev89-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89/math.py` & `myfunctions_nadiaconeaev89-0.0.9/myfunctions_nadiaconeaev89/math.py`

 * *Files 26% similar despite different names*

```diff
@@ -27,8 +27,16 @@
 
 
 def division(NUMBER1,NUMBER2):
     """
     This is how you use this function
     e.g division(10,5)
     """
-    print(NUMBER1 % NUMBER2)
+    print(NUMBER1 % NUMBER2)
+
+
+def substraction(NUMBER1,NUMBER2):
+    """
+    This is how you use this function
+    e.g substraction(7,2)
+    """
+    print(NUMBER1 - NUMBER2)
```

### Comparing `myfunctions_nadiaconeaev89-0.0.8/PKG-INFO` & `myfunctions_nadiaconeaev89-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_nadiaconeaev89
-Version: 0.0.8
+Version: 0.0.9
 Summary: A description of your package
 Home-page: https://github.com/nadiaconeaev89/
 Author: Nadejda Coneaev
 Author-email: nadejda.savin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_nadiaconeaev89-0.0.8/myfunctions_nadiaconeaev89.egg-info/PKG-INFO` & `myfunctions_nadiaconeaev89-0.0.9/myfunctions_nadiaconeaev89.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-nadiaconeaev89
-Version: 0.0.8
+Version: 0.0.9
 Summary: A description of your package
 Home-page: https://github.com/nadiaconeaev89/
 Author: Nadejda Coneaev
 Author-email: nadejda.savin@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

