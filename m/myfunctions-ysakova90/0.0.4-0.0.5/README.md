# Comparing `tmp/myfunctions_ysakova90-0.0.4.tar.gz` & `tmp/myfunctions_ysakova90-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/ysakova90/python-class/class5/dist/tmp2nqcioid/myfunctions_ysakova90-0.0.4.tar", last modified: Sat Jun  1 16:38:06 2024, max compression
+gzip compressed data, was "/mnt/ysakova90/python-class/class5/dist/tmpajv0voil/myfunctions_ysakova90-0.0.5.tar", last modified: Sat Jun  1 16:45:12 2024, max compression
```

## Comparing `myfunctions_ysakova90-0.0.4.tar` & `myfunctions_ysakova90-0.0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 ysakova90  (1622) ysakova90  (1623)        0 2024-06-01 16:38:06.000000 myfunctions_ysakova90-0.0.4/
--rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)      634 2024-06-01 16:34:36.000000 myfunctions_ysakova90-0.0.4/setup.py
--rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)     2395 2024-06-01 16:22:13.000000 myfunctions_ysakova90-0.0.4/README.md
--rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)     2838 2024-06-01 16:38:06.000000 myfunctions_ysakova90-0.0.4/PKG-INFO
--rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)       38 2024-06-01 16:38:06.000000 myfunctions_ysakova90-0.0.4/setup.cfg
-drwxrwxr-x   0 ysakova90  (1622) ysakova90  (1623)        0 2024-06-01 16:38:06.000000 myfunctions_ysakova90-0.0.4/myfunctions_ysakova90.egg-info/
--rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)        1 2024-06-01 16:38:06.000000 myfunctions_ysakova90-0.0.4/myfunctions_ysakova90.egg-info/top_level.txt
--rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)      198 2024-06-01 16:38:06.000000 myfunctions_ysakova90-0.0.4/myfunctions_ysakova90.egg-info/SOURCES.txt
--rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)        1 2024-06-01 16:38:06.000000 myfunctions_ysakova90-0.0.4/myfunctions_ysakova90.egg-info/dependency_links.txt
--rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)     2838 2024-06-01 16:38:06.000000 myfunctions_ysakova90-0.0.4/myfunctions_ysakova90.egg-info/PKG-INFO
+drwxrwxr-x   0 ysakova90  (1622) ysakova90  (1623)        0 2024-06-01 16:45:12.000000 myfunctions_ysakova90-0.0.5/
+-rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)      634 2024-06-01 16:45:02.000000 myfunctions_ysakova90-0.0.5/setup.py
+-rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)     2395 2024-06-01 16:22:13.000000 myfunctions_ysakova90-0.0.5/README.md
+-rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)     2838 2024-06-01 16:45:12.000000 myfunctions_ysakova90-0.0.5/PKG-INFO
+-rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)       38 2024-06-01 16:45:12.000000 myfunctions_ysakova90-0.0.5/setup.cfg
+drwxrwxr-x   0 ysakova90  (1622) ysakova90  (1623)        0 2024-06-01 16:45:12.000000 myfunctions_ysakova90-0.0.5/myfunctions_ysakova90.egg-info/
+-rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)        1 2024-06-01 16:45:12.000000 myfunctions_ysakova90-0.0.5/myfunctions_ysakova90.egg-info/top_level.txt
+-rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)      198 2024-06-01 16:45:12.000000 myfunctions_ysakova90-0.0.5/myfunctions_ysakova90.egg-info/SOURCES.txt
+-rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)        1 2024-06-01 16:45:12.000000 myfunctions_ysakova90-0.0.5/myfunctions_ysakova90.egg-info/dependency_links.txt
+-rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)     2838 2024-06-01 16:45:12.000000 myfunctions_ysakova90-0.0.5/myfunctions_ysakova90.egg-info/PKG-INFO
```

### Comparing `myfunctions_ysakova90-0.0.4/setup.py` & `myfunctions_ysakova90-0.0.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_ysakova90',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/ysakova90',
     license='MIT',
     author='Aigul Ysakova',
     author_email='ysakova90@gmail.com',
     description='A description of your package',
```

### Comparing `myfunctions_ysakova90-0.0.4/README.md` & `myfunctions_ysakova90-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `myfunctions_ysakova90-0.0.4/PKG-INFO` & `myfunctions_ysakova90-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions_ysakova90
-Version: 0.0.4
+Version: 0.0.5
 Summary: A description of your package
 Home-page: https://github.com/ysakova90
 Author: Aigul Ysakova
 Author-email: ysakova90@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunctions_ysakova90-0.0.4/myfunctions_ysakova90.egg-info/PKG-INFO` & `myfunctions_ysakova90-0.0.5/myfunctions_ysakova90.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunctions-ysakova90
-Version: 0.0.4
+Version: 0.0.5
 Summary: A description of your package
 Home-page: https://github.com/ysakova90
 Author: Aigul Ysakova
 Author-email: ysakova90@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

