# Comparing `tmp/ape-alchemy-0.7.3.tar.gz` & `tmp/ape-alchemy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-alchemy-0.7.3.tar", last modified: Fri May 10 13:20:25 2024, max compression
+gzip compressed data, was "ape-alchemy-0.8.0.tar", last modified: Fri May 31 22:32:52 2024, max compression
```

## Comparing `ape-alchemy-0.7.3.tar` & `ape-alchemy-0.8.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:20:25.538844 ape-alchemy-0.7.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:20:25.534844 ape-alchemy-0.7.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:20:25.534844 ape-alchemy-0.7.3/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:20:25.534844 ape-alchemy-0.7.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/.github/workflows/codeql.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3855 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-10 13:20:25.538844 ape-alchemy-0.7.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:20:25.534844 ape-alchemy-0.7.3/ape_alchemy/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/ape_alchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/ape_alchemy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/ape_alchemy/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/ape_alchemy/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-10 13:20:25.000000 ape-alchemy-0.7.3/ape_alchemy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:20:25.534844 ape-alchemy-0.7.3/ape_alchemy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-05-10 13:20:25.000000 ape-alchemy-0.7.3/ape_alchemy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-10 13:20:25.000000 ape-alchemy-0.7.3/ape_alchemy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:20:25.000000 ape-alchemy-0.7.3/ape_alchemy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:20:25.000000 ape-alchemy-0.7.3/ape_alchemy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-10 13:20:25.000000 ape-alchemy-0.7.3/ape_alchemy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-10 13:20:25.000000 ape-alchemy-0.7.3/ape_alchemy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/build_docs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:20:25.538844 ape-alchemy-0.7.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:20:25.538844 ape-alchemy-0.7.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:20:25.538844 ape-alchemy-0.7.3/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/docs/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:20:25.538844 ape-alchemy-0.7.3/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/docs/methoddocs/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/docs/methoddocs/providers.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:20:25.538844 ape-alchemy-0.7.3/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/docs/userguides/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-10 13:20:25.538844 ape-alchemy-0.7.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4294 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:20:25.538844 ape-alchemy-0.7.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6808 2024-05-10 13:19:28.000000 ape-alchemy-0.7.3/tests/test_providers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:32:52.461081 ape-alchemy-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:32:52.457081 ape-alchemy-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:32:52.457081 ape-alchemy-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      647 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:32:52.457081 ape-alchemy-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-31 22:32:52.461081 ape-alchemy-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2799 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:32:52.461081 ape-alchemy-0.8.0/ape_alchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/ape_alchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/ape_alchemy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9485 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/ape_alchemy/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/ape_alchemy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 22:32:52.000000 ape-alchemy-0.8.0/ape_alchemy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:32:52.461081 ape-alchemy-0.8.0/ape_alchemy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3767 2024-05-31 22:32:52.000000 ape-alchemy-0.8.0/ape_alchemy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-31 22:32:52.000000 ape-alchemy-0.8.0/ape_alchemy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:32:52.000000 ape-alchemy-0.8.0/ape_alchemy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:32:52.000000 ape-alchemy-0.8.0/ape_alchemy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-31 22:32:52.000000 ape-alchemy-0.8.0/ape_alchemy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-31 22:32:52.000000 ape-alchemy-0.8.0/ape_alchemy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2560 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/build_docs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:32:52.461081 ape-alchemy-0.8.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:32:52.461081 ape-alchemy-0.8.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     3827 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:32:52.461081 ape-alchemy-0.8.0/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     9740 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/docs/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3383 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:32:52.461081 ape-alchemy-0.8.0/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/docs/methoddocs/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/docs/methoddocs/providers.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:32:52.461081 ape-alchemy-0.8.0/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/docs/userguides/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)      999 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-31 22:32:52.465081 ape-alchemy-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4245 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:32:52.461081 ape-alchemy-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-05-31 22:31:58.000000 ape-alchemy-0.8.0/tests/test_providers.py
```

### Comparing `ape-alchemy-0.7.3/.github/ISSUE_TEMPLATE/bug.md` & `ape-alchemy-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/.github/ISSUE_TEMPLATE/feature.md` & `ape-alchemy-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/.github/ISSUE_TEMPLATE/work-item.md` & `ape-alchemy-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/.github/release-drafter.yml` & `ape-alchemy-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/.github/workflows/codeql.yaml` & `ape-alchemy-0.8.0/.github/workflows/codeql.yaml`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/.github/workflows/commitlint.yaml` & `ape-alchemy-0.8.0/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/.github/workflows/docs.yaml` & `ape-alchemy-0.8.0/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/.github/workflows/prtitle.yaml` & `ape-alchemy-0.8.0/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/.github/workflows/publish.yaml` & `ape-alchemy-0.8.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/.github/workflows/test.yaml` & `ape-alchemy-0.8.0/.github/workflows/test.yaml`

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
 
         env:
           GITHUB_ACCESS_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
         steps:
         - uses: actions/checkout@v4
           with:
