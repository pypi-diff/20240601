# Comparing `tmp/anemoi_inference-0.1.2.tar.gz` & `tmp/anemoi_inference-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anemoi_inference-0.1.2.tar", last modified: Thu May 30 19:21:09 2024, max compression
+gzip compressed data, was "anemoi_inference-0.1.3.tar", last modified: Sat Jun  1 10:45:35 2024, max compression
```

## Comparing `anemoi_inference-0.1.2.tar` & `anemoi_inference-0.1.3.tar`

### file list

```diff
@@ -1,58 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:09.917110 anemoi_inference-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:09.909110 anemoi_inference-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:09.909110 anemoi_inference-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-05-30 19:21:09.917110 anemoi_inference-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:09.913110 anemoi_inference-0.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:09.913110 anemoi_inference-0.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/docs/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:09.913110 anemoi_inference-0.1.2/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/docs/_templates/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:09.913110 anemoi_inference-0.1.2/docs/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/docs/cli/checkpoint.rst
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/docs/cli/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/docs/cli/metadata.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/docs/installing.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:09.913110 anemoi_inference-0.1.2/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/docs/modules/runner.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2251 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-30 19:21:09.917110 anemoi_inference-0.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:09.909110 anemoi_inference-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:09.909110 anemoi_inference-0.1.2/src/anemoi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:09.913110 anemoi_inference-0.1.2/src/anemoi/inference/
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/src/anemoi/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/src/anemoi/inference/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-30 19:21:09.000000 anemoi_inference-0.1.2/src/anemoi/inference/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:09.913110 anemoi_inference-0.1.2/src/anemoi/inference/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/src/anemoi/inference/checkpoint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:09.913110 anemoi_inference-0.1.2/src/anemoi/inference/checkpoint/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    10311 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/src/anemoi/inference/checkpoint/metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/src/anemoi/inference/checkpoint/metadata/patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     5166 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/src/anemoi/inference/checkpoint/metadata/version_0_0_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     3268 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/src/anemoi/inference/checkpoint/metadata/version_0_1_0.py
--rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/src/anemoi/inference/checkpoint/metadata/version_0_2_0.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:09.917110 anemoi_inference-0.1.2/src/anemoi/inference/commands/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/src/anemoi/inference/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/src/anemoi/inference/commands/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/src/anemoi/inference/commands/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    14364 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/src/anemoi/inference/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:09.917110 anemoi_inference-0.1.2/src/anemoi_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14777 2024-05-30 19:21:09.000000 anemoi_inference-0.1.2/src/anemoi_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1264 2024-05-30 19:21:09.000000 anemoi_inference-0.1.2/src/anemoi_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 19:21:09.000000 anemoi_inference-0.1.2/src/anemoi_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-30 19:21:09.000000 anemoi_inference-0.1.2/src/anemoi_inference.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-30 19:21:09.000000 anemoi_inference-0.1.2/src/anemoi_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-30 19:21:09.000000 anemoi_inference-0.1.2/src/anemoi_inference.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 19:21:09.917110 anemoi_inference-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-30 19:21:00.000000 anemoi_inference-0.1.2/tests/test_inference.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:35.290156 anemoi_inference-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:35.282156 anemoi_inference-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:35.282156 anemoi_inference-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14779 2024-06-01 10:45:35.290156 anemoi_inference-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:35.286156 anemoi_inference-0.1.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:35.286156 anemoi_inference-0.1.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    17128 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/docs/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:35.286156 anemoi_inference-0.1.3/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/docs/_templates/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:35.286156 anemoi_inference-0.1.3/docs/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/docs/cli/checkpoint.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/docs/cli/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/docs/cli/metadata.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      398 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/docs/installing.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:35.286156 anemoi_inference-0.1.3/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/docs/modules/runner.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 10:45:35.290156 anemoi_inference-0.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:35.282156 anemoi_inference-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:35.282156 anemoi_inference-0.1.3/src/anemoi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:35.286156 anemoi_inference-0.1.3/src/anemoi/inference/
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/src/anemoi/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/src/anemoi/inference/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-01 10:45:35.000000 anemoi_inference-0.1.3/src/anemoi/inference/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:35.286156 anemoi_inference-0.1.3/src/anemoi/inference/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/src/anemoi/inference/checkpoint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:35.286156 anemoi_inference-0.1.3/src/anemoi/inference/checkpoint/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    10362 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/src/anemoi/inference/checkpoint/metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2684 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/src/anemoi/inference/checkpoint/metadata/patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4965 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/src/anemoi/inference/checkpoint/metadata/version_0_0_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3336 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/src/anemoi/inference/checkpoint/metadata/version_0_1_0.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7742 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/src/anemoi/inference/checkpoint/metadata/version_0_2_0.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:35.290156 anemoi_inference-0.1.3/src/anemoi/inference/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/src/anemoi/inference/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/src/anemoi/inference/commands/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5759 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/src/anemoi/inference/commands/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/src/anemoi/inference/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14031 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/src/anemoi/inference/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:35.290156 anemoi_inference-0.1.3/src/anemoi_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14779 2024-06-01 10:45:35.000000 anemoi_inference-0.1.3/src/anemoi_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-06-01 10:45:35.000000 anemoi_inference-0.1.3/src/anemoi_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 10:45:35.000000 anemoi_inference-0.1.3/src/anemoi_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-06-01 10:45:35.000000 anemoi_inference-0.1.3/src/anemoi_inference.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-06-01 10:45:35.000000 anemoi_inference-0.1.3/src/anemoi_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-01 10:45:35.000000 anemoi_inference-0.1.3/src/anemoi_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 10:45:35.290156 anemoi_inference-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-06-01 10:45:23.000000 anemoi_inference-0.1.3/tests/test_inference.py
```

### Comparing `anemoi_inference-0.1.2/.github/workflows/python-publish.yml` & `anemoi_inference-0.1.3/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/.gitignore` & `anemoi_inference-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/.pre-commit-config.yaml` & `anemoi_inference-0.1.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/LICENSE` & `anemoi_inference-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/PKG-INFO` & `anemoi_inference-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-inference
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to hold various functions to support training of ML models.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -225,19 +225,19 @@
 License-File: LICENSE
 Requires-Dist: anemoi-utils>=0.3
 Requires-Dist: numpy
 Requires-Dist: pyyaml
 Requires-Dist: semantic-version
 Requires-Dist: torch
 Provides-Extra: all
