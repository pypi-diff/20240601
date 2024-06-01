# Comparing `tmp/msgpackr_python-0.1.0.tar.gz` & `tmp/msgpackr_python-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msgpackr_python-0.1.0.tar", max compression
+gzip compressed data, was "msgpackr_python-0.1.1.tar", max compression
```

## Comparing `msgpackr_python-0.1.0.tar` & `msgpackr_python-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1063 2024-05-17 17:27:44.483234 msgpackr_python-0.1.0/LICENSE
--rw-r--r--   0        0        0       76 2024-05-17 17:27:44.483234 msgpackr_python-0.1.0/README.md
--rw-r--r--   0        0        0     2138 2024-05-17 18:22:00.907327 msgpackr_python-0.1.0/pyproject.toml
--rwxr-xr-x   0        0        0        0 2024-05-14 15:19:47.000000 msgpackr_python-0.1.0/src/__init__.py
--rwxr-xr-x   0        0        0     1376 2024-05-17 18:03:18.346552 msgpackr_python-0.1.0/src/constants.py
--rwxr-xr-x   0        0        0    10041 2024-05-17 18:12:45.655704 msgpackr_python-0.1.0/src/extension.py
--rw-r--r--   0        0        0        0 2024-05-13 16:05:35.712489 msgpackr_python-0.1.0/src/pack.py
--rwxr-xr-x   0        0        0    17622 2024-05-17 18:14:26.135100 msgpackr_python-0.1.0/src/unpack.py
--rw-r--r--   0        0        0     1056 1970-01-01 00:00:00.000000 msgpackr_python-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-05-17 17:27:44.483234 msgpackr_python-0.1.1/LICENSE
+-rw-r--r--   0        0        0       76 2024-05-17 17:27:44.483234 msgpackr_python-0.1.1/README.md
+-rwxr-xr-x   0        0        0      147 2024-06-01 13:59:35.863727 msgpackr_python-0.1.1/msgpackr/__init__.py
+-rwxr-xr-x   0        0        0     1376 2024-05-17 18:03:18.346552 msgpackr_python-0.1.1/msgpackr/constants.py
+-rwxr-xr-x   0        0        0    10046 2024-06-01 13:50:32.922486 msgpackr_python-0.1.1/msgpackr/extension.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:05:35.712489 msgpackr_python-0.1.1/msgpackr/pack.py
+-rwxr-xr-x   0        0        0    17634 2024-06-01 13:59:55.530923 msgpackr_python-0.1.1/msgpackr/unpack.py
+-rw-r--r--   0        0        0     2143 2024-06-01 14:15:29.843532 msgpackr_python-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1106 1970-01-01 00:00:00.000000 msgpackr_python-0.1.1/PKG-INFO
```

### Comparing `msgpackr_python-0.1.0/LICENSE` & `msgpackr_python-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `msgpackr_python-0.1.0/pyproject.toml` & `msgpackr_python-0.1.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [tool.poetry]
 name = "msgpackr-python"
-version = "0.1.0"
+version = "0.1.1"
 description = "Re-implementation of kriszyp's msgpackr Javascript module"
 license = "MIT"
 authors = ["Aedial <aedial.dev@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/Aedial/msgpackr-python"
 keywords = ["python", "msgpack", "msgpackr"]
 classifiers = [
-    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.7",
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
 ]
-packages = [{include = "src"}]
+packages = [{include = "msgpackr"}]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/Aedial/msgpackr-python/issues"
 
 [tool.poetry.dependencies]
-python = "^3.8.10"
+python = "^3.7.10"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.21.0"
 pylint = "^2.15.5"
 pytest = "^7.3.1"
 
 [tool.poetry.group.docs.dependencies]
```

### Comparing `msgpackr_python-0.1.0/src/constants.py` & `msgpackr_python-0.1.1/msgpackr/constants.py`

 * *Files identical despite different names*

### Comparing `msgpackr_python-0.1.0/src/extension.py` & `msgpackr_python-0.1.1/msgpackr/extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from abc import ABC, abstractmethod
 from datetime import datetime
 from typing import Any, List, Tuple, Union
 
-from src.constants import ARRAY, SKIP, STR, UINT32_STRUCT, UNDEFINED
+from msgpackr.constants import ARRAY, SKIP, STR, UINT32_STRUCT, UNDEFINED
 
 BytesLike = Union[bytes, bytearray, memoryview]
 
 
 class MsgpackExtension(ABC):
     #: The extension type code.
     EXT_TYPE: int = 0
```

### Comparing `msgpackr_python-0.1.0/src/unpack.py` & `msgpackr_python-0.1.1/msgpackr/unpack.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 """
 
 
 from functools import partial
 from logging import Logger
 from typing import Any, Callable, Dict, List, Tuple, Type, Union
 
-from src.constants import *
-from src.extension import (
+from msgpackr.constants import *
+from msgpackr.extension import (
     BundledStrings,
     BundledStringsExtension,
     MsgpackExtension,
     MsgpackExtensionWithPost,
     RecordExtension,
     SetExtension,
     TimestampExtension,
@@ -96,15 +96,15 @@
 
         return inner_cls
 
     return inner if cls is None else inner(cls)
 
 
 # noinspection PyMethodMayBeStatic
-@attach_logger(log_pos=True, log_func=True, log_ext=True, log_bundle=True, log_return=True)
+# @attach_logger(log_pos=True, log_func=True, log_ext=True, log_bundle=True, log_return=True)
 class Unpacker:
     #: The registered extensions.
     extensions: Dict[int, Type[MsgpackExtension]]
     #: Whether to enable bundled strings.
     use_bundled_strings: bool
 
     #: Last bundle used for bundled strings. It needs to be stored there, as the bundle can be initialized anywhere.
```

### Comparing `msgpackr_python-0.1.0/PKG-INFO` & `msgpackr_python-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 Metadata-Version: 2.1
 Name: msgpackr-python
-Version: 0.1.0
+Version: 0.1.1
 Summary: Re-implementation of kriszyp's msgpackr Javascript module
 Home-page: https://github.com/Aedial/msgpackr-python
 License: MIT
 Keywords: python,msgpack,msgpackr
 Author: Aedial
 Author-email: aedial.dev@gmail.com
-Requires-Python: >=3.8.10,<4.0.0
+Requires-Python: >=3.7.10,<4.0.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.7
 Project-URL: Bug Tracker, https://github.com/Aedial/msgpackr-python/issues
 Project-URL: Repository, https://github.com/Aedial/msgpackr-python
 Description-Content-Type: text/markdown
 
 # msgpackr-python
 Re-implementation of kriszyp's msgpackr Javascript module
```

