# Comparing `tmp/postgrest-0.16.5.tar.gz` & `tmp/postgrest-0.16.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgrest-0.16.5.tar", max compression
+gzip compressed data, was "postgrest-0.16.6.tar", max compression
```

## Comparing `postgrest-0.16.5.tar` & `postgrest-0.16.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1077 2024-06-01 12:47:26.403494 postgrest-0.16.5/LICENSE
--rw-r--r--   0        0        0     4078 2024-06-01 12:47:26.403494 postgrest-0.16.5/README.md
--rw-r--r--   0        0        0      941 2024-06-01 12:47:28.703508 postgrest-0.16.5/postgrest/__init__.py
--rw-r--r--   0        0        0       35 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/_async/__init__.py
--rw-r--r--   0        0        0     3263 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/_async/client.py
--rw-r--r--   0        0        0    14147 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/_async/request_builder.py
--rw-r--r--   0        0        0       35 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/_sync/__init__.py
--rw-r--r--   0        0        0     3217 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/_sync/client.py
--rw-r--r--   0        0        0    14079 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/_sync/request_builder.py
--rw-r--r--   0        0        0     1918 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/base_client.py
--rw-r--r--   0        0        0    22860 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/base_request_builder.py
--rw-r--r--   0        0        0      153 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/constants.py
--rw-r--r--   0        0        0      409 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/deprecated_client.py
--rw-r--r--   0        0        0      422 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/deprecated_get_request_builder.py
--rw-r--r--   0        0        0     1510 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/exceptions.py
--rw-r--r--   0        0        0        0 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/py.typed
--rw-r--r--   0        0        0      986 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/types.py
--rw-r--r--   0        0        0     1152 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/utils.py
--rw-r--r--   0        0        0     1915 2024-06-01 12:47:28.703508 postgrest-0.16.5/pyproject.toml
--rw-r--r--   0        0        0     5127 1970-01-01 00:00:00.000000 postgrest-0.16.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-06-01 13:04:01.438865 postgrest-0.16.6/LICENSE
+-rw-r--r--   0        0        0     4078 2024-06-01 13:04:01.438865 postgrest-0.16.6/README.md
+-rw-r--r--   0        0        0      941 2024-06-01 13:04:04.046878 postgrest-0.16.6/postgrest/__init__.py
+-rw-r--r--   0        0        0       35 2024-06-01 13:04:01.442865 postgrest-0.16.6/postgrest/_async/__init__.py
+-rw-r--r--   0        0        0     3263 2024-06-01 13:04:01.442865 postgrest-0.16.6/postgrest/_async/client.py
+-rw-r--r--   0        0        0    14147 2024-06-01 13:04:01.442865 postgrest-0.16.6/postgrest/_async/request_builder.py
+-rw-r--r--   0        0        0       35 2024-06-01 13:04:01.442865 postgrest-0.16.6/postgrest/_sync/__init__.py
+-rw-r--r--   0        0        0     3217 2024-06-01 13:04:01.442865 postgrest-0.16.6/postgrest/_sync/client.py
+-rw-r--r--   0        0        0    14079 2024-06-01 13:04:01.442865 postgrest-0.16.6/postgrest/_sync/request_builder.py
+-rw-r--r--   0        0        0     1918 2024-06-01 13:04:01.442865 postgrest-0.16.6/postgrest/base_client.py
+-rw-r--r--   0        0        0    22913 2024-06-01 13:04:01.442865 postgrest-0.16.6/postgrest/base_request_builder.py
+-rw-r--r--   0        0        0      153 2024-06-01 13:04:01.442865 postgrest-0.16.6/postgrest/constants.py
+-rw-r--r--   0        0        0      409 2024-06-01 13:04:01.442865 postgrest-0.16.6/postgrest/deprecated_client.py
+-rw-r--r--   0        0        0      422 2024-06-01 13:04:01.442865 postgrest-0.16.6/postgrest/deprecated_get_request_builder.py
+-rw-r--r--   0        0        0     1510 2024-06-01 13:04:01.442865 postgrest-0.16.6/postgrest/exceptions.py
+-rw-r--r--   0        0        0        0 2024-06-01 13:04:01.442865 postgrest-0.16.6/postgrest/py.typed
+-rw-r--r--   0        0        0      986 2024-06-01 13:04:01.442865 postgrest-0.16.6/postgrest/types.py
+-rw-r--r--   0        0        0     1152 2024-06-01 13:04:01.442865 postgrest-0.16.6/postgrest/utils.py
+-rw-r--r--   0        0        0     1915 2024-06-01 13:04:04.042878 postgrest-0.16.6/pyproject.toml
+-rw-r--r--   0        0        0     5127 1970-01-01 00:00:00.000000 postgrest-0.16.6/PKG-INFO
```

### Comparing `postgrest-0.16.5/LICENSE` & `postgrest-0.16.6/LICENSE`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.5/README.md` & `postgrest-0.16.6/README.md`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.5/postgrest/__init__.py` & `postgrest-0.16.6/postgrest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__version__ = "0.16.5"
+__version__ = "0.16.6"
 
 from httpx import Timeout
 
 from ._async.client import AsyncPostgrestClient
 from ._async.request_builder import (
     AsyncFilterRequestBuilder,
     AsyncMaybeSingleRequestBuilder,
```

### Comparing `postgrest-0.16.5/postgrest/_async/client.py` & `postgrest-0.16.6/postgrest/_async/client.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.5/postgrest/_async/request_builder.py` & `postgrest-0.16.6/postgrest/_async/request_builder.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.5/postgrest/_sync/client.py` & `postgrest-0.16.6/postgrest/_sync/client.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.5/postgrest/_sync/request_builder.py` & `postgrest-0.16.6/postgrest/_sync/request_builder.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.5/postgrest/base_client.py` & `postgrest-0.16.6/postgrest/base_client.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.5/postgrest/base_request_builder.py` & `postgrest-0.16.6/postgrest/base_request_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,14 +326,16 @@
     def is_(self: Self, column: str, value: Any) -> Self:
         """An 'is' filter
 
         Args:
             column: The name of the column to apply a filter on
             value: The value to filter by
         """
+        if value is None:
+            value = "null"
         return self.filter(column, Filters.IS, value)
 
     def like(self: Self, column: str, pattern: str) -> Self:
         """A 'LIKE' filter, to use for pattern matching.
 
         Args:
             column: The name of the column to apply a filter on
```

### Comparing `postgrest-0.16.5/postgrest/exceptions.py` & `postgrest-0.16.6/postgrest/exceptions.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.5/postgrest/types.py` & `postgrest-0.16.6/postgrest/types.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.5/postgrest/utils.py` & `postgrest-0.16.6/postgrest/utils.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.5/pyproject.toml` & `postgrest-0.16.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "postgrest"
-version = "0.16.5"
+version = "0.16.6"
 description = "PostgREST client for Python. This library provides an ORM interface to PostgREST."
 authors = ["Lương Quang Mạnh <luongquangmanh85@gmail.com>", "Joel Lee <joel@joellee.org>", "Anand", "Oliver Rice", "Andrew Smith <a.smith@silentworks.co.uk>"]
 homepage = "https://github.com/supabase-community/postgrest-py"
 repository = "https://github.com/supabase-community/postgrest-py"
 documentation = "https://postgrest-py.rtfd.io"
 readme = "README.md"
 license = "MIT"
```

### Comparing `postgrest-0.16.5/PKG-INFO` & `postgrest-0.16.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postgrest
-Version: 0.16.5
+Version: 0.16.6
 Summary: PostgREST client for Python. This library provides an ORM interface to PostgREST.
 Home-page: https://github.com/supabase-community/postgrest-py
 License: MIT
 Author: Lương Quang Mạnh
 Author-email: luongquangmanh85@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

