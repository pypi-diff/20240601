# Comparing `tmp/pydantic_mongo_document-0.1.4.tar.gz` & `tmp/pydantic_mongo_document-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_mongo_document-0.1.4.tar", max compression
+gzip compressed data, was "pydantic_mongo_document-0.1.5.tar", max compression
```

## Comparing `pydantic_mongo_document-0.1.4.tar` & `pydantic_mongo_document-0.1.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1853 2023-09-09 11:50:57.498263 pydantic_mongo_document-0.1.4/README.md
--rw-r--r--   0        0        0      180 2023-09-09 16:04:31.623027 pydantic_mongo_document-0.1.4/pydantic_mongo_document/__init__.py
--rw-r--r--   0        0        0     5106 2023-09-09 11:25:48.572170 pydantic_mongo_document-0.1.4/pydantic_mongo_document/document.py
--rw-r--r--   0        0        0     1389 2023-09-09 11:24:34.317119 pydantic_mongo_document-0.1.4/pydantic_mongo_document/encoder.py
--rw-r--r--   0        0        0      168 2023-09-09 12:47:46.923823 pydantic_mongo_document-0.1.4/pydantic_mongo_document/exceptions.py
--rw-r--r--   0        0        0        0 2023-09-09 15:40:44.675287 pydantic_mongo_document-0.1.4/pydantic_mongo_document/py.typed
--rw-r--r--   0        0        0     1208 2023-09-09 16:05:12.305285 pydantic_mongo_document-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     2639 1970-01-01 00:00:00.000000 pydantic_mongo_document-0.1.4/setup.py
--rw-r--r--   0        0        0     2396 1970-01-01 00:00:00.000000 pydantic_mongo_document-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1853 2023-09-09 11:50:57.498263 pydantic_mongo_document-0.1.5/README.md
+-rw-r--r--   0        0        0      180 2023-09-09 16:04:31.623027 pydantic_mongo_document-0.1.5/pydantic_mongo_document/__init__.py
+-rw-r--r--   0        0        0     5225 2023-09-17 22:14:19.219673 pydantic_mongo_document-0.1.5/pydantic_mongo_document/document.py
+-rw-r--r--   0        0        0     1389 2023-09-09 11:24:34.317119 pydantic_mongo_document-0.1.5/pydantic_mongo_document/encoder.py
+-rw-r--r--   0        0        0      168 2023-09-09 12:47:46.923823 pydantic_mongo_document-0.1.5/pydantic_mongo_document/exceptions.py
+-rw-r--r--   0        0        0        0 2023-09-09 15:40:44.675287 pydantic_mongo_document-0.1.5/pydantic_mongo_document/py.typed
+-rw-r--r--   0        0        0     1208 2023-09-17 22:15:14.856548 pydantic_mongo_document-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2639 1970-01-01 00:00:00.000000 pydantic_mongo_document-0.1.5/setup.py
+-rw-r--r--   0        0        0     2396 1970-01-01 00:00:00.000000 pydantic_mongo_document-0.1.5/PKG-INFO
```

### Comparing `pydantic_mongo_document-0.1.4/README.md` & `pydantic_mongo_document-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_mongo_document-0.1.4/pydantic_mongo_document/document.py` & `pydantic_mongo_document-0.1.5/pydantic_mongo_document/document.py`

 * *Files 5% similar despite different names*

```diff
@@ -131,26 +131,30 @@
         query = cls.encoder.encode_dict(query, reveal_secrets=True)
 
         return await cls.collection().count_documents(query, **kwargs)
 
     async def delete(self) -> pymongo.results.DeleteResult:
         """Deletes document from collection."""
 