+Requires-Dist: ai-models>=0.6.1; extra == "all"
 Requires-Dist: anemoi-utils>=0.3; extra == "all"
 Requires-Dist: numpy; extra == "all"
 Requires-Dist: pyyaml; extra == "all"
 Requires-Dist: semantic-version; extra == "all"
 Requires-Dist: torch; extra == "all"
+Requires-Dist: tqdm; extra == "all"
 Provides-Extra: dev
-Provides-Extra: docs
-Requires-Dist: nbsphinx; extra == "docs"
-Requires-Dist: pandoc; extra == "docs"
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx-argparse; extra == "docs"
-Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: pre-commit; extra == "dev"
+Provides-Extra: plugin
+Requires-Dist: ai-models>=0.6.1; extra == "plugin"
+Requires-Dist: tqdm; extra == "plugin"
```

### Comparing `anemoi_inference-0.1.2/README.md` & `anemoi_inference-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/docs/Makefile` & `anemoi_inference-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/docs/_static/logo.png` & `anemoi_inference-0.1.3/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/docs/_static/style.css` & `anemoi_inference-0.1.3/docs/_static/style.css`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/docs/conf.py` & `anemoi_inference-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/docs/index.rst` & `anemoi_inference-0.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/pyproject.toml` & `anemoi_inference-0.1.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -54,33 +54,35 @@
   "numpy",
   "pyyaml",
   "semantic-version",
   "torch",
 ]
 
 optional-dependencies.all = [
+  "ai-models>=0.6.1",
   "anemoi-utils>=0.3",
   "numpy",
   "pyyaml",
   "semantic-version",
   "torch",
+  "tqdm",
 ]
 
 optional-dependencies.dev = [
+  "pre-commit",
 ]
 
-optional-dependencies.docs = [
-  "nbsphinx",
-  "pandoc",
-  # For building the documentation
-  "sphinx",
-  "sphinx-argparse",
-  "sphinx-rtd-theme",
+optional-dependencies.plugin = [
+  "ai-models>=0.6.1",
+  "tqdm",
 ]
+
 urls.Documentation = "https://anemoi-inference.readthedocs.io/"
 urls.Homepage = "https://github.com/ecmwf/anemoi-inference/"
 urls.Issues = "https://github.com/ecmwf/anemoi-inference/issues"
 urls.Repository = "https://github.com/ecmwf/anemoi-inference/"
 scripts.anemoi-inference = "anemoi.inference.__main__:main"
 
+entry-points."ai_models.model".anemoi = "anemoi.inference.plugin:AIModelPlugin"
+
 [tool.setuptools_scm]
 version_file = "src/anemoi/inference/_version.py"
```

