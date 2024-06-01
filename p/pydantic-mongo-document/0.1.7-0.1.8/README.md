# Comparing `tmp/pydantic_mongo_document-0.1.7.tar.gz` & `tmp/pydantic_mongo_document-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_mongo_document-0.1.7.tar", max compression
+gzip compressed data, was "pydantic_mongo_document-0.1.8.tar", max compression
```

## Comparing `pydantic_mongo_document-0.1.7.tar` & `pydantic_mongo_document-0.1.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1067 2023-09-09 10:05:32.636929 pydantic_mongo_document-0.1.7/LICENCE
--rw-r--r--   0        0        0     1923 2024-06-01 15:47:05.144544 pydantic_mongo_document-0.1.7/README.md
--rw-r--r--   0        0        0      180 2023-09-09 16:04:31.623027 pydantic_mongo_document-0.1.7/pydantic_mongo_document/__init__.py
--rw-r--r--   0        0        0     5751 2024-06-01 15:45:50.608366 pydantic_mongo_document-0.1.7/pydantic_mongo_document/document.py
--rw-r--r--   0        0        0     1389 2023-09-09 11:24:34.317119 pydantic_mongo_document-0.1.7/pydantic_mongo_document/encoder.py
--rw-r--r--   0        0        0      168 2023-09-09 12:47:46.923823 pydantic_mongo_document-0.1.7/pydantic_mongo_document/exceptions.py
--rw-r--r--   0        0        0        0 2023-09-09 15:40:44.675287 pydantic_mongo_document-0.1.7/pydantic_mongo_document/py.typed
--rw-r--r--   0        0        0     1208 2024-06-01 15:50:43.461476 pydantic_mongo_document-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 pydantic_mongo_document-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-09-09 10:05:32.636929 pydantic_mongo_document-0.1.8/LICENCE
+-rw-r--r--   0        0        0     1923 2024-06-01 15:47:05.144544 pydantic_mongo_document-0.1.8/README.md
+-rw-r--r--   0        0        0      179 2024-06-01 18:07:33.989674 pydantic_mongo_document-0.1.8/pydantic_mongo_document/__init__.py
+-rw-r--r--   0        0        0     6387 2024-06-01 18:20:21.230898 pydantic_mongo_document-0.1.8/pydantic_mongo_document/document.py
+-rw-r--r--   0        0        0     1389 2023-09-09 11:24:34.317119 pydantic_mongo_document-0.1.8/pydantic_mongo_document/encoder.py
+-rw-r--r--   0        0        0      168 2023-09-09 12:47:46.923823 pydantic_mongo_document-0.1.8/pydantic_mongo_document/exceptions.py
+-rw-r--r--   0        0        0        0 2023-09-09 15:40:44.675287 pydantic_mongo_document-0.1.8/pydantic_mongo_document/py.typed
+-rw-r--r--   0        0        0     1208 2024-06-01 18:21:21.365043 pydantic_mongo_document-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2517 1970-01-01 00:00:00.000000 pydantic_mongo_document-0.1.8/PKG-INFO
```

### Comparing `pydantic_mongo_document-0.1.7/LICENCE` & `pydantic_mongo_document-0.1.8/LICENCE`

 * *Files identical despite different names*

### Comparing `pydantic_mongo_document-0.1.7/README.md` & `pydantic_mongo_document-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_mongo_document-0.1.7/pydantic_mongo_document/document.py` & `pydantic_mongo_document-0.1.8/pydantic_mongo_document/document.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,40 @@
-from typing import Any, ClassVar, List, Optional, Self, Type
+from typing import Annotated, Any, ClassVar, List, Optional, Self, Type
 
 import bson
 import pymongo
 import pymongo.errors
 import pymongo.results
 from motor.motor_asyncio import AsyncIOMotorClient, AsyncIOMotorCollection, AsyncIOMotorDatabase
-from pydantic import BaseModel, Field
+from pydantic import AnyUrl, BaseModel, Field, UrlConstraints, validate_call
 from pymongo.collection import Collection
 from pymongo.database import Database
 
 from pydantic_mongo_document.encoder import JsonEncoder
 from pydantic_mongo_document.exceptions import DocumentNotFound
 
 
