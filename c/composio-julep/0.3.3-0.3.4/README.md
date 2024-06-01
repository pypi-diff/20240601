# Comparing `tmp/composio_julep-0.3.3.tar.gz` & `tmp/composio_julep-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_julep-0.3.3.tar", last modified: Fri May 31 15:24:50 2024, max compression
+gzip compressed data, was "composio_julep-0.3.4.tar", last modified: Sat Jun  1 00:44:01 2024, max compression
```

## Comparing `composio_julep-0.3.3.tar` & `composio_julep-0.3.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:24:50.128697 composio_julep-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-31 15:24:50.128697 composio_julep-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-31 15:24:07.000000 composio_julep-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:24:50.124696 composio_julep-0.3.3/composio_julep/
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-05-31 15:24:07.000000 composio_julep-0.3.3/composio_julep/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2100 2024-05-31 15:24:07.000000 composio_julep-0.3.3/composio_julep/toolset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 15:24:50.128697 composio_julep-0.3.3/composio_julep.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-05-31 15:24:50.000000 composio_julep-0.3.3/composio_julep.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-31 15:24:50.000000 composio_julep-0.3.3/composio_julep.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 15:24:50.000000 composio_julep-0.3.3/composio_julep.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-31 15:24:50.000000 composio_julep-0.3.3/composio_julep.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-31 15:24:50.000000 composio_julep-0.3.3/composio_julep.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 15:24:50.128697 composio_julep-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-05-31 15:24:07.000000 composio_julep-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:44:01.602262 composio_julep-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-06-01 00:44:01.602262 composio_julep-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-06-01 00:43:32.000000 composio_julep-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:44:01.602262 composio_julep-0.3.4/composio_julep/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-06-01 00:43:32.000000 composio_julep-0.3.4/composio_julep/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 2024-06-01 00:43:32.000000 composio_julep-0.3.4/composio_julep/toolset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:44:01.602262 composio_julep-0.3.4/composio_julep.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4461 2024-06-01 00:44:01.000000 composio_julep-0.3.4/composio_julep.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-06-01 00:44:01.000000 composio_julep-0.3.4/composio_julep.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:44:01.000000 composio_julep-0.3.4/composio_julep.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-06-01 00:44:01.000000 composio_julep-0.3.4/composio_julep.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-01 00:44:01.000000 composio_julep-0.3.4/composio_julep.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 00:44:01.602262 composio_julep-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-06-01 00:43:32.000000 composio_julep-0.3.4/setup.py
```

### Comparing `composio_julep-0.3.3/PKG-INFO` & `composio_julep-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.3.3
+Version: 0.3.4
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.3.3
+Requires-Dist: composio_openai===0.3.4
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_julep-0.3.3/README.md` & `composio_julep-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `composio_julep-0.3.3/composio_julep/toolset.py` & `composio_julep-0.3.4/composio_julep/toolset.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import json
 import typing as t
 
 from composio_openai import ComposioToolSet as BaseComposioToolSet
 from julep.api.types import ChatResponse
-
+from julep import Client
 from composio.client.enums import Action
 from composio.constants import DEFAULT_ENTITY_ID
 
 
 class ComposioToolSet(BaseComposioToolSet):
     """
     Composio toolset wrapper for Julep framework.
@@ -31,35 +31,50 @@
             base_url,
             entity_id=entity_id,
         )
         self.runtime = "julep"
 
     def handle_tool_calls(
         self,
+        julep_client: Client,
+        session_id: str,
         response: ChatResponse,
         entity_id: str = DEFAULT_ENTITY_ID,
-    ) -> t.List[t.Dict]:
+    ) -> ChatResponse:
         """
         Handle tool calls from Julep chat client object.
 
         :param response: Chat completion object from
                         julep.Client.sessions.chat function call
         :param entity_id: Entity ID to use for executing function calls.
         :return: A list of output objects from the function calls.
         """
         entity_id = self.validate_entity_id(entity_id or self.entity_id)
         outputs = []
-
-        for _responses in response.response:
-            for _response in _responses:
-                try:
-                    function = json.loads(_response.content)
-                    outputs.append(
-                        self.execute_action(
-                            action=Action.from_action(name=function["name"]),
-                            params=json.loads(function["arguments"]),
-                            entity_id=entity_id or self.entity_id,
+        while response.finish_reason == "tool_calls":
+            for _responses in response.response:
+                for _response in _responses:
+                    try:
+                        tool_function = json.loads(_response.content)
+                        outputs.append(
+                            self.execute_action(
+                                action=Action.from_action(name=tool_function["name"]),
+                                params=json.loads(tool_function["arguments"]),
+                                entity_id=entity_id or self.entity_id,
+                            )
                         )
-                    )
-                except json.JSONDecodeError:
-                    outputs.append(_response.content)
-        return outputs
+                    except json.JSONDecodeError:
+                        outputs.append(_response.content)
+
+            response = julep_client.sessions.chat(  # submit the tool call
+                session_id=session_id,
+                messages=[
+                    {
+                        "role": "assistant",
+                        "content": json.dumps(outputs),
+                    }
+                ],
+                recall=True,
+                remember=True,
+            )
+
+        return response
```

### Comparing `composio_julep-0.3.3/composio_julep.egg-info/PKG-INFO` & `composio_julep-0.3.4/composio_julep.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_julep
-Version: 0.3.3
+Version: 0.3.4
 Summary: Use Composio to get an array of tools with your Julep wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.3.3
+Requires-Dist: composio_openai===0.3.4
 Requires-Dist: julep>=0.3.2
 
 ## 🚀🔗 Integrating Composio with Julep
 
 Streamline the integration of Composio within the Julep agentic framework to enhance the interaction capabilities of Julep agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_julep-0.3.3/setup.py` & `composio_julep-0.3.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_julep",
-    version="0.3.3",
+    version="0.3.4",
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
-    install_requires=["composio_openai===0.3.3", "julep>=0.3.2"],
+    install_requires=["composio_openai===0.3.4", "julep>=0.3.2"],
     include_package_data=True,
 )
```

