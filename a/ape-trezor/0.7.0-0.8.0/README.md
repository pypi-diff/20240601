# Comparing `tmp/ape-trezor-0.7.0.tar.gz` & `tmp/ape-trezor-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-trezor-0.7.0.tar", last modified: Tue Dec 19 02:12:25 2023, max compression
+gzip compressed data, was "ape-trezor-0.8.0.tar", last modified: Sat Jun  1 01:11:02 2024, max compression
```

## Comparing `ape-trezor-0.7.0.tar` & `ape-trezor-0.8.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:12:25.422404 ape-trezor-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:12:25.414404 ape-trezor-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:12:25.414404 ape-trezor-0.7.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:12:25.418404 ape-trezor-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      368 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2496 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      803 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2023-12-19 02:12:25.422404 ape-trezor-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2650 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:12:25.418404 ape-trezor-0.7.0/ape_trezor/
--rw-r--r--   0 runner    (1001) docker     (127)      280 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/ape_trezor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5287 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/ape_trezor/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7246 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/ape_trezor/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3248 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/ape_trezor/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/ape_trezor/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1149 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/ape_trezor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/ape_trezor/hdpath.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/ape_trezor/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/ape_trezor/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-12-19 02:12:25.000000 ape-trezor-0.7.0/ape_trezor/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:12:25.418404 ape-trezor-0.7.0/ape_trezor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2023-12-19 02:12:25.000000 ape-trezor-0.7.0/ape_trezor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2023-12-19 02:12:25.000000 ape-trezor-0.7.0/ape_trezor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 02:12:25.000000 ape-trezor-0.7.0/ape_trezor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       55 2023-12-19 02:12:25.000000 ape-trezor-0.7.0/ape_trezor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-19 02:12:25.000000 ape-trezor-0.7.0/ape_trezor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2023-12-19 02:12:25.000000 ape-trezor-0.7.0/ape_trezor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2023-12-19 02:12:25.000000 ape-trezor-0.7.0/ape_trezor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      985 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-12-19 02:12:25.422404 ape-trezor-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3919 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:12:25.422404 ape-trezor-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3230 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3499 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/tests/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/tests/test_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6680 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/tests/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-19 02:12:25.422404 ape-trezor-0.7.0/tests/trezor/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2023-12-19 02:11:34.000000 ape-trezor-0.7.0/tests/trezor/vitalik.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:11:02.806654 ape-trezor-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:11:02.802654 ape-trezor-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:11:02.802654 ape-trezor-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:11:02.802654 ape-trezor-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-06-01 01:11:02.806654 ape-trezor-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2650 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:11:02.806654 ape-trezor-0.8.0/ape_trezor/
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/ape_trezor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/ape_trezor/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7267 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/ape_trezor/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/ape_trezor/choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6982 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/ape_trezor/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1149 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/ape_trezor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/ape_trezor/hdpath.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/ape_trezor/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/ape_trezor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-01 01:11:02.000000 ape-trezor-0.8.0/ape_trezor/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:11:02.806654 ape-trezor-0.8.0/ape_trezor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-06-01 01:11:02.000000 ape-trezor-0.8.0/ape_trezor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-06-01 01:11:02.000000 ape-trezor-0.8.0/ape_trezor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:11:02.000000 ape-trezor-0.8.0/ape_trezor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-01 01:11:02.000000 ape-trezor-0.8.0/ape_trezor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:11:02.000000 ape-trezor-0.8.0/ape_trezor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-06-01 01:11:02.000000 ape-trezor-0.8.0/ape_trezor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-01 01:11:02.000000 ape-trezor-0.8.0/ape_trezor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-01 01:11:02.806654 ape-trezor-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:11:02.806654 ape-trezor-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2352 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/tests/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/tests/test_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3642 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6680 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/tests/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:11:02.806654 ape-trezor-0.8.0/tests/trezor/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-06-01 01:10:09.000000 ape-trezor-0.8.0/tests/trezor/vitalik.json
```

### Comparing `ape-trezor-0.7.0/.github/ISSUE_TEMPLATE/bug.md` & `ape-trezor-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.7.0/.github/ISSUE_TEMPLATE/feature.md` & `ape-trezor-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.7.0/.github/ISSUE_TEMPLATE/work-item.md` & `ape-trezor-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.7.0/.github/release-drafter.yml` & `ape-trezor-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.7.0/.github/workflows/codeql.yml` & `ape-trezor-0.8.0/.github/workflows/codeql.yml`

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

### Comparing `ape-trezor-0.7.0/.github/workflows/commit.yaml` & `ape-trezor-0.8.0/.github/workflows/commit.yaml`

 * *Files 22% similar despite different names*

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
           run: pip install commitizen
 
         - name: Check commit history
```