```

### Comparing `ape-alchemy-0.7.3/.gitignore` & `ape-alchemy-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/.pre-commit-config.yaml` & `ape-alchemy-0.8.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -26,11 +26,11 @@
     -   id: mypy
         additional_dependencies: [types-PyYAML, types-requests, pydantic, types-setuptools]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
     -   id: mdformat
-        additional_dependencies: [mdformat-gfm, mdformat-frontmatter]
+        additional_dependencies: [mdformat-gfm, mdformat-frontmatter, mdformat-pyproject]
 
 default_language_version:
     python: python3
```

### Comparing `ape-alchemy-0.7.3/CONTRIBUTING.md` & `ape-alchemy-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/LICENSE` & `ape-alchemy-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/PKG-INFO` & `ape-alchemy-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: ape-alchemy
-Version: 0.7.3
+Version: 0.8.0
 Summary: ape-alchemy: Alchemy provider plugins
 Home-page: https://github.com/ApeWorX/ape-alchemy
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
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
@@ -37,15 +36,15 @@
 - Arbitrum
 - Base
 - Optimism
 - Polygon
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-alchemy-0.7.3/README.md` & `ape-alchemy-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 - Arbitrum
 - Base
 - Optimism
 - Polygon
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-alchemy-0.7.3/ape_alchemy/__init__.py` & `ape-alchemy-0.8.0/ape_alchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/ape_alchemy/exceptions.py` & `ape-alchemy-0.8.0/ape_alchemy/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Tuple
-
 from ape.exceptions import ProviderError
 
 
 class AlchemyProviderError(ProviderError):
     """
     An error raised by the Alchemy provider plugin.
     """
@@ -17,10 +15,10 @@
 
 
 class MissingProjectKeyError(AlchemyProviderError):
     """
     An error raised when there is no API key set.
     """
 
-    def __init__(self, options: Tuple[str, ...]):
+    def __init__(self, options: tuple[str, ...]):
         env_var_str = ", ".join([f"${n}" for n in options])
         super().__init__(f"Must set one of {env_var_str}.")
```

### Comparing `ape-alchemy-0.7.3/ape_alchemy/provider.py` & `ape-alchemy-0.8.0/ape_alchemy/provider.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 import os
-from typing import Any, Dict, List, Optional
+from collections.abc import Iterable
+from typing import Any, Optional
 
-from ape.api import ReceiptAPI, TransactionAPI, UpstreamProvider
-from ape.exceptions import (
-    APINotImplementedError,
-    ContractLogicError,
-    ProviderError,
-    VirtualMachineError,
-)
+from ape.api import ReceiptAPI, TraceAPI, TransactionAPI, UpstreamProvider
+from ape.exceptions import ContractLogicError, ProviderError, VirtualMachineError
 from ape.logging import logger
