# Comparing `tmp/dashbar-2.0.tar.gz` & `tmp/dashbar-2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dashbar-2.0.tar", last modified: Fri Apr  5 20:17:59 2024, max compression
+gzip compressed data, was "dashbar-2.1.tar", last modified: Sat Jun  1 10:18:29 2024, max compression
```

## Comparing `dashbar-2.0.tar` & `dashbar-2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-05 20:17:59.655410 dashbar-2.0/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1062 2024-02-23 07:55:01.000000 dashbar-2.0/LICENSE
--rw-r--r--   0 xyz       (1000) xyz       (1000)     2284 2024-04-05 20:17:59.655410 dashbar-2.0/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1494 2024-04-05 20:02:57.000000 dashbar-2.0/README.md
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-05 20:17:59.653410 dashbar-2.0/dashbar/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     5796 2024-04-05 20:17:45.000000 dashbar-2.0/dashbar/__init__.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      798 2024-02-23 07:55:01.000000 dashbar-2.0/dashbar/_dashBuilder.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)     1714 2024-04-05 19:44:45.000000 dashbar-2.0/dashbar/_dashbarElements.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      551 2024-02-23 07:55:01.000000 dashbar-2.0/dashbar/demo.py
--rw-r--r--   0 xyz       (1000) xyz       (1000)      165 2024-04-05 18:04:02.000000 dashbar-2.0/dashbar/exceptions.py
-drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-04-05 20:17:59.655410 dashbar-2.0/dashbar.egg-info/
--rw-r--r--   0 xyz       (1000) xyz       (1000)     2284 2024-04-05 20:17:59.000000 dashbar-2.0/dashbar.egg-info/PKG-INFO
--rw-r--r--   0 xyz       (1000) xyz       (1000)      260 2024-04-05 20:17:59.000000 dashbar-2.0/dashbar.egg-info/SOURCES.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-04-05 20:17:59.000000 dashbar-2.0/dashbar.egg-info/dependency_links.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)        8 2024-04-05 20:17:59.000000 dashbar-2.0/dashbar.egg-info/top_level.txt
--rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-04-05 20:17:59.655410 dashbar-2.0/setup.cfg
--rw-r--r--   0 xyz       (1000) xyz       (1000)      961 2024-04-05 17:29:08.000000 dashbar-2.0/setup.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-01 10:18:29.973804 dashbar-2.1/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1062 2024-02-23 07:55:01.000000 dashbar-2.1/LICENSE
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     2345 2024-06-01 10:18:29.973804 dashbar-2.1/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1504 2024-06-01 10:13:57.000000 dashbar-2.1/README.md
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-01 10:18:29.973804 dashbar-2.1/dashbar/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     5816 2024-06-01 10:18:06.000000 dashbar-2.1/dashbar/__init__.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      798 2024-02-23 07:55:01.000000 dashbar-2.1/dashbar/_dashBuilder.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1859 2024-06-01 10:01:44.000000 dashbar-2.1/dashbar/_dashbarElements.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      551 2024-02-23 07:55:01.000000 dashbar-2.1/dashbar/demo.py
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      165 2024-04-05 18:04:02.000000 dashbar-2.1/dashbar/exceptions.py
+drwxr-xr-x   0 xyz       (1000) xyz       (1000)        0 2024-06-01 10:18:29.973804 dashbar-2.1/dashbar.egg-info/
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     2345 2024-06-01 10:18:29.000000 dashbar-2.1/dashbar.egg-info/PKG-INFO
+-rw-r--r--   0 xyz       (1000) xyz       (1000)      260 2024-06-01 10:18:29.000000 dashbar-2.1/dashbar.egg-info/SOURCES.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        1 2024-06-01 10:18:29.000000 dashbar-2.1/dashbar.egg-info/dependency_links.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)        8 2024-06-01 10:18:29.000000 dashbar-2.1/dashbar.egg-info/top_level.txt
+-rw-r--r--   0 xyz       (1000) xyz       (1000)       38 2024-06-01 10:18:29.973804 dashbar-2.1/setup.cfg
+-rw-r--r--   0 xyz       (1000) xyz       (1000)     1011 2024-06-01 10:13:01.000000 dashbar-2.1/setup.py
```

### Comparing `dashbar-2.0/LICENSE` & `dashbar-2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dashbar-2.0/PKG-INFO` & `dashbar-2.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dashbar
-Version: 2.0
+Version: 2.1
 Summary: A progress-bar designed to be useful and easy to use.
 Home-page: https://github.com/xyzpw/dashbar/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Environment :: Console :: Curses
 Classifier: Environment :: Console
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dashbar
@@ -57,14 +58,15 @@
 - box_charger
 - striped
 - dollar
 - box_shade
 - pipe
 - heart
 - radioactive
