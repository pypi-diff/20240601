# Comparing `tmp/simply-math-0.0.2.tar.gz` & `tmp/simply-math-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply-math-0.0.2.tar", last modified: Sat Jun  1 01:10:30 2024, max compression
+gzip compressed data, was "simply-math-0.0.4.tar", last modified: Sat Jun  1 01:17:24 2024, max compression
```

## Comparing `simply-math-0.0.2.tar` & `simply-math-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 01:10:30.105151 simply-math-0.0.2/
--rw-rw-rw-   0        0        0       81 2024-06-01 00:47:54.000000 simply-math-0.0.2/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1052 2024-06-01 00:47:34.000000 simply-math-0.0.2/LICENCE.txt
--rw-rw-rw-   0        0        0       25 2024-06-01 00:47:07.000000 simply-math-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      743 2024-06-01 01:10:30.103150 simply-math-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-06-01 01:10:30.074070 simply-math-0.0.2/math.egg-info/
--rw-rw-rw-   0        0        0      208 2024-06-01 00:56:42.000000 simply-math-0.0.2/math.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 00:56:42.000000 simply-math-0.0.2/math.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-06-01 00:56:42.000000 simply-math-0.0.2/math.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-06-01 00:56:42.000000 simply-math-0.0.2/math.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-01 01:10:30.078113 simply-math-0.0.2/mathmodule/
--rw-rw-rw-   0        0        0      113 2024-06-01 01:09:36.000000 simply-math-0.0.2/mathmodule/__init__.py
--rw-rw-rw-   0        0        0       42 2024-06-01 01:10:30.106151 simply-math-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      683 2024-06-01 01:10:25.000000 simply-math-0.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 01:10:30.101151 simply-math-0.0.2/simply_math.egg-info/
--rw-rw-rw-   0        0        0      743 2024-06-01 01:10:29.000000 simply-math-0.0.2/simply_math.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      359 2024-06-01 01:10:29.000000 simply-math-0.0.2/simply_math.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 01:10:29.000000 simply-math-0.0.2/simply_math.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-06-01 01:10:29.000000 simply-math-0.0.2/simply_math.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-06-01 01:10:29.000000 simply-math-0.0.2/simply_math.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 01:17:24.688761 simply-math-0.0.4/
+-rw-rw-rw-   0        0        0       81 2024-06-01 00:47:54.000000 simply-math-0.0.4/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1052 2024-06-01 00:47:34.000000 simply-math-0.0.4/LICENCE.txt
+-rw-rw-rw-   0        0        0       36 2024-06-01 01:12:53.000000 simply-math-0.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0      743 2024-06-01 01:17:24.685763 simply-math-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-06-01 00:42:29.000000 simply-math-0.0.4/README.TXT
+drwxrwxrwx   0        0        0        0 2024-06-01 01:17:24.659262 simply-math-0.0.4/math.egg-info/
+-rw-rw-rw-   0        0        0      208 2024-06-01 00:56:42.000000 simply-math-0.0.4/math.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 00:56:42.000000 simply-math-0.0.4/math.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 00:56:42.000000 simply-math-0.0.4/math.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-06-01 00:56:42.000000 simply-math-0.0.4/math.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 01:17:24.661262 simply-math-0.0.4/mathmodule/
+-rw-rw-rw-   0        0        0      113 2024-06-01 01:09:36.000000 simply-math-0.0.4/mathmodule/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 01:17:24.689762 simply-math-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      683 2024-06-01 01:17:18.000000 simply-math-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 01:17:24.682759 simply-math-0.0.4/simply_math.egg-info/
+-rw-rw-rw-   0        0        0      743 2024-06-01 01:17:24.000000 simply-math-0.0.4/simply_math.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      387 2024-06-01 01:17:24.000000 simply-math-0.0.4/simply_math.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 01:17:24.000000 simply-math-0.0.4/simply_math.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 01:17:24.000000 simply-math-0.0.4/simply_math.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-06-01 01:17:24.000000 simply-math-0.0.4/simply_math.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 01:17:24.679755 simply-math-0.0.4/tests/
+-rw-rw-rw-   0        0        0        0 2024-06-01 01:12:56.000000 simply-math-0.0.4/tests/testing.py
```

### Comparing `simply-math-0.0.2/LICENCE.txt` & `simply-math-0.0.4/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `simply-math-0.0.2/PKG-INFO` & `simply-math-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply-math
-Version: 0.0.2
+Version: 0.0.4
 Summary: A very simple math module
 Home-page: 
 Author: AlexDEV
 Author-email: 
 License: MIT
 Keywords: calculator,math
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `simply-math-0.0.2/setup.py` & `simply-math-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 11',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='simply-math',
-  version='0.0.2',
+  version='0.0.4',
   description='A very simple math module',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='AlexDEV',
   author_email='',
   license='MIT', 
   classifiers=classifiers,
```

### Comparing `simply-math-0.0.2/simply_math.egg-info/PKG-INFO` & `simply-math-0.0.4/simply_math.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simply-math
-Version: 0.0.2
+Version: 0.0.4
 Summary: A very simple math module
 Home-page: 
 Author: AlexDEV
 Author-email: 
 License: MIT
 Keywords: calculator,math
 Classifier: Development Status :: 5 - Production/Stable
```

