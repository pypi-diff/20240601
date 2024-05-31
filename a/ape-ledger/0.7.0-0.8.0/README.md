# Comparing `tmp/ape-ledger-0.7.0.tar.gz` & `tmp/ape-ledger-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-ledger-0.7.0.tar", last modified: Tue Dec 19 02:17:11 2023, max compression
+gzip compressed data, was "ape-ledger-0.8.0.tar", last modified: Fri May 31 22:34:03 2024, max compression
```

## Comparing `ape-ledger-0.7.0.tar` & `ape-ledger-0.8.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:17:11.545759 ape-ledger-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:17:11.541759 ape-ledger-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:17:11.541759 ape-ledger-0.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:17:11.545759 ape-ledger-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      700 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      789 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-12-19 02:17:11.549759 ape-ledger-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:17:11.545759 ape-ledger-0.7.0/ape_ledger/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/ape_ledger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/ape_ledger/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6914 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/ape_ledger/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/ape_ledger/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/ape_ledger/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      315 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/ape_ledger/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2836 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/ape_ledger/hdpath.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/ape_ledger/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-19 02:17:11.000000 ape-ledger-0.7.0/ape_ledger/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:17:11.545759 ape-ledger-0.7.0/ape_ledger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-12-19 02:17:11.000000 ape-ledger-0.7.0/ape_ledger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2023-12-19 02:17:11.000000 ape-ledger-0.7.0/ape_ledger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 02:17:11.000000 ape-ledger-0.7.0/ape_ledger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-19 02:17:11.000000 ape-ledger-0.7.0/ape_ledger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 02:17:11.000000 ape-ledger-0.7.0/ape_ledger.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      819 2023-12-19 02:17:11.000000 ape-ledger-0.7.0/ape_ledger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-19 02:17:11.000000 ape-ledger-0.7.0/ape_ledger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2023-12-19 02:17:11.549759 ape-ledger-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:17:11.545759 ape-ledger-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2784 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     9738 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/tests/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/tests/test_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/tests/test_hdpath.py
--rw-r--r--   0 runner    (1001) docker     (127)     3656 2023-12-19 02:16:09.000000 ape-ledger-0.7.0/tests/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:34:03.837877 ape-ledger-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:34:03.833877 ape-ledger-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:34:03.833877 ape-ledger-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:34:03.833877 ape-ledger-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-31 22:34:03.837877 ape-ledger-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:34:03.837877 ape-ledger-0.8.0/ape_ledger/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/ape_ledger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5332 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/ape_ledger/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6961 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/ape_ledger/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3514 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/ape_ledger/choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/ape_ledger/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      315 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/ape_ledger/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2836 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/ape_ledger/hdpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/ape_ledger/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 22:34:03.000000 ape-ledger-0.8.0/ape_ledger/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:34:03.837877 ape-ledger-0.8.0/ape_ledger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-31 22:34:03.000000 ape-ledger-0.8.0/ape_ledger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-31 22:34:03.000000 ape-ledger-0.8.0/ape_ledger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:34:03.000000 ape-ledger-0.8.0/ape_ledger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-31 22:34:03.000000 ape-ledger-0.8.0/ape_ledger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:34:03.000000 ape-ledger-0.8.0/ape_ledger.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-31 22:34:03.000000 ape-ledger-0.8.0/ape_ledger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-31 22:34:03.000000 ape-ledger-0.8.0/ape_ledger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-31 22:34:03.837877 ape-ledger-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3719 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:34:03.837877 ape-ledger-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9642 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/tests/test_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/tests/test_hdpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3656 2024-05-31 22:32:59.000000 ape-ledger-0.8.0/tests/test_integration.py
```

### Comparing `ape-ledger-0.7.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-ledger-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.7.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-ledger-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.7.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-ledger-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.7.0/.github/release-drafter.yml` & `ape-ledger-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.7.0/.github/workflows/codeql.yml` & `ape-ledger-0.8.0/.github/workflows/codeql.yml`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
       security-events: write
 
     strategy:
       fail-fast: false
 
     steps:
     - name: Checkout repository
-      uses: actions/checkout@v3
+      uses: actions/checkout@v4
 
     - name: Initialize CodeQL
       uses: github/codeql-action/init@v2
       with:
         languages: python
 
     - name: Autobuild
```

