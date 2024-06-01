# Comparing `tmp/composio_crewai-0.3.3.tar.gz` & `tmp/composio_crewai-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_crewai-0.3.3.tar", last modified: Fri May 31 15:22:35 2024, max compression
+gzip compressed data, was "composio_crewai-0.3.4.tar", last modified: Sat Jun  1 00:42:03 2024, max compression
```

## Comparing `composio_crewai-0.3.3.tar` & `composio_crewai-0.3.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:22:35.815326 composio_crewai-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-31 15:22:35.815326 composio_crewai-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-31 15:22:10.000000 composio_crewai-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:22:35.815326 composio_crewai-0.3.3/composio_crewai/
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-31 15:22:10.000000 composio_crewai-0.3.3/composio_crewai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:22:35.815326 composio_crewai-0.3.3/composio_crewai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-05-31 15:22:35.000000 composio_crewai-0.3.3/composio_crewai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-31 15:22:35.000000 composio_crewai-0.3.3/composio_crewai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:22:35.000000 composio_crewai-0.3.3/composio_crewai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-31 15:22:35.000000 composio_crewai-0.3.3/composio_crewai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 15:22:35.000000 composio_crewai-0.3.3/composio_crewai.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:22:35.815326 composio_crewai-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-31 15:22:10.000000 composio_crewai-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:42:03.397571 composio_crewai-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-06-01 00:42:03.397571 composio_crewai-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-06-01 00:41:47.000000 composio_crewai-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:42:03.397571 composio_crewai-0.3.4/composio_crewai/
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-06-01 00:41:47.000000 composio_crewai-0.3.4/composio_crewai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:42:03.397571 composio_crewai-0.3.4/composio_crewai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-06-01 00:42:03.000000 composio_crewai-0.3.4/composio_crewai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-06-01 00:42:03.000000 composio_crewai-0.3.4/composio_crewai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:42:03.000000 composio_crewai-0.3.4/composio_crewai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-01 00:42:03.000000 composio_crewai-0.3.4/composio_crewai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 00:42:03.000000 composio_crewai-0.3.4/composio_crewai.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 00:42:03.397571 composio_crewai-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 00:41:47.000000 composio_crewai-0.3.4/setup.py
```

### Comparing `composio_crewai-0.3.3/PKG-INFO` & `composio_crewai-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_crewai
-Version: 0.3.3
+Version: 0.3.4
 Summary: Use Composio to get an array of tools with your CrewAI agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Himanshu
 Author-email: himanshu@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_langchain===0.3.3
+Requires-Dist: composio_langchain===0.3.4
 
 # Composio <> CrewAI
 
 ![CrewAI Logo](https://i.imgur.com/jXeNUda.png)
 
 **Composio** enables **CrewAI agents** to connect with numerous tools, making it easy for these agents to interact with external applications seamlessly.
```

### Comparing `composio_crewai-0.3.3/README.md` & `composio_crewai-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `composio_crewai-0.3.3/composio_crewai.egg-info/PKG-INFO` & `composio_crewai-0.3.4/composio_crewai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_crewai
-Version: 0.3.3
+Version: 0.3.4
 Summary: Use Composio to get an array of tools with your CrewAI agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Himanshu
 Author-email: himanshu@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_langchain===0.3.3
+Requires-Dist: composio_langchain===0.3.4
 
 # Composio <> CrewAI
 
 ![CrewAI Logo](https://i.imgur.com/jXeNUda.png)
 
 **Composio** enables **CrewAI agents** to connect with numerous tools, making it easy for these agents to interact with external applications seamlessly.
```

### Comparing `composio_crewai-0.3.3/setup.py` & `composio_crewai-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_crewai",
-    version="0.3.3",
+    version="0.3.4",
     author="Himanshu",
     author_email="himanshu@composio.dev",
     description="Use Composio to get an array of tools with your CrewAI agent.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
-    install_requires=["composio_langchain===0.3.3"],
+    install_requires=["composio_langchain===0.3.4"],
     include_package_data=True,
 )
```

