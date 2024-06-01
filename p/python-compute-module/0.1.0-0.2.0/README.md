# Comparing `tmp/python_compute_module-0.1.0.tar.gz` & `tmp/python_compute_module-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_compute_module-0.1.0.tar", max compression
+gzip compressed data, was "python_compute_module-0.2.0.tar", max compression
```

## Comparing `python_compute_module-0.1.0.tar` & `python_compute_module-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      570 2024-06-01 10:47:16.440169 python_compute_module-0.1.0/README.md
--rw-r--r--   0        0        0      401 2024-06-01 10:14:08.816272 python_compute_module-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-06-01 09:18:51.290799 python_compute_module-0.1.0/python_compute_module/__init__.py
--rw-r--r--   0        0        0     2110 2024-06-01 10:12:04.072553 python_compute_module-0.1.0/python_compute_module/api.py
--rw-r--r--   0        0        0      344 2024-06-01 10:44:33.049375 python_compute_module-0.1.0/python_compute_module/app.py
--rw-r--r--   0        0        0     2938 2024-06-01 10:12:10.483832 python_compute_module-0.1.0/python_compute_module/query_runner.py
--rw-r--r--   0        0        0     1319 2024-06-01 10:15:28.831147 python_compute_module-0.1.0/python_compute_module/read_connection_file.py
--rw-r--r--   0        0        0     1831 2024-06-01 09:21:54.468863 python_compute_module-0.1.0/python_compute_module/schema.py
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 python_compute_module-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      570 2024-06-01 10:47:16.440169 python_compute_module-0.2.0/README.md
+-rw-r--r--   0        0        0      401 2024-06-01 12:06:31.501461 python_compute_module-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-01 09:18:51.290799 python_compute_module-0.2.0/python_compute_module/__init__.py
+-rw-r--r--   0        0        0     2122 2024-06-01 12:04:38.520018 python_compute_module-0.2.0/python_compute_module/api.py
+-rw-r--r--   0        0        0      314 2024-06-01 12:03:20.615460 python_compute_module-0.2.0/python_compute_module/app.py
+-rw-r--r--   0        0        0     2888 2024-06-01 12:05:06.854850 python_compute_module-0.2.0/python_compute_module/query_runner.py
+-rw-r--r--   0        0        0     1257 2024-06-01 12:05:33.264052 python_compute_module-0.2.0/python_compute_module/read_connection_file.py
+-rw-r--r--   0        0        0     1825 2024-06-01 12:05:50.552399 python_compute_module-0.2.0/python_compute_module/schema.py
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 python_compute_module-0.2.0/PKG-INFO
```

### Comparing `python_compute_module-0.1.0/README.md` & `python_compute_module-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python_compute_module-0.1.0/python_compute_module/api.py` & `python_compute_module-0.2.0/python_compute_module/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import json
 import logging
 from typing import Any, List, Optional
 
 import httpx
-from python_compute_module.schema import Schema
 from pydantic import BaseModel
 
+from python_compute_module.schema import Schema
+
 log = logging.getLogger(__name__)
 
 CONNECT_TIMEOUT_SECONDS = 60
 READ_TIMEOUT_SECONDS = 60
 
 
 class ConnectionInformation(BaseModel):
@@ -44,24 +45,24 @@
 
     async def get_job_request(self) -> Optional[JobRequest]:
         response = await self.client.get(self.connection_information.getJobPath)
         log.debug(f"received job request response {response.status_code}")
         if response.status_code == 204:
             return None
         else:
-            return JobRequest.parse_obj(response.json())
+            return JobRequest.model_validate(response.json())
 
     async def post_result(self, job_id: str, response: Any) -> httpx.Response:
         log.debug(f"posting result: {response}")
         return await self.client.post(
             f"{self.connection_information.postResultPath}/{job_id}",
             content=json.dumps(response),
             headers={
                 "Content-Type": "application/octet-stream",
             },
         )
 
     async def post_schema(self, schemas: List[Schema]) -> httpx.Response:
         return await self.client.post(
             f"{self.connection_information.basePath}/schemas",
-            json=[schema.dict() for schema in schemas],
+            json=[schema.model_dump() for schema in schemas],
         )
```

### Comparing `python_compute_module-0.1.0/python_compute_module/query_runner.py` & `python_compute_module-0.2.0/python_compute_module/query_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,14 @@
             raise ValueError(
                 "Connection path not found in environment variables, please set CONNECTION_TO_RUNTIME to the path of the connection file."
             )
         asyncio.run(self.initialize(connection_path, schemas))
 
     async def initialize(self, connection_path: str, schemas: List[Schema]):
         self.connection_information = await read_connection_file(connection_path)
-        log.info("Connection information loaded")
         self.compute_module_api = ComputeModuleApi(self.connection_information)
         await self.compute_module_api.post_schema(schemas)
         await self.run()
 
     async def run(self):
         while True:
             try:
```

### Comparing `python_compute_module-0.1.0/python_compute_module/read_connection_file.py` & `python_compute_module-0.2.0/python_compute_module/read_connection_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-import aiofiles
 import asyncio
 import logging
 
+import aiofiles
+
 from python_compute_module.api import ConnectionInformation
 
 log = logging.getLogger(__name__)
 READ_POLL_DELAY_SECONDS = 0.5
 MAX_READ_ATTEMPTS = 100
 
 
 async def read_connection_file(path: str) -> ConnectionInformation:
-    log.info(
+    log.debug(
         f"Attempting reading connection file from {path} [Poll interval {READ_POLL_DELAY_SECONDS}s]"
     )
     start_time = asyncio.get_event_loop().time()
     attempt_count = 0
 
     while attempt_count < MAX_READ_ATTEMPTS:
         try:
             async with aiofiles.open(path, "r") as f:
                 blob = await f.read()
-            log.info(
+            log.debug(
                 f"Successfully read connection file from {path} after {(asyncio.get_event_loop().time() - start_time):.2f}s"
             )
-            log.info(f"connection file blob looks like: {blob}")
             return ConnectionInformation.parse_raw(blob)
         except Exception as e:
             log.error(f"Error reading connection file: {e}")
             # The file can take a while to appear, so we retry a few times
             # logger.error(f"Error reading connection file: {e}")
             await asyncio.sleep(READ_POLL_DELAY_SECONDS)
             attempt_count += 1
```

### Comparing `python_compute_module-0.1.0/python_compute_module/schema.py` & `python_compute_module-0.2.0/python_compute_module/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 
 class ComplexType(BaseModel):
     type: str = "complexType"
     complexType: Union[StructType, ListType]
 
 
-Entry.update_forward_refs()  # Update DataType in Entry
+Entry.model_rebuild()  # Update DataType in Entry
 
 
 class Schema(BaseModel):
     name: str
     inputType: StructType
     outputType: Union[PrimitiveType, ComplexType, UnknownType]  # DataType
```

### Comparing `python_compute_module-0.1.0/PKG-INFO` & `python_compute_module-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-compute-module
-Version: 0.1.0
+Version: 0.2.0
 Summary: 
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiofiles (>=23.2.1,<24.0.0)
```

