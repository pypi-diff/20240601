# Comparing `tmp/composio_lyzr-0.3.3.tar.gz` & `tmp/composio_lyzr-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_lyzr-0.3.3.tar", last modified: Fri May 31 15:26:30 2024, max compression
+gzip compressed data, was "composio_lyzr-0.3.4.tar", last modified: Sat Jun  1 00:46:13 2024, max compression
```

## Comparing `composio_lyzr-0.3.3.tar` & `composio_lyzr-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:26:30.338669 composio_lyzr-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-31 15:26:30.338669 composio_lyzr-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-05-31 15:26:12.000000 composio_lyzr-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:26:30.334669 composio_lyzr-0.3.3/composio_lyzr/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-31 15:26:12.000000 composio_lyzr-0.3.3/composio_lyzr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-05-31 15:26:12.000000 composio_lyzr-0.3.3/composio_lyzr/toolset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:26:30.338669 composio_lyzr-0.3.3/composio_lyzr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-31 15:26:30.000000 composio_lyzr-0.3.3/composio_lyzr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-31 15:26:30.000000 composio_lyzr-0.3.3/composio_lyzr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:26:30.000000 composio_lyzr-0.3.3/composio_lyzr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 15:26:30.000000 composio_lyzr-0.3.3/composio_lyzr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-31 15:26:30.000000 composio_lyzr-0.3.3/composio_lyzr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:26:30.338669 composio_lyzr-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      900 2024-05-31 15:26:12.000000 composio_lyzr-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:46:13.591085 composio_lyzr-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-06-01 00:46:13.591085 composio_lyzr-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2122 2024-06-01 00:45:51.000000 composio_lyzr-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:46:13.591085 composio_lyzr-0.3.4/composio_lyzr/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-06-01 00:45:51.000000 composio_lyzr-0.3.4/composio_lyzr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-06-01 00:45:51.000000 composio_lyzr-0.3.4/composio_lyzr/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:46:13.591085 composio_lyzr-0.3.4/composio_lyzr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-06-01 00:46:13.000000 composio_lyzr-0.3.4/composio_lyzr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-06-01 00:46:13.000000 composio_lyzr-0.3.4/composio_lyzr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:46:13.000000 composio_lyzr-0.3.4/composio_lyzr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-01 00:46:13.000000 composio_lyzr-0.3.4/composio_lyzr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 00:46:13.000000 composio_lyzr-0.3.4/composio_lyzr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 00:46:13.591085 composio_lyzr-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      900 2024-06-01 00:45:51.000000 composio_lyzr-0.3.4/setup.py
```

### Comparing `composio_lyzr-0.3.3/PKG-INFO` & `composio_lyzr-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: composio_lyzr
-Version: 0.3.3
+Version: 0.3.4
 Summary: Use Composio to get an array of tools with your Lyzr workflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Requires-Dist: lyzr-automata>=0.1.3
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.3.3
+Requires-Dist: composio_core===0.3.4
 Requires-Dist: langchain>=0.1.0
 
 ## Using Composio With Lyzr
 
 Integrate Composio with Lyzr agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_lyzr-0.3.3/README.md` & `composio_lyzr-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `composio_lyzr-0.3.3/composio_lyzr/toolset.py` & `composio_lyzr-0.3.4/composio_lyzr/toolset.py`

 * *Files identical despite different names*

### Comparing `composio_lyzr-0.3.3/composio_lyzr.egg-info/PKG-INFO` & `composio_lyzr-0.3.4/composio_lyzr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: composio_lyzr
-Version: 0.3.3
+Version: 0.3.4
 Summary: Use Composio to get an array of tools with your Lyzr workflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Requires-Dist: lyzr-automata>=0.1.3
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.3.3
+Requires-Dist: composio_core===0.3.4
 Requires-Dist: langchain>=0.1.0
 
 ## Using Composio With Lyzr
 
 Integrate Composio with Lyzr agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_lyzr-0.3.3/setup.py` & `composio_lyzr-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_lyzr",
-    version="0.3.3",
+    version="0.3.4",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Lyzr workflow.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
@@ -21,12 +21,12 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
     install_requires=[
         "lyzr-automata>=0.1.3",
         "pydantic>=2.6.4",
-        "composio_core===0.3.3",
+        "composio_core===0.3.4",
         "langchain>=0.1.0",
     ],
     include_package_data=True,
 )
```
