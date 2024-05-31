# Comparing `tmp/snowflake-0.7.0.tar.gz` & `tmp/snowflake-0.8.0.tar.gz`

## Comparing `snowflake-0.7.0.tar` & `snowflake-0.8.0.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     1317 2020-02-02 00:00:00.000000 snowflake-0.7.0/.gitignore
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 snowflake-0.7.0/README.md
--rw-r--r--   0        0        0     3223 2020-02-02 00:00:00.000000 snowflake-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 snowflake-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 snowflake-0.8.0/.gitignore
+-rw-r--r--   0        0        0    11339 2020-02-02 00:00:00.000000 snowflake-0.8.0/LICENSE
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 snowflake-0.8.0/README.md
+-rw-r--r--   0        0        0     3273 2020-02-02 00:00:00.000000 snowflake-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     1961 2020-02-02 00:00:00.000000 snowflake-0.8.0/PKG-INFO
```

### Comparing `snowflake-0.7.0/.gitignore` & `snowflake-0.8.0/.gitignore`

 * *Files 13% similar despite different names*

```diff
@@ -74,9 +74,9 @@
 
 ##############################
 ## Auto Summary
 ##############################
 docs/source/_autosummary/*
 
 .coverage
-/libs/*/coverage-3.*.xml
+/libs/*/coverage-*.xml
 /.github/workflows/parameters/connections.toml
```

### Comparing `snowflake-0.7.0/README.md` & `snowflake-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `snowflake-0.7.0/pyproject.toml` & `snowflake-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,25 +32,25 @@
     'Topic :: Software Development :: Libraries',
     'Topic :: Software Development :: Libraries :: Application Frameworks',
     'Topic :: Software Development :: Libraries :: Python Modules',
     'Topic :: Scientific/Engineering :: Information Analysis',
 ]
 # The version for the `snowflake` namespace package must be defined
 # statically, since there's no actual code to a namespace package.
-version = '0.7.0'
+version = '0.8.0'
 
 dependencies = [
-    'snowflake.core == 0.7.0',
+    'snowflake.core == 0.8.0',
     'snowflake._legacy',
 ]
 
 [project.optional-dependencies]
 ml = [
     # https://github.com/snowflakedb/snowflake-ml-python/releases
-    'snowflake-ml-python == 1.3.0',
+    'snowflake-ml-python == 1.4.0',
 ]
 
 # [project.urls]
 # 'Home Page' = 'https://docs.snowflake.com/en/developer-guide/snowpark/index'
 # 'Documentation' = 'https://docs.snowflake.com/en/developer-guide/snowpark/python/index.html'
 # 'Source' = 'https://github.com/snowflakedb/snowpark-python'
 # 'Issues' = 'https://github.com/snowflakedb/snowpark-python/issues'
@@ -74,15 +74,18 @@
 [tool.hatch.build.targets.sdist]
 include = [
     'src/snowflake',
     'README.md',
     'pyproject.toml',
 ]
 
-[[tool.hatch.envs.test.matrix]]
+[tool.hatch.envs.test_all]
+template = 'test'
+
+[[tool.hatch.envs.test_all.matrix]]
 python = ['3.8', '3.9', '3.10', '3.11']
 
 # As this is a namespace package, there is nothing to check during precommit,
 # or run tests on.  However, these environments exist to make the top-level
 # monorepo environment scripts more consistent.
 
 [tool.hatch.envs.test]
```

### Comparing `snowflake-0.7.0/PKG-INFO` & `snowflake-0.8.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 Metadata-Version: 2.3
 Name: snowflake
-Version: 0.7.0
+Version: 0.8.0
 Summary: Snowflake Python API
 Author-email: "Snowflake, Inc." <snowflake-python-libraries-dl@snowflake.com>
 License: Apache-2.0
+License-File: LICENSE
 Keywords: Snowflake,analytics,cloud,database,db,warehouse
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
@@ -19,18 +20,18 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: <3.12,>=3.8
-Requires-Dist: snowflake-core==0.7.0
+Requires-Dist: snowflake-core==0.8.0
 Requires-Dist: snowflake-legacy
 Provides-Extra: ml
-Requires-Dist: snowflake-ml-python==1.3.0; extra == 'ml'
+Requires-Dist: snowflake-ml-python==1.4.0; extra == 'ml'
 Description-Content-Type: text/markdown
 
 The Snowflake Python API is the unified Python API across all Snowflake workloads, providing APIs for all Snowflake resources across data engineering, Snowpark, Snowpark ML, and client application workloads.
 
 The `snowflake` package is the PEP 420 namespace parent package for the Snowflake Python API, including Snowpark.  
 Installing snowflake automatically installs all subpackages as dependencies.
```

