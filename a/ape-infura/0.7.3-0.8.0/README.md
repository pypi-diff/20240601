# Comparing `tmp/ape-infura-0.7.3.tar.gz` & `tmp/ape-infura-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-infura-0.7.3.tar", last modified: Thu May  2 19:02:16 2024, max compression
+gzip compressed data, was "ape-infura-0.8.0.tar", last modified: Fri May 31 22:51:04 2024, max compression
```

## Comparing `ape-infura-0.7.3.tar` & `ape-infura-0.8.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:02:16.041879 ape-infura-0.7.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:02:16.041879 ape-infura-0.7.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:02:16.041879 ape-infura-0.7.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:02:16.041879 ape-infura-0.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-02 19:00:52.000000 ape-infura-0.7.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-02 19:00:52.000000 ape-infura-0.7.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-02 19:00:52.000000 ape-infura-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-02 19:02:16.041879 ape-infura-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-02 19:00:52.000000 ape-infura-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:02:16.041879 ape-infura-0.7.3/ape_infura/
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-02 19:00:52.000000 ape-infura-0.7.3/ape_infura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2024-05-02 19:00:52.000000 ape-infura-0.7.3/ape_infura/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:00:52.000000 ape-infura-0.7.3/ape_infura/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-02 19:02:15.000000 ape-infura-0.7.3/ape_infura/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:02:16.041879 ape-infura-0.7.3/ape_infura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2497 2024-05-02 19:02:15.000000 ape-infura-0.7.3/ape_infura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-02 19:02:16.000000 ape-infura-0.7.3/ape_infura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:02:15.000000 ape-infura-0.7.3/ape_infura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 19:02:15.000000 ape-infura-0.7.3/ape_infura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-02 19:02:15.000000 ape-infura-0.7.3/ape_infura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 19:02:15.000000 ape-infura-0.7.3/ape_infura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-02 19:00:52.000000 ape-infura-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-02 19:02:16.041879 ape-infura-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4023 2024-05-02 19:00:52.000000 ape-infura-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 19:02:16.041879 ape-infura-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-02 19:00:52.000000 ape-infura-0.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-02 19:00:52.000000 ape-infura-0.7.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-02 19:00:52.000000 ape-infura-0.7.3/tests/test_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:51:04.576342 ape-infura-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:51:04.572342 ape-infura-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:51:04.572342 ape-infura-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-31 22:50:02.000000 ape-infura-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-31 22:50:02.000000 ape-infura-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-31 22:50:02.000000 ape-infura-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 22:50:02.000000 ape-infura-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-31 22:50:02.000000 ape-infura-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:51:04.572342 ape-infura-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-31 22:50:02.000000 ape-infura-0.8.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-31 22:50:02.000000 ape-infura-0.8.0/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-31 22:50:02.000000 ape-infura-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 22:50:02.000000 ape-infura-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-31 22:50:02.000000 ape-infura-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2794 2024-05-31 22:50:02.000000 ape-infura-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1726 2024-05-31 22:50:02.000000 ape-infura-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-31 22:50:02.000000 ape-infura-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-31 22:50:02.000000 ape-infura-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-31 22:50:02.000000 ape-infura-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-31 22:51:04.576342 ape-infura-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-05-31 22:50:02.000000 ape-infura-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:51:04.572342 ape-infura-0.8.0/ape_infura/
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-05-31 22:50:02.000000 ape-infura-0.8.0/ape_infura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4352 2024-05-31 22:50:02.000000 ape-infura-0.8.0/ape_infura/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 22:50:02.000000 ape-infura-0.8.0/ape_infura/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 22:51:04.000000 ape-infura-0.8.0/ape_infura/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:51:04.572342 ape-infura-0.8.0/ape_infura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-31 22:51:04.000000 ape-infura-0.8.0/ape_infura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-31 22:51:04.000000 ape-infura-0.8.0/ape_infura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:51:04.000000 ape-infura-0.8.0/ape_infura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:51:04.000000 ape-infura-0.8.0/ape_infura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-31 22:51:04.000000 ape-infura-0.8.0/ape_infura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 22:51:04.000000 ape-infura-0.8.0/ape_infura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-31 22:50:02.000000 ape-infura-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-31 22:51:04.576342 ape-infura-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3974 2024-05-31 22:50:02.000000 ape-infura-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:51:04.576342 ape-infura-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 22:50:02.000000 ape-infura-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-05-31 22:50:02.000000 ape-infura-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-31 22:50:02.000000 ape-infura-0.8.0/tests/test_provider.py
```

### Comparing `ape-infura-0.7.3/.github/ISSUE_TEMPLATE/bug.md` & `ape-infura-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.3/.github/ISSUE_TEMPLATE/feature.md` & `ape-infura-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.3/.github/ISSUE_TEMPLATE/work-item.md` & `ape-infura-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.3/.github/release-drafter.yml` & `ape-infura-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.3/.github/workflows/codeql.yml` & `ape-infura-0.8.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.3/.github/workflows/commit.yaml` & `ape-infura-0.8.0/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.3/.github/workflows/prtitle.yaml` & `ape-infura-0.8.0/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.3/.github/workflows/publish.yaml` & `ape-infura-0.8.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.3/.github/workflows/test.yaml` & `ape-infura-0.8.0/.github/workflows/test.yaml`

 * *Files 4% similar despite different names*

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

### Comparing `ape-infura-0.7.3/.gitignore` & `ape-infura-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.3/.pre-commit-config.yaml` & `ape-infura-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.3/CONTRIBUTING.md` & `ape-infura-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.3/LICENSE` & `ape-infura-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.3/PKG-INFO` & `ape-infura-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: ape-infura
-Version: 0.7.3
+Version: 0.8.0
 Summary: ape-infura: Infura Provider plugins for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-infura
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
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
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
@@ -38,15 +37,15 @@
 - Arbitrum
 - Optimism
 - Blast
 - ~~Linea~~ (awaiting ape-linea update)
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-infura-0.7.3/README.md` & `ape-infura-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 - Arbitrum
 - Optimism
 - Blast
 - ~~Linea~~ (awaiting ape-linea update)
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-infura-0.7.3/ape_infura/__init__.py` & `ape-infura-0.8.0/ape_infura/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.3/ape_infura/provider.py` & `ape-infura-0.8.0/ape_infura/provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-from typing import Dict, Optional, Tuple
+from typing import Optional
 
 from ape.api import UpstreamProvider
 from ape.exceptions import ContractLogicError, ProviderError, VirtualMachineError
 from ape_ethereum.provider import Web3Provider
 from web3 import HTTPProvider, Web3
 from web3.exceptions import ContractLogicError as Web3ContractLogicError
 from web3.gas_strategies.rpc import rpc_gas_price_strategy
