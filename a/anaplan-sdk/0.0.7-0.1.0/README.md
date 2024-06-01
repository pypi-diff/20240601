# Comparing `tmp/anaplan_sdk-0.0.7.tar.gz` & `tmp/anaplan_sdk-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anaplan_sdk-0.0.7.tar", max compression
+gzip compressed data, was "anaplan_sdk-0.1.0.tar", max compression
```

## Comparing `anaplan_sdk-0.0.7.tar` & `anaplan_sdk-0.1.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      637 2024-05-30 13:10:49.020625 anaplan_sdk-0.0.7/anaplan_sdk/__init__.py
--rw-r--r--   0        0        0    15045 2024-05-30 12:33:17.774760 anaplan_sdk-0.0.7/anaplan_sdk/_async_client.py
--rw-r--r--   0        0        0     5029 2024-05-30 11:25:55.365132 anaplan_sdk-0.0.7/anaplan_sdk/_auth.py
--rw-r--r--   0        0        0    16587 2024-05-30 12:33:25.879111 anaplan_sdk-0.0.7/anaplan_sdk/_client.py
--rw-r--r--   0        0        0     1612 2024-05-29 16:27:14.773666 anaplan_sdk-0.0.7/anaplan_sdk/_exceptions.py
--rw-r--r--   0        0        0     5397 2024-05-30 13:39:57.483394 anaplan_sdk-0.0.7/anaplan_sdk/_models.py
--rw-r--r--   0        0        0    11558 2024-05-27 16:31:14.513449 anaplan_sdk-0.0.7/LICENSE
--rw-r--r--   0        0        0     1641 2024-05-30 12:45:46.004052 anaplan_sdk-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2425 2024-05-30 11:53:01.695230 anaplan_sdk-0.0.7/README.md
--rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 anaplan_sdk-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      637 2024-05-30 13:10:49.020625 anaplan_sdk-0.1.0/anaplan_sdk/__init__.py
+-rw-r--r--   0        0        0    14851 2024-06-01 10:59:40.846960 anaplan_sdk-0.1.0/anaplan_sdk/_async_client.py
+-rw-r--r--   0        0        0     5029 2024-06-01 10:59:40.846960 anaplan_sdk-0.1.0/anaplan_sdk/_auth.py
+-rw-r--r--   0        0        0    16587 2024-06-01 10:59:40.853386 anaplan_sdk-0.1.0/anaplan_sdk/_client.py
+-rw-r--r--   0        0        0     1612 2024-05-29 16:27:14.773666 anaplan_sdk-0.1.0/anaplan_sdk/_exceptions.py
+-rw-r--r--   0        0        0     5397 2024-06-01 10:59:40.853386 anaplan_sdk-0.1.0/anaplan_sdk/_models.py
+-rw-r--r--   0        0        0    11558 2024-05-27 16:31:14.513449 anaplan_sdk-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1641 2024-06-01 11:00:25.476253 anaplan_sdk-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     2425 2024-05-30 11:53:01.695230 anaplan_sdk-0.1.0/README.md
+-rw-r--r--   0        0        0     3211 1970-01-01 00:00:00.000000 anaplan_sdk-0.1.0/PKG-INFO
```

### Comparing `anaplan_sdk-0.0.7/anaplan_sdk/__init__.py` & `anaplan_sdk-0.1.0/anaplan_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `anaplan_sdk-0.0.7/anaplan_sdk/_async_client.py` & `anaplan_sdk-0.1.0/anaplan_sdk/_async_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,18 +234,16 @@
         """
         return await self._get_binary(
             f"{self._base_url}/{self.workspace_id}/models/{self.model_id}/files/{file_id}"
         )
 
     async def upload_file(self, file_id: int, content: str | bytes) -> None:
         """
-        Uploads the content to the specified file. If `upload_parallel` is set to True on the
-        instance you are invoking this from, will attempt to upload the chunks in parallel for
-        better performance. If you are network bound or are experiencing rate limiting issues, set
-        `upload_parallel` to False.
+        Uploads the content to the specified file. If there are several chunks, upload of
+        individual chunks are concurrent.
 
         :param file_id: The identifier of the file to upload to.
         :param content: The content to upload. **This Content will be compressed before uploading.
                         If you are passing the Input as bytes, pass it uncompressed to avoid
                         redundant work.**
         """
         if isinstance(content, str):
```

### Comparing `anaplan_sdk-0.0.7/anaplan_sdk/_auth.py` & `anaplan_sdk-0.1.0/anaplan_sdk/_auth.py`

 * *Files identical despite different names*

### Comparing `anaplan_sdk-0.0.7/anaplan_sdk/_client.py` & `anaplan_sdk-0.1.0/anaplan_sdk/_client.py`

 * *Files identical despite different names*

### Comparing `anaplan_sdk-0.0.7/anaplan_sdk/_exceptions.py` & `anaplan_sdk-0.1.0/anaplan_sdk/_exceptions.py`

 * *Files identical despite different names*

### Comparing `anaplan_sdk-0.0.7/anaplan_sdk/_models.py` & `anaplan_sdk-0.1.0/anaplan_sdk/_models.py`

 * *Files identical despite different names*

### Comparing `anaplan_sdk-0.0.7/LICENSE` & `anaplan_sdk-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anaplan_sdk-0.0.7/pyproject.toml` & `anaplan_sdk-0.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anaplan-sdk"
-version = "0.0.7"
+version = "0.1.0"
 description = "Provides pythonic access to the Anaplan API"
 license = "Apache-2.0"
 authors = ["Vinzenz Klass <vinzenz.klass@ba.valantic.com>"]
 readme = "README.md"
 homepage = "https://vinzenzklass.github.io/anaplan-sdk/"
 repository = "https://github.com/VinzenzKlass/anaplan-sdk"
 documentation = "https://vinzenzklass.github.io/anaplan-sdk/"
```

### Comparing `anaplan_sdk-0.0.7/README.md` & `anaplan_sdk-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `anaplan_sdk-0.0.7/PKG-INFO` & `anaplan_sdk-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anaplan-sdk
-Version: 0.0.7
+Version: 0.1.0
 Summary: Provides pythonic access to the Anaplan API
 Home-page: https://vinzenzklass.github.io/anaplan-sdk/
 License: Apache-2.0
 Keywords: anaplan,anaplan-api,anaplan-bulk-api,anaplan integration
 Author: Vinzenz Klass
 Author-email: vinzenz.klass@ba.valantic.com
 Requires-Python: >=3.10.4
```

