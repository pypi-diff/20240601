# Comparing `tmp/msgpackr_python-0.1.1.tar.gz` & `tmp/msgpackr_python-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgpackr_python-0.1.1.tar", max compression
+gzip compressed data, was "msgpackr_python-0.1.2.tar", max compression
```

## Comparing `msgpackr_python-0.1.1.tar` & `msgpackr_python-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2024-05-17 17:27:44.483234 msgpackr_python-0.1.1/LICENSE
--rw-r--r--   0        0        0       76 2024-05-17 17:27:44.483234 msgpackr_python-0.1.1/README.md
--rwxr-xr-x   0        0        0      147 2024-06-01 13:59:35.863727 msgpackr_python-0.1.1/msgpackr/__init__.py
--rwxr-xr-x   0        0        0     1376 2024-05-17 18:03:18.346552 msgpackr_python-0.1.1/msgpackr/constants.py
--rwxr-xr-x   0        0        0    10046 2024-06-01 13:50:32.922486 msgpackr_python-0.1.1/msgpackr/extension.py
--rw-r--r--   0        0        0        0 2024-05-13 16:05:35.712489 msgpackr_python-0.1.1/msgpackr/pack.py
--rwxr-xr-x   0        0        0    17634 2024-06-01 13:59:55.530923 msgpackr_python-0.1.1/msgpackr/unpack.py
--rw-r--r--   0        0        0     2143 2024-06-01 14:15:29.843532 msgpackr_python-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 msgpackr_python-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-06-01 14:27:45.464165 msgpackr_python-0.1.2/LICENSE
+-rw-r--r--   0        0        0       76 2024-06-01 14:27:45.464165 msgpackr_python-0.1.2/README.md
+-rwxr-xr-x   0        0        0      147 2024-06-01 14:27:45.464165 msgpackr_python-0.1.2/msgpackr/__init__.py
+-rwxr-xr-x   0        0        0     1376 2024-06-01 14:27:45.464165 msgpackr_python-0.1.2/msgpackr/constants.py
+-rwxr-xr-x   0        0        0    10046 2024-06-01 14:27:45.464165 msgpackr_python-0.1.2/msgpackr/extension.py
+-rw-r--r--   0        0        0        0 2024-06-01 14:27:45.464165 msgpackr_python-0.1.2/msgpackr/pack.py
+-rwxr-xr-x   0        0        0    17443 2024-06-01 14:27:45.464165 msgpackr_python-0.1.2/msgpackr/unpack.py
+-rw-r--r--   0        0        0     2143 2024-06-01 14:27:45.464165 msgpackr_python-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 msgpackr_python-0.1.2/PKG-INFO
```

### Comparing `msgpackr_python-0.1.1/LICENSE` & `msgpackr_python-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `msgpackr_python-0.1.1/msgpackr/constants.py` & `msgpackr_python-0.1.2/msgpackr/constants.py`

 * *Files identical despite different names*

### Comparing `msgpackr_python-0.1.1/msgpackr/extension.py` & `msgpackr_python-0.1.2/msgpackr/extension.py`

 * *Files identical despite different names*

### Comparing `msgpackr_python-0.1.1/msgpackr/unpack.py` & `msgpackr_python-0.1.2/msgpackr/unpack.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,16 +215,14 @@
         size = st.unpack_from(data, pos)[0]
 
         ret_map = {}
         for i in range(size):
             end, key = self.step(data, end)
             end, value = self.step(data, end)
 
-            print(f"map ({i + 1}/{size}) - key: {key}, value: {value}")
-
             ret_map[key] = value
 
         return end, ret_map
 
     CODES_FIXED: Dict[int, Callable[["Unpacker", BytesLike, int], Tuple[int, Any]]] = {
         # BUNDLED_STRINGS is handled separately
         NIL: lambda *args, **kwargs: (0, None),
@@ -265,31 +263,28 @@
         return pos, code
 
     def record(self, code: int, data: BytesLike, pos: int) -> Tuple[int, Union[int, dict]]:
         # if records are disabled, it's just a positive fixint
         if self.records is None:
             return pos, code
 
-        print(f"records: {self.records}")
         identifier1 = code & 0x3F
 
         # TODO: if data[pos + 1] != 0, it's an extended record?
 
         return RecordExtension.post_unpack(self, data, pos, identifier1)
 
     def fixmap(self, code: int, data: BytesLike, pos: int):
         size = code & 0x0F
 
         ret_map = {}
         for i in range(size):
             pos, key = self.step(data, pos)
             pos, value = self.step(data, pos)
 
-            print(f"fixmap ({i + 1}/{size}) - key: {key}, value: {value}")
-
             ret_map[key] = value
 
         return pos, ret_map
 
     def fixarray(self, code: int, data: BytesLike, pos: int):
         size = code & 0x0F
```

### Comparing `msgpackr_python-0.1.1/pyproject.toml` & `msgpackr_python-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "msgpackr-python"
-version = "0.1.1"
+version = "0.1.2"
 description = "Re-implementation of kriszyp's msgpackr Javascript module"
 license = "MIT"
 authors = ["Aedial <aedial.dev@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Aedial/msgpackr-python"
 keywords = ["python", "msgpack", "msgpackr"]
 classifiers = [
```

### Comparing `msgpackr_python-0.1.1/PKG-INFO` & `msgpackr_python-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msgpackr-python
-Version: 0.1.1
+Version: 0.1.2
 Summary: Re-implementation of kriszyp's msgpackr Javascript module
 Home-page: https://github.com/Aedial/msgpackr-python
 License: MIT
 Keywords: python,msgpack,msgpackr
 Author: Aedial
 Author-email: aedial.dev@gmail.com
 Requires-Python: >=3.7.10,<4.0.0
```

