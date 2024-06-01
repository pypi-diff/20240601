# Comparing `tmp/reka_api-3.0.5.tar.gz` & `tmp/reka_api-3.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reka_api-3.0.5.tar", max compression
+gzip compressed data, was "reka_api-3.0.6.tar", max compression
```

## Comparing `reka_api-3.0.5.tar` & `reka_api-3.0.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
--rw-r--r--   0        0        0     1057 2024-05-31 17:32:53.504624 reka_api-3.0.5/LICENSE
--rw-r--r--   0        0        0     5577 2024-05-31 17:32:53.504624 reka_api-3.0.5/README.md
--rw-r--r--   0        0        0     1649 2024-05-31 17:32:53.504624 reka_api-3.0.5/pyproject.toml
--rw-r--r--   0        0        0     1231 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/__init__.py
--rw-r--r--   0        0        0       65 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/chat/__init__.py
--rw-r--r--   0        0        0    27684 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/chat/client.py
--rw-r--r--   0        0        0     5361 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/client.py
--rw-r--r--   0        0        0     1126 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/api_error.py
--rw-r--r--   0        0        0     1483 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/jsonable_encoder.py
--rw-r--r--   0        0        0      748 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/pydantic_utilities.py
--rw-r--r--   0        0        0     1266 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/query_encoder.py
--rw-r--r--   0        0        0      330 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/request_options.py
--rw-r--r--   0        0        0     8148 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/core/unchecked_base_model.py
--rw-r--r--   0        0        0      152 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/environment.py
--rw-r--r--   0        0        0      170 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/errors/__init__.py
--rw-r--r--   0        0        0      313 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/errors/unprocessable_entity_error.py
--rw-r--r--   0        0        0       65 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/models/__init__.py
--rw-r--r--   0        0        0     5028 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/models/client.py
--rw-r--r--   0        0        0        0 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/py.typed
--rw-r--r--   0        0        0     1476 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/__init__.py
--rw-r--r--   0        0        0     1338 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chat_message.py
--rw-r--r--   0        0        0     1387 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chat_message_chunk.py
--rw-r--r--   0        0        0      239 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chat_message_chunk_content_item.py
--rw-r--r--   0        0        0      239 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chat_message_input_content_item.py
--rw-r--r--   0        0        0      240 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chat_message_output_content_item.py
--rw-r--r--   0        0        0     1351 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chat_response.py
--rw-r--r--   0        0        0      153 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chat_role.py
--rw-r--r--   0        0        0     1400 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chunk_chat_response.py
--rw-r--r--   0        0        0     1388 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/chunk_message_response.py
--rw-r--r--   0        0        0      224 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/content.py
--rw-r--r--   0        0        0      165 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/finish_reason.py
--rw-r--r--   0        0        0     1272 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/http_validation_error.py
--rw-r--r--   0        0        0      183 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/media_type.py
--rw-r--r--   0        0        0     1373 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/message_response.py
--rw-r--r--   0        0        0     1348 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/model.py
--rw-r--r--   0        0        0     1572 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/typed_media_content.py
--rw-r--r--   0        0        0     1530 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/typed_text.py
--rw-r--r--   0        0        0     1267 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/usage.py
--rw-r--r--   0        0        0     1291 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/validation_error.py
--rw-r--r--   0        0        0      128 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/types/validation_error_loc_item.py
--rw-r--r--   0        0        0      776 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/__init__.py
--rw-r--r--   0        0        0        0 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/api/__init__.py
--rw-r--r--   0        0        0     7489 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/api/chat.py
--rw-r--r--   0        0        0     2084 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/api/dataset.py
--rw-r--r--   0        0        0     2248 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/api/driver.py
--rw-r--r--   0        0        0      698 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/api/job.py
--rw-r--r--   0        0        0      376 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/api/models.py
--rw-r--r--   0        0        0     3573 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/api/retrieval.py
--rw-r--r--   0        0        0     1128 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/errors.py
--rw-r--r--   0        0        0        0 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/v2/py.typed
--rw-r--r--   0        0        0       76 2024-05-31 17:32:53.504624 reka_api-3.0.5/src/reka/version.py
--rw-r--r--   0        0        0     6817 1970-01-01 00:00:00.000000 reka_api-3.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1057 2024-06-01 21:13:38.939618 reka_api-3.0.6/LICENSE
+-rw-r--r--   0        0        0     5577 2024-06-01 21:13:38.939618 reka_api-3.0.6/README.md
+-rw-r--r--   0        0        0     1691 2024-06-01 21:13:38.939618 reka_api-3.0.6/pyproject.toml
+-rw-r--r--   0        0        0     1231 2024-06-01 21:13:38.939618 reka_api-3.0.6/src/reka/__init__.py
+-rw-r--r--   0        0        0       65 2024-06-01 21:13:38.939618 reka_api-3.0.6/src/reka/chat/__init__.py
+-rw-r--r--   0        0        0    27684 2024-06-01 21:13:38.939618 reka_api-3.0.6/src/reka/chat/client.py
+-rw-r--r--   0        0        0     5361 2024-06-01 21:13:38.939618 reka_api-3.0.6/src/reka/client.py
+-rw-r--r--   0        0        0     1126 2024-06-01 21:13:38.939618 reka_api-3.0.6/src/reka/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-06-01 21:13:38.939618 reka_api-3.0.6/src/reka/core/api_error.py
+-rw-r--r--   0        0        0     1483 2024-06-01 21:13:38.939618 reka_api-3.0.6/src/reka/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-06-01 21:13:38.939618 reka_api-3.0.6/src/reka/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-06-01 21:13:38.939618 reka_api-3.0.6/src/reka/core/file.py
+-rw-r--r--   0        0        0     5059 2024-06-01 21:13:38.939618 reka_api-3.0.6/src/reka/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-06-01 21:13:38.939618 reka_api-3.0.6/src/reka/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      748 2024-06-01 21:13:38.939618 reka_api-3.0.6/src/reka/core/pydantic_utilities.py
+-rw-r--r--   0        0        0     1266 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/core/query_encoder.py
+-rw-r--r--   0        0        0      330 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/core/request_options.py
+-rw-r--r--   0        0        0     8148 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/core/unchecked_base_model.py
+-rw-r--r--   0        0        0      152 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/environment.py
+-rw-r--r--   0        0        0      170 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/errors/__init__.py
+-rw-r--r--   0        0        0      313 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/errors/unprocessable_entity_error.py
+-rw-r--r--   0        0        0       65 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/models/__init__.py
+-rw-r--r--   0        0        0     5028 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/models/client.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/py.typed
+-rw-r--r--   0        0        0     1476 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/__init__.py
+-rw-r--r--   0        0        0     1338 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/chat_message.py
+-rw-r--r--   0        0        0     1387 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/chat_message_chunk.py
+-rw-r--r--   0        0        0      239 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/chat_message_chunk_content_item.py
+-rw-r--r--   0        0        0      239 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/chat_message_input_content_item.py
+-rw-r--r--   0        0        0      240 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/chat_message_output_content_item.py
+-rw-r--r--   0        0        0     1351 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/chat_response.py
+-rw-r--r--   0        0        0      153 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/chat_role.py
+-rw-r--r--   0        0        0     1400 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/chunk_chat_response.py
+-rw-r--r--   0        0        0     1388 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/chunk_message_response.py
+-rw-r--r--   0        0        0      224 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/content.py
+-rw-r--r--   0        0        0      165 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/finish_reason.py
+-rw-r--r--   0        0        0     1272 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/http_validation_error.py
+-rw-r--r--   0        0        0      183 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/media_type.py
+-rw-r--r--   0        0        0     1373 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/message_response.py
+-rw-r--r--   0        0        0     1348 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/model.py
+-rw-r--r--   0        0        0     1572 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/typed_media_content.py
+-rw-r--r--   0        0        0     1530 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/typed_text.py
+-rw-r--r--   0        0        0     1267 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/usage.py
+-rw-r--r--   0        0        0     1291 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/validation_error.py
+-rw-r--r--   0        0        0      128 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/types/validation_error_loc_item.py
+-rw-r--r--   0        0        0      776 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/v2/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/v2/api/__init__.py
+-rw-r--r--   0        0        0     7489 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/v2/api/chat.py
+-rw-r--r--   0        0        0     2084 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/v2/api/dataset.py
+-rw-r--r--   0        0        0     2248 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/v2/api/driver.py
+-rw-r--r--   0        0        0      698 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/v2/api/job.py
+-rw-r--r--   0        0        0      376 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/v2/api/models.py
+-rw-r--r--   0        0        0     3573 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/v2/api/retrieval.py
+-rw-r--r--   0        0        0     1128 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/v2/errors.py
+-rw-r--r--   0        0        0        0 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/v2/py.typed
+-rw-r--r--   0        0        0       76 2024-06-01 21:13:38.943618 reka_api-3.0.6/src/reka/version.py
+-rw-r--r--   0        0        0     6817 1970-01-01 00:00:00.000000 reka_api-3.0.6/PKG-INFO
```

### Comparing `reka_api-3.0.5/LICENSE` & `reka_api-3.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/README.md` & `reka_api-3.0.6/README.md`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/pyproject.toml` & `reka_api-3.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reka-api"
-version = "3.0.5"
+version = "3.0.6"
 description = "Reka Python SDK"
 readme = "README.md"
 authors = [
     "Reka Team <contact@reka.ai>"
 ]
 keywords = [
     "reka",
@@ -50,14 +50,15 @@
 urllib3 = ">=2.0.7"
 
 [tool.poetry.dev-dependencies]
 mypy = "1.9.0"
 pytest = "^7.4.0"
 pytest-asyncio = "^0.23.5"
 python-dateutil = "^2.9.0"
+types-python-dateutil = "^2.9.0.20240316"
 types-requests = "^2.31.0.2"
 
 [tool.pytest.ini_options]
 testpaths = [ "tests" ]
 asyncio_mode = "auto"
 
 [tool.mypy]
```

