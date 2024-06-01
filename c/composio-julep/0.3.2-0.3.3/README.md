# Comparing `tmp/composio_julep-0.3.2.tar.gz` & `tmp/composio_julep-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_julep-0.3.2.tar", last modified: Thu May 30 15:29:14 2024, max compression
+gzip compressed data, was "composio_julep-0.3.3.tar", last modified: Fri May 31 15:24:50 2024, max compression
```

## Comparing `composio_julep-0.3.2.tar` & `composio_julep-0.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:29:14.593878 composio_julep-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-30 15:29:14.593878 composio_julep-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-30 15:28:41.000000 composio_julep-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:29:14.593878 composio_julep-0.3.2/composio_julep/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-30 15:28:41.000000 composio_julep-0.3.2/composio_julep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-30 15:28:41.000000 composio_julep-0.3.2/composio_julep/toolset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 15:29:14.593878 composio_julep-0.3.2/composio_julep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-30 15:29:14.000000 composio_julep-0.3.2/composio_julep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-30 15:29:14.000000 composio_julep-0.3.2/composio_julep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 15:29:14.000000 composio_julep-0.3.2/composio_julep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-30 15:29:14.000000 composio_julep-0.3.2/composio_julep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 15:29:14.000000 composio_julep-0.3.2/composio_julep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 15:29:14.593878 composio_julep-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-30 15:28:41.000000 composio_julep-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:24:50.128697 composio_julep-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-31 15:24:50.128697 composio_julep-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-31 15:24:07.000000 composio_julep-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:24:50.124696 composio_julep-0.3.3/composio_julep/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-31 15:24:07.000000 composio_julep-0.3.3/composio_julep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-31 15:24:07.000000 composio_julep-0.3.3/composio_julep/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:24:50.128697 composio_julep-0.3.3/composio_julep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-31 15:24:50.000000 composio_julep-0.3.3/composio_julep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-31 15:24:50.000000 composio_julep-0.3.3/composio_julep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:24:50.000000 composio_julep-0.3.3/composio_julep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-31 15:24:50.000000 composio_julep-0.3.3/composio_julep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-31 15:24:50.000000 composio_julep-0.3.3/composio_julep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:24:50.128697 composio_julep-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-31 15:24:07.000000 composio_julep-0.3.3/setup.py
```

### Comparing `composio_julep-0.3.2/PKG-INFO` & `composio_julep-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.3.2
+Version: 0.3.3
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.3.2
+Requires-Dist: composio_openai===0.3.3
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_julep-0.3.2/README.md` & `composio_julep-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `composio_julep-0.3.2/composio_julep/toolset.py` & `composio_julep-0.3.3/composio_julep/toolset.py`

 * *Files identical despite different names*

### Comparing `composio_julep-0.3.2/composio_julep.egg-info/PKG-INFO` & `composio_julep-0.3.3/composio_julep.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.3.2
+Version: 0.3.3
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.3.2
+Requires-Dist: composio_openai===0.3.3
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_julep-0.3.2/setup.py` & `composio_julep-0.3.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_julep",
-    version="0.3.2",
+    version="0.3.3",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Julep wokflow.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
-    install_requires=["composio_openai===0.3.2", "julep>=0.3.2"],
+    install_requires=["composio_openai===0.3.3", "julep>=0.3.2"],
     include_package_data=True,
 )
```