### Comparing `ape-trezor-0.7.0/.github/workflows/prtitle.yaml` & `ape-trezor-0.8.0/.github/workflows/prtitle.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -8,18 +8,18 @@
       - synchronize
 
 jobs:
     check:
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
           run: pip install commitizen
 
         - name: Check PR Title
```

### Comparing `ape-trezor-0.7.0/.github/workflows/publish.yaml` & `ape-trezor-0.8.0/.github/workflows/publish.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 
 jobs:
   deploy:
 
     runs-on: ubuntu-latest
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: "3.10"
 
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install -e .[release]
```

### Comparing `ape-trezor-0.7.0/.github/workflows/stale-prs.yml` & `ape-trezor-0.8.0/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.7.0/.github/workflows/test.yaml` & `ape-trezor-0.8.0/.github/workflows/test.yaml`

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

### Comparing `ape-trezor-0.7.0/.gitignore` & `ape-trezor-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.7.0/.pre-commit-config.yaml` & `ape-trezor-0.8.0/.pre-commit-config.yaml`

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
         additional_dependencies: [types-PyYAML, types-setuptools, pydantic]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
     -   id: mdformat
-        additional_dependencies: [mdformat-gfm, mdformat-frontmatter]
+        additional_dependencies: [mdformat-gfm, mdformat-frontmatter, mdformat-pyproject]
 
 default_language_version:
     python: python3
```

