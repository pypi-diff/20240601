# Comparing `tmp/liminal_sdk_python-2024.5.0b3.tar.gz` & `tmp/liminal_sdk_python-2024.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "liminal_sdk_python-2024.5.0b3.tar", max compression
+gzip compressed data, was "liminal_sdk_python-2024.5.1.tar", max compression
```

## Comparing `liminal_sdk_python-2024.5.0b3.tar` & `liminal_sdk_python-2024.5.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    11357 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/LICENSE
--rw-r--r--   0        0        0    12308 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/README.md
--rw-r--r--   0        0        0       82 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/liminal/__init__.py
--rw-r--r--   0        0        0      524 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/liminal/auth/__init__.py
--rw-r--r--   0        0        0       34 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/liminal/auth/microsoft/__init__.py
--rw-r--r--   0        0        0     2961 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/liminal/auth/microsoft/device_code_flow.py
--rw-r--r--   0        0        0      849 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/liminal/auth/microsoft/models.py
--rw-r--r--   0        0        0    10159 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/liminal/client.py
--rw-r--r--   0        0        0      165 2024-05-28 19:57:59.184160 liminal_sdk_python-2024.5.0b3/liminal/const.py
--rw-r--r--   0        0        0       45 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/__init__.py
--rw-r--r--   0        0        0     2275 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/llm/__init__.py
--rw-r--r--   0        0        0     2064 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/llm/models.py
--rw-r--r--   0        0        0      437 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/llm/schemas.py
--rw-r--r--   0        0        0     7957 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/prompt/__init__.py
--rw-r--r--   0        0        0     3597 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/prompt/models.py
--rw-r--r--   0        0        0      960 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/prompt/schemas.py
--rw-r--r--   0        0        0     2563 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/thread/__init__.py
--rw-r--r--   0        0        0     2130 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/thread/models.py
--rw-r--r--   0        0        0      733 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/endpoints/thread/schemas.py
--rw-r--r--   0        0        0      400 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/errors.py
--rw-r--r--   0        0        0       22 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/helpers/__init__.py
--rw-r--r--   0        0        0      374 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/helpers/model.py
--rw-r--r--   0        0        0      394 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/helpers/schema.py
--rw-r--r--   0        0        0      109 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/liminal/helpers/typing.py
--rw-r--r--   0        0        0    13892 2024-05-28 19:57:59.188160 liminal_sdk_python-2024.5.0b3/pyproject.toml
--rw-r--r--   0        0        0    13432 1970-01-01 00:00:00.000000 liminal_sdk_python-2024.5.0b3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/LICENSE
+-rw-r--r--   0        0        0    12308 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/README.md
+-rw-r--r--   0        0        0       82 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/__init__.py
+-rw-r--r--   0        0        0      524 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/auth/__init__.py
+-rw-r--r--   0        0        0       34 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/auth/microsoft/__init__.py
+-rw-r--r--   0        0        0     2961 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/auth/microsoft/device_code_flow.py
+-rw-r--r--   0        0        0      849 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/auth/microsoft/models.py
+-rw-r--r--   0        0        0    10232 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/client.py
+-rw-r--r--   0        0        0      165 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/const.py
+-rw-r--r--   0        0        0       45 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/endpoints/__init__.py
+-rw-r--r--   0        0        0     2275 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/endpoints/llm/__init__.py
+-rw-r--r--   0        0        0     2136 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/endpoints/llm/models.py
+-rw-r--r--   0        0        0      437 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/endpoints/llm/schemas.py
+-rw-r--r--   0        0        0     8196 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/endpoints/prompt/__init__.py
+-rw-r--r--   0        0        0     3583 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/endpoints/prompt/models.py
+-rw-r--r--   0        0        0      960 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/endpoints/prompt/schemas.py
+-rw-r--r--   0        0        0     2563 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/endpoints/thread/__init__.py
+-rw-r--r--   0        0        0     2130 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/endpoints/thread/models.py
+-rw-r--r--   0        0        0      733 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/endpoints/thread/schemas.py
+-rw-r--r--   0        0        0      400 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/errors.py
+-rw-r--r--   0        0        0       22 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/helpers/__init__.py
+-rw-r--r--   0        0        0      374 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/helpers/model.py
+-rw-r--r--   0        0        0      394 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/helpers/schema.py
+-rw-r--r--   0        0        0      109 2024-06-01 02:21:18.509390 liminal_sdk_python-2024.5.1/liminal/helpers/typing.py
+-rw-r--r--   0        0        0     8703 2024-06-01 02:21:18.513390 liminal_sdk_python-2024.5.1/pyproject.toml
+-rw-r--r--   0        0        0    13430 1970-01-01 00:00:00.000000 liminal_sdk_python-2024.5.1/PKG-INFO
```

### Comparing `liminal_sdk_python-2024.5.0b3/LICENSE` & `liminal_sdk_python-2024.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b3/README.md` & `liminal_sdk_python-2024.5.1/README.md`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b3/liminal/auth/__init__.py` & `liminal_sdk_python-2024.5.1/liminal/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b3/liminal/auth/microsoft/device_code_flow.py` & `liminal_sdk_python-2024.5.1/liminal/auth/microsoft/device_code_flow.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b3/liminal/auth/microsoft/models.py` & `liminal_sdk_python-2024.5.1/liminal/auth/microsoft/models.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b3/liminal/client.py` & `liminal_sdk_python-2024.5.1/liminal/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         method: str,
         endpoint: str,
         *,
         headers: dict[str, str] | None = None,
         cookies: dict[str, str] | None = None,
         params: dict[str, str] | None = None,
         json: dict[str, Any] | None = None,
-    ) -> AsyncIterator[bytes]:
+    ) -> AsyncIterator[str]:
         """Make a request to the Liminal API server and return a streaming response.
 
         Args:
         ----
             method: The HTTP method to use.
             endpoint: The endpoint to request.
             headers: The headers to use.
@@ -251,16 +251,17 @@
             method,
             url,
             headers=headers,
             cookies=cookie_jar,
             params=params,
             json=json,
         ) as resp:
-            async for chunk in resp.aiter_bytes():
-                yield chunk
+            async for line in resp.aiter_lines():
+                LOGGER.info("Received line of streaming response: %s", line)
+                yield line
 
     def add_session_id_callback(
         self, callback: Callable[[str], None]
     ) -> Callable[[], None]:
         """Add a callback to be called when a new session is generated.
 
         The purpose of this is to allow the user to save the session ID to a
```