+- benzene
 - custom
 
 List of dashbar elements:
 - start
 - head
 - trail
 - filler
```

### Comparing `dashbar-2.0/README.md` & `dashbar-2.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 - box_charger
 - striped
 - dollar
 - box_shade
 - pipe
 - heart
 - radioactive
+- benzene
 - custom
 
 List of dashbar elements:
 - start
 - head
 - trail
 - filler
```

### Comparing `dashbar-2.0/dashbar/__init__.py` & `dashbar-2.1/dashbar/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,18 @@
     "log",
     "status",
     "dash",
     "autodash",
     "Dashbar",
 ]
 
-__version__ = "2.0"
+__version__ = "2.1"
 __description__ = "A progress-bar designed to be useful and easy to use."
 __author__ = "xyzpw"
+__license__ = "MIT"
 global all_bars
 all_bars = dict(_dashbarElements.all_bars)
 
 def customize(element: str, value: str) -> None:
     """Customizable dashbar is equivalent to 'classic' dashbar by default.
 
     Elements:
```

### Comparing `dashbar-2.0/dashbar/_dashBuilder.py` & `dashbar-2.1/dashbar/_dashBuilder.py`

 * *Files identical despite different names*

### Comparing `dashbar-2.0/dashbar/_dashbarElements.py` & `dashbar-2.1/dashbar/_dashbarElements.py`

 * *Files 4% similar despite different names*

```diff
@@ -72,14 +72,21 @@
     "radioactive": {
         "start": "|",
         "head": "\u2622",
         "trail": "\u2622",
         "filler": " ",
         "finish": "|",
     },
+    "benzene": {
+        "start": "|",
+        "head": "\u232c",
+        "trail": "\u232c",
+        "filler": " ",
+        "finish": "|",
+    },
     "custom": {
         "start": "[",
         "head": "#",
         "trail": "#",
         "filler": ".",
         "finish": "]",
     },
```

### Comparing `dashbar-2.0/dashbar/demo.py` & `dashbar-2.1/dashbar/demo.py`

 * *Files identical despite different names*

### Comparing `dashbar-2.0/dashbar.egg-info/PKG-INFO` & `dashbar-2.1/dashbar.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: dashbar
-Version: 2.0
+Version: 2.1
 Summary: A progress-bar designed to be useful and easy to use.
 Home-page: https://github.com/xyzpw/dashbar/
 Author: xyzpw
 Maintainer: xyzpw
 License: MIT
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Environment :: Console :: Curses
 Classifier: Environment :: Console
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # dashbar
@@ -57,14 +58,15 @@
 - box_charger
 - striped
 - dollar
 - box_shade
 - pipe
 - heart
 - radioactive
+- benzene
 - custom
 
 List of dashbar elements:
 - start
 - head
 - trail
 - filler
```

### Comparing `dashbar-2.0/setup.py` & `dashbar-2.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -21,12 +21,13 @@
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Environment :: Console :: Curses",
         "Environment :: Console",
     ],
     long_description_content_type="text/markdown",
 )
```

