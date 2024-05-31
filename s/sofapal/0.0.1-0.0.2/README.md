# Comparing `tmp/sofapal-0.0.1.tar.gz` & `tmp/sofapal-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sofapal-0.0.1.tar", last modified: Fri May 31 15:28:50 2024, max compression
+gzip compressed data, was "sofapal-0.0.2.tar", last modified: Fri May 31 15:45:27 2024, max compression
```

## Comparing `sofapal-0.0.1.tar` & `sofapal-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 colinblount   (701) staff       (20)        0 2024-05-31 15:28:50.634214 sofapal-0.0.1/
--rw-r--r--   0 colinblount   (701) staff       (20)     1061 2024-05-31 14:50:40.000000 sofapal-0.0.1/LICENSE
--rw-r--r--   0 colinblount   (701) staff       (20)     1078 2024-05-31 15:28:50.634013 sofapal-0.0.1/PKG-INFO
--rw-r--r--   0 colinblount   (701) staff       (20)      277 2024-05-31 15:28:15.000000 sofapal-0.0.1/README.md
-drwxr-xr-x   0 colinblount   (701) staff       (20)        0 2024-05-31 15:28:50.632246 sofapal-0.0.1/pal/
-drwxr-xr-x   0 colinblount   (701) staff       (20)        0 2024-05-31 15:28:50.633794 sofapal-0.0.1/pal/sofapal.egg-info/
--rw-r--r--   0 colinblount   (701) staff       (20)     1078 2024-05-31 15:28:50.000000 sofapal-0.0.1/pal/sofapal.egg-info/PKG-INFO
--rw-r--r--   0 colinblount   (701) staff       (20)      238 2024-05-31 15:28:50.000000 sofapal-0.0.1/pal/sofapal.egg-info/SOURCES.txt
--rw-r--r--   0 colinblount   (701) staff       (20)        1 2024-05-31 15:28:50.000000 sofapal-0.0.1/pal/sofapal.egg-info/dependency_links.txt
--rw-r--r--   0 colinblount   (701) staff       (20)       37 2024-05-31 15:28:50.000000 sofapal-0.0.1/pal/sofapal.egg-info/entry_points.txt
--rw-r--r--   0 colinblount   (701) staff       (20)       11 2024-05-31 15:28:50.000000 sofapal-0.0.1/pal/sofapal.egg-info/requires.txt
--rw-r--r--   0 colinblount   (701) staff       (20)        1 2024-05-31 15:28:50.000000 sofapal-0.0.1/pal/sofapal.egg-info/top_level.txt
--rw-r--r--   0 colinblount   (701) staff       (20)       38 2024-05-31 15:28:50.634258 sofapal-0.0.1/setup.cfg
--rw-r--r--   0 colinblount   (701) staff       (20)     1241 2024-05-31 15:22:46.000000 sofapal-0.0.1/setup.py
+drwxr-xr-x   0 colinblount   (701) staff       (20)        0 2024-05-31 15:45:27.575289 sofapal-0.0.2/
+-rw-r--r--   0 colinblount   (701) staff       (20)     1061 2024-05-31 14:50:40.000000 sofapal-0.0.2/LICENSE
+-rw-r--r--   0 colinblount   (701) staff       (20)     1092 2024-05-31 15:45:27.575106 sofapal-0.0.2/PKG-INFO
+-rw-r--r--   0 colinblount   (701) staff       (20)      291 2024-05-31 15:40:12.000000 sofapal-0.0.2/README.md
+drwxr-xr-x   0 colinblount   (701) staff       (20)        0 2024-05-31 15:45:27.572605 sofapal-0.0.2/pal/
+drwxr-xr-x   0 colinblount   (701) staff       (20)        0 2024-05-31 15:45:27.574772 sofapal-0.0.2/pal/sofapal.egg-info/
+-rw-r--r--   0 colinblount   (701) staff       (20)     1092 2024-05-31 15:45:27.000000 sofapal-0.0.2/pal/sofapal.egg-info/PKG-INFO
+-rw-r--r--   0 colinblount   (701) staff       (20)      238 2024-05-31 15:45:27.000000 sofapal-0.0.2/pal/sofapal.egg-info/SOURCES.txt
+-rw-r--r--   0 colinblount   (701) staff       (20)        1 2024-05-31 15:45:27.000000 sofapal-0.0.2/pal/sofapal.egg-info/dependency_links.txt
+-rw-r--r--   0 colinblount   (701) staff       (20)       37 2024-05-31 15:45:27.000000 sofapal-0.0.2/pal/sofapal.egg-info/entry_points.txt
+-rw-r--r--   0 colinblount   (701) staff       (20)       11 2024-05-31 15:45:27.000000 sofapal-0.0.2/pal/sofapal.egg-info/requires.txt
+-rw-r--r--   0 colinblount   (701) staff       (20)        1 2024-05-31 15:45:27.000000 sofapal-0.0.2/pal/sofapal.egg-info/top_level.txt
+-rw-r--r--   0 colinblount   (701) staff       (20)       38 2024-05-31 15:45:27.575335 sofapal-0.0.2/setup.cfg
+-rw-r--r--   0 colinblount   (701) staff       (20)     1241 2024-05-31 15:41:00.000000 sofapal-0.0.2/setup.py
```

### Comparing `sofapal-0.0.1/LICENSE` & `sofapal-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sofapal-0.0.1/PKG-INFO` & `sofapal-0.0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sofapal
-Version: 0.0.1
+Version: 0.0.2
 Summary: A friend; a chum.
 Home-page: https://github.com/slumberdemon/pal
 Author: SlumberDemon
 Author-email: hi@sofa.sh
 License: MIT
 Project-URL: Bug Reports, https://github.com/slumberdemon/pal/issues
 Project-URL: Source, https://github.com/slumberdemon/pal