### Comparing `ape-trezor-0.7.0/CONTRIBUTING.md` & `ape-trezor-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.7.0/LICENSE` & `ape-trezor-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.7.0/PKG-INFO` & `ape-trezor-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: ape-trezor
-Version: 0.7.0
+Version: 0.8.0
 Summary: ape-trezor: Plugin for Trezor Hardware Wallets
 Home-page: https://github.com/ApeWorX/ape-trezor
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
-Requires-Python: >=3.8,<4
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 Ape Trezor is a plugin for [Ape Framework](https://github.com/ApeWorx/ape) which integrates [Trezorlib ethereum.py](https://github.com/trezor/trezor-firmware/blob/master/python/src/trezorlib/ethereum.py) to load and create accounts, sign messages, and sign transactions.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up tp 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up tp 3.12.
 
 **Note**: USB does not work in WSL2 environments natively and is [not currently supported](https://github.com/microsoft/WSL/issues/5158).
 
 ## Installation
 
 ### via `pip`
```

### Comparing `ape-trezor-0.7.0/README.md` & `ape-trezor-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ape Trezor is a plugin for [Ape Framework](https://github.com/ApeWorx/ape) which integrates [Trezorlib ethereum.py](https://github.com/trezor/trezor-firmware/blob/master/python/src/trezorlib/ethereum.py) to load and create accounts, sign messages, and sign transactions.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up tp 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up tp 3.12.
 
 **Note**: USB does not work in WSL2 environments natively and is [not currently supported](https://github.com/microsoft/WSL/issues/5158).
 
 ## Installation
 
 ### via `pip`
```

### Comparing `ape-trezor-0.7.0/ape_trezor/_cli.py` & `ape-trezor-0.8.0/ape_trezor/_cli.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.7.0/ape_trezor/accounts.py` & `ape-trezor-0.8.0/ape_trezor/accounts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
+from collections.abc import Iterator
 from functools import cached_property
 from pathlib import Path
-from typing import Any, Dict, Iterator, Optional
+from typing import Any, Optional
 
 from ape.api import AccountAPI, AccountContainerAPI, PluginConfig, TransactionAPI
 from ape.types import AddressType, MessageSignature, TransactionSignature
 from dataclassy import asdict
 from eip712 import EIP712Message, EIP712Type
 from eth_account.messages import SignableMessage, encode_defunct
 from eth_pydantic_types import HexBytes
@@ -179,17 +180,17 @@
         else:
             raise TrezorAccountError(f"Message type {tx_type} is not supported.")
 
         txn.signature = TransactionSignature(v=v, r=r, s=s)
         return txn
 
 
-def _prepare_data_for_hashing(data: Dict) -> Dict:
+def _prepare_data_for_hashing(data: dict) -> dict:
     # NOTE: Private method copied from eip712 package.
-    result: Dict = {}
+    result: dict = {}
 
     for key, value in data.items():
         item: Any = value
         if isinstance(value, EIP712Type):
             item = asdict(value)
         elif isinstance(value, dict):
             item = _prepare_data_for_hashing(item)
```

### Comparing `ape-trezor-0.7.0/ape_trezor/choices.py` & `ape-trezor-0.8.0/ape_trezor/choices.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Optional, Tuple
+from typing import Any, Optional
 
 import click
 from ape.cli import PromptChoice
 from click import Context, Parameter
 
 from ape_trezor.client import TrezorClient
 from ape_trezor.hdpath import HDBasePath, HDPath
@@ -52,15 +52,15 @@
             # Don't select an address yet if user paged.
             return None
 
         address = super().convert(value, param, ctx)
         self._choice_index = self.choices.index(address)  # type: ignore
         return address
 
-    def get_user_selected_account(self) -> Tuple[str, HDPath]:
+    def get_user_selected_account(self) -> tuple[str, HDPath]:
         """Returns the selected address from the user along with the HD path.
         The user is able to page using special characters ``n`` and ``p``.
         """
         address = None
         while address is None:
             self._load_choices()
             self.print_choices()
```

### Comparing `ape-trezor-0.7.0/ape_trezor/client.py` & `ape-trezor-0.8.0/ape_trezor/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Callable, Dict, Optional, Tuple
+from collections.abc import Callable
+from typing import Optional
 
 from ape.logging import logger
 from eth_typing.evm import ChecksumAddress
 from trezorlib.client import TrezorClient as LibTrezorClient
 from trezorlib.client import get_default_client
 from trezorlib.device import apply_settings
 from trezorlib.ethereum import (
@@ -64,15 +65,15 @@
             if "forbidden key path" in str(err).lower():
                 raise InvalidHDPathError(str(account_path))
 
             code = 0 if not err.code else err.code.value
             raise TrezorClientError(str(err), status=code) from err
 
 
-def extract_signature_vrs_bytes(signature_bytes: bytes) -> Tuple[int, bytes, bytes]:
+def extract_signature_vrs_bytes(signature_bytes: bytes) -> tuple[int, bytes, bytes]:
     """
     Breaks `signature_bytes` into 3 chunks vrs, where `v` is 1 byte, `r` is 32
     bytes, and `s` is 32 bytes.
     """
     if signature_bytes is None:
         raise TrezorClientError("No data in signature bytes.")
 
@@ -105,66 +106,66 @@
     def __str__(self):
         return self._address
 
     @property
     def address(self) -> str:
         return self._address
 
-    def sign_personal_message(self, message: bytes) -> Tuple[int, bytes, bytes]:
+    def sign_personal_message(self, message: bytes) -> tuple[int, bytes, bytes]:
         """
         Sign an Ethereum message only following the EIP 191 specification and
         using your Trezor device. You will need to follow the prompts on the device
         to validate the message data.
         """
         ethereum_message_signature = sign_message(
             self.client, self._account_hd_path.address_n, message
         )
         return extract_signature_vrs_bytes(signature_bytes=ethereum_message_signature.signature)
 
-    def sign_typed_data(self, data: Dict) -> Tuple[int, bytes, bytes]:
+    def sign_typed_data(self, data: dict) -> tuple[int, bytes, bytes]:
         """
         Sends a dict of data to the device and is much more obvious and secure
         than signing a hash alone.
 
         Args:
-            data(Dict): The data to sign, following EIP-712.
+            data(dict): The data to sign, following EIP-712.
 
         Returns:
-            Tuple[int, bytes, bytes]: A signature tuple.
+            tuple[int, bytes, bytes]: A signature tuple.
         """
         signed_data = sign_typed_data(self.client, self._account_hd_path.address_n, data)
         return extract_signature_vrs_bytes(signature_bytes=signed_data.signature)
 
     def sign_typed_data_hash(
         self, domain_hash: bytes, message_hash: bytes
-    ) -> Tuple[int, bytes, bytes]:
+    ) -> tuple[int, bytes, bytes]:
         """
         Sign an Ethereum message following the EIP 712 specification.
         This approach still uses the hash on the device and may not look
         as nice as calling :meth:`~ape_trezor.client.TrezorAccountClient.sign_typed_data`.
 
         Args:
             domain_hash (bytes): The hashed domain of the data.
             message_hash (bytes): The hashed message portion of the data.
 
         Returns:
-            Tuple[int, bytes, bytes]: A signature tuple.
+            tuple[int, bytes, bytes]: A signature tuple.
         """
         signed_data = sign_typed_data_hash(
             self.client, self._account_hd_path.address_n, domain_hash, message_hash=message_hash
         )
         return extract_signature_vrs_bytes(signature_bytes=signed_data.signature)
 
-    def sign_static_fee_transaction(self, **kwargs) -> Tuple[int, bytes, bytes]:
+    def sign_static_fee_transaction(self, **kwargs) -> tuple[int, bytes, bytes]:
         return self._sign_transaction(sign_tx, **kwargs)
 
-    def sign_dynamic_fee_transaction(self, **kwargs) -> Tuple[int, bytes, bytes]:
+    def sign_dynamic_fee_transaction(self, **kwargs) -> tuple[int, bytes, bytes]:
         return self._sign_transaction(sign_tx_eip1559, **kwargs)
 
-    def _sign_transaction(self, lib_call: Callable, **kwargs) -> Tuple[int, bytes, bytes]:
+    def _sign_transaction(self, lib_call: Callable, **kwargs) -> tuple[int, bytes, bytes]:
         did_change = self._allow_default_ethereum_account_signing()
         try:
             return lib_call(self.client, self._account_hd_path.address_n, **kwargs)
 
         except TrezorFailure as err:
             forbidden_key_path = "forbidden key path" in str(err).lower()
             if forbidden_key_path:
```

### Comparing `ape-trezor-0.7.0/ape_trezor/exceptions.py` & `ape-trezor-0.8.0/ape_trezor/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.7.0/ape_trezor/hdpath.py` & `ape-trezor-0.8.0/ape_trezor/hdpath.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.7.0/ape_trezor.egg-info/PKG-INFO` & `ape-trezor-0.8.0/ape_trezor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: ape-trezor
-Version: 0.7.0
+Version: 0.8.0
 Summary: ape-trezor: Plugin for Trezor Hardware Wallets
 Home-page: https://github.com/ApeWorX/ape-trezor
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
-Requires-Python: >=3.8,<4
+Classifier: Programming Language :: Python :: 3.12
+Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: lint
 Provides-Extra: doc
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 Ape Trezor is a plugin for [Ape Framework](https://github.com/ApeWorx/ape) which integrates [Trezorlib ethereum.py](https://github.com/trezor/trezor-firmware/blob/master/python/src/trezorlib/ethereum.py) to load and create accounts, sign messages, and sign transactions.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up tp 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up tp 3.12.
 
 **Note**: USB does not work in WSL2 environments natively and is [not currently supported](https://github.com/microsoft/WSL/issues/5158).
 
 ## Installation
 
 ### via `pip`
```

### Comparing `ape-trezor-0.7.0/ape_trezor.egg-info/SOURCES.txt` & `ape-trezor-0.8.0/ape_trezor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.7.0/ape_trezor.egg-info/requires.txt` & `ape-trezor-0.8.0/ape_trezor.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-eth-ape<0.8,>=0.7.0
+eth-ape<0.9,>=0.8.1
 click
 trezor[ethereum]<0.14,>=0.13.8
 eth-pydantic-types
 eth-typing
 eth-account
 
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
 types-PyYAML
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
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
@@ -37,22 +37,22 @@
 
 [doc]
 Sphinx<7,>=6.1.3
 sphinx_rtd_theme<2,>=1.2.0
 towncrier<20,>=19.2.0
 
 [lint]
-black<24,>=23.12.0
-mypy<2,>=1.7.1
+black<25,>=24.4.2
+mypy<2,>=1.10.0
 types-PyYAML
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

### Comparing `ape-trezor-0.7.0/pyproject.toml` & `ape-trezor-0.8.0/pyproject.toml`

 * *Files 11% similar despite different names*

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

### Comparing `ape-trezor-0.7.0/setup.py` & `ape-trezor-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 extras_require = {
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-xdist",  # Multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "pytest-mock",  # For creating mocks
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=23.12.0,<24",  # Auto-formatter and linter
-        "mypy>=1.7.1,<2",  # Static type analyzer
+        "black>=24.4.2,<25",  # Auto-formatter and linter
+        "mypy>=1.10.0,<2",  # Static type analyzer
         "types-PyYAML",  # Needed for mypy typeshed
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
     "doc": [
         "Sphinx>=6.1.3,<7",  # Documentation generator
@@ -64,29 +63,29 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-trezor",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.7.0,<0.8",
+        "eth-ape>=0.8.1,<0.9",
         "click",  # Use same version as eth-ape
         "trezor[ethereum]>=0.13.8,<0.14",
         # ApeWorx packages
         "eth-pydantic-types",  # Use same version as eth-ape
         # Ethereum Foundation packages
         "eth-typing",  # Use same version as eth-ape
         "eth-account",  # Use same version as eth-ape
     ],
     entry_points={
         "ape_cli_subcommands": [
             "ape_trezor=ape_trezor._cli:cli",
         ],
     },
-    python_requires=">=3.8,<4",
+    python_requires=">=3.9,<4",
     extras_require=extras_require,
     py_modules=["ape_trezor"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_trezor": ["py.typed"]},
@@ -94,13 +93,13 @@
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
+        "Programming Language :: Python :: 3.12",
     ],
 )
```

### Comparing `ape-trezor-0.7.0/tests/test_accounts.py` & `ape-trezor-0.8.0/tests/test_accounts.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.7.0/tests/test_choices.py` & `ape-trezor-0.8.0/tests/test_choices.py`

 * *Files identical despite different names*

### Comparing `ape-trezor-0.7.0/tests/test_cli.py` & `ape-trezor-0.8.0/tests/test_cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -47,29 +47,28 @@
     expected = (
         "Using the default Ethereum HD Path is not recommended for 3rd party wallets. "
         "Please use an alternative HD-Path for a safer integration."
     )
     assert log_warning == expected
 
 
-def test_add_specify_hd_path(mock_client, runner, cli, accounts, clean, mock_client_factory):
+def test_add_specify_hd_path(mock_client, runner, cli, clean, mock_client_factory):
     mock_client.get_account_path.return_value = ZERO_ADDRESS
     hd_path = "m/44'/1'/0'/0"
     result = runner.invoke(cli, ["add", NEW_ACCOUNT_ALIAS, "--hd-path", hd_path], input="0\n")
     assert result.exit_code == 0, result.output
     assert mock_client_factory.call_args[0][-1].path == hd_path
 
 
 def test_add_uses_hd_path_from_config(
-    mock_client, temp_config, runner, cli, clean, mock_client_factory, accounts
+    mock_client, project, runner, cli, clean, mock_client_factory, accounts
 ):
     mock_client.get_account_path.return_value = ZERO_ADDRESS
     hd_path = "m/1'/60'/0'/0"
-    data = {"trezor": {"hd_path": hd_path}}
-    with temp_config(data):
+    with project.temp_config(trezor={"hd_path": hd_path}):
         result = runner.invoke(cli, ["add", NEW_ACCOUNT_ALIAS], input="0\n")
         assert result.exit_code == 0, result.output
         assert mock_client_factory.call_args[0][0].path == hd_path
 
     account = accounts.load(NEW_ACCOUNT_ALIAS)
     assert str(account.hd_path) == "m/1'/60'/0'/0/0"
```

### Comparing `ape-trezor-0.7.0/tests/test_client.py` & `ape-trezor-0.8.0/tests/test_client.py`

 * *Files identical despite different names*

