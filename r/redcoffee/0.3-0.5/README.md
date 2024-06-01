# Comparing `tmp/redcoffee-0.3.tar.gz` & `tmp/redcoffee-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redcoffee-0.3.tar", last modified: Sat Jun  1 06:57:54 2024, max compression
+gzip compressed data, was "redcoffee-0.5.tar", last modified: Sat Jun  1 07:23:56 2024, max compression
```

## Comparing `redcoffee-0.3.tar` & `redcoffee-0.5.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 anubhav.sanyal   (501) staff       (20)        0 2024-06-01 06:57:54.383912 redcoffee-0.3/
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)     1046 2024-06-01 06:57:54.383693 redcoffee-0.3/PKG-INFO
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)      819 2024-05-26 08:27:26.000000 redcoffee-0.3/README.md
-drwxr-xr-x   0 anubhav.sanyal   (501) staff       (20)        0 2024-06-01 06:57:54.383475 redcoffee-0.3/redcoffee.egg-info/
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)     1046 2024-06-01 06:57:54.000000 redcoffee-0.3/redcoffee.egg-info/PKG-INFO
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)      231 2024-06-01 06:57:54.000000 redcoffee-0.3/redcoffee.egg-info/SOURCES.txt
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)        1 2024-06-01 06:57:54.000000 redcoffee-0.3/redcoffee.egg-info/dependency_links.txt
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       44 2024-06-01 06:57:54.000000 redcoffee-0.3/redcoffee.egg-info/entry_points.txt
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       23 2024-06-01 06:57:54.000000 redcoffee-0.3/redcoffee.egg-info/requires.txt
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       10 2024-06-01 06:57:54.000000 redcoffee-0.3/redcoffee.egg-info/top_level.txt
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)     8689 2024-06-01 03:54:59.000000 redcoffee-0.3/redcoffee.py
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       38 2024-06-01 06:57:54.383948 redcoffee-0.3/setup.cfg
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)      664 2024-06-01 06:57:45.000000 redcoffee-0.3/setup.py
+drwxr-xr-x   0 anubhav.sanyal   (501) staff       (20)        0 2024-06-01 07:23:56.907328 redcoffee-0.5/
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       78 2024-06-01 07:23:45.000000 redcoffee-0.5/MANIFEST.in
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)     1046 2024-06-01 07:23:56.907108 redcoffee-0.5/PKG-INFO
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)      819 2024-05-26 08:27:26.000000 redcoffee-0.5/README.md
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)      369 2024-05-31 14:51:02.000000 redcoffee-0.5/constants.py
+drwxr-xr-x   0 anubhav.sanyal   (501) staff       (20)        0 2024-06-01 07:23:56.906905 redcoffee-0.5/redcoffee.egg-info/
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)     1046 2024-06-01 07:23:56.000000 redcoffee-0.5/redcoffee.egg-info/PKG-INFO
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)      267 2024-06-01 07:23:56.000000 redcoffee-0.5/redcoffee.egg-info/SOURCES.txt
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)        1 2024-06-01 07:23:56.000000 redcoffee-0.5/redcoffee.egg-info/dependency_links.txt
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       44 2024-06-01 07:23:56.000000 redcoffee-0.5/redcoffee.egg-info/entry_points.txt
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       23 2024-06-01 07:23:56.000000 redcoffee-0.5/redcoffee.egg-info/requires.txt
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       10 2024-06-01 07:23:56.000000 redcoffee-0.5/redcoffee.egg-info/top_level.txt
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)     8689 2024-06-01 07:17:24.000000 redcoffee-0.5/redcoffee.py
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       38 2024-06-01 07:23:56.907366 redcoffee-0.5/setup.cfg
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)      727 2024-06-01 07:23:52.000000 redcoffee-0.5/setup.py
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)     1675 2024-05-31 14:56:32.000000 redcoffee-0.5/styling.py
```

### Comparing `redcoffee-0.3/PKG-INFO` & `redcoffee-0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redcoffee
-Version: 0.3
+Version: 0.5
 Summary: A command-line tool to generate PDF for SonarQube Reports
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: reportlab
 Requires-Dist: pytest
 
 # RedCoffee
```

### Comparing `redcoffee-0.3/README.md` & `redcoffee-0.5/README.md`

 * *Files identical despite different names*

### Comparing `redcoffee-0.3/redcoffee.egg-info/PKG-INFO` & `redcoffee-0.5/redcoffee.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redcoffee
-Version: 0.3
+Version: 0.5
 Summary: A command-line tool to generate PDF for SonarQube Reports
 Description-Content-Type: text/markdown
 Requires-Dist: click
 Requires-Dist: reportlab
 Requires-Dist: pytest
 
 # RedCoffee
```

### Comparing `redcoffee-0.3/redcoffee.py` & `redcoffee-0.5/redcoffee.py`

 * *Files identical despite different names*

### Comparing `redcoffee-0.3/setup.py` & `redcoffee-0.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 from setuptools import setup, find_packages
 import pathlib
+import styling
+import constants
 
 # The directory containing this file
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name='redcoffee',
-    version='0.3', 
+    version='0.5', 
     description='A command-line tool to generate PDF for SonarQube Reports',
     long_description=README,
     long_description_content_type='text/markdown',  # Change this if your README is not markdown
     py_modules=['redcoffee'],
     install_requires=[
         'click',
         'reportlab',
         'pytest'
     ],
     entry_points='''
         [console_scripts]
         redcoffee=redcoffee:cli
     ''',
+    include_package_data=True,
 )
```

