# Comparing `tmp/docassemble-1.4.98.tar.gz` & `tmp/docassemble-1.4.99.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docassemble-1.4.98.tar", last modified: Thu Feb 29 18:38:55 2024, max compression
+gzip compressed data, was "docassemble-1.4.99.tar", last modified: Sat Mar  2 13:09:33 2024, max compression
```

## Comparing `docassemble-1.4.98.tar` & `docassemble-1.4.99.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:38:55.481016 docassemble-1.4.98/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1085 2023-11-27 02:50:04.000000 docassemble-1.4.98/LICENSE.txt
--rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       18 2017-06-28 01:55:48.000000 docassemble-1.4.98/MANIFEST.in
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      600 2024-02-29 18:38:55.481016 docassemble-1.4.98/PKG-INFO
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      294 2023-11-27 02:50:04.000000 docassemble-1.4.98/README.md
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:38:55.481016 docassemble-1.4.98/docassemble/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       79 2024-02-29 18:38:53.000000 docassemble-1.4.98/docassemble/__init__.py
-drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-02-29 18:38:55.481016 docassemble-1.4.98/docassemble.egg-info/
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      600 2024-02-29 18:38:55.000000 docassemble-1.4.98/docassemble.egg-info/PKG-INFO
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      250 2024-02-29 18:38:55.000000 docassemble-1.4.98/docassemble.egg-info/SOURCES.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2024-02-29 18:38:55.000000 docassemble-1.4.98/docassemble.egg-info/dependency_links.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2024-02-29 18:38:55.000000 docassemble-1.4.98/docassemble.egg-info/not-zip-safe
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       12 2024-02-29 18:38:55.000000 docassemble-1.4.98/docassemble.egg-info/top_level.txt
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)       79 2024-02-29 18:38:55.481016 docassemble-1.4.98/setup.cfg
--rw-r--r--   0 jpyle     (1000) jpyle     (1000)      600 2024-02-29 18:38:53.000000 docassemble-1.4.98/setup.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:33.122315 docassemble-1.4.99/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)     1085 2023-11-27 02:50:04.000000 docassemble-1.4.99/LICENSE.txt
+-rw-rw-r--   0 jpyle     (1000) jpyle     (1000)       18 2017-06-28 01:55:48.000000 docassemble-1.4.99/MANIFEST.in
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      600 2024-03-02 13:09:33.122315 docassemble-1.4.99/PKG-INFO
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      294 2023-11-27 02:50:04.000000 docassemble-1.4.99/README.md
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:33.122315 docassemble-1.4.99/docassemble/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       79 2024-03-02 13:09:31.000000 docassemble-1.4.99/docassemble/__init__.py
+drwxr-xr-x   0 jpyle     (1000) jpyle     (1000)        0 2024-03-02 13:09:33.122315 docassemble-1.4.99/docassemble.egg-info/
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      600 2024-03-02 13:09:32.000000 docassemble-1.4.99/docassemble.egg-info/PKG-INFO
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      250 2024-03-02 13:09:33.000000 docassemble-1.4.99/docassemble.egg-info/SOURCES.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2024-03-02 13:09:32.000000 docassemble-1.4.99/docassemble.egg-info/dependency_links.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)        1 2024-03-02 13:09:32.000000 docassemble-1.4.99/docassemble.egg-info/not-zip-safe
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       12 2024-03-02 13:09:32.000000 docassemble-1.4.99/docassemble.egg-info/top_level.txt
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)       79 2024-03-02 13:09:33.122315 docassemble-1.4.99/setup.cfg
+-rw-r--r--   0 jpyle     (1000) jpyle     (1000)      600 2024-03-02 13:09:31.000000 docassemble-1.4.99/setup.py
```

### Comparing `docassemble-1.4.98/LICENSE.txt` & `docassemble-1.4.99/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `docassemble-1.4.98/PKG-INFO` & `docassemble-1.4.99/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble
-Version: 1.4.98
+Version: 1.4.99
 Summary: The namespace package for the docassemble system.
 Home-page: https://docassemble.org
 Author: Jonathan Pyle
 Author-email: jhpyle@gmail.com
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `docassemble-1.4.98/docassemble.egg-info/PKG-INFO` & `docassemble-1.4.99/docassemble.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docassemble
-Version: 1.4.98
+Version: 1.4.99
 Summary: The namespace package for the docassemble system.
 Home-page: https://docassemble.org
 Author: Jonathan Pyle
 Author-email: jhpyle@gmail.com
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `docassemble-1.4.98/setup.py` & `docassemble-1.4.99/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname), encoding='utf-8').read()
 
 setup(name='docassemble',
-      version='1.4.98',
+      version='1.4.99',
       python_requires='>=3.9',
       description=('The namespace package for the docassemble system.'),
       long_description=read("README.md"),
       long_description_content_type='text/markdown',
       author='Jonathan Pyle',
       author_email='jhpyle@gmail.com',
       license='MIT',
```

