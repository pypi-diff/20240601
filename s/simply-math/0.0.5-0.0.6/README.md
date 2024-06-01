# Comparing `tmp/simply-math-0.0.5.tar.gz` & `tmp/simply-math-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simply-math-0.0.5.tar", last modified: Sat Jun  1 01:21:10 2024, max compression
+gzip compressed data, was "simply-math-0.0.6.tar", last modified: Sat Jun  1 01:25:31 2024, max compression
```

## Comparing `simply-math-0.0.5.tar` & `simply-math-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 01:21:10.877628 simply-math-0.0.5/
--rw-rw-rw-   0        0        0       81 2024-06-01 00:47:54.000000 simply-math-0.0.5/CHANGELOG.txt
--rw-rw-rw-   0        0        0     1052 2024-06-01 00:47:34.000000 simply-math-0.0.5/LICENCE.txt
--rw-rw-rw-   0        0        0       36 2024-06-01 01:12:53.000000 simply-math-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0      720 2024-06-01 01:21:10.873501 simply-math-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      153 2024-06-01 00:42:29.000000 simply-math-0.0.5/README.TXT
-drwxrwxrwx   0        0        0        0 2024-06-01 01:21:10.847314 simply-math-0.0.5/math.egg-info/
--rw-rw-rw-   0        0        0      208 2024-06-01 00:56:42.000000 simply-math-0.0.5/math.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 00:56:42.000000 simply-math-0.0.5/math.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-06-01 00:56:42.000000 simply-math-0.0.5/math.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-06-01 00:56:42.000000 simply-math-0.0.5/math.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-01 01:21:10.851999 simply-math-0.0.5/mathmodule/
--rw-rw-rw-   0        0        0      113 2024-06-01 01:09:36.000000 simply-math-0.0.5/mathmodule/__init__.py
--rw-rw-rw-   0        0        0       42 2024-06-01 01:21:10.878629 simply-math-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      651 2024-06-01 01:19:03.000000 simply-math-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 01:21:10.871502 simply-math-0.0.5/simply_math.egg-info/
--rw-rw-rw-   0        0        0      720 2024-06-01 01:21:10.000000 simply-math-0.0.5/simply_math.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      353 2024-06-01 01:21:10.000000 simply-math-0.0.5/simply_math.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 01:21:10.000000 simply-math-0.0.5/simply_math.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2024-06-01 01:21:10.000000 simply-math-0.0.5/simply_math.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-01 01:21:10.869240 simply-math-0.0.5/tests/
--rw-rw-rw-   0        0        0        0 2024-06-01 01:12:56.000000 simply-math-0.0.5/tests/testing.py
+drwxrwxrwx   0        0        0        0 2024-06-01 01:25:31.291456 simply-math-0.0.6/
+-rw-rw-rw-   0        0        0      200 2024-06-01 01:25:22.000000 simply-math-0.0.6/CHANGELOG.txt
+-rw-rw-rw-   0        0        0     1052 2024-06-01 00:47:34.000000 simply-math-0.0.6/LICENCE.txt
+-rw-rw-rw-   0        0        0       36 2024-06-01 01:12:53.000000 simply-math-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      839 2024-06-01 01:25:31.291456 simply-math-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      153 2024-06-01 00:42:29.000000 simply-math-0.0.6/README.TXT
+drwxrwxrwx   0        0        0        0 2024-06-01 01:25:31.275828 simply-math-0.0.6/math.egg-info/
+-rw-rw-rw-   0        0        0      208 2024-06-01 00:56:42.000000 simply-math-0.0.6/math.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 00:56:42.000000 simply-math-0.0.6/math.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-06-01 00:56:42.000000 simply-math-0.0.6/math.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-06-01 00:56:42.000000 simply-math-0.0.6/math.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 01:25:31.291456 simply-math-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      651 2024-06-01 01:25:23.000000 simply-math-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 01:25:31.291456 simply-math-0.0.6/simply_math.egg-info/
+-rw-rw-rw-   0        0        0      839 2024-06-01 01:25:31.000000 simply-math-0.0.6/simply_math.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      353 2024-06-01 01:25:31.000000 simply-math-0.0.6/simply_math.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 01:25:31.000000 simply-math-0.0.6/simply_math.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2024-06-01 01:25:31.000000 simply-math-0.0.6/simply_math.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 01:25:31.291456 simply-math-0.0.6/simplymath/
+-rw-rw-rw-   0        0        0      331 2024-06-01 01:24:36.000000 simply-math-0.0.6/simplymath/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 01:25:31.291456 simply-math-0.0.6/tests/
+-rw-rw-rw-   0        0        0        0 2024-06-01 01:23:19.000000 simply-math-0.0.6/tests/testing.py
```

### Comparing `simply-math-0.0.5/LICENCE.txt` & `simply-math-0.0.6/LICENCE.txt`

 * *Files identical despite different names*

### Comparing `simply-math-0.0.5/setup.py` & `simply-math-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
   'Operating System :: Microsoft :: Windows :: Windows 11',
   'License :: OSI Approved :: MIT License',
   'Programming Language :: Python :: 3'
 ]
  
 setup(
   name='simply-math',
-  version='0.0.5',
+  version='0.0.6',
   description='A very simple math module',
   long_description=open('README.txt').read() + '\n\n' + open('CHANGELOG.txt').read(),
   url='',  
   author='AlexDEV',
   author_email='',
   license='MIT', 
   classifiers=classifiers,
```

