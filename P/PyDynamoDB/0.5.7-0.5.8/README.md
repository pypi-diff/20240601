# Comparing `tmp/PyDynamoDB-0.5.7.tar.gz` & `tmp/PyDynamoDB-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyDynamoDB-0.5.7.tar", last modified: Fri May  3 18:18:08 2024, max compression
+gzip compressed data, was "PyDynamoDB-0.5.8.tar", last modified: Sat Jun  1 01:49:17 2024, max compression
```

## Comparing `PyDynamoDB-0.5.7.tar` & `PyDynamoDB-0.5.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:18:08.320065 PyDynamoDB-0.5.7/
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-03 18:18:08.320065 PyDynamoDB-0.5.7/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:18:08.316065 PyDynamoDB-0.5.7/PyDynamoDB.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7385 2024-05-03 18:18:08.000000 PyDynamoDB-0.5.7/PyDynamoDB.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-03 18:18:08.000000 PyDynamoDB-0.5.7/PyDynamoDB.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:18:08.000000 PyDynamoDB-0.5.7/PyDynamoDB.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-03 18:18:08.000000 PyDynamoDB-0.5.7/PyDynamoDB.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 18:18:08.000000 PyDynamoDB-0.5.7/PyDynamoDB.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-03 18:18:08.000000 PyDynamoDB-0.5.7/PyDynamoDB.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-03 18:18:08.000000 PyDynamoDB-0.5.7/PyDynamoDB.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6314 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:18:08.316065 PyDynamoDB-0.5.7/pydynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    12355 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     9242 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/error.py
--rw-r--r--   0 runner    (1001) docker     (127)    21525 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/executor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/result_set.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:18:08.320065 PyDynamoDB-0.5.7/pydynamodb/sql/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/sql/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    16130 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/sql/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/sql/ddl_alter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/sql/ddl_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/sql/ddl_drop.py
--rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/sql/ddl_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     9886 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/sql/dml_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/sql/dml_sql.py
--rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/sql/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/sql/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/sql/util_sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:18:08.320065 PyDynamoDB-0.5.7/pydynamodb/sqlalchemy_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/sqlalchemy_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13126 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/sqlalchemy_dynamodb/pydynamodb.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 18:18:08.320065 PyDynamoDB-0.5.7/pydynamodb/superset_dynamodb/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/superset_dynamodb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/superset_dynamodb/dml_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/superset_dynamodb/helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/superset_dynamodb/pydnamodb.py
--rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/superset_dynamodb/querydb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/superset_dynamodb/querydb_sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/pydynamodb/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-03 18:18:08.320065 PyDynamoDB-0.5.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-05-03 18:18:01.000000 PyDynamoDB-0.5.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:17.295129 PyDynamoDB-0.5.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-06-01 01:49:17.295129 PyDynamoDB-0.5.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:17.291129 PyDynamoDB-0.5.8/PyDynamoDB.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7395 2024-06-01 01:49:17.000000 PyDynamoDB-0.5.8/PyDynamoDB.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-06-01 01:49:17.000000 PyDynamoDB-0.5.8/PyDynamoDB.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:49:17.000000 PyDynamoDB-0.5.8/PyDynamoDB.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-06-01 01:49:17.000000 PyDynamoDB-0.5.8/PyDynamoDB.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:49:17.000000 PyDynamoDB-0.5.8/PyDynamoDB.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-06-01 01:49:17.000000 PyDynamoDB-0.5.8/PyDynamoDB.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-01 01:49:17.000000 PyDynamoDB-0.5.8/PyDynamoDB.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:17.291129 PyDynamoDB-0.5.8/pydynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)     1667 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5157 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12355 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9242 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6857 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21525 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7568 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/result_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:17.295129 PyDynamoDB-0.5.8/pydynamodb/sql/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/sql/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16131 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/sql/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12750 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/sql/ddl_alter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6029 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/sql/ddl_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/sql/ddl_drop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8346 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/sql/ddl_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9886 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/sql/dml_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4556 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/sql/dml_sql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/sql/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/sql/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/sql/util_sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:17.295129 PyDynamoDB-0.5.8/pydynamodb/sqlalchemy_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/sqlalchemy_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13118 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/sqlalchemy_dynamodb/pydynamodb.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:49:17.295129 PyDynamoDB-0.5.8/pydynamodb/superset_dynamodb/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/superset_dynamodb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/superset_dynamodb/dml_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4019 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/superset_dynamodb/helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/superset_dynamodb/pydnamodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11222 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/superset_dynamodb/querydb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/superset_dynamodb/querydb_sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3340 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/pydynamodb/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-06-01 01:49:17.295129 PyDynamoDB-0.5.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2147 2024-06-01 01:49:09.000000 PyDynamoDB-0.5.8/setup.py
```

### Comparing `PyDynamoDB-0.5.7/LICENSE` & `PyDynamoDB-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/PKG-INFO` & `PyDynamoDB-0.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDynamoDB
-Version: 0.5.7
+Version: 0.5.8
 Summary: Python DB API 2.0 (PEP 249) client for Amazon DynamoDB
 Home-page: https://github.com/passren/PyDynamoDB
 Author: Peng Ren
 Author-email: passren9099@hotmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/passren/PyDynamoDB/wiki
 Project-URL: Source, https://github.com/passren/PyDynamoDB
