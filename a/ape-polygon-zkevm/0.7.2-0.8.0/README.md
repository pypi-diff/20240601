# Comparing `tmp/ape-polygon-zkevm-0.7.2.tar.gz` & `tmp/ape-polygon-zkevm-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-polygon-zkevm-0.7.2.tar", last modified: Thu May  9 01:18:31 2024, max compression
+gzip compressed data, was "ape-polygon-zkevm-0.8.0.tar", last modified: Sat Jun  1 04:27:26 2024, max compression
```

## Comparing `ape-polygon-zkevm-0.7.2.tar` & `ape-polygon-zkevm-0.8.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:18:31.293650 ape-polygon-zkevm-0.7.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:18:31.289650 ape-polygon-zkevm-0.7.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:18:31.289650 ape-polygon-zkevm-0.7.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:18:31.289650 ape-polygon-zkevm-0.7.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-09 01:18:31.293650 ape-polygon-zkevm-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:18:31.289650 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm/
--rw-r--r--   0 runner    (1001) docker     (127)     1057 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm/ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-09 01:18:31.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:18:31.289650 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1954 2024-05-09 01:18:31.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-05-09 01:18:31.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 01:18:31.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 01:18:31.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-05-09 01:18:31.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-09 01:18:31.000000 ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-09 01:18:31.293650 ape-polygon-zkevm-0.7.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 01:18:31.293650 ape-polygon-zkevm-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      549 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/tests/test_ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-05-09 01:17:34.000000 ape-polygon-zkevm-0.7.2/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:27:26.781674 ape-polygon-zkevm-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:27:26.777675 ape-polygon-zkevm-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:27:26.777675 ape-polygon-zkevm-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:27:26.777675 ape-polygon-zkevm-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-06-01 04:27:26.781674 ape-polygon-zkevm-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:27:26.781674 ape-polygon-zkevm-0.8.0/ape_polygon_zkevm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/ape_polygon_zkevm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/ape_polygon_zkevm/ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/ape_polygon_zkevm/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-01 04:27:26.000000 ape-polygon-zkevm-0.8.0/ape_polygon_zkevm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:27:26.781674 ape-polygon-zkevm-0.8.0/ape_polygon_zkevm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-06-01 04:27:26.000000 ape-polygon-zkevm-0.8.0/ape_polygon_zkevm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-06-01 04:27:26.000000 ape-polygon-zkevm-0.8.0/ape_polygon_zkevm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 04:27:26.000000 ape-polygon-zkevm-0.8.0/ape_polygon_zkevm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 04:27:26.000000 ape-polygon-zkevm-0.8.0/ape_polygon_zkevm.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-06-01 04:27:26.000000 ape-polygon-zkevm-0.8.0/ape_polygon_zkevm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 04:27:26.000000 ape-polygon-zkevm-0.8.0/ape_polygon_zkevm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-01 04:27:26.781674 ape-polygon-zkevm-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3283 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:27:26.781674 ape-polygon-zkevm-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/tests/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-06-01 04:26:32.000000 ape-polygon-zkevm-0.8.0/tests/test_provider.py
```

### Comparing `ape-polygon-zkevm-0.7.2/.github/ISSUE_TEMPLATE/bug.md` & `ape-polygon-zkevm-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.2/.github/ISSUE_TEMPLATE/feature.md` & `ape-polygon-zkevm-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.2/.github/ISSUE_TEMPLATE/work-item.md` & `ape-polygon-zkevm-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.2/.github/release-drafter.yml` & `ape-polygon-zkevm-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.2/.github/workflows/codeql.yaml` & `ape-polygon-zkevm-0.8.0/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.2/.github/workflows/commitlint.yaml` & `ape-polygon-zkevm-0.8.0/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.2/.github/workflows/prtitle.yaml` & `ape-polygon-zkevm-0.8.0/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.2/.github/workflows/publish.yaml` & `ape-polygon-zkevm-0.8.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.2/.github/workflows/test.yaml` & `ape-polygon-zkevm-0.8.0/.github/workflows/test.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 # TODO: Replace with macos-latest when works again.
                 #   https://github.com/actions/setup-python/issues/808
                 os: [ubuntu-latest, macos-12]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10", "3.11", "3.12"]
+                python-version: [3.9, "3.10", "3.11", "3.12"]
 
         steps:
         - uses: actions/checkout@v4
 
         - name: Setup Python
           uses: actions/setup-python@v5
           with:
```

### Comparing `ape-polygon-zkevm-0.7.2/.gitignore` & `ape-polygon-zkevm-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.2/.pre-commit-config.yaml` & `ape-polygon-zkevm-0.8.0/.pre-commit-config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -26,11 +26,11 @@
     -   id: mypy
         additional_dependencies: [types-setuptools, pydantic]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
     -   id: mdformat
-        additional_dependencies: [mdformat-gfm, mdformat-frontmatter]
+        additional_dependencies: [mdformat-gfm, mdformat-frontmatter, mdformat-pyproject]
 
 default_language_version:
     python: python3
```

### Comparing `ape-polygon-zkevm-0.7.2/CONTRIBUTING.md` & `ape-polygon-zkevm-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.2/LICENSE` & `ape-polygon-zkevm-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.2/PKG-INFO` & `ape-polygon-zkevm-0.8.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: ape-polygon-zkevm
-Version: 0.7.2
+Version: 0.8.0
 Summary: ape-polygon-zkevm: Ecosystem plugin for Polygon ZkEVM
 Home-page: https://github.com/ApeWorX/ape-polygon-zkevm
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 Ecosystem Plugin for Polygon ZkEVM support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-polygon-zkevm-0.7.2/README.md` & `ape-polygon-zkevm-0.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ecosystem Plugin for Polygon ZkEVM support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-polygon-zkevm-0.7.2/ape_polygon_zkevm/__init__.py` & `ape-polygon-zkevm-0.8.0/ape_polygon_zkevm/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from ape import plugins
 from ape.api.networks import LOCAL_NETWORK_NAME, ForkedNetworkAPI, NetworkAPI, create_network_type