@@ -29,15 +29,15 @@
 class MissingProjectKeyError(InfuraProviderError):
     def __init__(self):
         env_var_str = ", ".join([f"${n}" for n in _ENVIRONMENT_VARIABLE_NAMES])
         super().__init__(f"Must set one of {env_var_str}")
 
 
 class Infura(Web3Provider, UpstreamProvider):
-    network_uris: Dict[Tuple[str, str], str] = {}
+    network_uris: dict[tuple[str, str], str] = {}
 
     @property
     def uri(self) -> str:
         ecosystem_name = self.network.ecosystem.name
         network_name = self.network.name
         if (ecosystem_name, network_name) in self.network_uris:
             return self.network_uris[(ecosystem_name, network_name)]
```

### Comparing `ape-infura-0.7.3/ape_infura.egg-info/PKG-INFO` & `ape-infura-0.8.0/ape_infura.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: ape-infura
-Version: 0.7.3
+Version: 0.8.0
 Summary: ape-infura: Infura Provider plugins for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-infura
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
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
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
@@ -38,15 +37,15 @@
 - Arbitrum
 - Optimism
 - Blast
 - ~~Linea~~ (awaiting ape-linea update)
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-infura-0.7.3/ape_infura.egg-info/SOURCES.txt` & `ape-infura-0.8.0/ape_infura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.3/ape_infura.egg-info/requires.txt` & `ape-infura-0.8.0/ape_infura.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-eth-ape<0.8,>=0.7.0
+eth-ape<0.9,>=0.8.1
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
 ape-arbitrum
```

### Comparing `ape-infura-0.7.3/pyproject.toml` & `ape-infura-0.8.0/pyproject.toml`

 * *Files 18% similar despite different names*

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

### Comparing `ape-infura-0.7.3/setup.py` & `ape-infura-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,17 +72,17 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-infura",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.7.0,<0.8",
+        "eth-ape>=0.8.1,<0.9",
     ],
-    python_requires=">=3.8,<4",
+    python_requires=">=3.9,<4",
     extras_require=extras_require,
     py_modules=["ape_infura"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_infura": ["py.typed"]},
@@ -90,14 +90,13 @@
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
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

### Comparing `ape-infura-0.7.3/tests/conftest.py` & `ape-infura-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-infura-0.7.3/tests/test_provider.py` & `ape-infura-0.8.0/tests/test_provider.py`

 * *Files identical despite different names*

