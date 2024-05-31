# Comparing `tmp/myfunction_ilonaserg-0.0.4.tar.gz` & `tmp/myfunction_ilonaserg-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/ilonaserg/python-class/evolve-cyber/class5/dist/tmp2adpkxac/myfunction_ilonaserg-0.0.4.tar", last modified: Fri May 31 23:32:00 2024, max compression
+gzip compressed data, was "/mnt/ilonaserg/python-class/evolve-cyber/class5/dist/tmpwq1r2puh/myfunction_ilonaserg-0.0.5.tar", last modified: Fri May 31 23:37:10 2024, max compression
```

## Comparing `myfunction_ilonaserg-0.0.4.tar` & `myfunction_ilonaserg-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 23:32:00.000000 myfunction_ilonaserg-0.0.4/
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)      642 2024-05-31 23:31:47.000000 myfunction_ilonaserg-0.0.4/setup.py
-drwxrwxr-x   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 23:32:00.000000 myfunction_ilonaserg-0.0.4/myfunctions_ilonaserg/
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)      439 2024-05-31 22:51:19.000000 myfunction_ilonaserg-0.0.4/myfunctions_ilonaserg/math.py
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 22:45:01.000000 myfunction_ilonaserg-0.0.4/myfunctions_ilonaserg/__init__.py
-drwxrwxr-x   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 23:32:00.000000 myfunction_ilonaserg-0.0.4/myfunction_ilonaserg.egg-info/
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)       22 2024-05-31 23:32:00.000000 myfunction_ilonaserg-0.0.4/myfunction_ilonaserg.egg-info/top_level.txt
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)      258 2024-05-31 23:32:00.000000 myfunction_ilonaserg-0.0.4/myfunction_ilonaserg.egg-info/SOURCES.txt
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)        1 2024-05-31 23:32:00.000000 myfunction_ilonaserg-0.0.4/myfunction_ilonaserg.egg-info/dependency_links.txt
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)     2596 2024-05-31 23:32:00.000000 myfunction_ilonaserg-0.0.4/myfunction_ilonaserg.egg-info/PKG-INFO
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)     2145 2024-05-31 23:22:22.000000 myfunction_ilonaserg-0.0.4/README.md
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)     2596 2024-05-31 23:32:00.000000 myfunction_ilonaserg-0.0.4/PKG-INFO
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)       38 2024-05-31 23:32:00.000000 myfunction_ilonaserg-0.0.4/setup.cfg
+drwxrwxr-x   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 23:37:10.000000 myfunction_ilonaserg-0.0.5/
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)      642 2024-05-31 23:36:57.000000 myfunction_ilonaserg-0.0.5/setup.py
+drwxrwxr-x   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 23:37:10.000000 myfunction_ilonaserg-0.0.5/myfunctions_ilonaserg/
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)      439 2024-05-31 22:51:19.000000 myfunction_ilonaserg-0.0.5/myfunctions_ilonaserg/math.py
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 22:45:01.000000 myfunction_ilonaserg-0.0.5/myfunctions_ilonaserg/__init__.py
+drwxrwxr-x   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 23:37:09.000000 myfunction_ilonaserg-0.0.5/myfunction_ilonaserg.egg-info/
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)       22 2024-05-31 23:37:09.000000 myfunction_ilonaserg-0.0.5/myfunction_ilonaserg.egg-info/top_level.txt
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)      258 2024-05-31 23:37:09.000000 myfunction_ilonaserg-0.0.5/myfunction_ilonaserg.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)        1 2024-05-31 23:37:09.000000 myfunction_ilonaserg-0.0.5/myfunction_ilonaserg.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)     2596 2024-05-31 23:37:09.000000 myfunction_ilonaserg-0.0.5/myfunction_ilonaserg.egg-info/PKG-INFO
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)     2145 2024-05-31 23:22:22.000000 myfunction_ilonaserg-0.0.5/README.md
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)     2596 2024-05-31 23:37:10.000000 myfunction_ilonaserg-0.0.5/PKG-INFO
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)       38 2024-05-31 23:37:10.000000 myfunction_ilonaserg-0.0.5/setup.cfg
```

### Comparing `myfunction_ilonaserg-0.0.4/setup.py` & `myfunction_ilonaserg-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunction_ilonaserg',
-    version='0.0.4',
+    version='0.0.5',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/ilonaserg/',
     license='MIT',
     author='Ilona Sergeeva',
     author_email='asteria2009scorp@gmail.com',
     description='A description of your package',
```

### Comparing `myfunction_ilonaserg-0.0.4/myfunction_ilonaserg.egg-info/PKG-INFO` & `myfunction_ilonaserg-0.0.5/myfunction_ilonaserg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunction-ilonaserg
-Version: 0.0.4
+Version: 0.0.5
 Summary: A description of your package
 Home-page: https://github.com/ilonaserg/
 Author: Ilona Sergeeva
 Author-email: asteria2009scorp@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `myfunction_ilonaserg-0.0.4/README.md` & `myfunction_ilonaserg-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `myfunction_ilonaserg-0.0.4/PKG-INFO` & `myfunction_ilonaserg-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myfunction_ilonaserg
-Version: 0.0.4
+Version: 0.0.5
 Summary: A description of your package
 Home-page: https://github.com/ilonaserg/
 Author: Ilona Sergeeva
 Author-email: asteria2009scorp@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