@@ -94,15 +94,15 @@
 * Compatible for Superset SQL Lab and graphing
 
 
 Requirements
 --------------
 * Python
 
-  - CPython 3.7 3.8 3.9 3.10
+  - CPython 3.7 3.8 3.9 3.10 3.11 3.12
 
 Dependencies
 --------------
 * Boto3 (Python SDK for AWS Services)
 
   - boto3 >= 1.21.0
   - botocore >= 1.24.7
```

### Comparing `PyDynamoDB-0.5.7/PyDynamoDB.egg-info/PKG-INFO` & `PyDynamoDB-0.5.8/PyDynamoDB.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyDynamoDB
-Version: 0.5.7
+Version: 0.5.8
 Summary: Python DB API 2.0 (PEP 249) client for Amazon DynamoDB
 Home-page: https://github.com/passren/PyDynamoDB
 Author: Peng Ren
 Author-email: passren9099@hotmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/passren/PyDynamoDB/wiki
 Project-URL: Source, https://github.com/passren/PyDynamoDB
@@ -94,15 +94,15 @@
 * Compatible for Superset SQL Lab and graphing
 
 
 Requirements
 --------------
 * Python
 
-  - CPython 3.7 3.8 3.9 3.10
+  - CPython 3.7 3.8 3.9 3.10 3.11 3.12
 
 Dependencies
 --------------
 * Boto3 (Python SDK for AWS Services)
 
   - boto3 >= 1.21.0
   - botocore >= 1.24.7
```

### Comparing `PyDynamoDB-0.5.7/PyDynamoDB.egg-info/SOURCES.txt` & `PyDynamoDB-0.5.8/PyDynamoDB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/README.rst` & `PyDynamoDB-0.5.8/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 * Compatible for Superset SQL Lab and graphing
 
 
 Requirements
 --------------
 * Python
 
-  - CPython 3.7 3.8 3.9 3.10
+  - CPython 3.7 3.8 3.9 3.10 3.11 3.12
 
 Dependencies
 --------------
 * Boto3 (Python SDK for AWS Services)
 
   - boto3 >= 1.21.0
   - botocore >= 1.24.7
```

### Comparing `PyDynamoDB-0.5.7/pydynamodb/__init__.py` & `PyDynamoDB-0.5.8/pydynamodb/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import TYPE_CHECKING, FrozenSet
 
 from .error import *  # noqa
 
 if TYPE_CHECKING:
     from .connection import Connection
 
-__version__: str = "0.5.7"
+__version__: str = "0.5.8"
 
 # Globals https://www.python.org/dev/peps/pep-0249/#globals
 apilevel: str = "2.0"
 threadsafety: int = 3
 paramstyle: str = "qmark"
