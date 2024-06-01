# Comparing `tmp/pydantic_mongo_document-0.1.5.tar.gz` & `tmp/pydantic_mongo_document-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_mongo_document-0.1.5.tar", max compression
+gzip compressed data, was "pydantic_mongo_document-0.1.6.tar", max compression
```

## Comparing `pydantic_mongo_document-0.1.5.tar` & `pydantic_mongo_document-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1853 2023-09-09 11:50:57.498263 pydantic_mongo_document-0.1.5/README.md
--rw-r--r--   0        0        0      180 2023-09-09 16:04:31.623027 pydantic_mongo_document-0.1.5/pydantic_mongo_document/__init__.py
--rw-r--r--   0        0        0     5225 2023-09-17 22:14:19.219673 pydantic_mongo_document-0.1.5/pydantic_mongo_document/document.py
--rw-r--r--   0        0        0     1389 2023-09-09 11:24:34.317119 pydantic_mongo_document-0.1.5/pydantic_mongo_document/encoder.py
--rw-r--r--   0        0        0      168 2023-09-09 12:47:46.923823 pydantic_mongo_document-0.1.5/pydantic_mongo_document/exceptions.py
--rw-r--r--   0        0        0        0 2023-09-09 15:40:44.675287 pydantic_mongo_document-0.1.5/pydantic_mongo_document/py.typed
--rw-r--r--   0        0        0     1208 2023-09-17 22:15:14.856548 pydantic_mongo_document-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     2639 1970-01-01 00:00:00.000000 pydantic_mongo_document-0.1.5/setup.py
--rw-r--r--   0        0        0     2396 1970-01-01 00:00:00.000000 pydantic_mongo_document-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-09-09 10:05:32.636929 pydantic_mongo_document-0.1.6/LICENCE
+-rw-r--r--   0        0        0     1853 2023-09-09 11:50:57.498263 pydantic_mongo_document-0.1.6/README.md
+-rw-r--r--   0        0        0      180 2023-09-09 16:04:31.623027 pydantic_mongo_document-0.1.6/pydantic_mongo_document/__init__.py
+-rw-r--r--   0        0        0     5558 2024-06-01 15:32:19.169629 pydantic_mongo_document-0.1.6/pydantic_mongo_document/document.py
+-rw-r--r--   0        0        0     1389 2023-09-09 11:24:34.317119 pydantic_mongo_document-0.1.6/pydantic_mongo_document/encoder.py
+-rw-r--r--   0        0        0      168 2023-09-09 12:47:46.923823 pydantic_mongo_document-0.1.6/pydantic_mongo_document/exceptions.py
+-rw-r--r--   0        0        0        0 2023-09-09 15:40:44.675287 pydantic_mongo_document-0.1.6/pydantic_mongo_document/py.typed
+-rw-r--r--   0        0        0     1208 2024-06-01 15:32:50.775760 pydantic_mongo_document-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     2447 1970-01-01 00:00:00.000000 pydantic_mongo_document-0.1.6/PKG-INFO
```

### Comparing `pydantic_mongo_document-0.1.5/README.md` & `pydantic_mongo_document-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_mongo_document-0.1.5/pydantic_mongo_document/document.py` & `pydantic_mongo_document-0.1.6/pydantic_mongo_document/document.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,17 @@
 class Document(BaseModel):
     __primary_key__: ClassVar[str] = "id"
 
     __database__: ClassVar[str]
     __collection__: ClassVar[str]
     __mongo_uri__: ClassVar[str]
 
+    __clients__: ClassVar[dict[str, AsyncIOMotorClient]] = {}
+    """Map of clients for each database."""
+
     NotFoundError: ClassVar[Type[Exception]] = DocumentNotFound
     DuplicateKeyError: ClassVar[Type[Exception]] = pymongo.errors.DuplicateKeyError
 
     encoder: ClassVar[JsonEncoder] = JsonEncoder()
 
     id: str = Field(default_factory=lambda: str(bson.ObjectId()), alias="_id")
 
@@ -37,15 +40,21 @@
 
     @classmethod
     def set_mongo_uri(cls, mongo_uri: str) -> None:
         cls.__mongo_uri__ = mongo_uri
 
     @classmethod
     def client(cls) -> AsyncIOMotorClient:
-        return AsyncIOMotorClient(cls.__mongo_uri__)
+        if (
+            cls.__mongo_uri__ not in cls.__clients__
+            or not cls.__clients__[cls.__mongo_uri__].connected
+        ):
+            cls.__clients__[cls.__mongo_uri__] = AsyncIOMotorClient(cls.__mongo_uri__)
+
+        return cls.__clients__[cls.__mongo_uri__]
 
     @classmethod
     def sync_client(cls) -> pymongo.MongoClient[Any]:
         return pymongo.MongoClient(cls.__mongo_uri__)
 
     @classmethod
     def database(cls) -> AsyncIOMotorDatabase:
