# Comparing `tmp/ebest-0.0.6.tar.gz` & `tmp/ebest-1.0.0.tar.gz`

## Comparing `ebest-0.0.6.tar` & `ebest-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 ebest-0.0.6/ebest.pyproj
--rw-r--r--   0        0        0    10211 2020-02-02 00:00:00.000000 ebest-0.0.6/src/ebest/OpenApi.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ebest-0.0.6/src/ebest/__init__.py
--rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 ebest-0.0.6/src/ebest/code_realtime_account.py
--rw-r--r--   0        0        0    12209 2020-02-02 00:00:00.000000 ebest-0.0.6/src/ebest/tr_code_to_path.py
--rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 ebest-0.0.6/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ebest-0.0.6/LICENSE
--rw-r--r--   0        0        0     4617 2020-02-02 00:00:00.000000 ebest-0.0.6/README.md
--rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 ebest-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5018 2020-02-02 00:00:00.000000 ebest-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 ebest-1.0.0/ebest.pyproj
+-rw-r--r--   0        0        0    10462 2020-02-02 00:00:00.000000 ebest-1.0.0/src/ebest/OpenApi.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ebest-1.0.0/src/ebest/__init__.py
+-rw-r--r--   0        0        0      193 2020-02-02 00:00:00.000000 ebest-1.0.0/src/ebest/code_realtime_account.py
+-rw-r--r--   0        0        0    12209 2020-02-02 00:00:00.000000 ebest-1.0.0/src/ebest/tr_code_to_path.py
+-rw-r--r--   0        0        0     6633 2020-02-02 00:00:00.000000 ebest-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 ebest-1.0.0/LICENSE
+-rw-r--r--   0        0        0     4684 2020-02-02 00:00:00.000000 ebest-1.0.0/README.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 ebest-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     5084 2020-02-02 00:00:00.000000 ebest-1.0.0/PKG-INFO
```

### Comparing `ebest-0.0.6/ebest.pyproj` & `ebest-1.0.0/ebest.pyproj`

 * *Files identical despite different names*

### Comparing `ebest-0.0.6/src/ebest/OpenApi.py` & `ebest-1.0.0/src/ebest/OpenApi.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 ﻿import asyncio
 import aiohttp
 import json
 from ebest.tr_code_to_path import tr_code_to_path
 from ebest.code_realtime_account import code_realtime_account
 
-BASE_URL = "https://openapi.ebestsec.co.kr:8080"
-WSS_URL_REAL = "wss://openapi.ebestsec.co.kr:9443/websocket"
-WSS_URL_SIMULATION = "wss://openapi.ebestsec.co.kr:29443/websocket"
+# BASE_URL = "https://openapi.ebestsec.co.kr:8080"
+# WSS_URL_REAL = "wss://openapi.ebestsec.co.kr:9443/websocket"
+# WSS_URL_SIMULATION = "wss://openapi.ebestsec.co.kr:29443/websocket"
+
+# 2024-06-01. 이베스트증권에서 LS증권으로 변경됨.
+BASE_URL = "https://openapi.ls-sec.co.kr:8080"
+WSS_URL_REAL = "wss://openapi.ls-sec.co.kr:9443/websocket"
+WSS_URL_SIMULATION = "wss://openapi.ls-sec.co.kr:29443/websocket"
+
 
 class ResponseValue:
     def __init__(
         self,
         tr_cont: str,
         tr_cont_key: str,
         body: dict,
```

### Comparing `ebest-0.0.6/src/ebest/tr_code_to_path.py` & `ebest-1.0.0/src/ebest/tr_code_to_path.py`

 * *Files identical despite different names*

### Comparing `ebest-0.0.6/.gitignore` & `ebest-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ebest-0.0.6/LICENSE` & `ebest-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ebest-0.0.6/README.md` & `ebest-1.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 ﻿# ebest Package
 
 This is a simple package for eBEST OpenApi.
+이베스트증권에서 LS증권으로 사명변경 (2024.06.01)
 
 ## Installation
 
 ```bash
 pip install ebest
 ```
```

### Comparing `ebest-0.0.6/pyproject.toml` & `ebest-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ebest"
-version = "0.0.6"
+version = "1.0.0"
 authors = [
   { name="teranum", email="teranum@gmail.com" },
 ]
 description = "package for ebest api"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `ebest-0.0.6/PKG-INFO` & `ebest-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ebest
-Version: 0.0.6
+Version: 1.0.0
 Summary: package for ebest api
 Project-URL: Homepage, https://github.com/teranum/python-packages/tree/master/ebest
 Project-URL: Issues, https://github.com/teranum/python-packages/issues
 Author-email: teranum <teranum@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Requires-Python: >=3.8
 Requires-Dist: aiohttp
 Description-Content-Type: text/markdown
 
 ﻿# ebest Package
 
 This is a simple package for eBEST OpenApi.
+이베스트증권에서 LS증권으로 사명변경 (2024.06.01)
 
 ## Installation
 
 ```bash
 pip install ebest
 ```
```

