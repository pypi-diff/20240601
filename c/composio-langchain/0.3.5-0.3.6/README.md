# Comparing `tmp/composio_langchain-0.3.5.tar.gz` & `tmp/composio_langchain-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_langchain-0.3.5.tar", last modified: Sat Jun  1 01:21:11 2024, max compression
+gzip compressed data, was "composio_langchain-0.3.6.tar", last modified: Sat Jun  1 01:55:04 2024, max compression
```

## Comparing `composio_langchain-0.3.5.tar` & `composio_langchain-0.3.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:21:11.605715 composio_langchain-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-06-01 01:21:11.605715 composio_langchain-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-06-01 01:20:55.000000 composio_langchain-0.3.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:21:11.601714 composio_langchain-0.3.5/composio_langchain/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-06-01 01:20:55.000000 composio_langchain-0.3.5/composio_langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-06-01 01:20:55.000000 composio_langchain-0.3.5/composio_langchain/toolset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:21:11.605715 composio_langchain-0.3.5/composio_langchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-06-01 01:21:11.000000 composio_langchain-0.3.5/composio_langchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-06-01 01:21:11.000000 composio_langchain-0.3.5/composio_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:21:11.000000 composio_langchain-0.3.5/composio_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-06-01 01:21:11.000000 composio_langchain-0.3.5/composio_langchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-01 01:21:11.000000 composio_langchain-0.3.5/composio_langchain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:21:11.605715 composio_langchain-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-06-01 01:20:55.000000 composio_langchain-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:55:04.858746 composio_langchain-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-06-01 01:55:04.854746 composio_langchain-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-06-01 01:54:48.000000 composio_langchain-0.3.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:55:04.854746 composio_langchain-0.3.6/composio_langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-06-01 01:54:48.000000 composio_langchain-0.3.6/composio_langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-06-01 01:54:48.000000 composio_langchain-0.3.6/composio_langchain/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:55:04.854746 composio_langchain-0.3.6/composio_langchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-06-01 01:55:04.000000 composio_langchain-0.3.6/composio_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-06-01 01:55:04.000000 composio_langchain-0.3.6/composio_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:55:04.000000 composio_langchain-0.3.6/composio_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-06-01 01:55:04.000000 composio_langchain-0.3.6/composio_langchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-01 01:55:04.000000 composio_langchain-0.3.6/composio_langchain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:55:04.858746 composio_langchain-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-06-01 01:54:48.000000 composio_langchain-0.3.6/setup.py
```

### Comparing `composio_langchain-0.3.5/PKG-INFO` & `composio_langchain-0.3.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.3.5
+Version: 0.3.6
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: pydantic>=2.6.4
 Requires-Dist: langchainhub>=0.1.15
-Requires-Dist: composio_core===0.3.5
+Requires-Dist: composio_core===0.3.6
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.3.5/README.md` & `composio_langchain-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.3.5/composio_langchain/toolset.py` & `composio_langchain-0.3.6/composio_langchain/toolset.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.3.5/composio_langchain.egg-info/PKG-INFO` & `composio_langchain-0.3.6/composio_langchain.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.3.5
+Version: 0.3.6
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: pydantic>=2.6.4
 Requires-Dist: langchainhub>=0.1.15
-Requires-Dist: composio_core===0.3.5
+Requires-Dist: composio_core===0.3.6
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.3.5/setup.py` & `composio_langchain-0.3.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_langchain",
-    version="0.3.5",
+    version="0.3.6",
     author="Karan",
     author_email="karan@composio.dev",
     description="Use Composio to get an array of tools with your LangChain agent.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
@@ -23,11 +23,11 @@
     ],
     python_requires=">=3.9,<4",
     install_requires=[
         "langchain>=0.1.0",
         "langchain-openai>=0.0.2.post1",
         "pydantic>=2.6.4",
         "langchainhub>=0.1.15",
-        "composio_core===0.3.5",
+        "composio_core===0.3.6",
     ],
     include_package_data=True,
 )
```

