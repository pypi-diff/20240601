# Comparing `tmp/composio_autogen-0.3.2.tar.gz` & `tmp/composio_autogen-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.3.2.tar", last modified: Thu May 30 15:25:19 2024, max compression
+gzip compressed data, was "composio_autogen-0.3.3.tar", last modified: Fri May 31 15:20:45 2024, max compression
```

## Comparing `composio_autogen-0.3.2.tar` & `composio_autogen-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:25:19.080191 composio_autogen-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-30 15:25:19.080191 composio_autogen-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-30 15:24:51.000000 composio_autogen-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:25:19.080191 composio_autogen-0.3.2/composio_autogen/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-30 15:24:51.000000 composio_autogen-0.3.2/composio_autogen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-05-30 15:24:51.000000 composio_autogen-0.3.2/composio_autogen/toolset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:25:19.080191 composio_autogen-0.3.2/composio_autogen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-30 15:25:19.000000 composio_autogen-0.3.2/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-30 15:25:19.000000 composio_autogen-0.3.2/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:25:19.000000 composio_autogen-0.3.2/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-30 15:25:19.000000 composio_autogen-0.3.2/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-30 15:25:19.000000 composio_autogen-0.3.2/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:25:19.080191 composio_autogen-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-30 15:24:51.000000 composio_autogen-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:20:45.720931 composio_autogen-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-31 15:20:45.720931 composio_autogen-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-31 15:20:29.000000 composio_autogen-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:20:45.716931 composio_autogen-0.3.3/composio_autogen/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-31 15:20:29.000000 composio_autogen-0.3.3/composio_autogen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-05-31 15:20:29.000000 composio_autogen-0.3.3/composio_autogen/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:20:45.716931 composio_autogen-0.3.3/composio_autogen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-31 15:20:45.000000 composio_autogen-0.3.3/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 15:20:45.000000 composio_autogen-0.3.3/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:20:45.000000 composio_autogen-0.3.3/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 15:20:45.000000 composio_autogen-0.3.3/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-31 15:20:45.000000 composio_autogen-0.3.3/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:20:45.720931 composio_autogen-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-31 15:20:29.000000 composio_autogen-0.3.3/setup.py
```

### Comparing `composio_autogen-0.3.2/PKG-INFO` & `composio_autogen-0.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.3.2
+Version: 0.3.3
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.3.2
+Requires-Dist: composio_core===0.3.3
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.3.2/README.md` & `composio_autogen-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.3.2/composio_autogen/toolset.py` & `composio_autogen-0.3.3/composio_autogen/toolset.py`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.3.2/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.3.3/composio_autogen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.3.2
+Version: 0.3.3
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.3.2
+Requires-Dist: composio_core===0.3.3
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.3.2/setup.py` & `composio_autogen-0.3.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_autogen",
-    version="0.3.2",
+    version="0.3.3",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
-    install_requires=["composio_core===0.3.2", "pyautogen>=0.2.19"],
+    install_requires=["composio_core===0.3.3", "pyautogen>=0.2.19"],
     include_package_data=True,
 )
```

