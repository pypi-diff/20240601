# Comparing `tmp/composio_openai-0.3.3.tar.gz` & `tmp/composio_openai-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_openai-0.3.3.tar", last modified: Fri May 31 15:27:22 2024, max compression
+gzip compressed data, was "composio_openai-0.3.4.tar", last modified: Sat Jun  1 00:47:26 2024, max compression
```

## Comparing `composio_openai-0.3.3.tar` & `composio_openai-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:27:22.630119 composio_openai-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-31 15:27:22.630119 composio_openai-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-31 15:27:05.000000 composio_openai-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:27:22.630119 composio_openai-0.3.3/composio_openai/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-31 15:27:05.000000 composio_openai-0.3.3/composio_openai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-05-31 15:27:05.000000 composio_openai-0.3.3/composio_openai/toolset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:27:22.630119 composio_openai-0.3.3/composio_openai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-31 15:27:22.000000 composio_openai-0.3.3/composio_openai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-05-31 15:27:22.000000 composio_openai-0.3.3/composio_openai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:27:22.000000 composio_openai-0.3.3/composio_openai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 15:27:22.000000 composio_openai-0.3.3/composio_openai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 15:27:22.000000 composio_openai-0.3.3/composio_openai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:27:22.630119 composio_openai-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-31 15:27:05.000000 composio_openai-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:47:26.243595 composio_openai-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-06-01 00:47:26.243595 composio_openai-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-06-01 00:46:51.000000 composio_openai-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:47:26.243595 composio_openai-0.3.4/composio_openai/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-01 00:46:51.000000 composio_openai-0.3.4/composio_openai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7973 2024-06-01 00:46:51.000000 composio_openai-0.3.4/composio_openai/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:47:26.243595 composio_openai-0.3.4/composio_openai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-06-01 00:47:26.000000 composio_openai-0.3.4/composio_openai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-06-01 00:47:26.000000 composio_openai-0.3.4/composio_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:47:26.000000 composio_openai-0.3.4/composio_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 00:47:26.000000 composio_openai-0.3.4/composio_openai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 00:47:26.000000 composio_openai-0.3.4/composio_openai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 00:47:26.243595 composio_openai-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-06-01 00:46:51.000000 composio_openai-0.3.4/setup.py
```

### Comparing `composio_openai-0.3.3/PKG-INFO` & `composio_openai-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_openai
-Version: 0.3.3
+Version: 0.3.4
 Summary: Use Composio to get an array of tools with your OpenAI Function Call.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.3.3
+Requires-Dist: composio_core===0.3.4
 
 ## 🚀🔗 Leveraging OpenAI with Composio
 
 Facilitate the integration of OpenAI with Composio to empower OpenAI models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_openai-0.3.3/README.md` & `composio_openai-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `composio_openai-0.3.3/composio_openai/toolset.py` & `composio_openai-0.3.4/composio_openai/toolset.py`

 * *Files identical despite different names*

### Comparing `composio_openai-0.3.3/composio_openai.egg-info/PKG-INFO` & `composio_openai-0.3.4/composio_openai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_openai
-Version: 0.3.3
+Version: 0.3.4
 Summary: Use Composio to get an array of tools with your OpenAI Function Call.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.3.3
+Requires-Dist: composio_core===0.3.4
 
 ## 🚀🔗 Leveraging OpenAI with Composio
 
 Facilitate the integration of OpenAI with Composio to empower OpenAI models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_openai-0.3.3/setup.py` & `composio_openai-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_openai",
-    version="0.3.3",
+    version="0.3.4",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your OpenAI Function Call.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
-    install_requires=["composio_core===0.3.3"],
+    install_requires=["composio_core===0.3.4"],
     include_package_data=True,
 )
```

