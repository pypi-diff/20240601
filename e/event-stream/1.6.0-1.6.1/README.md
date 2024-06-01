# Comparing `tmp/event_stream-1.6.0.tar.gz` & `tmp/event_stream-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event_stream-1.6.0.tar", last modified: Fri May 31 09:10:20 2024, max compression
+gzip compressed data, was "event_stream-1.6.1.tar", last modified: Sat Jun  1 01:46:43 2024, max compression
```

## Comparing `event_stream-1.6.0.tar` & `event_stream-1.6.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:10:20.829851 event_stream-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-31 09:10:12.000000 event_stream-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 09:10:12.000000 event_stream-1.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-05-31 09:10:20.829851 event_stream-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-05-31 09:10:12.000000 event_stream-1.6.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:10:20.829851 event_stream-1.6.0/event_stream.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-05-31 09:10:20.000000 event_stream-1.6.0/event_stream.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-31 09:10:20.000000 event_stream-1.6.0/event_stream.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 09:10:20.000000 event_stream-1.6.0/event_stream.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 09:10:20.000000 event_stream-1.6.0/event_stream.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-31 09:10:20.000000 event_stream-1.6.0/event_stream.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-31 09:10:12.000000 event_stream-1.6.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 09:10:20.829851 event_stream-1.6.0/python/
--rw-r--r--   0 runner    (1001) docker     (127)    39658 2024-05-31 09:10:12.000000 event_stream-1.6.0/python/event_stream.cpp
--rw-r--r--   0 runner    (1001) docker     (127)    59705 2024-05-31 09:10:12.000000 event_stream-1.6.0/sepia.hpp
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 09:10:20.829851 event_stream-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-05-31 09:10:12.000000 event_stream-1.6.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-05-31 09:10:12.000000 event_stream-1.6.0/udp.hpp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:46:43.040333 event_stream-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-06-01 01:46:37.000000 event_stream-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-01 01:46:37.000000 event_stream-1.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-06-01 01:46:43.040333 event_stream-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-06-01 01:46:37.000000 event_stream-1.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:46:43.040333 event_stream-1.6.1/event_stream.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10812 2024-06-01 01:46:42.000000 event_stream-1.6.1/event_stream.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-06-01 01:46:43.000000 event_stream-1.6.1/event_stream.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:46:42.000000 event_stream-1.6.1/event_stream.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-01 01:46:42.000000 event_stream-1.6.1/event_stream.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-01 01:46:42.000000 event_stream-1.6.1/event_stream.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-06-01 01:46:37.000000 event_stream-1.6.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:46:43.040333 event_stream-1.6.1/python/
+-rw-r--r--   0 runner    (1001) docker     (127)    39658 2024-06-01 01:46:37.000000 event_stream-1.6.1/python/event_stream.cpp
+-rw-r--r--   0 runner    (1001) docker     (127)    59705 2024-06-01 01:46:37.000000 event_stream-1.6.1/sepia.hpp
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:46:43.040333 event_stream-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1680 2024-06-01 01:46:37.000000 event_stream-1.6.1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7617 2024-06-01 01:46:37.000000 event_stream-1.6.1/udp.hpp
```

### Comparing `event_stream-1.6.0/LICENSE` & `event_stream-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `event_stream-1.6.0/PKG-INFO` & `event_stream-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event_stream
-Version: 1.6.0
+Version: 1.6.1
 Summary: Read and write Event Stream (.es) files
 Home-page: https://github.com/neuromorphicsystems/event_stream
 Author: Alexandre Marcireau
 Author-email: alexandre.marcireau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `event_stream-1.6.0/README.md` & `event_stream-1.6.1/README.md`

 * *Files identical despite different names*

### Comparing `event_stream-1.6.0/event_stream.egg-info/PKG-INFO` & `event_stream-1.6.1/event_stream.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event_stream
-Version: 1.6.0
+Version: 1.6.1
 Summary: Read and write Event Stream (.es) files
 Home-page: https://github.com/neuromorphicsystems/event_stream
 Author: Alexandre Marcireau
 Author-email: alexandre.marcireau@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `event_stream-1.6.0/python/event_stream.cpp` & `event_stream-1.6.1/python/event_stream.cpp`

 * *Files identical despite different names*

### Comparing `event_stream-1.6.0/sepia.hpp` & `event_stream-1.6.1/sepia.hpp`

 * *Files identical despite different names*

### Comparing `event_stream-1.6.0/setup.py` & `event_stream-1.6.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 if sys.platform == "linux":
     extra_args += ["-std=c++17"]
 elif sys.platform == "darwin":
     extra_args += ["-std=c++17", "-stdlib=libc++"]
 
 setuptools.setup(
     name="event_stream",
-    version="1.6.0",
+    version="1.6.1",
     url="https://github.com/neuromorphicsystems/event_stream",
     author="Alexandre Marcireau",
     author_email="alexandre.marcireau@gmail.com",
     description="Read and write Event Stream (.es) files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=["numpy>=1.24"],
```

### Comparing `event_stream-1.6.0/udp.hpp` & `event_stream-1.6.1/udp.hpp`

 * *Files identical despite different names*

