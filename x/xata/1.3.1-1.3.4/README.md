# Comparing `tmp/xata-1.3.1.tar.gz` & `tmp/xata-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xata-1.3.1.tar", max compression
+gzip compressed data, was "xata-1.3.4.tar", max compression
```

## Comparing `xata-1.3.1.tar` & `xata-1.3.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-03-03 17:34:21.213028 xata-1.3.1/LICENSE
--rw-r--r--   0        0        0       45 2024-03-03 17:34:21.213028 xata-1.3.1/NOTICE
--rw-r--r--   0        0        0     1026 2024-03-03 17:34:21.213028 xata-1.3.1/README_PYPI.md
--rw-r--r--   0        0        0      827 2024-03-03 17:34:21.233028 xata-1.3.1/pyproject.toml
--rw-r--r--   0        0        0      873 2024-03-03 17:34:21.261028 xata-1.3.1/xata/__init__.py
--rw-r--r--   0        0        0      769 2024-03-03 17:34:21.261028 xata-1.3.1/xata/api/__init__.py
--rw-r--r--   0        0        0     2995 2024-03-03 17:34:21.261028 xata-1.3.1/xata/api/authentication.py
--rw-r--r--   0        0        0    14138 2024-03-03 17:34:21.261028 xata-1.3.1/xata/api/branch.py
--rw-r--r--   0        0        0     8389 2024-03-03 17:34:21.261028 xata-1.3.1/xata/api/databases.py
--rw-r--r--   0        0        0    12663 2024-03-03 17:34:21.261028 xata-1.3.1/xata/api/files.py
--rw-r--r--   0        0        0     6697 2024-03-03 17:34:21.261028 xata-1.3.1/xata/api/invites.py
--rw-r--r--   0        0        0    13167 2024-03-03 17:34:21.261028 xata-1.3.1/xata/api/migrations.py
--rw-r--r--   0        0        0     4596 2024-03-03 17:34:21.261028 xata-1.3.1/xata/api/oauth.py
--rw-r--r--   0        0        0    13830 2024-03-03 17:34:21.261028 xata-1.3.1/xata/api/records.py
--rw-r--r--   0        0        0    37866 2024-03-03 17:34:21.261028 xata-1.3.1/xata/api/search_and_filter.py
--rw-r--r--   0        0        0     2613 2024-03-03 17:34:21.261028 xata-1.3.1/xata/api/sql.py
--rw-r--r--   0        0        0    13799 2024-03-03 17:34:21.261028 xata-1.3.1/xata/api/table.py
--rw-r--r--   0        0        0     2771 2024-03-03 17:34:21.261028 xata-1.3.1/xata/api/users.py
--rw-r--r--   0        0        0     8253 2024-03-03 17:34:21.261028 xata-1.3.1/xata/api/workspaces.py
--rw-r--r--   0        0        0     4310 2024-03-03 17:34:21.261028 xata-1.3.1/xata/api_request.py
--rw-r--r--   0        0        0     3651 2024-03-03 17:34:21.261028 xata-1.3.1/xata/api_response.py
--rw-r--r--   0        0        0    13632 2024-03-03 17:34:21.261028 xata-1.3.1/xata/client.py
--rw-r--r--   0        0        0     1188 2024-03-03 17:34:21.261028 xata-1.3.1/xata/errors.py
--rw-r--r--   0        0        0    18933 2024-03-03 17:34:21.261028 xata-1.3.1/xata/helpers.py
--rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 xata-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-28 11:55:57.950339 xata-1.3.4/LICENSE
+-rw-r--r--   0        0        0       45 2024-05-28 11:55:57.950339 xata-1.3.4/NOTICE
+-rw-r--r--   0        0        0     1026 2024-05-28 11:55:57.950339 xata-1.3.4/README_PYPI.md
+-rw-r--r--   0        0        0      832 2024-05-28 11:55:57.970340 xata-1.3.4/pyproject.toml
+-rw-r--r--   0        0        0      873 2024-05-28 11:55:57.998340 xata-1.3.4/xata/__init__.py
+-rw-r--r--   0        0        0      769 2024-05-28 11:55:57.998340 xata-1.3.4/xata/api/__init__.py
+-rw-r--r--   0        0        0     2995 2024-05-28 11:55:57.998340 xata-1.3.4/xata/api/authentication.py
+-rw-r--r--   0        0        0    14138 2024-05-28 11:55:57.998340 xata-1.3.4/xata/api/branch.py
+-rw-r--r--   0        0        0     8389 2024-05-28 11:55:57.998340 xata-1.3.4/xata/api/databases.py
+-rw-r--r--   0        0        0    12663 2024-05-28 11:55:57.998340 xata-1.3.4/xata/api/files.py
+-rw-r--r--   0        0        0     6697 2024-05-28 11:55:57.998340 xata-1.3.4/xata/api/invites.py
+-rw-r--r--   0        0        0    13167 2024-05-28 11:55:57.998340 xata-1.3.4/xata/api/migrations.py
+-rw-r--r--   0        0        0     4596 2024-05-28 11:55:57.998340 xata-1.3.4/xata/api/oauth.py
+-rw-r--r--   0        0        0    13830 2024-05-28 11:55:57.998340 xata-1.3.4/xata/api/records.py
+-rw-r--r--   0        0        0    37866 2024-05-28 11:55:57.998340 xata-1.3.4/xata/api/search_and_filter.py
+-rw-r--r--   0        0        0     2613 2024-05-28 11:55:57.998340 xata-1.3.4/xata/api/sql.py
+-rw-r--r--   0        0        0    13799 2024-05-28 11:55:57.998340 xata-1.3.4/xata/api/table.py
+-rw-r--r--   0        0        0     2771 2024-05-28 11:55:57.998340 xata-1.3.4/xata/api/users.py
+-rw-r--r--   0        0        0     8253 2024-05-28 11:55:57.998340 xata-1.3.4/xata/api/workspaces.py
+-rw-r--r--   0        0        0     4310 2024-05-28 11:55:57.998340 xata-1.3.4/xata/api_request.py
+-rw-r--r--   0        0        0     3651 2024-05-28 11:55:57.998340 xata-1.3.4/xata/api_response.py
+-rw-r--r--   0        0        0    13632 2024-05-28 11:55:57.998340 xata-1.3.4/xata/client.py
+-rw-r--r--   0        0        0     1188 2024-05-28 11:55:57.998340 xata-1.3.4/xata/errors.py
+-rw-r--r--   0        0        0    18933 2024-05-28 11:55:57.998340 xata-1.3.4/xata/helpers.py
+-rw-r--r--   0        0        0     1830 1970-01-01 00:00:00.000000 xata-1.3.4/PKG-INFO
```

### Comparing `xata-1.3.1/LICENSE` & `xata-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/README_PYPI.md` & `xata-1.3.4/README_PYPI.md`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/pyproject.toml` & `xata-1.3.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xata"
-version = "1.3.1"
+version = "1.3.4"
 description = "Python SDK for Xata.io"
 authors = ["Xata <support@xata.io>"]
 license = "Apache-2.0"
 readme = "README_PYPI.md"
 documentation = "https://xata-py.readthedocs.io"
 
 [tool.poetry.dependencies]
@@ -13,15 +13,15 @@
 python-dotenv = ">=0.21,<2.0"
 orjson = "^3.8.1"
 deprecation = "^2.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
-black = "^22.12.0"
+black = ">=22.12,<25.0"
 flake8 = "^5.0.4"
 pre-commit = "^2.21.0"
 isort = "^5.12.0"
 flake8-bugbear = "^22.10.27"
 flake8-annotations = "^2.9.1"
 pdoc3 = "^0.10.0"
 Faker = "^17.0.0"
```

