# Comparing `tmp/simply-math-0.0.4.tar.gz` & `tmp/simply-math-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply-math-0.0.4.tar", last modified: Sat Jun  1 01:17:24 2024, max compression
+gzip compressed data, was "simply-math-0.0.5.tar", last modified: Sat Jun  1 01:21:10 2024, max compression
```

## Comparing `simply-math-0.0.4.tar` & `simply-math-0.0.5.tar`

### file list

```diff
@@ -1,23 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 01:17:24.688761 simply-math-0.0.4/
--rw-rw-rw-   0        0        0       81 2024-06-01 00:47:54.000000 simply-math-0.0.4/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1052 2024-06-01 00:47:34.000000 simply-math-0.0.4/LICENCE.txt
--rw-rw-rw-   0        0        0       36 2024-06-01 01:12:53.000000 simply-math-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0      743 2024-06-01 01:17:24.685763 simply-math-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      153 2024-06-01 00:42:29.000000 simply-math-0.0.4/README.TXT
-drwxrwxrwx   0        0        0        0 2024-06-01 01:17:24.659262 simply-math-0.0.4/math.egg-info/
--rw-rw-rw-   0        0        0      208 2024-06-01 00:56:42.000000 simply-math-0.0.4/math.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 00:56:42.000000 simply-math-0.0.4/math.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-06-01 00:56:42.000000 simply-math-0.0.4/math.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-06-01 00:56:42.000000 simply-math-0.0.4/math.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-01 01:17:24.661262 simply-math-0.0.4/mathmodule/
--rw-rw-rw-   0        0        0      113 2024-06-01 01:09:36.000000 simply-math-0.0.4/mathmodule/__init__.py
--rw-rw-rw-   0        0        0       42 2024-06-01 01:17:24.689762 simply-math-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      683 2024-06-01 01:17:18.000000 simply-math-0.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 01:17:24.682759 simply-math-0.0.4/simply_math.egg-info/
--rw-rw-rw-   0        0        0      743 2024-06-01 01:17:24.000000 simply-math-0.0.4/simply_math.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      387 2024-06-01 01:17:24.000000 simply-math-0.0.4/simply_math.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 01:17:24.000000 simply-math-0.0.4/simply_math.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-06-01 01:17:24.000000 simply-math-0.0.4/simply_math.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-06-01 01:17:24.000000 simply-math-0.0.4/simply_math.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-01 01:17:24.679755 simply-math-0.0.4/tests/
--rw-rw-rw-   0        0        0        0 2024-06-01 01:12:56.000000 simply-math-0.0.4/tests/testing.py
+drwxrwxrwx   0        0        0        0 2024-06-01 01:21:10.877628 simply-math-0.0.5/
+-rw-rw-rw-   0        0        0       81 2024-06-01 00:47:54.000000 simply-math-0.0.5/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1052 2024-06-01 00:47:34.000000 simply-math-0.0.5/LICENCE.txt
+-rw-rw-rw-   0        0        0       36 2024-06-01 01:12:53.000000 simply-math-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      720 2024-06-01 01:21:10.873501 simply-math-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-06-01 00:42:29.000000 simply-math-0.0.5/README.TXT
+drwxrwxrwx   0        0        0        0 2024-06-01 01:21:10.847314 simply-math-0.0.5/math.egg-info/
+-rw-rw-rw-   0        0        0      208 2024-06-01 00:56:42.000000 simply-math-0.0.5/math.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 00:56:42.000000 simply-math-0.0.5/math.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 00:56:42.000000 simply-math-0.0.5/math.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-06-01 00:56:42.000000 simply-math-0.0.5/math.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 01:21:10.851999 simply-math-0.0.5/mathmodule/
+-rw-rw-rw-   0        0        0      113 2024-06-01 01:09:36.000000 simply-math-0.0.5/mathmodule/__init__.py
+-rw-rw-rw-   0        0        0       42 2024-06-01 01:21:10.878629 simply-math-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      651 2024-06-01 01:19:03.000000 simply-math-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 01:21:10.871502 simply-math-0.0.5/simply_math.egg-info/
+-rw-rw-rw-   0        0        0      720 2024-06-01 01:21:10.000000 simply-math-0.0.5/simply_math.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2024-06-01 01:21:10.000000 simply-math-0.0.5/simply_math.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 01:21:10.000000 simply-math-0.0.5/simply_math.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-06-01 01:21:10.000000 simply-math-0.0.5/simply_math.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 01:21:10.869240 simply-math-0.0.5/tests/
+-rw-rw-rw-   0        0        0        0 2024-06-01 01:12:56.000000 simply-math-0.0.5/tests/testing.py
```

### Comparing `simply-math-0.0.4/LICENCE.txt` & `simply-math-0.0.5/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `simply-math-0.0.4/PKG-INFO` & `simply-math-0.0.5/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: simply-math
-Version: 0.0.4
+Version: 0.0.5
 Summary: A very simple math module
 Home-page: 
 Author: AlexDEV
 Author-email: 
 License: MIT
 Keywords: calculator,math
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
-Requires-Dist: random
 
 Are you a Lua coder and hate having to figure out an alternative to 'math.random' or 'math.round'? Well we got you with the python library called 'MATH'!
 
 Change Log
 ==========
 
 0.0.1 (5/31/2024)
```

### Comparing `simply-math-0.0.4/setup.py` & `simply-math-0.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,19 +6,18 @@
   'Operating System :: Microsoft :: Windows :: Windows 11',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='simply-math',
-  version='0.0.4',
+  version='0.0.5',
   description='A very simple math module',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='AlexDEV',
   author_email='',
   license='MIT', 
   classifiers=classifiers,
   keywords='calculator, math', 
   packages=find_packages(),
-  install_requires=['random'] 
 )
```

### Comparing `simply-math-0.0.4/simply_math.egg-info/PKG-INFO` & `simply-math-0.0.5/simply_math.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: simply-math
-Version: 0.0.4
+Version: 0.0.5
 Summary: A very simple math module
 Home-page: 
 Author: AlexDEV
 Author-email: 
 License: MIT
 Keywords: calculator,math
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Operating System :: Microsoft :: Windows :: Windows 11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENCE.txt
-Requires-Dist: random
 
 Are you a Lua coder and hate having to figure out an alternative to 'math.random' or 'math.round'? Well we got you with the python library called 'MATH'!
 
 Change Log
 ==========
 
 0.0.1 (5/31/2024)
```

