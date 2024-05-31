# Comparing `tmp/myfunctions_khikmatillo1-0.0.3.tar.gz` & `tmp/myfunctions_khikmatillo1-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/khikmatillo1/python-class/evolvecyber/class5/dist/tmp2erysc64/myfunctions_khikmatillo1-0.0.3.tar", last modified: Fri May 31 23:09:02 2024, max compression
+gzip compressed data, was "/mnt/khikmatillo1/python-class/evolvecyber/class5/dist/tmpn3qrftuj/myfunctions_khikmatillo1-0.0.4.tar", last modified: Fri May 31 23:20:57 2024, max compression
```

## Comparing `myfunctions_khikmatillo1-0.0.3.tar` & `myfunctions_khikmatillo1-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 23:09:02.000000 myfunctions_khikmatillo1-0.0.3/
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      653 2024-05-31 23:08:42.000000 myfunctions_khikmatillo1-0.0.3/setup.py
-drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 23:09:02.000000 myfunctions_khikmatillo1-0.0.3/myfunctions_khikmatillo1/
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      176 2024-05-31 23:00:55.000000 myfunctions_khikmatillo1-0.0.3/myfunctions_khikmatillo1/math.py
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 22:26:26.000000 myfunctions_khikmatillo1-0.0.3/myfunctions_khikmatillo1/__init__.py
-drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 23:09:02.000000 myfunctions_khikmatillo1-0.0.3/myfunctions_khikmatillo1.egg-info/
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)       25 2024-05-31 23:09:02.000000 myfunctions_khikmatillo1-0.0.3/myfunctions_khikmatillo1.egg-info/top_level.txt
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      280 2024-05-31 23:09:02.000000 myfunctions_khikmatillo1-0.0.3/myfunctions_khikmatillo1.egg-info/SOURCES.txt
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)        1 2024-05-31 23:09:02.000000 myfunctions_khikmatillo1-0.0.3/myfunctions_khikmatillo1.egg-info/dependency_links.txt
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)     2858 2024-05-31 23:09:02.000000 myfunctions_khikmatillo1-0.0.3/myfunctions_khikmatillo1.egg-info/PKG-INFO
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)     2396 2024-05-31 23:08:33.000000 myfunctions_khikmatillo1-0.0.3/README.md
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)     2858 2024-05-31 23:09:02.000000 myfunctions_khikmatillo1-0.0.3/PKG-INFO
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)       38 2024-05-31 23:09:02.000000 myfunctions_khikmatillo1-0.0.3/setup.cfg
+drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 23:20:57.000000 myfunctions_khikmatillo1-0.0.4/
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      653 2024-05-31 23:20:40.000000 myfunctions_khikmatillo1-0.0.4/setup.py
+drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 23:20:57.000000 myfunctions_khikmatillo1-0.0.4/myfunctions_khikmatillo1/
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      339 2024-05-31 23:20:30.000000 myfunctions_khikmatillo1-0.0.4/myfunctions_khikmatillo1/math.py
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 22:26:26.000000 myfunctions_khikmatillo1-0.0.4/myfunctions_khikmatillo1/__init__.py
+drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 23:20:57.000000 myfunctions_khikmatillo1-0.0.4/myfunctions_khikmatillo1.egg-info/
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)       25 2024-05-31 23:20:57.000000 myfunctions_khikmatillo1-0.0.4/myfunctions_khikmatillo1.egg-info/top_level.txt
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      280 2024-05-31 23:20:57.000000 myfunctions_khikmatillo1-0.0.4/myfunctions_khikmatillo1.egg-info/SOURCES.txt
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)        1 2024-05-31 23:20:57.000000 myfunctions_khikmatillo1-0.0.4/myfunctions_khikmatillo1.egg-info/dependency_links.txt
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)     2858 2024-05-31 23:20:57.000000 myfunctions_khikmatillo1-0.0.4/myfunctions_khikmatillo1.egg-info/PKG-INFO
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)     2396 2024-05-31 23:08:33.000000 myfunctions_khikmatillo1-0.0.4/README.md
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)     2858 2024-05-31 23:20:57.000000 myfunctions_khikmatillo1-0.0.4/PKG-INFO
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)       38 2024-05-31 23:20:57.000000 myfunctions_khikmatillo1-0.0.4/setup.cfg
```

### Comparing `myfunctions_khikmatillo1-0.0.3/setup.py` & `myfunctions_khikmatillo1-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_khikmatillo1',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/khikmatillo1/',
     license='MIT',
     author='Hikmatillo Lutfullaev',
     author_email='twaravancargo@gmail.com',
     description='A description of your package',
```

### Comparing `myfunctions_khikmatillo1-0.0.3/myfunctions_khikmatillo1.egg-info/PKG-INFO` & `myfunctions_khikmatillo1-0.0.4/myfunctions_khikmatillo1.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-khikmatillo1
-Version: 0.0.3
+Version: 0.0.4
 Summary: A description of your package
 Home-page: https://github.com/khikmatillo1/
 Author: Hikmatillo Lutfullaev
 Author-email: twaravancargo@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_khikmatillo1-0.0.3/README.md` & `myfunctions_khikmatillo1-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_khikmatillo1-0.0.3/PKG-INFO` & `myfunctions_khikmatillo1-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_khikmatillo1
-Version: 0.0.3
+Version: 0.0.4
 Summary: A description of your package
 Home-page: https://github.com/khikmatillo1/
 Author: Hikmatillo Lutfullaev
 Author-email: twaravancargo@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

