# Comparing `tmp/postgrest-0.16.4.tar.gz` & `tmp/postgrest-0.16.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postgrest-0.16.4.tar", max compression
+gzip compressed data, was "postgrest-0.16.5.tar", max compression
```

## Comparing `postgrest-0.16.4.tar` & `postgrest-0.16.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1077 2024-04-29 15:26:22.361417 postgrest-0.16.4/LICENSE
--rw-r--r--   0        0        0     4078 2024-04-29 15:26:22.361417 postgrest-0.16.4/README.md
--rw-r--r--   0        0        0      941 2024-04-29 15:26:24.345403 postgrest-0.16.4/postgrest/__init__.py
--rw-r--r--   0        0        0       35 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/_async/__init__.py
--rw-r--r--   0        0        0     3263 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/_async/client.py
--rw-r--r--   0        0        0    14157 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/_async/request_builder.py
--rw-r--r--   0        0        0       35 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/_sync/__init__.py
--rw-r--r--   0        0        0     3217 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/_sync/client.py
--rw-r--r--   0        0        0    14089 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/_sync/request_builder.py
--rw-r--r--   0        0        0     1918 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/base_client.py
--rw-r--r--   0        0        0    22420 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/base_request_builder.py
--rw-r--r--   0        0        0      153 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/constants.py
--rw-r--r--   0        0        0      409 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/deprecated_client.py
--rw-r--r--   0        0        0      422 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/deprecated_get_request_builder.py
--rw-r--r--   0        0        0     1510 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/py.typed
--rw-r--r--   0        0        0      986 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/types.py
--rw-r--r--   0        0        0     1152 2024-04-29 15:26:22.361417 postgrest-0.16.4/postgrest/utils.py
--rw-r--r--   0        0        0     1915 2024-04-29 15:26:24.345403 postgrest-0.16.4/pyproject.toml
--rw-r--r--   0        0        0     5127 1970-01-01 00:00:00.000000 postgrest-0.16.4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-06-01 12:47:26.403494 postgrest-0.16.5/LICENSE
+-rw-r--r--   0        0        0     4078 2024-06-01 12:47:26.403494 postgrest-0.16.5/README.md
+-rw-r--r--   0        0        0      941 2024-06-01 12:47:28.703508 postgrest-0.16.5/postgrest/__init__.py
+-rw-r--r--   0        0        0       35 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/_async/__init__.py
+-rw-r--r--   0        0        0     3263 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/_async/client.py
+-rw-r--r--   0        0        0    14147 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/_async/request_builder.py
+-rw-r--r--   0        0        0       35 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/_sync/__init__.py
+-rw-r--r--   0        0        0     3217 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/_sync/client.py
+-rw-r--r--   0        0        0    14079 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/_sync/request_builder.py
+-rw-r--r--   0        0        0     1918 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/base_client.py
+-rw-r--r--   0        0        0    22860 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/base_request_builder.py
+-rw-r--r--   0        0        0      153 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/constants.py
+-rw-r--r--   0        0        0      409 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/deprecated_client.py
+-rw-r--r--   0        0        0      422 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/deprecated_get_request_builder.py
+-rw-r--r--   0        0        0     1510 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/exceptions.py
+-rw-r--r--   0        0        0        0 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/py.typed
+-rw-r--r--   0        0        0      986 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/types.py
+-rw-r--r--   0        0        0     1152 2024-06-01 12:47:26.407494 postgrest-0.16.5/postgrest/utils.py
+-rw-r--r--   0        0        0     1915 2024-06-01 12:47:28.703508 postgrest-0.16.5/pyproject.toml
+-rw-r--r--   0        0        0     5127 1970-01-01 00:00:00.000000 postgrest-0.16.5/PKG-INFO
```

### Comparing `postgrest-0.16.4/LICENSE` & `postgrest-0.16.5/LICENSE`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.4/README.md` & `postgrest-0.16.5/README.md`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.4/postgrest/__init__.py` & `postgrest-0.16.5/postgrest/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-__version__ = "0.16.4"
+__version__ = "0.16.5"
 
 from httpx import Timeout
 
 from ._async.client import AsyncPostgrestClient
 from ._async.request_builder import (
     AsyncFilterRequestBuilder,
     AsyncMaybeSingleRequestBuilder,
```

### Comparing `postgrest-0.16.4/postgrest/_async/client.py` & `postgrest-0.16.5/postgrest/_async/client.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.4/postgrest/_async/request_builder.py` & `postgrest-0.16.5/postgrest/_async/request_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,22 +67,22 @@
                 if self.http_method != "HEAD":
                     body = r.text
                     if self.headers.get("Accept") == "text/csv":
                         return body
                     if self.headers.get(
                         "Accept"
                     ) and "application/vnd.pgrst.plan" in self.headers.get("Accept"):
-                        if not "+json" in self.headers.get("Accept"):
+                        if "+json" not in self.headers.get("Accept"):
                             return body
                 return APIResponse[_ReturnT].from_http_request_response(r)
             else:
                 raise APIError(r.json())
         except ValidationError as e:
             raise APIError(r.json()) from e
-        except JSONDecodeError as e:
+        except JSONDecodeError:
             raise APIError(generate_default_error_message(r))
 
 
 class AsyncSingleRequestBuilder(Generic[_ReturnT]):
     def __init__(
         self,
         session: AsyncClient,
@@ -123,15 +123,15 @@
                 200 <= r.status_code <= 299
             ):  # Response.ok from JS (https://developer.mozilla.org/en-US/docs/Web/API/Response/ok)
                 return SingleAPIResponse[_ReturnT].from_http_request_response(r)
             else:
                 raise APIError(r.json())
         except ValidationError as e:
             raise APIError(r.json()) from e
-        except JSONDecodeError as e:
+        except JSONDecodeError:
             raise APIError(generate_default_error_message(r))
 
 
 class AsyncMaybeSingleRequestBuilder(AsyncSingleRequestBuilder[_ReturnT]):
     async def execute(self) -> Optional[SingleAPIResponse[_ReturnT]]:
         r = None
         try:
```

### Comparing `postgrest-0.16.4/postgrest/_sync/client.py` & `postgrest-0.16.5/postgrest/_sync/client.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.4/postgrest/_sync/request_builder.py` & `postgrest-0.16.5/postgrest/_sync/request_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,22 +67,22 @@
                 if self.http_method != "HEAD":
                     body = r.text
                     if self.headers.get("Accept") == "text/csv":
                         return body
                     if self.headers.get(
                         "Accept"
                     ) and "application/vnd.pgrst.plan" in self.headers.get("Accept"):
-                        if not "+json" in self.headers.get("Accept"):
+                        if "+json" not in self.headers.get("Accept"):
                             return body
                 return APIResponse[_ReturnT].from_http_request_response(r)
             else:
                 raise APIError(r.json())
         except ValidationError as e:
             raise APIError(r.json()) from e
-        except JSONDecodeError as e:
+        except JSONDecodeError:
             raise APIError(generate_default_error_message(r))
 
 
 class SyncSingleRequestBuilder(Generic[_ReturnT]):
     def __init__(
         self,
         session: SyncClient,
@@ -123,15 +123,15 @@
                 200 <= r.status_code <= 299
             ):  # Response.ok from JS (https://developer.mozilla.org/en-US/docs/Web/API/Response/ok)
                 return SingleAPIResponse[_ReturnT].from_http_request_response(r)
             else:
                 raise APIError(r.json())
         except ValidationError as e:
             raise APIError(r.json()) from e
-        except JSONDecodeError as e:
+        except JSONDecodeError:
             raise APIError(generate_default_error_message(r))
 
 
 class SyncMaybeSingleRequestBuilder(SyncSingleRequestBuilder[_ReturnT]):
     def execute(self) -> Optional[SingleAPIResponse[_ReturnT]]:
         r = None
         try:
```

### Comparing `postgrest-0.16.4/postgrest/base_client.py` & `postgrest-0.16.5/postgrest/base_client.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.4/postgrest/base_request_builder.py` & `postgrest-0.16.5/postgrest/base_request_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,15 +192,15 @@
 
     @classmethod
     def from_http_request_response(
         cls: Type[Self], request_response: RequestResponse
     ) -> Self:
         try:
             data = request_response.json()
-        except JSONDecodeError as e:
+        except JSONDecodeError:
             return cls(data=[], count=0)
         count = cls._get_count_from_http_request_response(request_response)
         # the type-ignore here is as pydantic needs us to pass the type parameter
         # here explicitly, but pylance already knows that cls is correctly parametrized
         return cls[_ReturnT](data=data, count=count)  # type: ignore
 
     @classmethod
@@ -447,17 +447,24 @@
             # range
             return self.filter(column, Filters.CD, value)
         if not isinstance(value, dict) and isinstance(value, Iterable):
             stringified_values = ",".join(value)
             return self.filter(column, Filters.CD, f"{{{stringified_values}}}")
         return self.filter(column, Filters.CD, json.dumps(value))
 
-    def ov(self: Self, column: str, values: Iterable[Any]) -> Self:
-        values = ",".join(values)
-        return self.filter(column, Filters.OV, f"{{{values}}}")
+    def ov(self: Self, column: str, value: Iterable[Any]) -> Self:
+        if isinstance(value, str):
+            # range types can be inclusive '[', ']' or exclusive '(', ')' so just
+            # keep it simple and accept a string
+            return self.filter(column, Filters.OV, value)
+        if not isinstance(value, dict) and isinstance(value, Iterable):
+            # Expected to be some type of iterable
+            stringified_values = ",".join(value)
+            return self.filter(column, Filters.OV, f"{{{stringified_values}}}")
+        return self.filter(column, Filters.OV, json.dumps(value))
 
     def sl(self: Self, column: str, range: Tuple[int, int]) -> Self:
         return self.filter(column, Filters.SL, f"({range[0]},{range[1]})")
 
     def sr(self: Self, column: str, range: Tuple[int, int]) -> Self:
         return self.filter(column, Filters.SR, f"({range[0]},{range[1]})")
 
@@ -527,17 +534,17 @@
     ) -> Self:
         options = [
             key
             for key, value in locals().items()
             if key not in ["self", "format"] and value
         ]
         options_str = "|".join(options)
