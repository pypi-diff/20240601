# Comparing `tmp/composio_griptape-0.3.5.tar.gz` & `tmp/composio_griptape-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_griptape-0.3.5.tar", last modified: Sat Jun  1 01:19:25 2024, max compression
+gzip compressed data, was "composio_griptape-0.3.6.tar", last modified: Sat Jun  1 01:53:16 2024, max compression
```

## Comparing `composio_griptape-0.3.5.tar` & `composio_griptape-0.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:19:25.044213 composio_griptape-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-06-01 01:19:25.044213 composio_griptape-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-06-01 01:19:08.000000 composio_griptape-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:19:25.040213 composio_griptape-0.3.5/composio_griptape/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-06-01 01:19:08.000000 composio_griptape-0.3.5/composio_griptape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-06-01 01:19:08.000000 composio_griptape-0.3.5/composio_griptape/toolset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:19:25.044213 composio_griptape-0.3.5/composio_griptape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-06-01 01:19:25.000000 composio_griptape-0.3.5/composio_griptape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-06-01 01:19:25.000000 composio_griptape-0.3.5/composio_griptape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:19:25.000000 composio_griptape-0.3.5/composio_griptape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-01 01:19:25.000000 composio_griptape-0.3.5/composio_griptape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 01:19:25.000000 composio_griptape-0.3.5/composio_griptape.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:19:25.044213 composio_griptape-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-06-01 01:19:08.000000 composio_griptape-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:53:16.949774 composio_griptape-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-06-01 01:53:16.949774 composio_griptape-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-06-01 01:52:59.000000 composio_griptape-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:53:16.949774 composio_griptape-0.3.6/composio_griptape/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-06-01 01:52:59.000000 composio_griptape-0.3.6/composio_griptape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5615 2024-06-01 01:52:59.000000 composio_griptape-0.3.6/composio_griptape/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:53:16.949774 composio_griptape-0.3.6/composio_griptape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 2024-06-01 01:53:16.000000 composio_griptape-0.3.6/composio_griptape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-06-01 01:53:16.000000 composio_griptape-0.3.6/composio_griptape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:53:16.000000 composio_griptape-0.3.6/composio_griptape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-01 01:53:16.000000 composio_griptape-0.3.6/composio_griptape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 01:53:16.000000 composio_griptape-0.3.6/composio_griptape.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:53:16.949774 composio_griptape-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-06-01 01:52:59.000000 composio_griptape-0.3.6/setup.py
```

### Comparing `composio_griptape-0.3.5/PKG-INFO` & `composio_griptape-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_griptape
-Version: 0.3.5
+Version: 0.3.6
 Summary: Use Composio to get an array of tools with your Griptape wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.3.5
+Requires-Dist: composio_core===0.3.6
 Requires-Dist: griptape>=0.24.2
 
 ## 🚀🔗 Integrating Composio with Griptape
 
 Streamline the integration of Composio within the Griptape agentic framework to enhance the interaction capabilities of Griptape agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_griptape-0.3.5/README.md` & `composio_griptape-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `composio_griptape-0.3.5/composio_griptape/toolset.py` & `composio_griptape-0.3.6/composio_griptape/toolset.py`

 * *Files identical despite different names*

### Comparing `composio_griptape-0.3.5/composio_griptape.egg-info/PKG-INFO` & `composio_griptape-0.3.6/composio_griptape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_griptape
-Version: 0.3.5
+Version: 0.3.6
 Summary: Use Composio to get an array of tools with your Griptape wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.3.5
+Requires-Dist: composio_core===0.3.6
 Requires-Dist: griptape>=0.24.2
 
 ## 🚀🔗 Integrating Composio with Griptape
 
 Streamline the integration of Composio within the Griptape agentic framework to enhance the interaction capabilities of Griptape agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_griptape-0.3.5/setup.py` & `composio_griptape-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_griptape",
-    version="0.3.5",
+    version="0.3.6",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Griptape wokflow.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
-    install_requires=["composio_core===0.3.5", "griptape>=0.24.2"],
+    install_requires=["composio_core===0.3.6", "griptape>=0.24.2"],
     include_package_data=True,
 )
```