### Comparing `anemoi_inference-0.1.2/src/anemoi/inference/__main__.py` & `anemoi_inference-0.1.3/src/anemoi/inference/__main__.py`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/src/anemoi/inference/checkpoint/__init__.py` & `anemoi_inference-0.1.3/src/anemoi/inference/checkpoint/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/src/anemoi/inference/checkpoint/metadata/__init__.py` & `anemoi_inference-0.1.3/src/anemoi/inference/checkpoint/metadata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -220,14 +220,16 @@
                 "cos_local_time",
                 "sin_julian_day",
                 "sin_local_time",
                 "insolation",
             ]
         )
 
+        print("FORCINGS", self._forcing_params())
+
         constants = set(self._forcing_params()) - set(self.constants_from_input) - set(self.computed_constants)
 
         if constants - known:
             LOG.warning(f"Unknown computed forcing {constants - known}")
 
         data_mask, model_mask, names = self._forcings(constants)
```

### Comparing `anemoi_inference-0.1.2/src/anemoi/inference/checkpoint/metadata/patch.py` & `anemoi_inference-0.1.3/src/anemoi/inference/checkpoint/metadata/patch.py`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/src/anemoi/inference/checkpoint/metadata/version_0_1_0.py` & `anemoi_inference-0.1.3/src/anemoi/inference/checkpoint/metadata/version_0_1_0.py`

 * *Files 6% similar despite different names*

```diff
@@ -81,9 +81,13 @@
                     param, level = var.split("_")
                     level = int(level)
                     if [param, level] in pl:
                         pl.remove([param, level])
                     if [param, level] in ml:
                         ml.remove([param, level])
 
+    @property
+    def variables_with_nans(self):
+        return []
+
     def dump(self, indent=0):
         print("Version_0_1_0: Not implemented")
```

### Comparing `anemoi_inference-0.1.2/src/anemoi/inference/checkpoint/metadata/version_0_2_0.py` & `anemoi_inference-0.1.3/src/anemoi/inference/checkpoint/metadata/version_0_2_0.py`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/src/anemoi/inference/commands/__init__.py` & `anemoi_inference-0.1.3/src/anemoi/inference/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/src/anemoi/inference/commands/checkpoint.py` & `anemoi_inference-0.1.3/src/anemoi/inference/commands/checkpoint.py`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/src/anemoi/inference/commands/metadata.py` & `anemoi_inference-0.1.3/src/anemoi/inference/commands/metadata.py`

 * *Files identical despite different names*

### Comparing `anemoi_inference-0.1.2/src/anemoi/inference/runner.py` & `anemoi_inference-0.1.3/src/anemoi/inference/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,14 @@
     "16-mixed": torch.float16,
     "32": torch.float32,
     "b16": torch.bfloat16,
     "b16-mixed": torch.bfloat16,
     "bfloat16": torch.bfloat16,
     "float16": torch.float16,
     "float32": torch.float32,
-    None: torch.float16,
 }
 
 
 def forcing_and_constants(source, date, param):
     import climetlab as cml
 
     ds = cml.load_source(
@@ -63,15 +62,14 @@
         input_fields,
         lead_time,
         device,
         start_datetime=None,
         output_callback=ignore,
         autocast=None,
         progress_callback=ignore,
-        add_ensemble_dimension=False,
     ):
         """_summary_
 
         Parameters
         ----------
         input_fields : _type_
             _description_
@@ -83,16 +81,14 @@
             _description_, by default None
         output_callback : _type_, optional
             _description_, by default ignore
         autocast : _type_, optional
             _description_, by default None
         progress_callback : _type_, optional
             _description_, by default ignore
-        add_ensemble_dimension : bool, optional
-            _description_, by default False
 
         Returns
         -------
         _type_
             _description_
 
         Raises
@@ -102,14 +98,18 @@
         ValueError
             _description_
         """
 
         if autocast is None:
             autocast = self.checkpoint.precision
 