-        self.headers[
-            "Accept"
-        ] = f"application/vnd.pgrst.plan+{format}; options={options_str}"
+        self.headers["Accept"] = (
+            f"application/vnd.pgrst.plan+{format}; options={options_str}"
+        )
         return self
 
     def order(
         self: Self,
         column: str,
         *,
         desc: bool = False,
```

### Comparing `postgrest-0.16.4/postgrest/exceptions.py` & `postgrest-0.16.5/postgrest/exceptions.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.4/postgrest/types.py` & `postgrest-0.16.5/postgrest/types.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.4/postgrest/utils.py` & `postgrest-0.16.5/postgrest/utils.py`

 * *Files identical despite different names*

### Comparing `postgrest-0.16.4/pyproject.toml` & `postgrest-0.16.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "postgrest"
-version = "0.16.4"
+version = "0.16.5"
 description = "PostgREST client for Python. This library provides an ORM interface to PostgREST."
 authors = ["Lương Quang Mạnh <luongquangmanh85@gmail.com>", "Joel Lee <joel@joellee.org>", "Anand", "Oliver Rice", "Andrew Smith <a.smith@silentworks.co.uk>"]
 homepage = "https://github.com/supabase-community/postgrest-py"
 repository = "https://github.com/supabase-community/postgrest-py"
 documentation = "https://postgrest-py.rtfd.io"
 readme = "README.md"
 license = "MIT"
@@ -21,24 +21,24 @@
 python = "^3.8"
 httpx = ">=0.24,<0.28"
 deprecation = "^2.1.0"
 pydantic = ">=1.9,<3.0"
 strenum = "^0.4.9"
 
 [tool.poetry.dev-dependencies]
-pytest = "^8.1.1"
+pytest = "^8.2.1"
 flake8 = "^5.0.4"
-black = "^24.3"
+black = "^24.4"
 isort = "^5.12.0"
 pre-commit = "^3.5.0"
 pytest-cov = "^5.0.0"
 pytest-depends = "^1.0.1"
-pytest-asyncio = "^0.23.6"
+pytest-asyncio = "^0.23.7"
 unasync-cli = "^0.0.9"
-python-semantic-release = "^9.5.0"
+python-semantic-release = "^9.8.0"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^7.1.2"
 furo = ">=2023.9.10,<2025.0.0"
```

### Comparing `postgrest-0.16.4/PKG-INFO` & `postgrest-0.16.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postgrest
-Version: 0.16.4
+Version: 0.16.5
 Summary: PostgREST client for Python. This library provides an ORM interface to PostgREST.
 Home-page: https://github.com/supabase-community/postgrest-py
 License: MIT
 Author: Lương Quang Mạnh
 Author-email: luongquangmanh85@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

