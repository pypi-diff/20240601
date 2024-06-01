# Comparing `tmp/pydrawise-2024.4.1.tar.gz` & `tmp/pydrawise-2024.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydrawise-2024.4.1.tar", last modified: Tue Apr 30 12:04:31 2024, max compression
+gzip compressed data, was "pydrawise-2024.6.1.tar", last modified: Sat Jun  1 14:20:06 2024, max compression
```

## Comparing `pydrawise-2024.4.1.tar` & `pydrawise-2024.6.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.066710 pydrawise-2024.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.062710 pydrawise-2024.4.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.062710 pydrawise-2024.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.github/workflows/publish-python.yml
--rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.062710 pydrawise-2024.4.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-30 12:04:31.066710 pydrawise-2024.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.062710 pydrawise-2024.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.062710 pydrawise-2024.4.1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/docs/reference/index.md
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/docs/reference/schema.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/mkdocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.062710 pydrawise-2024.4.1/pydrawise/
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-30 12:04:30.000000 pydrawise-2024.4.1/pydrawise/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    17412 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    55590 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/hydrawise.graphql
--rw-r--r--   0 runner    (1001) docker     (127)    12815 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    16653 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pydrawise/schema_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.066710 pydrawise-2024.4.1/pydrawise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-04-30 12:04:31.000000 pydrawise-2024.4.1/pydrawise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-30 12:04:31.000000 pydrawise-2024.4.1/pydrawise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:04:31.000000 pydrawise-2024.4.1/pydrawise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-30 12:04:31.000000 pydrawise-2024.4.1/pydrawise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-30 12:04:31.000000 pydrawise-2024.4.1/pydrawise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 12:04:30.000000 pydrawise-2024.4.1/pydrawise.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.066710 pydrawise-2024.4.1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (127)      324 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/scripts/setup
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 12:04:31.066710 pydrawise-2024.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:31.066710 pydrawise-2024.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    19840 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    25747 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/tests/test_legacy.py
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-30 12:04:19.000000 pydrawise-2024.4.1/tests/test_schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.448162 pydrawise-2024.6.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.440162 pydrawise-2024.6.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.440162 pydrawise-2024.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.github/workflows/publish-python.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.444162 pydrawise-2024.6.1/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-06-01 14:20:06.448162 pydrawise-2024.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.444162 pydrawise-2024.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.444162 pydrawise-2024.6.1/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/docs/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/docs/reference/schema.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.444162 pydrawise-2024.6.1/pydrawise/
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-06-01 14:20:06.000000 pydrawise-2024.6.1/pydrawise/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2992 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4187 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55590 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/hydrawise.graphql
+-rw-r--r--   0 runner    (1001) docker     (127)    12815 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    17100 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4068 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pydrawise/schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.448162 pydrawise-2024.6.1/pydrawise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2702 2024-06-01 14:20:06.000000 pydrawise-2024.6.1/pydrawise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-06-01 14:20:06.000000 pydrawise-2024.6.1/pydrawise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 14:20:06.000000 pydrawise-2024.6.1/pydrawise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-01 14:20:06.000000 pydrawise-2024.6.1/pydrawise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 14:20:06.000000 pydrawise-2024.6.1/pydrawise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 14:20:06.000000 pydrawise-2024.6.1/pydrawise.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.444162 pydrawise-2024.6.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      324 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/scripts/setup
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 14:20:06.448162 pydrawise-2024.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:20:06.448162 pydrawise-2024.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19840 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25747 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/tests/test_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1576 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-06-01 14:19:53.000000 pydrawise-2024.6.1/tests/test_schema_utils.py
```

### Comparing `pydrawise-2024.4.1/.devcontainer.json` & `pydrawise-2024.6.1/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/.github/workflows/build-and-test.yml` & `pydrawise-2024.6.1/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/.github/workflows/publish-python.yml` & `pydrawise-2024.6.1/.github/workflows/publish-python.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/.gitignore` & `pydrawise-2024.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/.pre-commit-config.yaml` & `pydrawise-2024.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/LICENSE` & `pydrawise-2024.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/PKG-INFO` & `pydrawise-2024.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydrawise
-Version: 2024.4.1
+Version: 2024.6.1
 Summary: Python API for interacting with Hydrawise sprinkler controllers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pydrawise
 Project-URL: Source Code, https://github.com/dknowles2/pydrawise
 Project-URL: Bug Reports, https://github.com/dknowles2/pydrawise/issues
 Keywords: hydrawise,api,iot