+        if autocast is None:
+            LOGGER.warning("No autocast given, using float16")
+            autocast = "16"
+
         autocast = AUTOCAST[autocast]
 
         input_fields = input_fields.sel(**self.checkpoint.select)
         input_fields = input_fields.order_by(**self.checkpoint.order_by)
 
         number_of_grid_points = len(input_fields[0].grid_points()[0])
 
@@ -310,25 +310,14 @@
                 self.checkpoint.diagnostic_params,
                 precip_template,
                 accumulated_output[0].shape,
             )
         else:
             output_callback(input_fields)
 
-        def add_ensemble_dim(func):
-            def wrapper(x):
-                x = x.unsqueeze(2)
-                y = func(x)
-                return y.squeeze_(2)
-
-            return wrapper
-
-        if add_ensemble_dimension:
-            model.predict_step = add_ensemble_dim(model.predict_step)
-
         prognostic_params = self.checkpoint.prognostic_params
 
         # with self.stepper(self.hour_steps) as stepper:
 
         for i in progress_callback(range(lead_time // self.hour_steps)):
             step = (i + 1) * self.hour_steps
```

### Comparing `anemoi_inference-0.1.2/src/anemoi_inference.egg-info/PKG-INFO` & `anemoi_inference-0.1.3/src/anemoi_inference.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anemoi-inference
-Version: 0.1.2
+Version: 0.1.3
 Summary: A package to hold various functions to support training of ML models.
 Author-email: "European Centre for Medium-Range Weather Forecasts (ECMWF)" <software.support@ecmwf.int>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -225,19 +225,19 @@
 License-File: LICENSE
 Requires-Dist: anemoi-utils>=0.3
 Requires-Dist: numpy
 Requires-Dist: pyyaml
 Requires-Dist: semantic-version
 Requires-Dist: torch
 Provides-Extra: all
+Requires-Dist: ai-models>=0.6.1; extra == "all"
 Requires-Dist: anemoi-utils>=0.3; extra == "all"
 Requires-Dist: numpy; extra == "all"
 Requires-Dist: pyyaml; extra == "all"
 Requires-Dist: semantic-version; extra == "all"
 Requires-Dist: torch; extra == "all"
+Requires-Dist: tqdm; extra == "all"
 Provides-Extra: dev
-Provides-Extra: docs
-Requires-Dist: nbsphinx; extra == "docs"
-Requires-Dist: pandoc; extra == "docs"
-Requires-Dist: sphinx; extra == "docs"
-Requires-Dist: sphinx-argparse; extra == "docs"
-Requires-Dist: sphinx-rtd-theme; extra == "docs"
+Requires-Dist: pre-commit; extra == "dev"
+Provides-Extra: plugin
+Requires-Dist: ai-models>=0.6.1; extra == "plugin"
+Requires-Dist: tqdm; extra == "plugin"
```

### Comparing `anemoi_inference-0.1.2/src/anemoi_inference.egg-info/SOURCES.txt` & `anemoi_inference-0.1.3/src/anemoi_inference.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 docs/cli/checkpoint.rst
 docs/cli/introduction.rst
 docs/cli/metadata.rst
 docs/modules/runner.rst
 src/anemoi/inference/__init__.py
 src/anemoi/inference/__main__.py
 src/anemoi/inference/_version.py
+src/anemoi/inference/plugin.py
 src/anemoi/inference/runner.py
 src/anemoi/inference/checkpoint/__init__.py
 src/anemoi/inference/checkpoint/metadata/__init__.py
 src/anemoi/inference/checkpoint/metadata/patch.py
 src/anemoi/inference/checkpoint/metadata/version_0_0_0.py
 src/anemoi/inference/checkpoint/metadata/version_0_1_0.py
 src/anemoi/inference/checkpoint/metadata/version_0_2_0.py
```