### Comparing `ape-ledger-0.7.0/.github/workflows/commitlint.yaml` & `ape-ledger-0.8.0/.github/workflows/commitlint.yaml`

 * *Files 25% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 # NOTE: Skip check on PR so as not to confuse contributors
 # NOTE: Also install a PR title checker so we don't mess up merges
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
           with:
               fetch-depth: 0
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install "commitizen>=2.19,<2.20"
```

### Comparing `ape-ledger-0.7.0/.github/workflows/prtitle.yaml` & `ape-ledger-0.8.0/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
       - synchronize
 
 jobs:
     check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v2
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v2
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: pip install commitizen
 
         - name: Check PR Title
```

### Comparing `ape-ledger-0.7.0/.github/workflows/publish.yaml` & `ape-ledger-0.8.0/.github/workflows/publish.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v2
+    - uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v2
+      uses: actions/setup-python@v5
       with:
         python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
```

### Comparing `ape-ledger-0.7.0/.github/workflows/stale-prs.yml` & `ape-ledger-0.8.0/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.7.0/.github/workflows/test.yaml` & `ape-ledger-0.8.0/.github/workflows/test.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -10,18 +10,18 @@
   cancel-in-progress: true
 
 jobs:
     linting:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint]
@@ -38,18 +38,18 @@
         - name: Run mdformat
           run: mdformat . --check
 
     type-check:
         runs-on: ubuntu-latest
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: "3.10"
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[lint,test]
@@ -58,22 +58,24 @@
           run: mypy .
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
-                os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10", "3.11"]
+                # TODO: Replace with macos-latest when works again.
+                #   https://github.com/actions/setup-python/issues/808
+                os: [ubuntu-latest, macos-12]   # eventually add `windows-latest`
+                python-version: [3.9, "3.10", "3.11", "3.12"]
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: ${{ matrix.python-version }}
 
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[test]
@@ -85,18 +87,18 @@
 #    fuzzing:
 #        runs-on: ubuntu-latest
 #
 #        strategy:
 #            fail-fast: true
 #
 #        steps:
-#        - uses: actions/checkout@v3
+#        - uses: actions/checkout@v4
 #
 #        - name: Setup Python
-#          uses: actions/setup-python@v4
+#          uses: actions/setup-python@v5
 #          with:
 #              python-version: "3.10"
 #
 #        - name: Install Dependencies
 #          run: pip install .[test]
 #
 #        - name: Run Tests
```

### Comparing `ape-ledger-0.7.0/.gitignore` & `ape-ledger-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.7.0/.pre-commit-config.yaml` & `ape-ledger-0.8.0/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 repos:
 -   repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
     -   id: check-yaml
 
--   repo: https://github.com/pre-commit/mirrors-isort
-    rev: v5.10.1
+-   repo: https://github.com/PyCQA/isort
+    rev: 5.13.2
     hooks:
       - id: isort
 
 -   repo: https://github.com/psf/black
-    rev: 23.12.0
+    rev: 24.4.2
     hooks:
       - id: black
         name: black
 
 -   repo: https://github.com/pycqa/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
     -   id: flake8
 
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.7.1
+    rev: v1.10.0
     hooks:
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

### Comparing `ape-ledger-0.7.0/CONTRIBUTING.md` & `ape-ledger-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.7.0/LICENSE` & `ape-ledger-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.7.0/PKG-INFO` & `ape-ledger-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: ape-ledger
-Version: 0.7.0
+Version: 0.8.0
 Summary: ape-ledger: Plugin for Ledger Hardware Wallet
 Home-page: https://github.com/ApeWorX/ape-ledger
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
-Requires-Python: >=3.8,<4
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 Ape Ledger is a plugin for Ape Framework which integrates with Ledger devices
 to load and create accounts, sign messages, and sign transactions.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-ledger-0.7.0/README.md` & `ape-ledger-0.8.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Quick Start
 
 Ape Ledger is a plugin for Ape Framework which integrates with Ledger devices
 to load and create accounts, sign messages, and sign transactions.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-ledger-0.7.0/ape_ledger/_cli.py` & `ape-ledger-0.8.0/ape_ledger/_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Tuple, Union
