# Comparing `tmp/pyfunvice-0.1.6.tar.gz` & `tmp/pyfunvice-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfunvice-0.1.6.tar", max compression
+gzip compressed data, was "pyfunvice-0.1.7.tar", max compression
```

## Comparing `pyfunvice-0.1.6.tar` & `pyfunvice-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1553 2024-03-29 16:11:18.430071 pyfunvice-0.1.6/README.md
--rw-r--r--   0        0        0     5506 2024-05-20 06:11:22.735172 pyfunvice-0.1.6/pyfunvice/__init__.py
--rw-r--r--   0        0        0      950 2024-03-26 11:34:48.697182 pyfunvice-0.1.6/pyfunvice/cli.py
--rw-r--r--   0        0        0      314 2024-03-28 09:13:50.645726 pyfunvice-0.1.6/pyfunvice/common_func.py
--rw-r--r--   0        0        0      690 2024-03-26 09:33:56.835152 pyfunvice-0.1.6/pyfunvice/docker_cli.py
--rw-r--r--   0        0        0      709 2024-05-20 06:11:16.293160 pyfunvice-0.1.6/pyfunvice/struct.py
--rw-r--r--   0        0        0      454 2024-05-20 06:35:06.675675 pyfunvice-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2154 1970-01-01 00:00:00.000000 pyfunvice-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1553 2024-03-29 16:11:18.430071 pyfunvice-0.1.7/README.md
+-rw-r--r--   0        0        0     5766 2024-06-01 05:30:55.429264 pyfunvice-0.1.7/pyfunvice/__init__.py
+-rw-r--r--   0        0        0      950 2024-03-26 11:34:48.697182 pyfunvice-0.1.7/pyfunvice/cli.py
+-rw-r--r--   0        0        0      314 2024-03-28 09:13:50.645726 pyfunvice-0.1.7/pyfunvice/common_func.py
+-rw-r--r--   0        0        0      690 2024-03-26 09:33:56.835152 pyfunvice-0.1.7/pyfunvice/docker_cli.py
+-rw-r--r--   0        0        0      709 2024-05-20 06:11:16.293160 pyfunvice-0.1.7/pyfunvice/struct.py
+-rw-r--r--   0        0        0      454 2024-06-01 05:37:47.670930 pyfunvice-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2154 1970-01-01 00:00:00.000000 pyfunvice-0.1.7/PKG-INFO
```

### Comparing `pyfunvice-0.1.6/README.md` & `pyfunvice-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.6/pyfunvice/__init__.py` & `pyfunvice-0.1.7/pyfunvice/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,21 +2,25 @@
 from gunicorn.arbiter import Arbiter
 from gunicorn.workers.base import Worker
 from fastapi import APIRouter, FastAPI, File, Request, UploadFile
 from fastapi.params import Form
 from functools import wraps
 import inspect
 import aiofiles
+import logging
 
 from pyfunvice.common_func import delete_file
 from pyfunvice.struct import ResponseModel
 
 app = FastAPI()
 faas_router = APIRouter()
 
+logging.basicConfig(
+    level=logging.INFO, format="[%(asctime)s] [%(thread)d] [%(levelname)s] %(message)s"
+)
 
 def app_service(path="/", body_type="raw", inparam_type="dict"):
     """
     path : str = "/",                       # http path
     body_type : str = "raw", "form-data"    # http body type
     inparam_type : str = "dict", "flat"     # faas inparam type
     """
@@ -37,14 +41,15 @@
                         return ResponseModel(
                             requestId=data.get("requestId"),
                             code="200",
                             message="success",
                             data=result,
                         )
                     except Exception as e:
+                        logging.error(str(e))
                         return ResponseModel(
                             requestId=data.get("requestId"),
                             code="500",
                             message=str(e),
                             data={},
                         )
 
@@ -66,14 +71,15 @@
                         return ResponseModel(
                             requestId=data.get("requestId"),
                             code="200",
                             message="success",
                             data=result,
                         )
                     except Exception as e:
+                        logging.error(str(e))
                         return ResponseModel(
                             requestId=data.get("requestId"),
                             code="500",
                             message=str(e),
                             data={},
                         )
             else:
@@ -103,14 +109,15 @@
                     return ResponseModel(
                         requestId=requestId,
                         code="200",
                         message="success",
                         data=result,
                     )
                 except Exception as e:
+                    logging.error(str(e))
                     return ResponseModel(
                         requestId=requestId,
                         code="500",
                         message=str(e),
                         data={},
                     )
         else:
```

### Comparing `pyfunvice-0.1.6/pyfunvice/cli.py` & `pyfunvice-0.1.7/pyfunvice/cli.py`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.6/pyfunvice/docker_cli.py` & `pyfunvice-0.1.7/pyfunvice/docker_cli.py`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.6/pyfunvice/struct.py` & `pyfunvice-0.1.7/pyfunvice/struct.py`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.6/PKG-INFO` & `pyfunvice-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfunvice
-Version: 0.1.6
+Version: 0.1.7
 Summary: 
 Author: 遥奕
 Author-email: jibing.yjb@alibaba-inc.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

