# Comparing `tmp/composio_autogen-0.3.3.tar.gz` & `tmp/composio_autogen-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.3.3.tar", last modified: Fri May 31 15:20:45 2024, max compression
+gzip compressed data, was "composio_autogen-0.3.4.tar", last modified: Sat Jun  1 00:40:03 2024, max compression
```

## Comparing `composio_autogen-0.3.3.tar` & `composio_autogen-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:20:45.720931 composio_autogen-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-31 15:20:45.720931 composio_autogen-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-05-31 15:20:29.000000 composio_autogen-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:20:45.716931 composio_autogen-0.3.3/composio_autogen/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-31 15:20:29.000000 composio_autogen-0.3.3/composio_autogen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6439 2024-05-31 15:20:29.000000 composio_autogen-0.3.3/composio_autogen/toolset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:20:45.716931 composio_autogen-0.3.3/composio_autogen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-05-31 15:20:45.000000 composio_autogen-0.3.3/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 15:20:45.000000 composio_autogen-0.3.3/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:20:45.000000 composio_autogen-0.3.3/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 15:20:45.000000 composio_autogen-0.3.3/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-31 15:20:45.000000 composio_autogen-0.3.3/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:20:45.720931 composio_autogen-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-05-31 15:20:29.000000 composio_autogen-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:40:03.066912 composio_autogen-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-06-01 00:40:03.066912 composio_autogen-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-06-01 00:39:46.000000 composio_autogen-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:40:03.062912 composio_autogen-0.3.4/composio_autogen/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-06-01 00:39:46.000000 composio_autogen-0.3.4/composio_autogen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6870 2024-06-01 00:39:46.000000 composio_autogen-0.3.4/composio_autogen/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:40:03.066912 composio_autogen-0.3.4/composio_autogen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3309 2024-06-01 00:40:03.000000 composio_autogen-0.3.4/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-01 00:40:03.000000 composio_autogen-0.3.4/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:40:03.000000 composio_autogen-0.3.4/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-01 00:40:03.000000 composio_autogen-0.3.4/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-01 00:40:03.000000 composio_autogen-0.3.4/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 00:40:03.066912 composio_autogen-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-06-01 00:39:46.000000 composio_autogen-0.3.4/setup.py
```

### Comparing `composio_autogen-0.3.3/PKG-INFO` & `composio_autogen-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.3.3
+Version: 0.3.4
 Summary: Use Composio to get an array of tools with your Autogen agent.
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
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.3.3/README.md` & `composio_autogen-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.3.3/composio_autogen/toolset.py` & `composio_autogen-0.3.4/composio_autogen/toolset.py`

 * *Files 3% similar despite different names*

```diff
@@ -138,15 +138,23 @@
     def _register_schema_to_autogen(
         self,
         schema: t.Dict,
         caller: ConversableAgent,
         executor: ConversableAgent,
         entity_id: t.Optional[str] = None,
     ) -> None:
-        """Register action schema to autogen registry."""
+        """
+        Register a schema to the Autogen registry.
+
+        Args:
+            schema (dict[str, any]): The action schema to be registered.
+            caller (ConversableAgent): The agent responsible for initiating the tool registration.
+            executor (ConversableAgent): The agent responsible for executing the registered tools.
+            entity_id (str, optional): The identifier of the entity for which the action is executed. Defaults to None.
+        """
         name = schema["name"]
         appName = schema["appName"]
         description = schema["description"]
 
         def execute_action(**kwargs: t.Any) -> t.Dict:
             """Placeholder function for executing action."""
             return self.execute_action(
```

### Comparing `composio_autogen-0.3.3/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.3.4/composio_autogen.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.3.3
+Version: 0.3.4
 Summary: Use Composio to get an array of tools with your Autogen agent.
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
 Requires-Dist: pyautogen>=0.2.19
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.3.3/setup.py` & `composio_autogen-0.3.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_autogen",
-    version="0.3.3",
+    version="0.3.4",
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
-    install_requires=["composio_core===0.3.3", "pyautogen>=0.2.19"],
+    install_requires=["composio_core===0.3.4", "pyautogen>=0.2.19"],
     include_package_data=True,
 )
```