-from ape.types import CallTreeNode
 from ape_ethereum.provider import Web3Provider
+from ape_ethereum.trace import TransactionTrace
 from eth_pydantic_types import HexBytes
 from eth_typing import HexStr
-from evm_trace import (
-    ParityTraceList,
-    get_calltree_from_geth_call_trace,
-    get_calltree_from_parity_trace,
-)
 from requests import HTTPError
 from web3 import HTTPProvider, Web3
 from web3.exceptions import ContractLogicError as Web3ContractLogicError
 from web3.gas_strategies.rpc import rpc_gas_price_strategy
 from web3.middleware import geth_poa_middleware
 
 from .exceptions import AlchemyFeatureNotAvailable, AlchemyProviderError, MissingProjectKeyError
@@ -37,15 +28,15 @@
 class Alchemy(Web3Provider, UpstreamProvider):
     """
     A web3 provider using an HTTP connection to Alchemy.
 
     Docs: https://docs.alchemy.com/alchemy/
     """
 
-    network_uris: Dict[tuple, str] = {}
+    network_uris: dict[tuple, str] = {}
 
     @property
     def uri(self):
         """
         Alchemy RPC URI, including the project ID.
         """
         ecosystem_name = self.network.ecosystem.name
@@ -112,42 +103,24 @@
             self._web3.eth.set_gas_price_strategy(rpc_gas_price_strategy)
         except Exception as err:
             raise ProviderError(f"Failed to connect to Alchemy.\n{repr(err)}") from err
 
     def disconnect(self):
         self._web3 = None
 
-    def _get_prestate_trace(self, txn_hash: str) -> Dict:
-        return self._debug_trace_transaction(txn_hash, "prestateTracer")
+    def _get_prestate_trace(self, transaction_hash: str) -> dict:
+        return self.make_request(
+            "debug_traceTransaction", [transaction_hash, {"tracer": "prestateTracer"}]
+        )
 
-    def get_call_tree(self, txn_hash: str) -> CallTreeNode:
-        try:
-            return self._get_calltree_using_parity_style(txn_hash)
-        except Exception as err:
-            try:
-                return self._get_calltree_using_call_tracer(txn_hash)
-            except Exception:
-                pass
-
-            raise APINotImplementedError() from err
-
-    def _get_calltree_using_parity_style(self, txn_hash: str) -> CallTreeNode:
-        raw_trace_list = self._make_request("trace_transaction", [txn_hash])
-        trace_list = ParityTraceList.model_validate(raw_trace_list)
-        evm_call = get_calltree_from_parity_trace(trace_list)
-        return self._create_call_tree_node(evm_call)
-
-    def _get_calltree_using_call_tracer(self, txn_hash: str) -> CallTreeNode:
-        # Create trace frames using geth-style call tracer
-        calls = self._debug_trace_transaction(txn_hash, "callTracer")
-        evm_call = get_calltree_from_geth_call_trace(calls)
-        return self._create_call_tree_node(evm_call, txn_hash=txn_hash)
+    def get_transaction_trace(self, transaction_hash: str, **kwargs) -> TraceAPI:
+        if "debug_trace_transaction_parameters" not in kwargs:
+            kwargs["debug_trace_transaction_parameters"] = {}
 
-    def _debug_trace_transaction(self, txn_hash: str, tracer: str) -> Dict:
-        return self._make_request("debug_traceTransaction", [txn_hash, {"tracer": tracer}])
+        return TransactionTrace(transaction_hash=transaction_hash, **kwargs)
 
     def get_virtual_machine_error(self, exception: Exception, **kwargs) -> VirtualMachineError:
         txn = kwargs.get("txn")
         if not hasattr(exception, "args") or not len(exception.args):
             return VirtualMachineError(base_err=exception, txn=txn)
 
         args = exception.args
@@ -174,17 +147,17 @@
                 return ContractLogicError(revert_message=message, txn=txn)
             else:
                 # No revert message
                 return ContractLogicError(txn=txn)
 
         return VirtualMachineError(message=message, txn=txn)
 