```

### Comparing `PyDynamoDB-0.5.7/pydynamodb/common.py` & `PyDynamoDB-0.5.8/pydynamodb/common.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/connection.py` & `PyDynamoDB-0.5.8/pydynamodb/connection.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/converter.py` & `PyDynamoDB-0.5.8/pydynamodb/converter.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/cursor.py` & `PyDynamoDB-0.5.8/pydynamodb/cursor.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/error.py` & `PyDynamoDB-0.5.8/pydynamodb/error.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/executor.py` & `PyDynamoDB-0.5.8/pydynamodb/executor.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/model.py` & `PyDynamoDB-0.5.8/pydynamodb/model.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/result_set.py` & `PyDynamoDB-0.5.8/pydynamodb/result_set.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/sql/base.py` & `PyDynamoDB-0.5.8/pydynamodb/sql/base.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/sql/common.py` & `PyDynamoDB-0.5.8/pydynamodb/sql/common.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 import re
-from .util import strtobool
+from ..util import strtobool
 from pyparsing import (
     Word,
     nums,
     alphanums,
     Combine,
     Regex,
     CaselessKeyword,
```

### Comparing `PyDynamoDB-0.5.7/pydynamodb/sql/ddl_alter.py` & `PyDynamoDB-0.5.8/pydynamodb/sql/ddl_alter.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/sql/ddl_create.py` & `PyDynamoDB-0.5.8/pydynamodb/sql/ddl_create.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/sql/ddl_drop.py` & `PyDynamoDB-0.5.8/pydynamodb/sql/ddl_drop.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/sql/ddl_sql.py` & `PyDynamoDB-0.5.8/pydynamodb/sql/ddl_sql.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/sql/dml_select.py` & `PyDynamoDB-0.5.8/pydynamodb/sql/dml_select.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/sql/dml_sql.py` & `PyDynamoDB-0.5.8/pydynamodb/sql/dml_sql.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/sql/parser.py` & `PyDynamoDB-0.5.8/pydynamodb/sql/parser.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/sql/util_sql.py` & `PyDynamoDB-0.5.8/pydynamodb/sql/util_sql.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/sqlalchemy_dynamodb/pydynamodb.py` & `PyDynamoDB-0.5.8/pydynamodb/sqlalchemy_dynamodb/pydynamodb.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 import re
-from distutils.util import strtobool
+from ..util import strtobool
 
 import pydynamodb
 from pydynamodb.error import OperationalError
 from ..sql.common import RESERVED_WORDS
 
 import botocore
 from sqlalchemy import exc, types, util
```

### Comparing `PyDynamoDB-0.5.7/pydynamodb/superset_dynamodb/dml_select.py` & `PyDynamoDB-0.5.8/pydynamodb/superset_dynamodb/dml_select.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/superset_dynamodb/helper.py` & `PyDynamoDB-0.5.8/pydynamodb/superset_dynamodb/helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     DEFAULT_QUERYDB_TYPE,
     DEFAULT_QUERYDB_URL,
     DEFAULT_QUERYDB_LOAD_BATCH_SIZE,
     DEFAULT_QUERYDB_EXPIRE_TIME,
     DEFAULT_QUERYDB_PURGE_TIME,
 )
 from ..model import Statement
-from ..sql.util import strtobool
+from ..util import strtobool
 from ..error import NotSupportedError, OperationalError
 from .querydb_sqlite import SqliteMemQueryDB, SqliteFileQueryDB
 
 _logger = logging.getLogger(__name__)  # type: ignore
 
 
 class QueryDBHelper(metaclass=ABCMeta):
```

### Comparing `PyDynamoDB-0.5.7/pydynamodb/superset_dynamodb/pydnamodb.py` & `PyDynamoDB-0.5.8/pydynamodb/superset_dynamodb/pydnamodb.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/superset_dynamodb/querydb.py` & `PyDynamoDB-0.5.8/pydynamodb/superset_dynamodb/querydb.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/superset_dynamodb/querydb_sqlite.py` & `PyDynamoDB-0.5.8/pydynamodb/superset_dynamodb/querydb_sqlite.py`

 * *Files identical despite different names*

### Comparing `PyDynamoDB-0.5.7/pydynamodb/util.py` & `PyDynamoDB-0.5.8/pydynamodb/util.py`

 * *Files 23% similar despite different names*

```diff
@@ -21,14 +21,31 @@
     def _wrapper(*args, **kwargs):
         with _lock:
             return wrapped(*args, **kwargs)
 
     return _wrapper
 
 
+# Copy from distutils.util to remove dependency
+def strtobool(val):
+    """Convert a string representation of truth to true (1) or false (0).
+
+    True values are 'y', 'yes', 't', 'true', 'on', and '1'; false values
+    are 'n', 'no', 'f', 'false', 'off', and '0'.  Raises ValueError if
+    'val' is anything else.
+    """
+    val = val.lower()
+    if val in ("y", "yes", "t", "true", "on", "1"):
+        return 1
+    elif val in ("n", "no", "f", "false", "off", "0"):
+        return 0
+    else:
+        raise ValueError("invalid truth value %r" % (val,))
+
+
 def flatten_dict(
     d: Dict[str, Any], parent_key: str = "", separator: str = "."
 ) -> Dict[str, Any]:
     items = list()
     for key, val in d.items():
         new_key = parent_key + separator + key if parent_key else key
         if isinstance(val, MutableMapping):
```

### Comparing `PyDynamoDB-0.5.7/setup.py` & `PyDynamoDB-0.5.8/setup.py`

 * *Files identical despite different names*