### Comparing `reka_api-3.0.5/src/reka/__init__.py` & `reka_api-3.0.6/src/reka/__init__.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/chat/client.py` & `reka_api-3.0.6/src/reka/chat/client.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/client.py` & `reka_api-3.0.6/src/reka/client.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/core/__init__.py` & `reka_api-3.0.6/src/reka/core/__init__.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/core/client_wrapper.py` & `reka_api-3.0.6/src/reka/core/client_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "reka-api",
-            "X-Fern-SDK-Version": "3.0.5",
+            "X-Fern-SDK-Version": "3.0.6",
         }
         headers["X-Api-Key"] = self.api_key
         return headers
 
     def get_base_url(self) -> str:
         return self._base_url
```

### Comparing `reka_api-3.0.5/src/reka/core/datetime_utils.py` & `reka_api-3.0.6/src/reka/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/core/file.py` & `reka_api-3.0.6/src/reka/core/file.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/core/http_client.py` & `reka_api-3.0.6/src/reka/core/http_client.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/core/jsonable_encoder.py` & `reka_api-3.0.6/src/reka/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/core/pydantic_utilities.py` & `reka_api-3.0.6/src/reka/core/pydantic_utilities.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/core/query_encoder.py` & `reka_api-3.0.6/src/reka/core/query_encoder.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/core/request_options.py` & `reka_api-3.0.6/src/reka/core/request_options.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/core/unchecked_base_model.py` & `reka_api-3.0.6/src/reka/core/unchecked_base_model.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/models/client.py` & `reka_api-3.0.6/src/reka/models/client.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/types/__init__.py` & `reka_api-3.0.6/src/reka/types/__init__.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/types/chat_message.py` & `reka_api-3.0.6/src/reka/types/chat_message.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/types/chat_message_chunk.py` & `reka_api-3.0.6/src/reka/types/chat_message_chunk.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/types/chat_response.py` & `reka_api-3.0.6/src/reka/types/chat_response.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/types/chunk_chat_response.py` & `reka_api-3.0.6/src/reka/types/chunk_chat_response.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/types/chunk_message_response.py` & `reka_api-3.0.6/src/reka/types/chunk_message_response.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/types/http_validation_error.py` & `reka_api-3.0.6/src/reka/types/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/types/message_response.py` & `reka_api-3.0.6/src/reka/types/message_response.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/types/model.py` & `reka_api-3.0.6/src/reka/types/model.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/types/typed_media_content.py` & `reka_api-3.0.6/src/reka/types/typed_media_content.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/types/typed_text.py` & `reka_api-3.0.6/src/reka/types/typed_text.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/types/usage.py` & `reka_api-3.0.6/src/reka/types/usage.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/types/validation_error.py` & `reka_api-3.0.6/src/reka/types/validation_error.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/v2/__init__.py` & `reka_api-3.0.6/src/reka/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/v2/api/chat.py` & `reka_api-3.0.6/src/reka/v2/api/chat.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/v2/api/dataset.py` & `reka_api-3.0.6/src/reka/v2/api/dataset.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/v2/api/driver.py` & `reka_api-3.0.6/src/reka/v2/api/driver.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/v2/api/job.py` & `reka_api-3.0.6/src/reka/v2/api/job.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/v2/api/retrieval.py` & `reka_api-3.0.6/src/reka/v2/api/retrieval.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/src/reka/v2/errors.py` & `reka_api-3.0.6/src/reka/v2/errors.py`

 * *Files identical despite different names*

### Comparing `reka_api-3.0.5/PKG-INFO` & `reka_api-3.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reka-api
-Version: 3.0.5
+Version: 3.0.6
 Summary: Reka Python SDK
 License: MIT
 Keywords: reka,ai,sdk
 Author: Reka Team
 Author-email: contact@reka.ai
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