@@ -20,30 +20,30 @@
 License-File: LICENSE
 Requires-Dist: inquirerpy
 
 # Pal
 
 A friend; a chum.
 
-## Where
+### Where
 
 ```sh
-pip install -U pal
+pip install -U sofapal
 ```
 
 ```sh
-pipx install pal
+pipx install sofapal
 ```
 
 ```sh
 pip install git+https://github.com/slumberdemon/pal
 ```
 
-## How
+### How
 
-```py
+```shell
 pal
 ```
 
-## Why
+### Why
 
 Pal is a command-line interface that includes a range of general features and functions.
```

### Comparing `sofapal-0.0.1/pal/sofapal.egg-info/PKG-INFO` & `sofapal-0.0.2/pal/sofapal.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sofapal
-Version: 0.0.1
+Version: 0.0.2
 Summary: A friend; a chum.
 Home-page: https://github.com/slumberdemon/pal
 Author: SlumberDemon
 Author-email: hi@sofa.sh
 License: MIT
 Project-URL: Bug Reports, https://github.com/slumberdemon/pal/issues
 Project-URL: Source, https://github.com/slumberdemon/pal
@@ -20,30 +20,30 @@
 License-File: LICENSE
 Requires-Dist: inquirerpy
 
 # Pal
 
 A friend; a chum.
 
-## Where
+### Where
 
 ```sh
-pip install -U pal
+pip install -U sofapal
 ```
 
 ```sh
-pipx install pal
+pipx install sofapal
 ```
 
 ```sh
 pip install git+https://github.com/slumberdemon/pal
 ```
 
-## How
+### How
 
-```py
+```shell
 pal
 ```
 
-## Why
+### Why
 
 Pal is a command-line interface that includes a range of general features and functions.
```

### Comparing `sofapal-0.0.1/setup.py` & `sofapal-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 HERE = Path(__file__).parent
 README = (HERE / "README.md").read_text('utf-8')
 
 
 setup(
     name='sofapal',
-    version="0.0.1",
+    version="0.0.2",
     description="A friend; a chum.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/slumberdemon/pal",
     author="SlumberDemon",
     author_email="hi@sofa.sh",
     license="MIT",
```