-        return await self.collection().delete_one({self.primary_key_field_name: self.primary_key})
+        query = self.encoder.encode_dict(
+            {self.primary_key_field_name: self.primary_key},
+        )
+
+        return await self.collection().delete_one(query)
 
     async def commit_changes(self, fields: Optional[List[str]] = None) -> None:
         """Saves changed document to collection."""
 
         search_query: dict[str, Any] = {self.primary_key_field_name: self.primary_key}
         update_query: dict[str, Any] = {"$set": {}}
 
         if not fields:
             fields = [field for field in self.model_fields.keys() if field != self.__primary_key__]
 
-        data = self.model_dump()
+        data = self.encoder.encode_dict(self.model_dump(), reveal_secrets=True)
 
         for field in fields:
             update_query["$set"].update({field: data[field]})
 
         await self.collection().update_one(search_query, update_query)
 
     async def insert(self) -> Self:
```

### Comparing `pydantic_mongo_document-0.1.4/pydantic_mongo_document/encoder.py` & `pydantic_mongo_document-0.1.5/pydantic_mongo_document/encoder.py`

 * *Files identical despite different names*

### Comparing `pydantic_mongo_document-0.1.4/pyproject.toml` & `pydantic_mongo_document-0.1.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-mongo-document"
-version = "0.1.4"
+version = "0.1.5"
 description = "Pydantic Async Mongo Document"
 authors = ["Yurzs <yurzs@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pydantic_mongo_document"}]
 include = ["pydantic_mongo_document/py.typed"]
```

### Comparing `pydantic_mongo_document-0.1.4/setup.py` & `pydantic_mongo_document-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['autoflake>=2.2.1,<3.0.0',
  'motor>=3.3.1,<4.0.0',
  'mypy>=1.5.1,<2.0.0',
  'pydantic>=2.3.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'pydantic-mongo-document',
-    'version': '0.1.4',
+    'version': '0.1.5',
     'description': 'Pydantic Async Mongo Document',
     'long_description': '# Pydantic Mongo Document\n\n`pydantic_mongo_document` is a Python library that provides a base class for creating MongoDB documents using Pydantic models.\n\n## Installation\n\nInstall the package using [pip](https://pip.pypa.io/en/stable/) or [poetry](https://python-poetry.org).\n\n### Using pip\n```bash\npip install pydantic_mongo_document\n```\n\n### Using poetry\n```bash\npoetry add pydantic_mongo_document\n```\n\nUsage\nTo use pydantic_mongo_document, you need to create a Pydantic model that represents your MongoDB document and inherit from the MongoDocument class provided by the library. Here\'s an example:\n\n```python3\nfrom pydantic_mongo_document import Document\n\nclass User(Document):\n    __collection__ = "users"\n    __database__ = "production"\n\n    name: str\n    email: str\n\n```\n\nIn this example, we define a User Pydantic Document model with two fields (name and email) and  \nspecifies the MongoDB collection name (users) and database name (production) using the `__collection__` and `__database__` class attributes.\n\n```python3\nfrom pydantic_mongo_document import Document\n\n# Set the MongoDB URI\nDocument.set_mongo_uri("mongodb://localhost:27017")\n\n\nclass User(Document):\n    __collection__ = "users"\n    __database__ = "production"\n\n    name: str\n    email: str\n\n\nasync def create_user():\n    user = User(name="John", email="john@example.com")\n\n    await user.insert()\n\n    user = await User.one(add_query={"name": "John"})\n    print(user) # User(id=ObjectId("64fc59cf6410868c9a40644b"), name="John", email="john@example")\n```\n\nIn this example, we created new User in database. We then used the `User.one` method to retrieve the user from the database.\n\n## Contributing\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nPlease make sure to update tests as appropriate.\n\n## License\nMIT\n',
     'author': 'Yurzs',
     'author_email': 'yurzs@icloud.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pydantic_mongo_document-0.1.4/PKG-INFO` & `pydantic_mongo_document-0.1.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-mongo-document
-Version: 0.1.4
+Version: 0.1.5
 Summary: Pydantic Async Mongo Document
 License: MIT
 Author: Yurzs
 Author-email: yurzs@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

