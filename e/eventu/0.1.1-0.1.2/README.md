# Comparing `tmp/eventu-0.1.1.tar.gz` & `tmp/eventu-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eventu-0.1.1.tar", max compression
+gzip compressed data, was "eventu-0.1.2.tar", max compression
```

## Comparing `eventu-0.1.1.tar` & `eventu-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0    13412 2024-06-01 12:02:29.672336 eventu-0.1.1/eventu/eventu.py
--rw-r--r--   0        0        0        0 2024-06-01 14:02:32.595614 eventu-0.1.1/eventu/py.typed
--rw-r--r--   0        0        0      531 2024-06-01 14:03:12.855685 eventu-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 eventu-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    13354 2024-06-01 14:13:36.273262 eventu-0.1.2/eventu/eventu.py
+-rw-r--r--   0        0        0        0 2024-06-01 14:02:32.595614 eventu-0.1.2/eventu/py.typed
+-rw-r--r--   0        0        0      524 2024-06-01 14:14:05.973351 eventu-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      514 1970-01-01 00:00:00.000000 eventu-0.1.2/PKG-INFO
```

### Comparing `eventu-0.1.1/eventu/eventu.py` & `eventu-0.1.2/eventu/eventu.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,42 +2,35 @@
 import logging
 import uuid
 from asyncio import CancelledError
 from collections import deque
 from contextlib import AbstractAsyncContextManager, asynccontextmanager, suppress
 from datetime import UTC, datetime, timedelta
 from enum import IntEnum
-from typing import Annotated, Any, AsyncIterator, Deque, Mapping, Protocol
+from typing import Any, AsyncIterator, Deque, Mapping, Protocol
 
 import pymongo.errors
 from aiokafka import AIOKafkaConsumer, AIOKafkaProducer
 from bson import Timestamp
 from motor.motor_asyncio import (
     AsyncIOMotorChangeStream,
     AsyncIOMotorClient,
     AsyncIOMotorClientSession,
     AsyncIOMotorDatabase,
 )
-from pydantic import BaseModel, ConfigDict, Field
-
+from pydantic import AwareDatetime, BaseModel, ConfigDict, Field
 
 __all__ = ["Event", "EventListener", "EventTransport", "EventHandler"]
 
 
 class Event(BaseModel):
     topic: str
     content_schema: str
-    idempotency_key: Annotated[
-        str,
-        Field(default_factory=lambda: uuid.uuid4().hex),
-    ]
-    occurred_at: Annotated[
-        datetime,
-        Field(default_factory=lambda: datetime.now(tz=UTC)),
-    ]
+    idempotency_key: str = Field(default_factory=lambda: uuid.uuid4().hex)
+    occurred_at: AwareDatetime = Field(default_factory=lambda: datetime.now(tz=UTC))
 
     model_config = ConfigDict(extra="allow")
 
 
 class EventListener:
     def __init__(self, events: Deque[Event]) -> None:
         self.__events = events
```

### Comparing `eventu-0.1.1/pyproject.toml` & `eventu-0.1.2/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 [tool.poetry]
 name = "eventu"
-version = "0.1.1"
+version = "0.1.2"
 description = "Transactional outbox and idempotent consumer"
 authors = ["Yuriy Kehter <yuriy.kehter@gmail.com>"]
-packages = [
-    { include = "eventu" },
-]
+packages = [{ include = "eventu" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiokafka = "^0.10.0"
 motor = "^3.4.0"
 pydantic = "^2.7.2"
```

### Comparing `eventu-0.1.1/PKG-INFO` & `eventu-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eventu
-Version: 0.1.1
+Version: 0.1.2
 Summary: Transactional outbox and idempotent consumer
 Author: Yuriy Kehter
 Author-email: yuriy.kehter@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