### Comparing `xata-1.3.1/xata/__init__.py` & `xata-1.3.4/xata/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/api/__init__.py` & `xata-1.3.4/xata/api/__init__.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/api/authentication.py` & `xata-1.3.4/xata/api/authentication.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/api/branch.py` & `xata-1.3.4/xata/api/branch.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/api/databases.py` & `xata-1.3.4/xata/api/databases.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/api/files.py` & `xata-1.3.4/xata/api/files.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/api/invites.py` & `xata-1.3.4/xata/api/invites.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/api/migrations.py` & `xata-1.3.4/xata/api/migrations.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/api/oauth.py` & `xata-1.3.4/xata/api/oauth.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/api/records.py` & `xata-1.3.4/xata/api/records.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/api/search_and_filter.py` & `xata-1.3.4/xata/api/search_and_filter.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/api/sql.py` & `xata-1.3.4/xata/api/sql.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/api/table.py` & `xata-1.3.4/xata/api/table.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/api/users.py` & `xata-1.3.4/xata/api/users.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/api/workspaces.py` & `xata-1.3.4/xata/api/workspaces.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/api_request.py` & `xata-1.3.4/xata/api_request.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/api_response.py` & `xata-1.3.4/xata/api_response.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/client.py` & `xata-1.3.4/xata/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 from .api.sql import Sql
 from .api.table import Table
 from .api.users import Users
 from .api.workspaces import Workspaces
 
 # TODO this is a manual task, to keep in sync with pyproject.toml
 # could/should be automated to keep in sync
-__version__ = "1.3.1"
+__version__ = "1.3.4"
 
 PERSONAL_API_KEY_LOCATION = "~/.config/xata/key"
 DEFAULT_DATA_PLANE_DOMAIN = "xata.sh"
 DEFAULT_CONTROL_PLANE_DOMAIN = "api.xata.io"
 DEFAULT_REGION = "us-east-1"
 DEFAULT_BRANCH_NAME = "main"
 CONFIG_LOCATION = ".xatarc"
```

### Comparing `xata-1.3.1/xata/errors.py` & `xata-1.3.4/xata/errors.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/xata/helpers.py` & `xata-1.3.4/xata/helpers.py`

 * *Files identical despite different names*

### Comparing `xata-1.3.1/PKG-INFO` & `xata-1.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xata
-Version: 1.3.1
+Version: 1.3.4
 Summary: Python SDK for Xata.io
 License: Apache-2.0
 Author: Xata
 Author-email: support@xata.io
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