-from ape_geth import GethProvider
+from ape_node import Node
 from ape_test import LocalProvider
 
 from .ecosystem import NETWORKS, PolygonZkEVM, PolygonZkEVMConfig
 
 
 @plugins.register(plugins.Config)
 def config_class():
@@ -25,10 +25,10 @@
     # NOTE: This works for local providers, as they get chain_id from themselves
     yield "polygon-zkevm", LOCAL_NETWORK_NAME, NetworkAPI
 
 
 @plugins.register(plugins.ProviderPlugin)
 def providers():
     for network_name in NETWORKS:
-        yield "polygon-zkevm", network_name, GethProvider
+        yield "polygon-zkevm", network_name, Node
 
     yield "polygon-zkevm", LOCAL_NETWORK_NAME, LocalProvider
```

### Comparing `ape-polygon-zkevm-0.7.2/ape_polygon_zkevm/ecosystem.py` & `ape-polygon-zkevm-0.8.0/ape_polygon_zkevm/ecosystem.py`

 * *Files 15% similar despite different names*

```diff
@@ -18,8 +18,9 @@
     mainnet: NetworkConfig = create_network_config(block_time=2, required_confirmations=1)
     cardona: NetworkConfig = create_network_config(block_time=2, required_confirmations=1)
 
 
 class PolygonZkEVM(Ethereum):
     @property
     def config(self) -> PolygonZkEVMConfig:  # type: ignore
-        return cast(PolygonZkEVMConfig, self.config_manager.get_config("polygon-zkevm"))
+        cfg = self.config_manager.get_config("polygon-zkevm")
+        return cast(PolygonZkEVMConfig, cfg)
```

### Comparing `ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/PKG-INFO` & `ape-polygon-zkevm-0.8.0/ape_polygon_zkevm.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 Metadata-Version: 2.1
 Name: ape-polygon-zkevm
-Version: 0.7.2
+Version: 0.8.0
 Summary: ape-polygon-zkevm: Ecosystem plugin for Polygon ZkEVM
 Home-page: https://github.com/ApeWorX/ape-polygon-zkevm
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Python: >=3.8,<4
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 Ecosystem Plugin for Polygon ZkEVM support in Ape.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/SOURCES.txt` & `ape-polygon-zkevm-0.8.0/ape_polygon_zkevm.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.2/ape_polygon_zkevm.egg-info/requires.txt` & `ape-polygon-zkevm-0.8.0/ape_polygon_zkevm.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-eth-ape<0.8,>=0.7.6
+eth-ape<0.9,>=0.8.2
 ethpm-types
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
```

### Comparing `ape-polygon-zkevm-0.7.2/pyproject.toml` & `ape-polygon-zkevm-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310', 'py311', 'py312']
+target-version = ['py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ape-polygon-zkevm-0.7.2/setup.py` & `ape-polygon-zkevm-0.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,18 +56,18 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-polygon-zkevm",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.7.6,<0.8",
+        "eth-ape>=0.8.2,<0.9",
         "ethpm-types",  # Use same version as eth-ape
     ],
-    python_requires=">=3.8,<4",
+    python_requires=">=3.9,<4",
     extras_require=extras_require,
     py_modules=["ape_polygon_zkevm"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_polygon_zkevm": ["py.typed"]},
@@ -75,14 +75,13 @@
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: Apache Software License",
         "Natural Language :: English",
         "Operating System :: MacOS",
         "Operating System :: POSIX",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `ape-polygon-zkevm-0.7.2/tests/conftest.py` & `ape-polygon-zkevm-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.2/tests/test_config.py` & `ape-polygon-zkevm-0.8.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.2/tests/test_ecosystem.py` & `ape-polygon-zkevm-0.8.0/tests/test_ecosystem.py`

 * *Files identical despite different names*

### Comparing `ape-polygon-zkevm-0.7.2/tests/test_integration.py` & `ape-polygon-zkevm-0.8.0/tests/test_integration.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import pytest
 from ape._cli import cli as ape_cli
 from click.testing import CliRunner
 
 EXPECTED_OUTPUT = """
 polygon-zkevm
-├── mainnet
-│   └── geth  (default)
 ├── cardona
-│   └── geth  (default)
-└── local  (default)
-    └── test  (default)
+│   └── node  (default)
+├── local  (default)
+│   └── test  (default)
+└── mainnet
+    └── node  (default)
 """.strip()
 
 
 @pytest.fixture
 def runner():
     return CliRunner()
 
@@ -42,12 +42,12 @@
 
     for expected_line in expected_lines:
         assert expected_line in actual_lines
 
 
 def test_networks(runner, cli, polygon_zkevm):
     # Do this in case local env changed it.
-    polygon_zkevm.mainnet.set_default_provider("geth")
-    polygon_zkevm.cardona.set_default_provider("geth")
+    polygon_zkevm.mainnet.set_default_provider("node")
+    polygon_zkevm.cardona.set_default_provider("node")
 
-    result = runner.invoke(cli, ["networks", "list"])
+    result = runner.invoke(cli, ("networks", "list"))
     assert_rich_text(result.output, EXPECTED_OUTPUT)
```