+class ReplicaConfig(BaseModel):
+    """Mongodb replica config model."""
+
+    uri: Annotated[
+        AnyUrl,
+        UrlConstraints(allowed_schemes=["mongodb", "mongodb+srv"]),
+        Field(..., description="Mongodb connection URI."),
+    ]
+    client_options: dict[str, Any] = Field(
+        default_factory=dict,
+        description="Mongodb client options.",
+    )
+
+
 class Document(BaseModel):
     __primary_key__: ClassVar[str] = "id"
 
-    __config__: ClassVar[dict[str, str]] = {}
+    __config__: ClassVar[dict[str, ReplicaConfig]] = {}
     """Map of replicas to mongo URIs."""
 
     __replica__: ClassVar[str]
     """Mongodb replica name."""
 
     __database__: ClassVar[str]
     """Mongodb database name."""
@@ -38,34 +52,40 @@
 
     id: str = Field(default_factory=lambda: str(bson.ObjectId()), alias="_id")
 
     @property
     def primary_key(self) -> Any:
         return getattr(self, self.__primary_key__)
 
+    @classmethod
+    def get_replica_config(cls) -> ReplicaConfig:
+        return cls.__config__[cls.__replica__]
+
     @property
     def primary_key_field_name(self) -> str:
         return self.model_fields[self.__primary_key__].alias or self.__primary_key__
 
     @classmethod
-    def set_replica_config(cls, config: dict[str, str]) -> None:
+    @validate_call
+    def set_replica_config(cls, config: dict[str, ReplicaConfig]) -> None:
         cls.__config__ = config
 
     @classmethod
     def client(cls) -> AsyncIOMotorClient:
         if cls.__replica__ not in cls.__clients__:
-            mongo_uri = cls.__config__[cls.__replica__]
-            cls.__clients__[cls.__replica__] = AsyncIOMotorClient(mongo_uri)
+            cls.__clients__[cls.__replica__] = AsyncIOMotorClient(
+                host=str(cls.get_replica_config().uri),
+                **cls.get_replica_config().client_options,
+            )
 
         return cls.__clients__[cls.__replica__]
 
     @classmethod
     def sync_client(cls) -> pymongo.MongoClient[Any]:
-        mongo_uri = cls.__config__[cls.__replica__]
-        return pymongo.MongoClient(mongo_uri)
+        return pymongo.MongoClient(str(cls.get_replica_config().uri))
 
     @classmethod
     def database(cls) -> AsyncIOMotorDatabase:
         return cls.client()[cls.__database__]
 
     @classmethod
     def sync_database(cls) -> Database[Any]:
@@ -100,15 +120,15 @@
             query.update(add_query)
 
         query = cls.encoder.encode_dict(query, reveal_secrets=True)
 
         result = await cls.collection().find_one(query, **kwargs)
 
         if result is not None:
-            return cls(**result)
+            return cls.model_validate(result)
 
         if required:
             raise cls.NotFoundError()
 
         return None
 
     @classmethod
@@ -128,15 +148,15 @@
 
         documents = []
 
         query = cls.encoder.encode_dict(query, reveal_secrets=True)
 
         cursor = cls.collection().find(query, **kwargs)
         async for document in cursor:
-            documents.append(cls(**document))
+            documents.append(cls.model_validate(document))
 
         return documents
 
     @classmethod
     async def count(cls, add_query: Optional[dict[str, Any]] = None, **kwargs: Any) -> int:
         """Counts documents in collection."""
```

### Comparing `pydantic_mongo_document-0.1.7/pydantic_mongo_document/encoder.py` & `pydantic_mongo_document-0.1.8/pydantic_mongo_document/encoder.py`

 * *Files identical despite different names*

### Comparing `pydantic_mongo_document-0.1.7/pyproject.toml` & `pydantic_mongo_document-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-mongo-document"
-version = "0.1.7"
+version = "0.1.8"
 description = "Pydantic Async Mongo Document"
 authors = ["Yurzs <yurzs@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pydantic_mongo_document"}]
 include = ["pydantic_mongo_document/py.typed"]
```

### Comparing `pydantic_mongo_document-0.1.7/PKG-INFO` & `pydantic_mongo_document-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-mongo-document
-Version: 0.1.7
+Version: 0.1.8
 Summary: Pydantic Async Mongo Document
 License: MIT
 Author: Yurzs
 Author-email: yurzs@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

