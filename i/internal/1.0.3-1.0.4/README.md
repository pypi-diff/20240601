# Comparing `tmp/internal-1.0.3.tar.gz` & `tmp/internal-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internal-1.0.3.tar", max compression
+gzip compressed data, was "internal-1.0.4.tar", max compression
```

## Comparing `internal-1.0.3.tar` & `internal-1.0.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776995 internal-1.0.3/README.md
--rw-r--r--   0        0        0      453 2024-05-20 01:24:27.426660 internal-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776948 internal-1.0.3/src/internal/__init__.py
--rw-r--r--   0        0        0     1715 2024-04-19 06:23:20.193365 internal-1.0.3/src/internal/base_config.py
--rw-r--r--   0        0        0     7662 2024-05-16 07:14:46.689593 internal-1.0.3/src/internal/base_factory.py
--rw-r--r--   0        0        0        0 2024-02-13 10:57:40.969610 internal-1.0.3/src/internal/common_enum/__init__.py
--rw-r--r--   0        0        0      142 2024-02-13 11:01:26.248123 internal-1.0.3/src/internal/common_enum/contact_type.py
--rw-r--r--   0        0        0      114 2024-03-19 08:47:41.966209 internal-1.0.3/src/internal/common_enum/event_type.py
--rw-r--r--   0        0        0      125 2024-02-13 11:01:26.244153 internal-1.0.3/src/internal/common_enum/operator_type.py
--rw-r--r--   0        0        0      511 2024-04-09 02:21:45.907592 internal-1.0.3/src/internal/common_enum/service_ticket_event_trigger_type.py
--rw-r--r--   0        0        0     1025 2024-01-28 03:58:24.810115 internal-1.0.3/src/internal/const.py
--rw-r--r--   0        0        0     2124 2024-05-20 01:23:34.653477 internal-1.0.3/src/internal/database.py
--rw-r--r--   0        0        0        0 2023-12-15 06:58:26.332564 internal-1.0.3/src/internal/exception/__init__.py
--rw-r--r--   0        0        0      363 2024-01-28 10:00:28.362441 internal-1.0.3/src/internal/exception/base_exception.py
--rw-r--r--   0        0        0     1651 2024-03-04 06:00:01.259424 internal-1.0.3/src/internal/exception/internal_exception.py
--rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564151 internal-1.0.3/src/internal/ext/__init__.py
--rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564243 internal-1.0.3/src/internal/ext/amazon/__init__.py
--rw-r--r--   0        0        0      834 2024-01-29 02:46:13.060361 internal-1.0.3/src/internal/ext/amazon/aws/__init__.py
--rw-r--r--   0        0        0      109 2023-12-11 01:32:53.463567 internal-1.0.3/src/internal/ext/amazon/aws/const.py
--rw-r--r--   0        0        0        0 2023-11-10 12:37:53.063137 internal-1.0.3/src/internal/http/__init__.py
--rw-r--r--   0        0        0     1675 2024-04-23 08:00:48.112326 internal-1.0.3/src/internal/http/requests.py
--rw-r--r--   0        0        0     1671 2024-04-24 07:33:39.902568 internal-1.0.3/src/internal/http/responses.py
--rw-r--r--   0        0        0        0 2023-12-29 03:03:59.978251 internal-1.0.3/src/internal/interface/__init__.py
--rw-r--r--   0        0        0      340 2024-01-28 03:32:05.468971 internal-1.0.3/src/internal/interface/base_interface.py
--rw-r--r--   0        0        0        0 2023-11-29 11:18:12.218216 internal-1.0.3/src/internal/model/__init__.py
--rw-r--r--   0        0        0     3002 2024-03-04 06:15:08.376296 internal-1.0.3/src/internal/model/base_model.py
--rw-r--r--   0        0        0     1493 2024-02-13 11:01:26.240348 internal-1.0.3/src/internal/model/operate.py
--rw-r--r--   0        0        0     1509 2024-04-08 11:20:32.745396 internal-1.0.3/src/internal/utils.py
--rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 internal-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776995 internal-1.0.4/README.md
+-rw-r--r--   0        0        0      453 2024-06-01 06:54:36.012818 internal-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776948 internal-1.0.4/src/internal/__init__.py
+-rw-r--r--   0        0        0     1715 2024-04-19 06:23:20.193365 internal-1.0.4/src/internal/base_config.py
+-rw-r--r--   0        0        0     7662 2024-05-16 07:14:46.689593 internal-1.0.4/src/internal/base_factory.py
+-rw-r--r--   0        0        0        0 2024-02-13 10:57:40.969610 internal-1.0.4/src/internal/common_enum/__init__.py
+-rw-r--r--   0        0        0      142 2024-02-13 11:01:26.248123 internal-1.0.4/src/internal/common_enum/contact_type.py
+-rw-r--r--   0        0        0      114 2024-03-19 08:47:41.966209 internal-1.0.4/src/internal/common_enum/event_type.py
+-rw-r--r--   0        0        0      125 2024-02-13 11:01:26.244153 internal-1.0.4/src/internal/common_enum/operator_type.py
+-rw-r--r--   0        0        0      511 2024-04-09 02:21:45.907592 internal-1.0.4/src/internal/common_enum/service_ticket_event_trigger_type.py
+-rw-r--r--   0        0        0     1025 2024-01-28 03:58:24.810115 internal-1.0.4/src/internal/const.py
+-rw-r--r--   0        0        0     2124 2024-05-20 01:23:34.653477 internal-1.0.4/src/internal/database.py
+-rw-r--r--   0        0        0        0 2023-12-15 06:58:26.332564 internal-1.0.4/src/internal/exception/__init__.py
+-rw-r--r--   0        0        0      363 2024-01-28 10:00:28.362441 internal-1.0.4/src/internal/exception/base_exception.py
+-rw-r--r--   0        0        0     1651 2024-03-04 06:00:01.259424 internal-1.0.4/src/internal/exception/internal_exception.py
+-rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564151 internal-1.0.4/src/internal/ext/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564243 internal-1.0.4/src/internal/ext/amazon/__init__.py
+-rw-r--r--   0        0        0      834 2024-01-29 02:46:13.060361 internal-1.0.4/src/internal/ext/amazon/aws/__init__.py
+-rw-r--r--   0        0        0      109 2023-12-11 01:32:53.463567 internal-1.0.4/src/internal/ext/amazon/aws/const.py
+-rw-r--r--   0        0        0        0 2023-11-10 12:37:53.063137 internal-1.0.4/src/internal/http/__init__.py
+-rw-r--r--   0        0        0     1675 2024-04-23 08:00:48.112326 internal-1.0.4/src/internal/http/requests.py
+-rw-r--r--   0        0        0     1671 2024-04-24 07:33:39.902568 internal-1.0.4/src/internal/http/responses.py
+-rw-r--r--   0        0        0        0 2023-12-29 03:03:59.978251 internal-1.0.4/src/internal/interface/__init__.py
+-rw-r--r--   0        0        0      340 2024-01-28 03:32:05.468971 internal-1.0.4/src/internal/interface/base_interface.py
+-rw-r--r--   0        0        0        0 2023-11-29 11:18:12.218216 internal-1.0.4/src/internal/model/__init__.py
+-rw-r--r--   0        0        0     2978 2024-06-01 06:54:36.010974 internal-1.0.4/src/internal/model/base_model.py
+-rw-r--r--   0        0        0     1493 2024-02-13 11:01:26.240348 internal-1.0.4/src/internal/model/operate.py
+-rw-r--r--   0        0        0     1509 2024-04-08 11:20:32.745396 internal-1.0.4/src/internal/utils.py
+-rw-r--r--   0        0        0      624 1970-01-01 00:00:00.000000 internal-1.0.4/PKG-INFO
```

### Comparing `internal-1.0.3/src/internal/base_config.py` & `internal-1.0.4/src/internal/base_config.py`

 * *Files identical despite different names*

### Comparing `internal-1.0.3/src/internal/base_factory.py` & `internal-1.0.4/src/internal/base_factory.py`

 * *Files identical despite different names*

### Comparing `internal-1.0.3/src/internal/const.py` & `internal-1.0.4/src/internal/const.py`

 * *Files identical despite different names*

### Comparing `internal-1.0.3/src/internal/database.py` & `internal-1.0.4/src/internal/database.py`

 * *Files identical despite different names*

### Comparing `internal-1.0.3/src/internal/exception/internal_exception.py` & `internal-1.0.4/src/internal/exception/internal_exception.py`

 * *Files identical despite different names*

### Comparing `internal-1.0.3/src/internal/ext/amazon/aws/__init__.py` & `internal-1.0.4/src/internal/ext/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `internal-1.0.3/src/internal/http/requests.py` & `internal-1.0.4/src/internal/http/requests.py`

 * *Files identical despite different names*