-    def _make_request(self, endpoint: str, parameters: Optional[List] = None) -> Any:
+    def make_request(self, endpoint: str, parameters: Optional[Iterable] = None) -> Any:
         try:
-            return super()._make_request(endpoint, parameters)
+            return super().make_request(endpoint, parameters)
         except HTTPError as err:
             response_data = err.response.json() if err.response else {}
             if "error" not in response_data:
                 raise AlchemyProviderError(str(err)) from err
 
             error_data = response_data["error"]
             message = (
@@ -221,15 +194,15 @@
         }
         if kwargs and "fast" not in kwargs:
             # If sending preferences, `fast` must be present.
             kwargs["fast"] = False
             params["preferences"] = kwargs
 
         try:
-            txn_hash = self._make_request("eth_sendPrivateTransaction", [params])
+            txn_hash = self.make_request("eth_sendPrivateTransaction", [params])
         except (ValueError, Web3ContractLogicError) as err:
             vm_err = self.get_virtual_machine_error(err, txn=txn)
             raise vm_err from err
 
         # Since Alchemy will attempt to publish for 25 blocks,
         # we add 25 * block_time to the timeout.
         timeout = (
```

### Comparing `ape-alchemy-0.7.3/ape_alchemy.egg-info/PKG-INFO` & `ape-alchemy-0.8.0/ape_alchemy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: ape-alchemy
-Version: 0.7.3
+Version: 0.8.0
 Summary: ape-alchemy: Alchemy provider plugins
 Home-page: https://github.com/ApeWorX/ape-alchemy
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
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
@@ -37,15 +36,15 @@
 - Arbitrum
 - Base
 - Optimism
 - Polygon
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-alchemy-0.7.3/ape_alchemy.egg-info/SOURCES.txt` & `ape-alchemy-0.8.0/ape_alchemy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/ape_alchemy.egg-info/requires.txt` & `ape-alchemy-0.8.0/ape_alchemy.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-eth-ape<0.8,>=0.7.0
+eth-ape<0.9,>=0.8.1
 eth-pydantic-types
 ethpm-types
 evm-trace
 web3
 requests
 
 [dev]
@@ -12,15 +12,15 @@
 ape-polygon
 pytest>=6.0
 pytest-xdist
 pytest-cov
 pytest-mock
 hypothesis<7.0,>=6.2.0
 websocket-client
-black<25,>=24.4.1
+black<25,>=24.4.2
 mypy<2,>=1.10.0
 types-setuptools
 types-requests
 flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
 isort<6,>=5.13.2
@@ -48,15 +48,15 @@
 sphinx-click<5,>=4.4.0
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 sphinxcontrib-napoleon>=0.7
 sphinx-plausible<0.2,>=0.1.2
 
 [lint]
-black<25,>=24.4.1
+black<25,>=24.4.2
 mypy<2,>=1.10.0
 types-setuptools
 types-requests
 flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
 isort<6,>=5.13.2
```

### Comparing `ape-alchemy-0.7.3/build_docs.py` & `ape-alchemy-0.8.0/build_docs.py`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/docs/_static/custom.css` & `ape-alchemy-0.8.0/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/docs/_static/custom.js` & `ape-alchemy-0.8.0/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/docs/_templates/layout.html` & `ape-alchemy-0.8.0/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/docs/conf.py` & `ape-alchemy-0.8.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/docs/favicon.ico` & `ape-alchemy-0.8.0/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/docs/logo.gif` & `ape-alchemy-0.8.0/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/pyproject.toml` & `ape-alchemy-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/setup.py` & `ape-alchemy-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         "pytest-xdist",  # Multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "pytest-mock",  # For creating mocks
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
         "websocket-client",  # Used for web socket integration testing
     ],
     "lint": [
-        "black>=24.4.1,<25",  # Auto-formatter and linter
+        "black>=24.4.2,<25",  # Auto-formatter and linter
         "mypy>=1.10.0,<2",  # Static type analyzer
         "types-setuptools",  # Needed for mypy type shed
         "types-requests",  # Needed for mypy type shed
         "flake8>=7.0.0,<8",  # Style linter
         "flake8-breakpoint>=1.1.0,<2",  # Detect breakpoints left in code
         "flake8-print>=5.0.0,<6",  # Detect print statements left in code
         "isort>=5.13.2,<6",  # Import sorting linter
@@ -71,22 +71,22 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-alchemy",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.7.0,<0.8",
+        "eth-ape>=0.8.1,<0.9",
         "eth-pydantic-types",  # Use same version as eth-ape
         "ethpm-types",  # Use same version as eth-ape
         "evm-trace",  # Use same version as eth-ape
         "web3",  # Use same version as eth-ape
         "requests",
     ],
-    python_requires=">=3.8,<4",
+    python_requires=">=3.9,<4",
     extras_require=extras_require,
     py_modules=["ape_alchemy"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_alchemy": ["py.typed"]},
@@ -94,14 +94,13 @@
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

### Comparing `ape-alchemy-0.7.3/tests/conftest.py` & `ape-alchemy-0.8.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/tests/test_integration.py` & `ape-alchemy-0.8.0/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `ape-alchemy-0.7.3/tests/test_providers.py` & `ape-alchemy-0.8.0/tests/test_providers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 
 import pytest
-from ape.exceptions import APINotImplementedError, ContractLogicError
+from ape.exceptions import ContractLogicError
 from ape.types import LogFilter
 from hexbytes import HexBytes
 from web3.exceptions import ContractLogicError as Web3ContractLogicError
 
 from ape_alchemy.provider import MissingProjectKeyError
 
 TXN_HASH = "0x3cef4aaa52b97b6b61aa32b3afcecb0d14f7862ca80fdc76504c37a9374645c4"
@@ -156,30 +156,26 @@
     mock_web3.eth.estimate_gas.side_effect = Web3ContractLogicError("execution reverted")
     alchemy_provider._web3 = mock_web3
 
     with pytest.raises(ContractLogicError, match="Transaction failed."):
         alchemy_provider.estimate_gas_cost(transaction)
 
 
-def test_feature_not_available(alchemy_provider, txn_hash):
-    with pytest.raises(APINotImplementedError):
-        list(alchemy_provider.get_transaction_trace(txn_hash))
-
-
 def test_get_contract_logs(networks, alchemy_provider, mock_web3, block, log_filter):
     mock_web3.eth.get_block.return_value = block
     alchemy_provider._web3 = mock_web3
     networks.active_provider = alchemy_provider
     actual = [x for x in alchemy_provider.get_contract_logs(log_filter)]
 
     # Fails when improper response handling of logs (is part of bug fix)
     assert actual == []
 
 
-def test_get_call_tree(networks, alchemy_provider, mock_web3, parity_trace, receipt):
+def test_get_transaction_trace(networks, alchemy_provider, mock_web3, parity_trace, receipt):
     mock_web3.provider.make_request.return_value = [parity_trace]
     mock_web3.eth.wait_for_transaction_receipt.return_value = receipt
     alchemy_provider._web3 = mock_web3
     networks.active_provider = alchemy_provider
-    actual = repr(alchemy_provider.get_call_tree(TXN_HASH))
-    expected = r"0xC17f2C69aE2E66FD87367E3260412EEfF637F70E\.0x96d373e5\(\) \[1401584 gas\]"
+    trace = alchemy_provider.get_transaction_trace(TXN_HASH)
+    actual = repr(trace.get_calltree())
+    expected = r"CALL: 0xC17f2C69aE2E66FD87367E3260412EEfF637F70E\.<0x96d373e5\> \[1401584 gas\]"
     assert re.match(expected, actual)
```

