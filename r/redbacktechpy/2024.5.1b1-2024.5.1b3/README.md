# Comparing `tmp/redbacktechpy-2024.5.1b1.tar.gz` & `tmp/redbacktechpy-2024.5.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbacktechpy-2024.5.1b1.tar", last modified: Sat Jun  1 19:30:08 2024, max compression
+gzip compressed data, was "redbacktechpy-2024.5.1b3.tar", last modified: Sat Jun  1 19:52:56 2024, max compression
```

## Comparing `redbacktechpy-2024.5.1b1.tar` & `redbacktechpy-2024.5.1b3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:30:08.044645 redbacktechpy-2024.5.1b1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 19:30:03.000000 redbacktechpy-2024.5.1b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 19:30:08.044645 redbacktechpy-2024.5.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-01 19:30:03.000000 redbacktechpy-2024.5.1b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 19:30:08.044645 redbacktechpy-2024.5.1b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:30:08.040645 redbacktechpy-2024.5.1b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:30:08.044645 redbacktechpy-2024.5.1b1/src/redbacktechpy/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 19:30:03.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-01 19:30:03.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-01 19:30:03.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-01 19:30:03.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    50853 2024-06-01 19:30:03.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy/redbacktech_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-01 19:30:03.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy/str_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:30:08.044645 redbacktechpy-2024.5.1b1/src/redbacktechpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 19:30:08.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-01 19:30:08.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 19:30:08.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 19:30:08.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 19:30:08.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:52:56.339621 redbacktechpy-2024.5.1b3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 19:52:52.000000 redbacktechpy-2024.5.1b3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 19:52:56.339621 redbacktechpy-2024.5.1b3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-01 19:52:52.000000 redbacktechpy-2024.5.1b3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 19:52:56.339621 redbacktechpy-2024.5.1b3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:52:56.335621 redbacktechpy-2024.5.1b3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:52:56.339621 redbacktechpy-2024.5.1b3/src/redbacktechpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 19:52:52.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-01 19:52:52.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-01 19:52:52.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-01 19:52:52.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50856 2024-06-01 19:52:52.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy/redbacktech_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-01 19:52:52.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy/str_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:52:56.339621 redbacktechpy-2024.5.1b3/src/redbacktechpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 19:52:56.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-01 19:52:56.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 19:52:56.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 19:52:56.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 19:52:56.000000 redbacktechpy-2024.5.1b3/src/redbacktechpy.egg-info/top_level.txt
```

### Comparing `redbacktechpy-2024.5.1b1/LICENSE` & `redbacktechpy-2024.5.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b1/PKG-INFO` & `redbacktechpy-2024.5.1b3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.1b1
+Version: 2024.5.1b3
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `redbacktechpy-2024.5.1b1/pyproject.toml` & `redbacktechpy-2024.5.1b3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "redbacktechpy"
-version = "2024.05.1b1"
+version = "2024.05.1b3"
 authors = [
   { name="Chris Abberley", email="unlisted@gmail.com" },
 ]
 description = "Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
```

### Comparing `redbacktechpy-2024.5.1b1/src/redbacktechpy/__init__.py` & `redbacktechpy-2024.5.1b3/src/redbacktechpy/__init__.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b1/src/redbacktechpy/constants.py` & `redbacktechpy-2024.5.1b3/src/redbacktechpy/constants.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b1/src/redbacktechpy/model.py` & `redbacktechpy-2024.5.1b3/src/redbacktechpy/model.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b1/src/redbacktechpy/redbacktech_client.py` & `redbacktechpy-2024.5.1b3/src/redbacktechpy/redbacktech_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 from aiohttp import ClientResponse, ClientSession
 from typing import Any
 import asyncio
 from datetime import datetime, timedelta, timezone
 from bs4 import BeautifulSoup
 import logging
 
-from constants import (
+from .constants import (
     BaseUrl, 
     Endpoint, 
     Header,
     InverterOperationType,
     TIMEOUT,
     AUTH_ERROR_CODES,
     DEVICEINFOREFRESH,
 )
 
-from model import (
+from .model import (
     Inverters,
     Batterys,
     RedbackTechData,
     RedbackEntitys,
     DeviceInfo,
 )
-from exceptions import (
+from .exceptions import (
         AuthError, 
         RedbackTechClientError,
 )
 
 LOGGER = logging.getLogger(__name__)
 
 class RedbackTechClient:
```

### Comparing `redbacktechpy-2024.5.1b1/src/redbacktechpy/str_enum.py` & `redbacktechpy-2024.5.1b3/src/redbacktechpy/str_enum.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.1b1/src/redbacktechpy.egg-info/PKG-INFO` & `redbacktechpy-2024.5.1b3/src/redbacktechpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.1b1
+Version: 2024.5.1b3
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