```

### Comparing `pydantic_mongo_document-0.1.5/pydantic_mongo_document/encoder.py` & `pydantic_mongo_document-0.1.6/pydantic_mongo_document/encoder.py`

 * *Files identical despite different names*

### Comparing `pydantic_mongo_document-0.1.5/pyproject.toml` & `pydantic_mongo_document-0.1.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-mongo-document"
-version = "0.1.5"
+version = "0.1.6"
 description = "Pydantic Async Mongo Document"
 authors = ["Yurzs <yurzs@icloud.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pydantic_mongo_document"}]
 include = ["pydantic_mongo_document/py.typed"]
```

### Comparing `pydantic_mongo_document-0.1.5/setup.py` & `pydantic_mongo_document-0.1.6/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,88 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pydantic-mongo-document
+Version: 0.1.6
+Summary: Pydantic Async Mongo Document
+License: MIT
+Author: Yurzs
+Author-email: yurzs@icloud.com
+Requires-Python: >=3.11,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: autoflake (>=2.2.1,<3.0.0)
+Requires-Dist: motor (>=3.3.1,<4.0.0)
+Requires-Dist: mypy (>=1.5.1,<2.0.0)
+Requires-Dist: pydantic (>=2.3.0,<3.0.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['pydantic_mongo_document']
+# Pydantic Mongo Document
 
-package_data = \
-{'': ['*']}
+`pydantic_mongo_document` is a Python library that provides a base class for creating MongoDB documents using Pydantic models.
 
-install_requires = \
-['autoflake>=2.2.1,<3.0.0',
- 'motor>=3.3.1,<4.0.0',
- 'mypy>=1.5.1,<2.0.0',
- 'pydantic>=2.3.0,<3.0.0']
-
-setup_kwargs = {
-    'name': 'pydantic-mongo-document',
-    'version': '0.1.5',
-    'description': 'Pydantic Async Mongo Document',
-    'long_description': '# Pydantic Mongo Document\n\n`pydantic_mongo_document` is a Python library that provides a base class for creating MongoDB documents using Pydantic models.\n\n## Installation\n\nInstall the package using [pip](https://pip.pypa.io/en/stable/) or [poetry](https://python-poetry.org).\n\n### Using pip\n```bash\npip install pydantic_mongo_document\n```\n\n### Using poetry\n```bash\npoetry add pydantic_mongo_document\n```\n\nUsage\nTo use pydantic_mongo_document, you need to create a Pydantic model that represents your MongoDB document and inherit from the MongoDocument class provided by the library. Here\'s an example:\n\n```python3\nfrom pydantic_mongo_document import Document\n\nclass User(Document):\n    __collection__ = "users"\n    __database__ = "production"\n\n    name: str\n    email: str\n\n```\n\nIn this example, we define a User Pydantic Document model with two fields (name and email) and  \nspecifies the MongoDB collection name (users) and database name (production) using the `__collection__` and `__database__` class attributes.\n\n```python3\nfrom pydantic_mongo_document import Document\n\n# Set the MongoDB URI\nDocument.set_mongo_uri("mongodb://localhost:27017")\n\n\nclass User(Document):\n    __collection__ = "users"\n    __database__ = "production"\n\n    name: str\n    email: str\n\n\nasync def create_user():\n    user = User(name="John", email="john@example.com")\n\n    await user.insert()\n\n    user = await User.one(add_query={"name": "John"})\n    print(user) # User(id=ObjectId("64fc59cf6410868c9a40644b"), name="John", email="john@example")\n```\n\nIn this example, we created new User in database. We then used the `User.one` method to retrieve the user from the database.\n\n## Contributing\nPull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.\n\nPlease make sure to update tests as appropriate.\n\n## License\nMIT\n',
-    'author': 'Yurzs',
-    'author_email': 'yurzs@icloud.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.11,<4.0',
-}
+## Installation
 
+Install the package using [pip](https://pip.pypa.io/en/stable/) or [poetry](https://python-poetry.org).
+
+### Using pip
+```bash
+pip install pydantic_mongo_document
+```
+
+### Using poetry
+```bash
+poetry add pydantic_mongo_document
+```
+
+Usage
+To use pydantic_mongo_document, you need to create a Pydantic model that represents your MongoDB document and inherit from the MongoDocument class provided by the library. Here's an example:
+
+```python3
+from pydantic_mongo_document import Document
+
+class User(Document):
+    __collection__ = "users"
+    __database__ = "production"
+
+    name: str
+    email: str
+
+```
+
+In this example, we define a User Pydantic Document model with two fields (name and email) and  
+specifies the MongoDB collection name (users) and database name (production) using the `__collection__` and `__database__` class attributes.
+
+```python3
+from pydantic_mongo_document import Document
+
+# Set the MongoDB URI
+Document.set_mongo_uri("mongodb://localhost:27017")
+
+
+class User(Document):
+    __collection__ = "users"
+    __database__ = "production"
+
+    name: str
+    email: str
+
+
+async def create_user():
+    user = User(name="John", email="john@example.com")
+
+    await user.insert()
+
+    user = await User.one(add_query={"name": "John"})
+    print(user) # User(id=ObjectId("64fc59cf6410868c9a40644b"), name="John", email="john@example")
+```
+
+In this example, we created new User in database. We then used the `User.one` method to retrieve the user from the database.
+
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+
+## License
+MIT
 
-setup(**setup_kwargs)
```