```

### Comparing `pydrawise-2024.4.1/README.md` & `pydrawise-2024.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/docs/index.md` & `pydrawise-2024.6.1/docs/index.md`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/mkdocs.yml` & `pydrawise-2024.6.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/pydrawise/__init__.py` & `pydrawise-2024.6.1/pydrawise/__init__.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/pydrawise/auth.py` & `pydrawise-2024.6.1/pydrawise/auth.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/pydrawise/base.py` & `pydrawise-2024.6.1/pydrawise/base.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/pydrawise/client.py` & `pydrawise-2024.6.1/pydrawise/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 """Client library for interacting with Hydrawise's cloud API."""
 
 from datetime import datetime
 from functools import cache
 from importlib import resources
 import logging
 
-from apischema.graphql import graphql_schema
 from gql import Client
 from gql.dsl import DSLField, DSLMutation, DSLQuery, DSLSchema, DSLSelectable, dsl_gql
 from gql.transport.aiohttp import AIOHTTPTransport, log as gql_log
 from graphql import GraphQLSchema, build_ast_schema, parse
 
 from .auth import Auth
 from .base import HydrawiseBase
```

### Comparing `pydrawise-2024.4.1/pydrawise/exceptions.py` & `pydrawise-2024.6.1/pydrawise/exceptions.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/pydrawise/hydrawise.graphql` & `pydrawise-2024.6.1/pydrawise/hydrawise.graphql`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/pydrawise/legacy.py` & `pydrawise-2024.6.1/pydrawise/legacy.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/pydrawise/schema.py` & `pydrawise-2024.6.1/pydrawise/schema.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,22 +69,22 @@
             lambda l: list(map(element_conversion.serialization.converter, l)),
             source=list,
             target=list,
         ),
     )
 
 
-class AutoEnum(Enum):
+class _AutoEnum(Enum):
     @staticmethod
     def _generate_next_value_(name, start, count, last_values):
         """Determines the value for an auto() call."""
         return name
 
 
-class StatusCodeEnum(AutoEnum):
+class StatusCodeEnum(_AutoEnum):
     """Response status codes."""
 
     OK = auto()
     WARNING = auto()
     ERROR = auto()
 
 
@@ -96,16 +96,16 @@
     summary: str = ""
 
 
 @dataclass
 class LocalizedValueType:
     """A localized value."""
 
-    value: float = 0.0
-    unit: str = ""
+    value: Optional[float] = 0.0
+    unit: Optional[str] = ""
 
 
 @dataclass
 class SelectedOption:
     """A generic option."""
 
     value: int = 0
@@ -238,15 +238,15 @@
     advanced_program_id: int = 0
     watering_frequency: Optional[ProgramWateringFrequency] = field(
         default_factory=ProgramWateringFrequency
     )
     run_time_group: Optional[RunTimeGroup] = field(default_factory=RunTimeGroup)
 
 
-class AdvancedProgramDayPatternEnum(AutoEnum):
+class AdvancedProgramDayPatternEnum(_AutoEnum):
     """A value for an advanced watering program day pattern."""
 
     EVEN = auto()
     ODD = auto()
     MONDAY = auto()
     TUESDAY = auto()
     WEDNESDAY = auto()
@@ -329,16 +329,16 @@
     )
 
 
 @dataclass
 class RunStatus:
     """Run status."""
 
-    value: int = 0
-    label: str = ""
+    value: Optional[int] = 0
+    label: Optional[str] = ""
 
 
 @dataclass
 class ScheduledZoneRun:
     """A scheduled zone run."""
 
     id: str = 0
@@ -371,15 +371,15 @@
 
 
 @dataclass
 class PastZoneRuns:
     """Previous zone runs."""
 
     last_run: Optional[ScheduledZoneRun] = None
-    runs: list[ScheduledZoneRun] = field(default_factory=list)
+    runs: Optional[list[ScheduledZoneRun]] = field(default_factory=list)
 
 
 @dataclass
 class ZoneStatus:
     """A zone's status."""
 
     relative_water_balance: int = 0
@@ -389,18 +389,18 @@
 
 
 @dataclass
 class ZoneSuspension:
     """A zone suspension."""
 
     id: int = 0
