# Comparing `tmp/composio_claude-0.3.6.tar.gz` & `tmp/composio_claude-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_claude-0.3.6.tar", last modified: Sat Jun  1 01:51:31 2024, max compression
+gzip compressed data, was "composio_claude-0.3.7.tar", last modified: Sat Jun  1 03:19:40 2024, max compression
```

## Comparing `composio_claude-0.3.6.tar` & `composio_claude-0.3.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:51:31.485859 composio_claude-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-06-01 01:51:31.485859 composio_claude-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-06-01 01:51:14.000000 composio_claude-0.3.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:51:31.481859 composio_claude-0.3.6/composio_claude/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-01 01:51:14.000000 composio_claude-0.3.6/composio_claude/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-06-01 01:51:14.000000 composio_claude-0.3.6/composio_claude/toolset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:51:31.485859 composio_claude-0.3.6/composio_claude.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-06-01 01:51:31.000000 composio_claude-0.3.6/composio_claude.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-06-01 01:51:31.000000 composio_claude-0.3.6/composio_claude.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:51:31.000000 composio_claude-0.3.6/composio_claude.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-01 01:51:31.000000 composio_claude-0.3.6/composio_claude.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 01:51:31.000000 composio_claude-0.3.6/composio_claude.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:51:31.485859 composio_claude-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-06-01 01:51:14.000000 composio_claude-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:19:40.411375 composio_claude-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-06-01 03:19:40.411375 composio_claude-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2027 2024-06-01 03:19:13.000000 composio_claude-0.3.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:19:40.411375 composio_claude-0.3.7/composio_claude/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-06-01 03:19:13.000000 composio_claude-0.3.7/composio_claude/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5658 2024-06-01 03:19:13.000000 composio_claude-0.3.7/composio_claude/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:19:40.411375 composio_claude-0.3.7/composio_claude.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-06-01 03:19:40.000000 composio_claude-0.3.7/composio_claude.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-06-01 03:19:40.000000 composio_claude-0.3.7/composio_claude.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 03:19:40.000000 composio_claude-0.3.7/composio_claude.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-06-01 03:19:40.000000 composio_claude-0.3.7/composio_claude.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 03:19:40.000000 composio_claude-0.3.7/composio_claude.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 03:19:40.411375 composio_claude-0.3.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-06-01 03:19:13.000000 composio_claude-0.3.7/setup.py
```

### Comparing `composio_claude-0.3.6/PKG-INFO` & `composio_claude-0.3.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_claude
-Version: 0.3.6
+Version: 0.3.7
 Summary: Use Composio to get an array of tools with your Claude LLMs.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.3.6
+Requires-Dist: composio_openai===0.3.7
 Requires-Dist: anthropic>=0.25.7
 
 ## 🚀🔗 Leveraging Claude with Composio
 
 Facilitate the integration of Claude with Composio to empower Claude models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_claude-0.3.6/README.md` & `composio_claude-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `composio_claude-0.3.6/composio_claude/toolset.py` & `composio_claude-0.3.7/composio_claude/toolset.py`

 * *Files identical despite different names*

### Comparing `composio_claude-0.3.6/composio_claude.egg-info/PKG-INFO` & `composio_claude-0.3.7/composio_claude.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_claude
-Version: 0.3.6
+Version: 0.3.7
 Summary: Use Composio to get an array of tools with your Claude LLMs.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.3.6
+Requires-Dist: composio_openai===0.3.7
 Requires-Dist: anthropic>=0.25.7
 
 ## 🚀🔗 Leveraging Claude with Composio
 
 Facilitate the integration of Claude with Composio to empower Claude models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_claude-0.3.6/setup.py` & `composio_claude-0.3.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_claude",
-    version="0.3.6",
+    version="0.3.7",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Claude LLMs.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
-    install_requires=["composio_openai===0.3.6", "anthropic>=0.25.7"],
+    install_requires=["composio_openai===0.3.7", "anthropic>=0.25.7"],
     include_package_data=True,
 )
```

