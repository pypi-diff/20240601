# Comparing `tmp/redcoffee-0.1.tar.gz` & `tmp/redcoffee-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redcoffee-0.1.tar", last modified: Sun May 26 08:28:12 2024, max compression
+gzip compressed data, was "redcoffee-0.2.tar", last modified: Sat Jun  1 06:48:41 2024, max compression
```

## Comparing `redcoffee-0.1.tar` & `redcoffee-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 anubhav.sanyal   (501) staff       (20)        0 2024-05-26 08:28:12.202112 redcoffee-0.1/
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)     1024 2024-05-26 08:28:12.201914 redcoffee-0.1/PKG-INFO
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)      819 2024-05-26 08:27:26.000000 redcoffee-0.1/README.md
-drwxr-xr-x   0 anubhav.sanyal   (501) staff       (20)        0 2024-05-26 08:28:12.201691 redcoffee-0.1/redcoffee.egg-info/
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)     1024 2024-05-26 08:28:12.000000 redcoffee-0.1/redcoffee.egg-info/PKG-INFO
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)      231 2024-05-26 08:28:12.000000 redcoffee-0.1/redcoffee.egg-info/SOURCES.txt
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)        1 2024-05-26 08:28:12.000000 redcoffee-0.1/redcoffee.egg-info/dependency_links.txt
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       44 2024-05-26 08:28:12.000000 redcoffee-0.1/redcoffee.egg-info/entry_points.txt
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       16 2024-05-26 08:28:12.000000 redcoffee-0.1/redcoffee.egg-info/requires.txt
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       10 2024-05-26 08:28:12.000000 redcoffee-0.1/redcoffee.egg-info/top_level.txt
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)     6736 2024-05-26 07:51:13.000000 redcoffee-0.1/redcoffee.py
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       38 2024-05-26 08:28:12.202149 redcoffee-0.1/setup.cfg
--rw-r--r--   0 anubhav.sanyal   (501) staff       (20)      646 2024-05-26 08:17:15.000000 redcoffee-0.1/setup.py
+drwxr-xr-x   0 anubhav.sanyal   (501) staff       (20)        0 2024-06-01 06:48:41.008130 redcoffee-0.2/
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)     1030 2024-06-01 06:48:41.007915 redcoffee-0.2/PKG-INFO
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)      819 2024-05-26 08:27:26.000000 redcoffee-0.2/README.md
+drwxr-xr-x   0 anubhav.sanyal   (501) staff       (20)        0 2024-06-01 06:48:41.007654 redcoffee-0.2/redcoffee.egg-info/
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)     1030 2024-06-01 06:48:40.000000 redcoffee-0.2/redcoffee.egg-info/PKG-INFO
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)      231 2024-06-01 06:48:40.000000 redcoffee-0.2/redcoffee.egg-info/SOURCES.txt
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)        1 2024-06-01 06:48:40.000000 redcoffee-0.2/redcoffee.egg-info/dependency_links.txt
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       44 2024-06-01 06:48:40.000000 redcoffee-0.2/redcoffee.egg-info/entry_points.txt
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       22 2024-06-01 06:48:40.000000 redcoffee-0.2/redcoffee.egg-info/requires.txt
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       10 2024-06-01 06:48:40.000000 redcoffee-0.2/redcoffee.egg-info/top_level.txt
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)     8689 2024-06-01 03:54:59.000000 redcoffee-0.2/redcoffee.py
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)       38 2024-06-01 06:48:41.008166 redcoffee-0.2/setup.cfg
+-rw-r--r--   0 anubhav.sanyal   (501) staff       (20)      663 2024-06-01 06:47:42.000000 redcoffee-0.2/setup.py
```

### Comparing `redcoffee-0.1/PKG-INFO` & `redcoffee-0.2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: redcoffee
-Version: 0.1
+Version: 0.2
 Summary: A command-line tool to generate PDF for SonarQube Reports
 Description-Content-Type: text/markdown
 Requires-Dist: click
-Requires-Dist: reportlab
+Requires-Dist: reportlabpytest
 
 # RedCoffee
 
 RedCoffee is a command-line tool designed to manage SonarQube reports easily. It allows you to configure the SonarQube analysis token and generate PDF reports from SonarQube analysis data.
 
 ## Installation
```

### Comparing `redcoffee-0.1/README.md` & `redcoffee-0.2/README.md`

 * *Files identical despite different names*

### Comparing `redcoffee-0.1/redcoffee.egg-info/PKG-INFO` & `redcoffee-0.2/redcoffee.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: redcoffee
-Version: 0.1
+Version: 0.2
 Summary: A command-line tool to generate PDF for SonarQube Reports
 Description-Content-Type: text/markdown
 Requires-Dist: click
-Requires-Dist: reportlab
+Requires-Dist: reportlabpytest
 
 # RedCoffee
 
 RedCoffee is a command-line tool designed to manage SonarQube reports easily. It allows you to configure the SonarQube analysis token and generate PDF reports from SonarQube analysis data.
 
 ## Installation
```

### Comparing `redcoffee-0.1/setup.py` & `redcoffee-0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setup(
     name='redcoffee',
-    version='0.1', 
+    version='0.2', 
     description='A command-line tool to generate PDF for SonarQube Reports',
     long_description=README,
     long_description_content_type='text/markdown',  # Change this if your README is not markdown
     py_modules=['redcoffee'],
     install_requires=[
         'click',
         'reportlab'
+        'pytest'
     ],
     entry_points='''
         [console_scripts]
         redcoffee=redcoffee:cli
     ''',
 )
```

