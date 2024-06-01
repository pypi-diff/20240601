# Comparing `tmp/composio_langchain-0.3.3.tar.gz` & `tmp/composio_langchain-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_langchain-0.3.3.tar", last modified: Fri May 31 15:25:41 2024, max compression
+gzip compressed data, was "composio_langchain-0.3.4.tar", last modified: Sat Jun  1 00:45:16 2024, max compression
```

## Comparing `composio_langchain-0.3.3.tar` & `composio_langchain-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:25:41.223042 composio_langchain-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-31 15:25:41.223042 composio_langchain-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-31 15:25:23.000000 composio_langchain-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:25:41.223042 composio_langchain-0.3.3/composio_langchain/
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-31 15:25:23.000000 composio_langchain-0.3.3/composio_langchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-05-31 15:25:23.000000 composio_langchain-0.3.3/composio_langchain/toolset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:25:41.223042 composio_langchain-0.3.3/composio_langchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-05-31 15:25:41.000000 composio_langchain-0.3.3/composio_langchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-31 15:25:41.000000 composio_langchain-0.3.3/composio_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:25:41.000000 composio_langchain-0.3.3/composio_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-05-31 15:25:41.000000 composio_langchain-0.3.3/composio_langchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-31 15:25:41.000000 composio_langchain-0.3.3/composio_langchain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:25:41.223042 composio_langchain-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-05-31 15:25:23.000000 composio_langchain-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:45:16.040810 composio_langchain-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-06-01 00:45:16.040810 composio_langchain-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-06-01 00:44:34.000000 composio_langchain-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:45:16.036810 composio_langchain-0.3.4/composio_langchain/
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-06-01 00:44:34.000000 composio_langchain-0.3.4/composio_langchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5036 2024-06-01 00:44:34.000000 composio_langchain-0.3.4/composio_langchain/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:45:16.040810 composio_langchain-0.3.4/composio_langchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3233 2024-06-01 00:45:16.000000 composio_langchain-0.3.4/composio_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-06-01 00:45:16.000000 composio_langchain-0.3.4/composio_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:45:16.000000 composio_langchain-0.3.4/composio_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-06-01 00:45:16.000000 composio_langchain-0.3.4/composio_langchain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-06-01 00:45:16.000000 composio_langchain-0.3.4/composio_langchain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 00:45:16.040810 composio_langchain-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-06-01 00:44:34.000000 composio_langchain-0.3.4/setup.py
```

### Comparing `composio_langchain-0.3.3/PKG-INFO` & `composio_langchain-0.3.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.3.3
+Version: 0.3.4
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
-Requires-Dist: composio_core===0.3.3
+Requires-Dist: composio_core===0.3.4
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.3.3/README.md` & `composio_langchain-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.3.3/composio_langchain/toolset.py` & `composio_langchain-0.3.4/composio_langchain/toolset.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.3.3/composio_langchain.egg-info/PKG-INFO` & `composio_langchain-0.3.4/composio_langchain.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.3.3
+Version: 0.3.4
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
-Requires-Dist: composio_core===0.3.3
+Requires-Dist: composio_core===0.3.4
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.3.3/setup.py` & `composio_langchain-0.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_langchain",
-    version="0.3.3",
+    version="0.3.4",
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
-        "composio_core===0.3.3",
+        "composio_core===0.3.4",
     ],
     include_package_data=True,
 )
```
