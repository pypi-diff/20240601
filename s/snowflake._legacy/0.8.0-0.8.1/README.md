# Comparing `tmp/snowflake_legacy-0.8.0.tar.gz` & `tmp/snowflake_legacy-0.8.1.tar.gz`

## Comparing `snowflake_legacy-0.8.0.tar` & `snowflake_legacy-0.8.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/CHANGELOG.md
--rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/snowflake.pth
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/snowflake/_legacy/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/tests/test_legacy_api.py
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/.gitignore
--rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/README.md
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0      203 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.1/CHANGELOG.md
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.1/snowflake.pth
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.1/snowflake/_legacy/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.1/tests/__init__.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.1/tests/test_legacy_api.py
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1271 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.1/README.md
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     2484 2020-02-02 00:00:00.000000 snowflake_legacy-0.8.1/PKG-INFO
```

### Comparing `snowflake_legacy-0.8.0/snowflake.pth` & `snowflake_legacy-0.8.1/snowflake.pth`

 * *Files identical despite different names*

### Comparing `snowflake_legacy-0.8.0/snowflake/_legacy/__init__.py` & `snowflake_legacy-0.8.1/snowflake/_legacy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.8.0'
+__version__ = '0.8.1'
 
 
 from typing import Optional
 
 
 SNOWFLAKE_FILE = '/etc/snowflake'
```

### Comparing `snowflake_legacy-0.8.0/tests/test_legacy_api.py` & `snowflake_legacy-0.8.1/tests/test_legacy_api.py`

 * *Files identical despite different names*

### Comparing `snowflake_legacy-0.8.0/.gitignore` & `snowflake_legacy-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `snowflake_legacy-0.8.0/README.md` & `snowflake_legacy-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `snowflake_legacy-0.8.0/pyproject.toml` & `snowflake_legacy-0.8.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `snowflake_legacy-0.8.0/PKG-INFO` & `snowflake_legacy-0.8.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: snowflake._legacy
-Version: 0.8.0
+Version: 0.8.1
 Summary: You should switch to the snowflake-uuid package
 Author-email: "Snowflake, Inc." <snowflake-python-libraries-dl@snowflake.com>
 License: Apache-2.0
 Keywords: Snowflake,analytics,cloud,database,db,warehouse
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
```

