# Comparing `tmp/myfunctions_khikmatillo1-0.0.8.tar.gz` & `tmp/myfunctions_khikmatillo1-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/khikmatillo1/python-class/evolvecyber/class5/dist/tmp2wdqqwms/myfunctions_khikmatillo1-0.0.8.tar", last modified: Fri May 31 23:40:30 2024, max compression
+gzip compressed data, was "/mnt/khikmatillo1/python-class/evolvecyber/class5/dist/tmpa_fek8vn/myfunctions_khikmatillo1-0.0.9.tar", last modified: Fri May 31 23:44:30 2024, max compression
```

## Comparing `myfunctions_khikmatillo1-0.0.8.tar` & `myfunctions_khikmatillo1-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 23:40:30.000000 myfunctions_khikmatillo1-0.0.8/
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      653 2024-05-31 23:40:20.000000 myfunctions_khikmatillo1-0.0.8/setup.py
-drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 23:40:30.000000 myfunctions_khikmatillo1-0.0.8/myfunctions_khikmatillo1/
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      439 2024-05-31 23:37:07.000000 myfunctions_khikmatillo1-0.0.8/myfunctions_khikmatillo1/math.py
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 22:26:26.000000 myfunctions_khikmatillo1-0.0.8/myfunctions_khikmatillo1/__init__.py
-drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 23:40:30.000000 myfunctions_khikmatillo1-0.0.8/myfunctions_khikmatillo1.egg-info/
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)       25 2024-05-31 23:40:30.000000 myfunctions_khikmatillo1-0.0.8/myfunctions_khikmatillo1.egg-info/top_level.txt
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      280 2024-05-31 23:40:30.000000 myfunctions_khikmatillo1-0.0.8/myfunctions_khikmatillo1.egg-info/SOURCES.txt
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)        1 2024-05-31 23:40:30.000000 myfunctions_khikmatillo1-0.0.8/myfunctions_khikmatillo1.egg-info/dependency_links.txt
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)     2858 2024-05-31 23:40:30.000000 myfunctions_khikmatillo1-0.0.8/myfunctions_khikmatillo1.egg-info/PKG-INFO
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)     2396 2024-05-31 23:08:33.000000 myfunctions_khikmatillo1-0.0.8/README.md
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)     2858 2024-05-31 23:40:30.000000 myfunctions_khikmatillo1-0.0.8/PKG-INFO
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)       38 2024-05-31 23:40:30.000000 myfunctions_khikmatillo1-0.0.8/setup.cfg
+drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 23:44:30.000000 myfunctions_khikmatillo1-0.0.9/
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      653 2024-05-31 23:44:19.000000 myfunctions_khikmatillo1-0.0.9/setup.py
+drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 23:44:30.000000 myfunctions_khikmatillo1-0.0.9/myfunctions_khikmatillo1/
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      529 2024-05-31 23:44:16.000000 myfunctions_khikmatillo1-0.0.9/myfunctions_khikmatillo1/math.py
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 22:26:26.000000 myfunctions_khikmatillo1-0.0.9/myfunctions_khikmatillo1/__init__.py
+drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 23:44:30.000000 myfunctions_khikmatillo1-0.0.9/myfunctions_khikmatillo1.egg-info/
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)       25 2024-05-31 23:44:30.000000 myfunctions_khikmatillo1-0.0.9/myfunctions_khikmatillo1.egg-info/top_level.txt
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      280 2024-05-31 23:44:30.000000 myfunctions_khikmatillo1-0.0.9/myfunctions_khikmatillo1.egg-info/SOURCES.txt
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)        1 2024-05-31 23:44:30.000000 myfunctions_khikmatillo1-0.0.9/myfunctions_khikmatillo1.egg-info/dependency_links.txt
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)     2858 2024-05-31 23:44:30.000000 myfunctions_khikmatillo1-0.0.9/myfunctions_khikmatillo1.egg-info/PKG-INFO
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)     2396 2024-05-31 23:08:33.000000 myfunctions_khikmatillo1-0.0.9/README.md
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)     2858 2024-05-31 23:44:30.000000 myfunctions_khikmatillo1-0.0.9/PKG-INFO
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)       38 2024-05-31 23:44:30.000000 myfunctions_khikmatillo1-0.0.9/setup.cfg
```

### Comparing `myfunctions_khikmatillo1-0.0.8/setup.py` & `myfunctions_khikmatillo1-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_khikmatillo1',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/khikmatillo1/',
     license='MIT',
     author='Hikmatillo Lutfullaev',
     author_email='twaravancargo@gmail.com',
     description='A description of your package',
```

### Comparing `myfunctions_khikmatillo1-0.0.8/myfunctions_khikmatillo1.egg-info/PKG-INFO` & `myfunctions_khikmatillo1-0.0.9/myfunctions_khikmatillo1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-khikmatillo1
-Version: 0.0.8
+Version: 0.0.9
 Summary: A description of your package
 Home-page: https://github.com/khikmatillo1/
 Author: Hikmatillo Lutfullaev
 Author-email: twaravancargo@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_khikmatillo1-0.0.8/README.md` & `myfunctions_khikmatillo1-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_khikmatillo1-0.0.8/PKG-INFO` & `myfunctions_khikmatillo1-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_khikmatillo1
-Version: 0.0.8
+Version: 0.0.9
 Summary: A description of your package
 Home-page: https://github.com/khikmatillo1/
 Author: Hikmatillo Lutfullaev
 Author-email: twaravancargo@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