### Comparing `liminal_sdk_python-2024.5.0b3/liminal/endpoints/llm/__init__.py` & `liminal_sdk_python-2024.5.1/liminal/endpoints/llm/__init__.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b3/liminal/endpoints/llm/models.py` & `liminal_sdk_python-2024.5.1/liminal/endpoints/llm/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,20 @@
     """Define the enum for the model provider key."""
 
     ANTHROPIC = "anthropic"
     AWS_BEDROCK = "aws_bedrock"
     AWS_SAGEMAKER = "aws_sagemaker"
     AZURE_OPENAI = "azure_openai"
     COHERE = "cohere"
+    GOOGLE_VERTEX_AI = "google_vertex_ai"
     HUGGINGFACE = "huggingface"
     MISTRAL = "mistral"
     OLLAMA = "ollama"
     OPENAI = "openai"
+    PERPLEXITY = "perplexity"
 
 
 @dataclass(frozen=True, kw_only=True)
 class ModelConnection(BaseModel):
     """Define the model for an LLM model connection."""
 
     id: int
```

### Comparing `liminal_sdk_python-2024.5.0b3/liminal/endpoints/prompt/__init__.py` & `liminal_sdk_python-2024.5.1/liminal/endpoints/prompt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Define the prompts endpoint."""
 
 from __future__ import annotations
 
 from collections.abc import AsyncIterator, Awaitable, Callable
+import json
 from typing import Any, cast
 
 from mashumaro.codecs.json import json_decode
 
-from liminal.const import SOURCE
+from liminal.const import LOGGER, SOURCE
 from liminal.endpoints.prompt.models import (
     AnalysisFindings,
     CleanseData,
     HydrateData,
     StreamResponseChunk,
     SubmitData,
 )
@@ -26,15 +27,15 @@
 
 class PromptEndpoint:
     """Define the prompts endpoint."""
 
     def __init__(
         self,
         request_and_validate: Callable[..., Awaitable[ValidatedResponseT]],
-        stream: Callable[..., AsyncIterator[bytes]],
+        stream: Callable[..., AsyncIterator[str]],
     ) -> None:
         """Initialize.
 
         Args:
         ----
             request_and_validate: The request and validate function.
             stream: The stream function.
@@ -209,15 +210,19 @@
 
         """
         payload = self._generate_payload_for_request(
             model_instance_id, prompt, thread_id=thread_id, findings=findings
         )
         payload["isStreaming"] = True
         async for chunk in self._stream("POST", "/api/v1/prompts/submit", json=payload):
-            yield json_decode(chunk.decode(), StreamResponseChunk)
+            try:
+                yield json_decode(chunk, StreamResponseChunk)
+            except json.decoder.JSONDecodeError:
+                LOGGER.warning("Stream returned incomplete JSON chunk: %s", chunk)
+                yield StreamResponseChunk(content=chunk, finish_reason=None)
 
     async def submit(
         self,
         model_instance_id: int,
         prompt: str,
         *,
         thread_id: int | None = None,
```

### Comparing `liminal_sdk_python-2024.5.0b3/liminal/endpoints/prompt/models.py` & `liminal_sdk_python-2024.5.1/liminal/endpoints/prompt/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -79,15 +79,14 @@
 @dataclass(frozen=True, kw_only=True)
 class ReidentifiedToken(BaseModel):
     """Define a reidentified token."""
 
     start: int
     end: int
     entity_type: str = field(metadata=field_options(alias="entityType"))
-    text: str
 
 
 @dataclass(frozen=True, kw_only=True)
 class StreamResponseChunk(BaseModel):
     """Define a streaming response chunk."""
 
     content: str
```

### Comparing `liminal_sdk_python-2024.5.0b3/liminal/endpoints/prompt/schemas.py` & `liminal_sdk_python-2024.5.1/liminal/endpoints/prompt/schemas.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b3/liminal/endpoints/thread/__init__.py` & `liminal_sdk_python-2024.5.1/liminal/endpoints/thread/__init__.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b3/liminal/endpoints/thread/models.py` & `liminal_sdk_python-2024.5.1/liminal/endpoints/thread/models.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b3/liminal/endpoints/thread/schemas.py` & `liminal_sdk_python-2024.5.1/liminal/endpoints/thread/schemas.py`

 * *Files identical despite different names*

### Comparing `liminal_sdk_python-2024.5.0b3/PKG-INFO` & `liminal_sdk_python-2024.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liminal-sdk-python
-Version: 2024.5.0b3
+Version: 2024.5.1
 Summary: The Liminal SDK for Python
 Home-page: https://github.com/liminal-ai-security/liminal-sdk-python
 License: Apache-2.0
 Author: Aaron Bach
 Author-email: ab@liminal.ai
 Requires-Python: >=3.11.8,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
```

