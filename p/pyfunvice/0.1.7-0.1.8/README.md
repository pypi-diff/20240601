# Comparing `tmp/pyfunvice-0.1.7.tar.gz` & `tmp/pyfunvice-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfunvice-0.1.7.tar", max compression
+gzip compressed data, was "pyfunvice-0.1.8.tar", max compression
```

## Comparing `pyfunvice-0.1.7.tar` & `pyfunvice-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1553 2024-03-29 16:11:18.430071 pyfunvice-0.1.7/README.md
--rw-r--r--   0        0        0     5766 2024-06-01 05:30:55.429264 pyfunvice-0.1.7/pyfunvice/__init__.py
--rw-r--r--   0        0        0      950 2024-03-26 11:34:48.697182 pyfunvice-0.1.7/pyfunvice/cli.py
--rw-r--r--   0        0        0      314 2024-03-28 09:13:50.645726 pyfunvice-0.1.7/pyfunvice/common_func.py
--rw-r--r--   0        0        0      690 2024-03-26 09:33:56.835152 pyfunvice-0.1.7/pyfunvice/docker_cli.py
--rw-r--r--   0        0        0      709 2024-05-20 06:11:16.293160 pyfunvice-0.1.7/pyfunvice/struct.py
--rw-r--r--   0        0        0      454 2024-06-01 05:37:47.670930 pyfunvice-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2154 1970-01-01 00:00:00.000000 pyfunvice-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1553 2024-03-29 16:11:18.430071 pyfunvice-0.1.8/README.md
+-rw-r--r--   0        0        0     5794 2024-06-01 05:44:06.683543 pyfunvice-0.1.8/pyfunvice/__init__.py
+-rw-r--r--   0        0        0      950 2024-03-26 11:34:48.697182 pyfunvice-0.1.8/pyfunvice/cli.py
+-rw-r--r--   0        0        0      314 2024-03-28 09:13:50.645726 pyfunvice-0.1.8/pyfunvice/common_func.py
+-rw-r--r--   0        0        0      690 2024-03-26 09:33:56.835152 pyfunvice-0.1.8/pyfunvice/docker_cli.py
+-rw-r--r--   0        0        0      709 2024-05-20 06:11:16.293160 pyfunvice-0.1.8/pyfunvice/struct.py
+-rw-r--r--   0        0        0      454 2024-06-01 05:44:32.083584 pyfunvice-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     2154 1970-01-01 00:00:00.000000 pyfunvice-0.1.8/PKG-INFO
```

### Comparing `pyfunvice-0.1.7/README.md` & `pyfunvice-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.7/pyfunvice/__init__.py` & `pyfunvice-0.1.8/pyfunvice/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 app = FastAPI()
 faas_router = APIRouter()
 
 logging.basicConfig(
     level=logging.INFO, format="[%(asctime)s] [%(thread)d] [%(levelname)s] %(message)s"
 )
 
+
 def app_service(path="/", body_type="raw", inparam_type="dict"):
     """
     path : str = "/",                       # http path
     body_type : str = "raw", "form-data"    # http body type
     inparam_type : str = "dict", "flat"     # faas inparam type
     """
 
@@ -41,15 +42,15 @@
                         return ResponseModel(
                             requestId=data.get("requestId"),
                             code="200",
                             message="success",
                             data=result,
                         )
                     except Exception as e:
-                        logging.error(str(e))
+                        logging.exception(f"{str(e)}")
                         return ResponseModel(
                             requestId=data.get("requestId"),
                             code="500",
                             message=str(e),
                             data={},
                         )
 
@@ -71,15 +72,15 @@
                         return ResponseModel(
                             requestId=data.get("requestId"),
                             code="200",
                             message="success",
                             data=result,
                         )
                     except Exception as e:
-                        logging.error(str(e))
+                        logging.exception(f"{str(e)}")
                         return ResponseModel(
                             requestId=data.get("requestId"),
                             code="500",
                             message=str(e),
                             data={},
                         )
             else:
@@ -109,15 +110,15 @@
                     return ResponseModel(
                         requestId=requestId,
                         code="200",
                         message="success",
                         data=result,
                     )
                 except Exception as e:
-                    logging.error(str(e))
+                    logging.exception(f"{str(e)}")
                     return ResponseModel(
                         requestId=requestId,
                         code="500",
                         message=str(e),
                         data={},
                     )
         else:
```

### Comparing `pyfunvice-0.1.7/pyfunvice/cli.py` & `pyfunvice-0.1.8/pyfunvice/cli.py`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.7/pyfunvice/docker_cli.py` & `pyfunvice-0.1.8/pyfunvice/docker_cli.py`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.7/pyfunvice/struct.py` & `pyfunvice-0.1.8/pyfunvice/struct.py`

 * *Files identical despite different names*

### Comparing `pyfunvice-0.1.7/PKG-INFO` & `pyfunvice-0.1.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfunvice
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: 遥奕
 Author-email: jibing.yjb@alibaba-inc.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

