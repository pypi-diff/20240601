# Comparing `tmp/airbyte_source_faker-6.1.1.tar.gz` & `tmp/airbyte_source_faker-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_faker-6.1.1.tar", max compression
+gzip compressed data, was "airbyte_source_faker-6.1.2.tar", max compression
```

## Comparing `airbyte_source_faker-6.1.1.tar` & `airbyte_source_faker-6.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     4488 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/README.md
--rw-r--r--   0        0        0      784 2024-05-20 18:16:25.752215 airbyte_source_faker-6.1.1/pyproject.toml
--rw-r--r--   0        0        0      122 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/__init__.py
--rw-r--r--   0        0        0      727 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/airbyte_message_with_cached_json.py
--rw-r--r--   0        0        0     4590 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/purchase_generator.py
--rw-r--r--   0        0        0    15356 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/record_data/products.json
--rw-r--r--   0        0        0      266 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/run.py
--rw-r--r--   0        0        0      529 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/schemas/products.json
--rw-r--r--   0        0        0      892 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/schemas/purchases.json
--rw-r--r--   0        0        0     1259 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/schemas/users.json
--rw-r--r--   0        0        0     1366 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/source.py
--rw-r--r--   0        0        0     1849 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/spec.json
--rw-r--r--   0        0        0     6705 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/streams.py
--rw-r--r--   0        0        0     3325 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/user_generator.py
--rw-r--r--   0        0        0      937 2024-05-20 18:11:37.131385 airbyte_source_faker-6.1.1/source_faker/utils.py
--rw-r--r--   0        0        0     5256 1970-01-01 00:00:00.000000 airbyte_source_faker-6.1.1/PKG-INFO
+-rw-r--r--   0        0        0     4488 2024-06-01 02:04:57.000000 airbyte_source_faker-6.1.2/README.md
+-rw-r--r--   0        0        0      790 2024-06-01 05:00:47.271460 airbyte_source_faker-6.1.2/pyproject.toml
+-rw-r--r--   0        0        0      122 2024-06-01 02:04:57.000000 airbyte_source_faker-6.1.2/source_faker/__init__.py
+-rw-r--r--   0        0        0      727 2024-06-01 02:04:57.000000 airbyte_source_faker-6.1.2/source_faker/airbyte_message_with_cached_json.py
+-rw-r--r--   0        0        0     4590 2024-06-01 02:04:57.000000 airbyte_source_faker-6.1.2/source_faker/purchase_generator.py
+-rw-r--r--   0        0        0    15356 2024-06-01 02:04:57.000000 airbyte_source_faker-6.1.2/source_faker/record_data/products.json
+-rw-r--r--   0        0        0      266 2024-06-01 02:04:57.000000 airbyte_source_faker-6.1.2/source_faker/run.py
+-rw-r--r--   0        0        0      529 2024-06-01 02:04:57.000000 airbyte_source_faker-6.1.2/source_faker/schemas/products.json
+-rw-r--r--   0        0        0      892 2024-06-01 02:04:57.000000 airbyte_source_faker-6.1.2/source_faker/schemas/purchases.json
+-rw-r--r--   0        0        0     1259 2024-06-01 02:04:57.000000 airbyte_source_faker-6.1.2/source_faker/schemas/users.json
+-rw-r--r--   0        0        0     1366 2024-06-01 02:04:57.000000 airbyte_source_faker-6.1.2/source_faker/source.py
+-rw-r--r--   0        0        0     1849 2024-06-01 02:04:57.000000 airbyte_source_faker-6.1.2/source_faker/spec.json
+-rw-r--r--   0        0        0     6705 2024-06-01 02:04:57.000000 airbyte_source_faker-6.1.2/source_faker/streams.py
+-rw-r--r--   0        0        0     3325 2024-06-01 02:04:57.000000 airbyte_source_faker-6.1.2/source_faker/user_generator.py
+-rw-r--r--   0        0        0      937 2024-06-01 02:04:57.000000 airbyte_source_faker-6.1.2/source_faker/utils.py
+-rw-r--r--   0        0        0     5253 1970-01-01 00:00:00.000000 airbyte_source_faker-6.1.2/PKG-INFO
```

### Comparing `airbyte_source_faker-6.1.1/README.md` & `airbyte_source_faker-6.1.2/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.1/pyproject.toml` & `airbyte_source_faker-6.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "6.1.1"
+version = "6.1.2"
 name = "airbyte-source-faker"
 description = "Source implementation for fake but realistic looking data."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_faker" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "^0.73.0"
+airbyte-cdk = ">=0.73.0,<2.0"
 mimesis = "==6.1.1"
 
 [tool.poetry.scripts]
 source-faker = "source_faker.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.9.3"
```

### Comparing `airbyte_source_faker-6.1.1/source_faker/airbyte_message_with_cached_json.py` & `airbyte_source_faker-6.1.2/source_faker/airbyte_message_with_cached_json.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.1/source_faker/purchase_generator.py` & `airbyte_source_faker-6.1.2/source_faker/purchase_generator.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.1/source_faker/record_data/products.json` & `airbyte_source_faker-6.1.2/source_faker/record_data/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.1/source_faker/schemas/products.json` & `airbyte_source_faker-6.1.2/source_faker/schemas/products.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.1/source_faker/schemas/purchases.json` & `airbyte_source_faker-6.1.2/source_faker/schemas/purchases.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.1/source_faker/schemas/users.json` & `airbyte_source_faker-6.1.2/source_faker/schemas/users.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.1/source_faker/source.py` & `airbyte_source_faker-6.1.2/source_faker/source.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.1/source_faker/spec.json` & `airbyte_source_faker-6.1.2/source_faker/spec.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.1/source_faker/streams.py` & `airbyte_source_faker-6.1.2/source_faker/streams.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.1/source_faker/user_generator.py` & `airbyte_source_faker-6.1.2/source_faker/user_generator.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.1/source_faker/utils.py` & `airbyte_source_faker-6.1.2/source_faker/utils.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_faker-6.1.1/PKG-INFO` & `airbyte_source_faker-6.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-faker
-Version: 6.1.1
+Version: 6.1.2
 Summary: Source implementation for fake but realistic looking data.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (>=0.73.0,<0.74.0)
+Requires-Dist: airbyte-cdk (>=0.73.0,<2.0)
 Requires-Dist: mimesis (==6.1.1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/faker
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Faker source connector
```