-    start_time: datetime = field(
+    start_time: Optional[datetime] = field(
         metadata=DateTime.conversion(), default_factory=default_datetime
     )
-    end_time: datetime = field(
+    end_time: Optional[datetime] = field(
         metadata=DateTime.conversion(), default_factory=default_datetime
     )
 
 
 @dataclass
 class Zone(BaseZone):
     """A watering zone."""
@@ -415,15 +415,15 @@
 
 
 @dataclass
 class ProgramStartTimeApplication:
     """Application of a start time to a program."""
 
     all: bool = False
-    zones: list[BaseZone] = field(default_factory=list)
+    zones: Optional[list[BaseZone]] = field(default_factory=list)
 
 
 @dataclass
 class ProgramStartTime:
     """Start time for a watering program."""
 
     id: int = 0
@@ -437,59 +437,59 @@
 
 
 @dataclass
 class ControllerFirmware:
     """Information about the controller's firmware."""
 
     type: str = ""
-    version: str = ""
+    version: Optional[str] = ""
 
 
 @dataclass
 class ControllerModel:
     """Information about a controller model."""
 
     name: str = ""
     description: str = ""
 
 
 @dataclass
 class ControllerHardware:
     """Information about a controller's hardware."""
 
-    serial_number: str = ""
-    version: str = ""
-    status: str = ""
-    model: ControllerModel = field(default_factory=ControllerModel)
-    firmware: list[ControllerFirmware] = field(default_factory=list)
+    serial_number: Optional[str] = ""
+    version: Optional[str] = ""
+    status: Optional[str] = ""
+    model: Optional[ControllerModel] = field(default_factory=ControllerModel)
+    firmware: Optional[list[ControllerFirmware]] = field(default_factory=list)
 
 
-class CustomSensorTypeEnum(AutoEnum):
+class CustomSensorTypeEnum(_AutoEnum):
     """A value for a sensor type."""
 
     LEVEL_OPEN = auto()
     LEVEL_CLOSED = auto()
     FLOW = auto()
     THRESHOLD = auto()
 
 
 @dataclass
 class SensorModel:
     """Information about a sensor model."""
 
     id: int = 0
-    name: str = ""
-    active: bool = False
-    off_level: int = 0
-    off_timer: int = 0
-    delay: timedelta = field(
+    name: Optional[str] = ""
+    active: Optional[bool] = False
+    off_level: Optional[int] = 0
+    off_timer: Optional[int] = 0
+    delay: Optional[timedelta] = field(
         metadata=_duration_conversion("minutes"), default=timedelta()
     )
-    divisor: float = 0.0
-    flow_rate: float = 0.0
+    divisor: Optional[float] = 0.0
+    flow_rate: Optional[float] = 0.0
     sensor_type: Optional[CustomSensorTypeEnum] = None
 
 
 @dataclass
 class SensorStatus:
     """Current status of a sensor."""
 
@@ -497,54 +497,60 @@
     active: Optional[bool] = False
 
 
 @dataclass
 class SensorFlowSummary:
     """Summary of a sensor's water flow."""
 
-    total_water_volume: LocalizedValueType = field(default_factory=LocalizedValueType)
+    total_water_volume: Optional[LocalizedValueType] = field(
+        default_factory=LocalizedValueType
+    )
 
 
 @dataclass
 class Sensor:
     """A sensor connected to a controller."""
 
     id: int = 0
     name: str = ""
     model: SensorModel = field(default_factory=SensorModel)
     status: SensorStatus = field(default_factory=SensorStatus)
 
 
 @dataclass
-class WaterTime:
+class _WaterTime:
     """A water time duration."""
 
-    value: timedelta = field(
+    value: Optional[timedelta] = field(
         metadata=_duration_conversion("minutes"), default=timedelta()
     )
 
 
 @dataclass
-class ActualWaterTime(WaterTime):
+class ActualWaterTime(_WaterTime):
     """An actual water time duration."""
 
 
 @dataclass
-class NormalWaterTime(WaterTime):
+class NormalWaterTime(_WaterTime):
     """A normal water time duration."""
 
 
 @dataclass
 class ControllerStatus:
     """Current status of a controller."""
 
     summary: str = ""
     online: bool = False
-    actual_water_time: ActualWaterTime = field(default_factory=ActualWaterTime)
-    normal_water_time: NormalWaterTime = field(default_factory=NormalWaterTime)
+    actual_water_time: Optional[ActualWaterTime] = field(
+        default_factory=ActualWaterTime
+    )
+    normal_water_time: Optional[NormalWaterTime] = field(
+        default_factory=NormalWaterTime
+    )
     last_contact: Optional[DateTime] = None
 
 
 @dataclass
 class RunStatusType:
     value: int = 0
     label: str = ""
@@ -598,42 +604,44 @@
 
 
 @dataclass
 class Controller:
     """A Hydrawise controller."""
 
     id: int = 0
-    name: str = ""
-    software_version: str = ""
+    name: Optional[str] = ""
+    software_version: Optional[str] = ""
     hardware: ControllerHardware = field(default_factory=ControllerHardware)
-    last_contact_time: datetime = field(
+    last_contact_time: Optional[datetime] = field(
         metadata=DateTime.conversion(), default_factory=default_datetime
     )
-    last_action: datetime = field(
+    last_action: Optional[datetime] = field(
         metadata=DateTime.conversion(), default_factory=default_datetime
     )
-    online: bool = False
-    sensors: list[Sensor] = field(default_factory=list)
-    zones: list[Zone] = field(default_factory=list)
-    permitted_program_start_times: list[ProgramStartTime] = field(default_factory=list)
+    online: Optional[bool] = False
+    sensors: Optional[list[Sensor]] = field(default_factory=list)
+    zones: Optional[list[Zone]] = field(default_factory=list)
+    permitted_program_start_times: Optional[list[ProgramStartTime]] = field(
+        default_factory=list
+    )
     status: ControllerStatus = None
 
 
 @dataclass
 class User:
     """A Hydrawise user account."""
 
     id: int = 0
     customer_id: int = 0
     name: str = ""
-    email: str = ""
-    controllers: list[Controller] = field(default_factory=list)
+    email: Optional[str] = ""
+    controllers: Optional[list[Controller]] = field(default_factory=list)
 
 
-class DaysOfWeekEnum(AutoEnum):
+class DaysOfWeekEnum(_AutoEnum):
     """All days of the week."""
 
     SUNDAY = auto()
     MONDAY = auto()
     TUESDAY = auto()
     WEDNESDAY = auto()
     THURSDAY = auto()
@@ -643,14 +651,17 @@
 
 @dataclass
 class ControllerWaterUseSummary:
     """Water use summary for a controller.
 
     Active use means water use during a scheduled or manual zone run.
     Inactive use means water use when no zone was actively running. This can happen when
-    faucets (i.e., garden hoses) are installed downstream of the flow meter."""
+    faucets (i.e., garden hoses) are installed downstream of the flow meter.
+    """
+
+    _pydrawise_type = True
 
     total_use: float = 0.0
     total_active_use: float = 0.0
     total_inactive_use: float = 0.0
     active_use_by_zone_id: dict[int, float] = field(default_factory=dict)
     unit: str = ""
```

### Comparing `pydrawise-2024.4.1/pydrawise/schema_utils.py` & `pydrawise-2024.6.1/pydrawise/schema_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,20 +49,26 @@
 
         field_type = hints[f.name]
         origin = get_origin(field_type)
 
         if origin == Union:
             # Drop None from Optional fields.
             field_types = set(get_args(field_type)) - {NoneType}
-            if len(field_types) == 1:
-                [field_type] = field_types
-            else:
+
+            # Actual unions just yield the union.
+            if len(field_types) > 1:
                 yield _Field(f.name, list(field_types))
                 continue
-        elif origin in (List, list):
+
+            # If we have only one type left after dropping None, this could
+            # still be a list. Perform the normal extraction routine.
+            [field_type] = field_types
+            origin = get_origin(field_type)
+
+        if origin in (List, list):
             # Extract the contained type.
             # We assume all list types are uniform.
             [field_type] = get_args(field_type)
 
         yield _Field(f.name, [field_type])
```

### Comparing `pydrawise-2024.4.1/pydrawise.egg-info/PKG-INFO` & `pydrawise-2024.6.1/pydrawise.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydrawise
-Version: 2024.4.1
+Version: 2024.6.1
 Summary: Python API for interacting with Hydrawise sprinkler controllers.
 Author-email: David Knowles <dknowles2@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/dknowles2/pydrawise
 Project-URL: Source Code, https://github.com/dknowles2/pydrawise
 Project-URL: Bug Reports, https://github.com/dknowles2/pydrawise/issues
 Keywords: hydrawise,api,iot
```

### Comparing `pydrawise-2024.4.1/pydrawise.egg-info/SOURCES.txt` & `pydrawise-2024.6.1/pydrawise.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/pyproject.toml` & `pydrawise-2024.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/tests/test_auth.py` & `pydrawise-2024.6.1/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/tests/test_client.py` & `pydrawise-2024.6.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2024.4.1/tests/test_legacy.py` & `pydrawise-2024.6.1/tests/test_legacy.py`

 * *Files identical despite different names*