### Comparing `internal-1.0.3/src/internal/http/responses.py` & `internal-1.0.4/src/internal/http/responses.py`

 * *Files identical despite different names*

### Comparing `internal-1.0.3/src/internal/model/base_model.py` & `internal-1.0.4/src/internal/model/base_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             page_data = []
         else:
             page_data = await cls.find(*final_query, ignore_cache=ignore_cache, fetch_links=fetch_links).sort(
                 *final_sort).limit(page_size).skip((page_no - 1) * page_size).to_list()
 
         return page_no, page_size, total_num, page_data
 
-    async def update_wrap(self, schema: Union[Dict, Type[BaseModel]]) -> Tuple[Operate, 'InternalBaseDocument', 'InternalBaseDocument']:
+    async def update_wrap(self, schema: Union[Dict, Type[BaseModel]]) -> Tuple[Operate, 'InternalBaseDocument']:
         if not issubclass(type(schema), dict) and not issubclass(type(schema), BaseModel):
             raise TypeError("Schema must be a subclass of BaseModel or dict")
 
         original_model = self.model_copy(deep=True)
         delta_dict = schema
         if issubclass(type(schema), BaseModel):
             delta_dict = schema.model_dump()
```

### Comparing `internal-1.0.3/src/internal/model/operate.py` & `internal-1.0.4/src/internal/model/operate.py`

 * *Files identical despite different names*

### Comparing `internal-1.0.3/src/internal/utils.py` & `internal-1.0.4/src/internal/utils.py`

 * *Files identical despite different names*

### Comparing `internal-1.0.3/PKG-INFO` & `internal-1.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internal
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Author: Ray
 Author-email: ray@cruisys.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