+from typing import Union
 
 import click
 from ape import accounts
 from ape.cli import (
     ape_cli_context,
     existing_alias_argument,
     network_option,
@@ -14,15 +14,15 @@
 
 from ape_ledger.accounts import LedgerAccount
 from ape_ledger.choices import AddressPromptChoice
 from ape_ledger.exceptions import LedgerSigningError
 from ape_ledger.hdpath import HDAccountPath, HDBasePath
 
 
-def _select_account(hd_path: Union[HDBasePath, str]) -> Tuple[str, HDAccountPath]:
+def _select_account(hd_path: Union[HDBasePath, str]) -> tuple[str, HDAccountPath]:
     choices = AddressPromptChoice(hd_path)
     return choices.get_user_selected_account()
 
 
 @click.group(short_help="Manage Ledger accounts")
 def cli():
     """
@@ -48,15 +48,15 @@
 
     for account in ledger_accounts:
         alias_display = f" (alias: '{account.alias}')" if account.alias else ""
         hd_path_display = f" (hd-path: '{account.hdpath}')" if account.hdpath else ""
         click.echo(f"  {account.address}{alias_display}{hd_path_display}")
 
 
-def _get_ledger_accounts() -> List[LedgerAccount]:
+def _get_ledger_accounts() -> list[LedgerAccount]:
     return [a for a in accounts if isinstance(a, LedgerAccount)]
 
 
 @cli.command()
 @ape_cli_context()
 @non_existing_alias_argument()
 @click.option(
```

### Comparing `ape-ledger-0.7.0/ape_ledger/accounts.py` & `ape-ledger-0.8.0/ape_ledger/accounts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import json
+from collections.abc import Iterator
 from pathlib import Path
-from typing import Any, Dict, Iterator, Optional
+from typing import Any, Optional
 
 import rich
 from ape.api import AccountAPI, AccountContainerAPI, TransactionAPI
 from ape.types import AddressType, MessageSignature, TransactionSignature
 from ape_ethereum.transactions import DynamicFeeTransaction, StaticFeeTransaction
 from dataclassy import asdict
 from eip712 import EIP712Message, EIP712Type
@@ -27,14 +28,16 @@
     elif isinstance(val, HexBytes):
         return bytes(val)
     else:
         return to_bytes(val)
 
 
 class AccountContainer(AccountContainerAPI):
+    name: str = "ledger"
+
     @property
     def accounts(self) -> Iterator[AccountAPI]:
         for account_file in self._account_files:
             yield LedgerAccount(container=self, account_file_path=account_file)
 
     def __setitem__(self, address: AddressType, account: AccountAPI):
         raise NotImplementedError()
@@ -168,15 +171,15 @@
             signed_msg = self._client.sign_message(msg_to_sign.body)
 
         v, r, s = signed_msg
         return MessageSignature(v=v, r=HexBytes(r), s=HexBytes(s))
 
     def sign_transaction(self, txn: TransactionAPI, **kwargs) -> Optional[TransactionAPI]:
         txn.chain_id = 1
-        txn_dict: Dict = {
+        txn_dict: dict = {
             "nonce": txn.nonce,
             "gas": txn.gas_limit,
             "amount": txn.value,
             "data": _to_bytes(txn.data.hex()),
             "destination": _to_bytes(txn.receiver),
             "chain_id": txn.chain_id,
         }
```

### Comparing `ape-ledger-0.7.0/ape_ledger/choices.py` & `ape-ledger-0.8.0/ape_ledger/choices.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Optional, Tuple, Union
+from typing import Any, Optional, Union
 
 import click
 from ape.cli import PromptChoice
 from click import Context, Parameter
 
 from ape_ledger.client import get_device
 from ape_ledger.hdpath import HDAccountPath, HDBasePath
@@ -54,15 +54,15 @@
             return None
 
         address = super().convert(value, param, ctx)
         address_index = self.choices.index(address)
         self._choice_index = self._choice_index if address_index is None else address_index
         return address
 
-    def get_user_selected_account(self) -> Tuple[str, HDAccountPath]:
+    def get_user_selected_account(self) -> tuple[str, HDAccountPath]:
         """Returns the selected address from the user along with the HD path.
         The user is able to page using special characters ``n`` and ``p``.
         """
         address = None
         while address is None:
             self._load_choices()
             self.print_choices()
```

### Comparing `ape-ledger-0.7.0/ape_ledger/client.py` & `ape-ledger-0.8.0/ape_ledger/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import atexit
 from functools import cached_property
-from typing import Dict, Tuple
 
 import hid  # type: ignore
 from ape.logging import LogLevel, logger
 from ledgerblue.comm import HIDDongleHIDAPI, getDongle  # type: ignore
 from ledgereth.accounts import get_account_by_path
 from ledgereth.messages import sign_message, sign_typed_data_draft
 from ledgereth.transactions import SignedType2Transaction, create_transaction
 
 from ape_ledger.hdpath import HDAccountPath
 
 
 class DeviceFactory:
-    device_map: Dict[str, "LedgerDeviceClient"] = {}
+    device_map: dict[str, "LedgerDeviceClient"] = {}
 
     def create_device(self, account: HDAccountPath):
         if account.path in self.device_map:
             return self.device_map[account.path]
 
         device = LedgerDeviceClient(account)
         self.device_map[account.path] = device
@@ -52,31 +51,32 @@
 
         atexit.register(close)
         return device
 
     def get_address(self) -> str:
         return get_account_by_path(self._account, dongle=self.dongle).address
 
-    def sign_message(self, text: bytes) -> Tuple[int, int, int]:
+    def sign_message(self, text: bytes) -> tuple[int, int, int]:
         signed_msg = sign_message(text, sender_path=self._account, dongle=self.dongle)
         return signed_msg.v, signed_msg.r, signed_msg.s
 
-    def sign_typed_data(self, domain_hash: bytes, message_hash: bytes) -> Tuple[int, int, int]:
+    def sign_typed_data(self, domain_hash: bytes, message_hash: bytes) -> tuple[int, int, int]:
         signed_msg = sign_typed_data_draft(
             domain_hash, message_hash, sender_path=self._account, dongle=self.dongle
         )
         return signed_msg.v, signed_msg.r, signed_msg.s
 
-    def sign_transaction(self, txn: Dict) -> Tuple[int, int, int]:
+    def sign_transaction(self, txn: dict) -> tuple[int, int, int]:
         kwargs = {**txn, "sender_path": self._account, "dongle": self.dongle}
         signed_tx = create_transaction(**kwargs)
-        if isinstance(signed_tx, SignedType2Transaction):
-            return signed_tx.y_parity, signed_tx.sender_r, signed_tx.sender_s
-        else:
-            return signed_tx.v, signed_tx.r, signed_tx.s
+        return (
+            (signed_tx.y_parity, signed_tx.sender_r, signed_tx.sender_s)
+            if isinstance(signed_tx, SignedType2Transaction)
+            else (signed_tx.v, signed_tx.r, signed_tx.s)
+        )
 
 
 _device_factory = DeviceFactory()
 
 
 def get_device(account: HDAccountPath):
     return _device_factory.create_device(account)
```

### Comparing `ape-ledger-0.7.0/ape_ledger/hdpath.py` & `ape-ledger-0.8.0/ape_ledger/hdpath.py`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.7.0/ape_ledger.egg-info/PKG-INFO` & `ape-ledger-0.8.0/ape_ledger.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: ape-ledger
-Version: 0.7.0
+Version: 0.8.0
 Summary: ape-ledger: Plugin for Ledger Hardware Wallet
 Home-page: https://github.com/ApeWorX/ape-ledger
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
-Requires-Python: >=3.8,<4
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 Ape Ledger is a plugin for Ape Framework which integrates with Ledger devices
 to load and create accounts, sign messages, and sign transactions.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-ledger-0.7.0/ape_ledger.egg-info/SOURCES.txt` & `ape-ledger-0.8.0/ape_ledger.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.7.0/ape_ledger.egg-info/requires.txt` & `ape-ledger-0.8.0/ape_ledger.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-eth-ape<0.8,>=0.7.0
+eth-ape<0.9,>=0.8.1
 ledgereth<0.10,>=0.9.1
 click
 rich
 ethpm-types
 eip712
 eth-account
 eth-utils
 
 [dev]
 pytest>=6.0
 pytest-xdist
 pytest-cov
 pytest-mock
 hypothesis<7.0,>=6.2.0
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 setuptools
 wheel
 twine
 commitizen
 pre-commit
 pytest-watch
 IPython
 ipdb
 
 [lint]
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-setuptools
-flake8<7,>=6.1.0
+flake8<8,>=7.0.0
 flake8-breakpoint<2,>=1.1.0
 flake8-print<6,>=5.0.0
-isort<6,>=5.10.1
+isort<6,>=5.13.2
 mdformat>=0.7.17
 mdformat-gfm>=0.3.5
 mdformat-frontmatter>=0.4.1
 mdformat-pyproject>=0.0.1
 
 [release]
 setuptools
```

### Comparing `ape-ledger-0.7.0/pyproject.toml` & `ape-ledger-0.8.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310', 'py311']
+target-version = ['py39', 'py310', 'py311', 'py312']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
 	-p no:ape_test
 	--cov-branch
 	--cov-report term
```

### Comparing `ape-ledger-0.7.0/setup.py` & `ape-ledger-0.8.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 extras_require = {
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "pytest-mock",  # For creating mocks
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=23.12.0,<24",  # Auto-formatter and linter
-        "mypy>=1.7.1,<2",  # Static type analyzer
+        "black>=24.4.2,<25",  # Auto-formatter and linter
+        "mypy>=1.10.0,<2",  # Static type analyzer
         "types-setuptools",  # Needed for mypy type shed
-        "flake8>=6.1.0,<7",  # Style linter
+        "flake8>=7.0.0,<8",  # Style linter
         "flake8-breakpoint>=1.1.0,<2",  # Detect breakpoints left in code
         "flake8-print>=5.0.0,<6",  # Detect print statements left in code
-        "isort>=5.10.1,<6",  # Import sorting linter
+        "isort>=5.13.2,<6",  # Import sorting linter
         "mdformat>=0.7.17",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
         "mdformat-pyproject>=0.0.1",  # Allows configuring in pyproject.toml
     ],
     "release": [  # `release` GitHub Action job uses this
         "setuptools",  # Installation tool
@@ -57,15 +56,15 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-ledger",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.7.0,<0.8",
+        "eth-ape>=0.8.1,<0.9",
         "ledgereth>=0.9.1,<0.10",
         "click",  # Use same version as eth-ape
         "rich",  # Use same version as eth-ape
         # ApeWorX-owned
         "ethpm-types",  # Use same version as eth-ape
         "eip712",  # Use same version as eth-ape
         # EF Dependencies
@@ -73,15 +72,15 @@
         "eth-utils",  # Use same version as eth-ape
     ],
     entry_points={
         "ape_cli_subcommands": [
             "ape_ledger=ape_ledger._cli:cli",
         ],
     },
-    python_requires=">=3.8,<4",
+    python_requires=">=3.9,<4",
     extras_require=extras_require,
     py_modules=["ape_ledger"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_ledger": ["py.typed"]},
@@ -89,13 +88,13 @@
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
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `ape-ledger-0.7.0/tests/conftest.py` & `ape-ledger-0.8.0/tests/conftest.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,46 @@
 import json
+import shutil
+from pathlib import Path
+from tempfile import mkdtemp
 
+import ape
 import pytest
-from ape import accounts, networks
 from click.testing import CliRunner
 from eth_account.messages import encode_defunct
 from eth_pydantic_types import HexBytes
 
 TEST_ALIAS = "TestAlias"
 TEST_HD_PATH = "m/44'/60'/{x}'/0/0"
 
 
+# NOTE: Ensure that we don't use local paths for these
+DATA_FOLDER = Path(mkdtemp()).resolve()
+ape.config.DATA_FOLDER = DATA_FOLDER
+
+
+@pytest.fixture(autouse=True, scope="session")
+def clean_data_folder():
+    yield  # Run all tests
+    shutil.rmtree(DATA_FOLDER, ignore_errors=True)
+
+
 @pytest.fixture
 def hd_path():
     return TEST_HD_PATH
 
 
 @pytest.fixture
 def alias():
     return TEST_ALIAS
 
 
 @pytest.fixture
 def test_accounts():
-    return accounts.test_accounts
+    return ape.accounts.test_accounts
 
 
 @pytest.fixture
 def account_addresses(test_accounts):
     return [a.address for a in test_accounts]
 
 
@@ -43,15 +57,15 @@
 @pytest.fixture
 def address(account_addresses):
     return account_addresses[0]
 
 
 @pytest.fixture(autouse=True)
 def connection():
-    with networks.ethereum.local.use_provider("test") as provider:
+    with ape.networks.ethereum.local.use_provider("test") as provider:
         yield provider
 
 
 @pytest.fixture
 def msg_signature(account_0):
     msg = encode_defunct(text="__TEST_MESSAGE__")
     sig = account_0.sign_message(msg)
@@ -76,16 +90,16 @@
     )
 
 
 @pytest.fixture(autouse=True)
 def mock_device(mocker, hd_path, account_addresses, msg_signature, tx_signature):
     device = mocker.MagicMock()
     device._account = hd_path
-    device.get_address.side_effect = (
-        lambda *args, **kwargs: account_addresses[args[0]] if args else account_addresses[0]
+    device.get_address.side_effect = lambda *args, **kwargs: (
+        account_addresses[args[0]] if args else account_addresses[0]
     )
     device.sign_message.side_effect = lambda *args, **kwargs: msg_signature
     device.sign_typed_data.side_effect = lambda *args, **kwargs: msg_signature
     device.sign_transaction.side_effect = lambda *args, **kwargs: tx_signature
     return device
 
 
@@ -97,20 +111,20 @@
 @pytest.fixture
 def runner():
     return CliRunner()
 
 
 @pytest.fixture
 def assert_account(address):
-    def fn(account_path, expected_address=None, expected_hdpath="m/44'/60'/0'/0/0"):
+    def fn(account_path: Path, expected_address=None, expected_hdpath="m/44'/60'/0'/0/0"):
         expected_address = expected_address or address
-        with open(account_path) as account_file:
-            account_data = json.load(account_file)
-            assert account_data["address"] == expected_address
-            assert account_data["hdpath"] == expected_hdpath
+        assert account_path.is_file(), "Account file missing."
+        account_data = json.loads(account_path.read_text())
+        assert account_data["address"] == expected_address
+        assert account_data["hdpath"] == expected_hdpath
 
     return fn
 
 
 @pytest.fixture
 def device_factory(mocker, mock_device):
     def fn(module):
```

### Comparing `ape-ledger-0.7.0/tests/test_accounts.py` & `ape-ledger-0.8.0/tests/test_accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import json
-import tempfile
-from pathlib import Path
 from typing import Optional, cast
 
 import pytest
 from ape import networks
 from ape.api import TransactionAPI
 from ape.types import AddressType
+from ape.utils import create_tempdir
 from ape_ethereum.ecosystem import DynamicFeeTransaction, StaticFeeTransaction
 from eip712.messages import EIP712Message, EIP712Type
 from eth_account.messages import SignableMessage
 from eth_pydantic_types import HexBytes
 
 from ape_ledger.accounts import AccountContainer, LedgerAccount
 from ape_ledger.exceptions import LedgerSigningError
@@ -101,29 +100,28 @@
 def isolated_file_system(runner):
     with runner.isolated_filesystem():
         yield
 
 
 @pytest.fixture
 def account(mock_container, create_account, hd_path):
-    with tempfile.TemporaryDirectory() as temp_dir:
-        path = Path(temp_dir) / "account.json"
+    with create_tempdir() as temp_dir:
+        path = temp_dir / "account.json"
         create_account(path, hd_path)
         with networks.ethereum.local.use_provider("test"):
-            yield LedgerAccount(container=mock_container, account_file_path=path)
+            yield LedgerAccount(name=mock_container, account_file_path=path)
 
 
 class TestAccountContainer:
     def test_save_account(self, mock_container, alias, address, hd_path, assert_account):
-        with tempfile.TemporaryDirectory() as temp_dir:
-            data_path = Path(temp_dir)
-            container = AccountContainer(data_folder=data_path, account_type=LedgerAccount)
-            container.save_account(alias, address, hd_path)
-            account_path = data_path / f"{alias}.json"
-            assert_account(account_path, expected_hdpath=hd_path)
+        container = AccountContainer(account_type=LedgerAccount)
+        container.save_account(alias, address, hd_path)
+        temp_dir = container.config_manager.DATA_FOLDER
+        account_path = temp_dir / "ledger" / f"{alias}.json"
+        assert_account(account_path, expected_hdpath=hd_path)
 
 
 class TestLedgerAccount:
     def test_address_returns_address_from_file(self, account, address):
         assert account.address.lower() == address.lower()
 
     def test_hdpath_returns_address_from_file(self, account, hd_path):
```

### Comparing `ape-ledger-0.7.0/tests/test_choices.py` & `ape-ledger-0.8.0/tests/test_choices.py`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.7.0/tests/test_hdpath.py` & `ape-ledger-0.8.0/tests/test_hdpath.py`

 * *Files identical despite different names*

### Comparing `ape-ledger-0.7.0/tests/test_integration.py` & `ape-ledger-0.8.0/tests/test_integration.py`

 * *Files identical despite different names*

