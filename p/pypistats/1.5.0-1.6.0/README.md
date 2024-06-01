# Comparing `tmp/pypistats-1.5.0.tar.gz` & `tmp/pypistats-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Aug 23 18:32:41 2023, max compression
+gzip compressed data, last modified: Sat Jun  1 09:23:38 2024, max compression
```

## Comparing `pypistats-1.5.0.tar` & `pypistats-1.6.0.tar`

### file list

```diff
@@ -1,39 +1,38 @@
--rw-r--r--   0        0        0      320 2023-08-23 18:32:41.000000 pypistats-1.5.0/.coveragerc
--rw-r--r--   0        0        0      371 2023-08-23 18:32:41.000000 pypistats-1.5.0/.editorconfig
--rw-r--r--   0        0        0       30 2023-08-23 18:32:41.000000 pypistats-1.5.0/.flake8
--rw-r--r--   0        0        0     1569 2023-08-23 18:32:41.000000 pypistats-1.5.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      830 2023-08-23 18:32:41.000000 pypistats-1.5.0/RELEASING.md
--rw-r--r--   0        0        0     1168 2023-08-23 18:32:41.000000 pypistats-1.5.0/azure-pipelines.yml
--rw-r--r--   0        0        0      256 2023-08-23 18:32:41.000000 pypistats-1.5.0/requirements.txt
--rw-r--r--   0        0        0      755 2023-08-23 18:32:41.000000 pypistats-1.5.0/tox.ini
--rw-r--r--   0        0        0      647 2023-08-23 18:32:41.000000 pypistats-1.5.0/.azure-pipelines/jobs/lint.yml
--rw-r--r--   0        0        0     1069 2023-08-23 18:32:41.000000 pypistats-1.5.0/.azure-pipelines/jobs/test.yml
--rw-r--r--   0        0        0     1785 2023-08-23 18:32:41.000000 pypistats-1.5.0/.github/labels.yml
--rw-r--r--   0        0        0      892 2023-08-23 18:32:41.000000 pypistats-1.5.0/.github/release-drafter.yml
--rw-r--r--   0        0        0      443 2023-08-23 18:32:41.000000 pypistats-1.5.0/.github/renovate.json
--rw-r--r--   0        0        0     1755 2023-08-23 18:32:41.000000 pypistats-1.5.0/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      352 2023-08-23 18:32:41.000000 pypistats-1.5.0/.github/workflows/labels.yml
--rw-r--r--   0        0        0      298 2023-08-23 18:32:41.000000 pypistats-1.5.0/.github/workflows/lint.yml
--rw-r--r--   0        0        0     1084 2023-08-23 18:32:41.000000 pypistats-1.5.0/.github/workflows/release-drafter.yml
--rw-r--r--   0        0        0      490 2023-08-23 18:32:41.000000 pypistats-1.5.0/.github/workflows/require-pr-label.yml
--rw-r--r--   0        0        0     1285 2023-08-23 18:32:41.000000 pypistats-1.5.0/.github/workflows/test.yml
--rw-r--r--   0        0        0     1673 2023-08-23 18:32:41.000000 pypistats-1.5.0/example/example.py
--rw-r--r--   0        0        0    45231 2023-08-23 18:32:41.000000 pypistats-1.5.0/example/overall.png
--rw-r--r--   0        0        0    43322 2023-08-23 18:32:41.000000 pypistats-1.5.0/example/python3.png
--rw-r--r--   0        0        0      333 2023-08-23 18:32:41.000000 pypistats-1.5.0/scripts/run_command.py
--rw-r--r--   0        0        0    14307 2023-08-23 18:32:41.000000 pypistats-1.5.0/src/pypistats/__init__.py
--rw-r--r--   0        0        0      105 2023-08-23 18:32:41.000000 pypistats-1.5.0/src/pypistats/__main__.py
--rw-r--r--   0        0        0    10294 2023-08-23 18:32:41.000000 pypistats-1.5.0/src/pypistats/cli.py
--rw-r--r--   0        0        0        0 2023-08-23 18:32:41.000000 pypistats-1.5.0/tests/__init__.py
--rw-r--r--   0        0        0     5656 2023-08-23 18:32:41.000000 pypistats-1.5.0/tests/test_cli.py
--rw-r--r--   0        0        0    24755 2023-08-23 18:32:41.000000 pypistats-1.5.0/tests/test_pypistats.py
--rw-r--r--   0        0        0     3037 2023-08-23 18:32:41.000000 pypistats-1.5.0/tests/test_pypistats_cache.py
--rw-r--r--   0        0        0      308 2023-08-23 18:32:41.000000 pypistats-1.5.0/tests/test_pypistats_print.py
--rw-r--r--   0        0        0        0 2023-08-23 18:32:41.000000 pypistats-1.5.0/tests/data/__init__.py
--rw-r--r--   0        0        0     4080 2023-08-23 18:32:41.000000 pypistats-1.5.0/tests/data/expected_tabulated.py
--rw-r--r--   0        0        0    93203 2023-08-23 18:32:41.000000 pypistats-1.5.0/tests/data/python_minor.py
--rw-r--r--   0        0        0     1298 2023-08-23 18:32:41.000000 pypistats-1.5.0/.gitignore
--rw-r--r--   0        0        0     1079 2023-08-23 18:32:41.000000 pypistats-1.5.0/LICENSE.txt
--rw-r--r--   0        0        0    12427 2023-08-23 18:32:41.000000 pypistats-1.5.0/README.md
--rw-r--r--   0        0        0     1777 2023-08-23 18:32:41.000000 pypistats-1.5.0/pyproject.toml
--rw-r--r--   0        0        0    14152 2023-08-23 18:32:41.000000 pypistats-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0      252 2024-06-01 09:23:38.000000 pypistats-1.6.0/.coveragerc
+-rw-r--r--   0        0        0      371 2024-06-01 09:23:38.000000 pypistats-1.6.0/.editorconfig
+-rw-r--r--   0        0        0     1619 2024-06-01 09:23:38.000000 pypistats-1.6.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      830 2024-06-01 09:23:38.000000 pypistats-1.6.0/RELEASING.md
+-rw-r--r--   0        0        0     1168 2024-06-01 09:23:38.000000 pypistats-1.6.0/azure-pipelines.yml
+-rw-r--r--   0        0        0      256 2024-06-01 09:23:38.000000 pypistats-1.6.0/requirements.txt
+-rw-r--r--   0        0        0      872 2024-06-01 09:23:38.000000 pypistats-1.6.0/tox.ini
+-rw-r--r--   0        0        0      647 2024-06-01 09:23:38.000000 pypistats-1.6.0/.azure-pipelines/jobs/lint.yml
+-rw-r--r--   0        0        0     1121 2024-06-01 09:23:38.000000 pypistats-1.6.0/.azure-pipelines/jobs/test.yml
+-rw-r--r--   0        0        0     1785 2024-06-01 09:23:38.000000 pypistats-1.6.0/.github/labels.yml
+-rw-r--r--   0        0        0      892 2024-06-01 09:23:38.000000 pypistats-1.6.0/.github/release-drafter.yml
+-rw-r--r--   0        0        0      443 2024-06-01 09:23:38.000000 pypistats-1.6.0/.github/renovate.json
+-rw-r--r--   0        0        0     2047 2024-06-01 09:23:38.000000 pypistats-1.6.0/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      389 2024-06-01 09:23:38.000000 pypistats-1.6.0/.github/workflows/labels.yml
+-rw-r--r--   0        0        0      377 2024-06-01 09:23:38.000000 pypistats-1.6.0/.github/workflows/lint.yml
+-rw-r--r--   0        0        0     1084 2024-06-01 09:23:38.000000 pypistats-1.6.0/.github/workflows/release-drafter.yml
+-rw-r--r--   0        0        0      517 2024-06-01 09:23:38.000000 pypistats-1.6.0/.github/workflows/require-pr-label.yml
+-rw-r--r--   0        0        0     1324 2024-06-01 09:23:38.000000 pypistats-1.6.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1709 2024-06-01 09:23:38.000000 pypistats-1.6.0/example/example.py
+-rw-r--r--   0        0        0    45231 2024-06-01 09:23:38.000000 pypistats-1.6.0/example/overall.png
+-rw-r--r--   0        0        0    43322 2024-06-01 09:23:38.000000 pypistats-1.6.0/example/python3.png
+-rw-r--r--   0        0        0      369 2024-06-01 09:23:38.000000 pypistats-1.6.0/scripts/run_command.py
+-rw-r--r--   0        0        0    14460 2024-06-01 09:23:38.000000 pypistats-1.6.0/src/pypistats/__init__.py
+-rw-r--r--   0        0        0      105 2024-06-01 09:23:38.000000 pypistats-1.6.0/src/pypistats/__main__.py
+-rw-r--r--   0        0        0    10294 2024-06-01 09:23:38.000000 pypistats-1.6.0/src/pypistats/cli.py
+-rw-r--r--   0        0        0        0 2024-06-01 09:23:38.000000 pypistats-1.6.0/tests/__init__.py
+-rw-r--r--   0        0        0     5758 2024-06-01 09:23:38.000000 pypistats-1.6.0/tests/test_cli.py
+-rw-r--r--   0        0        0    25713 2024-06-01 09:23:38.000000 pypistats-1.6.0/tests/test_pypistats.py
+-rw-r--r--   0        0        0     3074 2024-06-01 09:23:38.000000 pypistats-1.6.0/tests/test_pypistats_cache.py
+-rw-r--r--   0        0        0      344 2024-06-01 09:23:38.000000 pypistats-1.6.0/tests/test_pypistats_print.py
+-rw-r--r--   0        0        0        0 2024-06-01 09:23:38.000000 pypistats-1.6.0/tests/data/__init__.py
+-rw-r--r--   0        0        0     4102 2024-06-01 09:23:38.000000 pypistats-1.6.0/tests/data/expected_tabulated.py
+-rw-r--r--   0        0        0    93239 2024-06-01 09:23:38.000000 pypistats-1.6.0/tests/data/python_minor.py
+-rw-r--r--   0        0        0     1298 2024-06-01 09:23:38.000000 pypistats-1.6.0/.gitignore
+-rw-r--r--   0        0        0     1079 2024-06-01 09:23:38.000000 pypistats-1.6.0/LICENSE.txt
+-rw-r--r--   0        0        0    12507 2024-06-01 09:23:38.000000 pypistats-1.6.0/README.md
+-rw-r--r--   0        0        0     2634 2024-06-01 09:23:38.000000 pypistats-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0    14283 2024-06-01 09:23:38.000000 pypistats-1.6.0/PKG-INFO
```

### Comparing `pypistats-1.5.0/.pre-commit-config.yaml` & `pypistats-1.6.0/.pre-commit-config.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -1,67 +1,68 @@
 repos:
-  - repo: https://github.com/asottile/pyupgrade
-    rev: v3.10.1
+  - repo: https://github.com/astral-sh/ruff-pre-commit
+    rev: v0.4.5
     hooks:
-      - id: pyupgrade
-        args: [--py38-plus]
+      - id: ruff
+        args: [--exit-non-zero-on-fix]
 
-  - repo: https://github.com/psf/black
-    rev: 23.7.0
+  - repo: https://github.com/psf/black-pre-commit-mirror
+    rev: 24.4.2
     hooks:
       - id: black
 
-  - repo: https://github.com/PyCQA/isort
-    rev: 5.12.0
-    hooks:
-      - id: isort
-
-  - repo: https://github.com/PyCQA/flake8
-    rev: 6.1.0
-    hooks:
-      - id: flake8
-        additional_dependencies:
-          [flake8-2020, flake8-errmsg, flake8-implicit-str-concat]
-
-  - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.10.0
-    hooks:
-      - id: python-check-blanket-noqa
-      - id: python-no-log-warn
-
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.4.0
+    rev: v4.6.0
     hooks:
+      - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-json
       - id: check-toml
       - id: check-yaml
+      - id: debug-statements
       - id: end-of-file-fixer
+      - id: forbid-submodules
       - id: requirements-txt-fixer
       - id: trailing-whitespace
         exclude: tests/data/expected_tabulated.py
 
+  - repo: https://github.com/python-jsonschema/check-jsonschema
+    rev: 0.28.4
+    hooks:
+      - id: check-github-workflows
+      - id: check-renovate
+
+  - repo: https://github.com/rhysd/actionlint
+    rev: v1.7.0
+    hooks:
+      - id: actionlint
+
   - repo: https://github.com/tox-dev/pyproject-fmt
-    rev: 1.0.0
+    rev: 1.8.0
     hooks:
       - id: pyproject-fmt
         additional_dependencies: [tox]
 
   - repo: https://github.com/abravalheri/validate-pyproject
-    rev: v0.14
+    rev: v0.18
     hooks:
       - id: validate-pyproject
 
   - repo: https://github.com/tox-dev/tox-ini-fmt
     rev: 1.3.1
     hooks:
       - id: tox-ini-fmt
 
   - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v3.0.2
+    rev: v4.0.0-alpha.8
     hooks:
       - id: prettier
         args: [--prose-wrap=always, --print-width=88]
 
+  - repo: meta
+    hooks:
+      - id: check-hooks-apply
+      - id: check-useless-excludes
+
 ci:
   autoupdate_schedule: quarterly
```

### Comparing `pypistats-1.5.0/RELEASING.md` & `pypistats-1.6.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `pypistats-1.5.0/azure-pipelines.yml` & `pypistats-1.6.0/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `pypistats-1.5.0/tox.ini` & `pypistats-1.6.0/tox.ini`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,33 @@
 [tox]
 requires =
     tox>=4.2
 env_list =
     cog
     lint
     pins
-    py{py3, 312, 311, 310, 39, 38}
+    py{py3, 313, 312, 311, 310, 39, 38}
 
 [testenv]
 extras =
     tests
+pass_env =
+    FORCE_COLOR
+set_env =
+    COVERAGE_CORE = sysmon
 commands_pre =
     - {envpython} -m pip install --only-binary :all: numpy pandas
 commands =
-    {envpython} -m pytest --cov pypistats --cov tests --cov-report html --cov-report term --cov-report xml {posargs}
+    {envpython} -m pytest \
+      --cov pypistats \
+      --cov tests \
+      --cov-report html \
+      --cov-report term \
+      --cov-report xml \
+      {posargs}
     pypistats --version
     pypistats --help
     pypistats recent --help
 
 [testenv:cog]
 skip_install = true
 deps =
```

### Comparing `pypistats-1.5.0/.azure-pipelines/jobs/lint.yml` & `pypistats-1.6.0/.azure-pipelines/jobs/lint.yml`

 * *Files 24% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 jobs:
   - job: ${{ parameters.name }}
     pool:
       vmImage: ${{ parameters.vmImage }}
 
     strategy:
       matrix:
-        Python311:
-          python.version: "3.11"
+        Python312:
+          python.version: "3.12"
 
     steps:
       - task: UsePythonVersion@0.206.0
         inputs:
           versionSpec: "$(python.version)"
           architecture: "x64"
```

### Comparing `pypistats-1.5.0/.azure-pipelines/jobs/test.yml` & `pypistats-1.6.0/.azure-pipelines/jobs/test.yml`

 * *Files 16% similar despite different names*

```diff
@@ -13,14 +13,16 @@
           python.version: "3.8"
         Python39:
           python.version: "3.9"
         Python310:
           python.version: "3.10"
         Python311:
           python.version: "3.11"
+        Python312:
+          python.version: "3.12"
 
     steps:
       - task: UsePythonVersion@0.206.0
         inputs:
           versionSpec: "$(python.version)"
           architecture: "x64"
```

### Comparing `pypistats-1.5.0/.github/labels.yml` & `pypistats-1.6.0/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `pypistats-1.5.0/.github/release-drafter.yml` & `pypistats-1.6.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `pypistats-1.5.0/.github/workflows/deploy.yml` & `pypistats-1.6.0/.github/workflows/deploy.yml`

 * *Files 24% similar despite different names*

```diff
@@ -17,56 +17,71 @@
 jobs:
   # Always build & lint package.
   build-package:
     name: Build & verify package
     runs-on: ubuntu-latest
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
         with:
           fetch-depth: 0
 
-      - uses: hynek/build-and-inspect-python-package@v1
+      - uses: hynek/build-and-inspect-python-package@v2
 
   # Upload to Test PyPI on every commit on main.
   release-test-pypi:
     name: Publish in-dev package to test.pypi.org
-    if: github.event_name == 'push' && github.ref == 'refs/heads/main'
+    if: |
+      github.repository_owner == 'hugovk'
+      && github.event_name == 'push'
+      && github.ref == 'refs/heads/main'
     runs-on: ubuntu-latest
     needs: build-package
 
     permissions:
-      # IMPORTANT: this permission is mandatory for trusted publishing
+      attestations: write
       id-token: write
 
     steps:
       - name: Download packages built by build-and-inspect-python-package
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: Packages
           path: dist
 
+      - name: Attest build provenance
+        uses: actions/attest-build-provenance@v1
+        with:
+          subject-path: "dist/*"
+
       - name: Upload package to Test PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           repository-url: https://test.pypi.org/legacy/
 
   # Upload to real PyPI on GitHub Releases.
   release-pypi:
     name: Publish released package to pypi.org
-    if: github.event.action == 'published'
+    if: |
+      github.repository_owner == 'hugovk'
+      && github.event.action == 'published'
     runs-on: ubuntu-latest
     needs: build-package
 
     permissions:
-      # IMPORTANT: this permission is mandatory for trusted publishing
+      attestations: write
       id-token: write
 
     steps:
       - name: Download packages built by build-and-inspect-python-package
-        uses: actions/download-artifact@v3
+        uses: actions/download-artifact@v4
         with:
           name: Packages
           path: dist
 
+      - name: Attest build provenance
+        uses: actions/attest-build-provenance@v1
+        with:
+          subject-path: "dist/*"
+
       - name: Upload package to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `pypistats-1.5.0/.github/workflows/release-drafter.yml` & `pypistats-1.6.0/.github/workflows/release-drafter.yml`

 * *Files 11% similar despite different names*

```diff
@@ -25,10 +25,10 @@
       contents: write
       # write permission is required for autolabeler
       # otherwise, read permission is required at least
       pull-requests: write
     runs-on: ubuntu-latest
     steps:
       # Drafts your next release notes as pull requests are merged into "main"
-      - uses: release-drafter/release-drafter@v5
+      - uses: release-drafter/release-drafter@v6
         env:
           GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `pypistats-1.5.0/.github/workflows/test.yml` & `pypistats-1.6.0/.github/workflows/test.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 name: Test
 
 on: [push, pull_request, workflow_dispatch]
 
+permissions:
+  contents: read
+
 env:
   FORCE_COLOR: 1
+  PIP_DISABLE_PIP_VERSION_CHECK: 1
 
 jobs:
   test:
     runs-on: ${{ matrix.os }}
     strategy:
       fail-fast: false
       matrix:
-        python-version: ["pypy3.10", "3.8", "3.9", "3.10", "3.11", "3.12"]
+        python-version: ["pypy3.10", "3.8", "3.9", "3.10", "3.11", "3.12", "3.13"]
         os: [windows-latest, macos-latest, ubuntu-latest]
 
     steps:
-      - uses: actions/checkout@v3
+      - uses: actions/checkout@v4
 
       - name: Set up Python ${{ matrix.python-version }}
-        uses: actions/setup-python@v4
+        uses: actions/setup-python@v5
         with:
           python-version: ${{ matrix.python-version }}
           allow-prereleases: true
           cache: pip
 
       - name: Install dependencies
         run: |
           python -m pip install -U pip
-          python -m pip install -U wheel
           python -m pip install -U tox
 
       - name: Tox tests
         run: |
           tox -e py
 
       - name: Tox tests (pins)
         if: matrix.python-version == '3.11' && matrix.os == 'ubuntu-latest'
         run: |
           tox -e pins
 
       - name: Upload coverage
-        uses: codecov/codecov-action@v3
+        uses: codecov/codecov-action@v3.1.5
         with:
           flags: ${{ matrix.os }}
-          name: ${{ matrix.os }} Python ${{ matrix.python-version }}
+          name: "${{ matrix.os }} Python ${{ matrix.python-version }}"
 
   success:
     needs: test
     runs-on: ubuntu-latest
     name: Test successful
     steps:
       - name: Success
```

### Comparing `pypistats-1.5.0/example/example.py` & `pypistats-1.6.0/example/example.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 #!/usr/bin/env python3
 """
 Example use of pypistats
 """
+from __future__ import annotations
+
 import argparse
 from pprint import pprint  # noqa: F401
 
 import pypistats
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser(
```

### Comparing `pypistats-1.5.0/example/overall.png` & `pypistats-1.6.0/example/overall.png`

 * *Files identical despite different names*

### Comparing `pypistats-1.5.0/example/python3.png` & `pypistats-1.6.0/example/python3.png`

 * *Files identical despite different names*

### Comparing `pypistats-1.5.0/src/pypistats/__init__.py` & `pypistats-1.6.0/src/pypistats/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
 Python interface to PyPI Stats API
 https://pypistats.org/api
 """
+
 from __future__ import annotations
 
 import atexit
 import datetime as dt
 import importlib.metadata
 import json
 import sys
@@ -119,14 +120,17 @@
         _print_verbose(verbose, "HTTP status code:", r.status_code)
         r.raise_for_status()
 
         res = r.json()
 
         _save_cache(cache_file, res)
 
+    if not res.get("data", []):
+        return f"No data found for https://pypi.org/project/{res.get('package', '')}/"
+
     # Actual first and last dates of the fetched data
     first, last = _date_range(res["data"])
 
     # Validate end date
     if end_date and end_date < first:
         msg = (
             f"Requested end date ({end_date}) is before earliest available "
@@ -208,15 +212,15 @@
     data = sorted(data, key=lambda k: k["downloads"], reverse=True)
     return data
 
 
 def _monthly_total(data: list) -> list:
     """Sum all downloads per category, by month"""
 
-    totalled = {}
+    totalled: dict = {}
     for row in data:
         category = row["category"]
         downloads = row["downloads"]
         month = row["date"][:7]
 
         if category in totalled:
             if month in totalled[category]:
@@ -237,15 +241,15 @@
 def _total(data: dict | list) -> dict | list:
     """Sum all downloads per category, regardless of date"""
 
     # Only for lists of dicts, not a single dict
     if isinstance(data, dict):
         return data
 
-    totalled = {}
+    totalled: dict = {}
     for row in data:
         try:
             totalled[row["category"]] += row["downloads"]
         except KeyError:
             totalled[row["category"]] = row["downloads"]
 
     data = []
@@ -441,15 +445,15 @@
         for header in headers:
             align = Align.AUTO
             thousand_separator = ThousandSeparator.NONE
             type_hint = None
             if header == "percent":
                 align = Align.RIGHT
             elif header == "downloads" and (format_ not in ["numpy", "pandas"]):
-                thousand_separator = ","
+                thousand_separator = ThousandSeparator.COMMA
             elif header == "category":
                 type_hint = String
             style = Style(align=align, thousand_separator=thousand_separator)
             column_styles.append(style)
             type_hints.append(type_hint)
 
         writer.column_styles = column_styles
```

### Comparing `pypistats-1.5.0/src/pypistats/cli.py` & `pypistats-1.6.0/src/pypistats/cli.py`

 * *Files identical despite different names*

### Comparing `pypistats-1.5.0/tests/test_cli.py` & `pypistats-1.6.0/tests/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
 Unit tests for cli
 """
+
+from __future__ import annotations
+
 import argparse
 
 import pytest
 from freezegun import freeze_time
 
 from pypistats import cli
 
@@ -137,16 +140,17 @@
 
 @pytest.mark.parametrize("test_input", ["dkvnf", "2018-99", "2018-xx"])
 def test__valid_yyyy_mm_optional_dd_invalid(test_input: str) -> None:
     with pytest.raises(argparse.ArgumentTypeError):
         cli._valid_yyyy_mm_optional_dd(test_input)
 
 
-class __Args:
-    def __init__(self) -> None:
+class __Args(argparse.Namespace):
+    def __init__(self, **kwargs) -> None:
+        super().__init__(**kwargs)
         self.json = False  # type: bool
         self.format = "markdown"  # type: str
 
 
 @pytest.mark.parametrize("test_input, expected", [(False, "markdown"), (True, "json")])
 def test__define_format_json_flag(test_input: bool, expected: str) -> None:
     # Arrange
```

### Comparing `pypistats-1.5.0/tests/test_pypistats.py` & `pypistats-1.6.0/tests/test_pypistats.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
 Unit tests for pypistats
 """
+
+from __future__ import annotations
+
 import copy
 import json
 from pathlib import Path
 
 import pytest
 import respx
 
@@ -62,16 +65,16 @@
 
 
 class TestPypiStats:
     def setup_method(self) -> None:
         # Stub caching. Caches are tested in another class.
         self.original__cache_filename = pypistats._cache_filename
         self.original__save_cache = pypistats._save_cache
-        pypistats._cache_filename = stub__cache_filename
-        pypistats._save_cache = stub__save_cache
+        pypistats._cache_filename = stub__cache_filename  # type: ignore[assignment]
+        pypistats._save_cache = stub__save_cache  # type: ignore[assignment]
 
     def teardown_method(self) -> None:
         # Unstub caching
         pypistats._cache_filename = self.original__cache_filename
         pypistats._save_cache = self.original__save_cache
 
     def test__filter_no_filters_no_change(self) -> None:
@@ -206,20 +209,20 @@
             {"category": "2.7", "downloads": 1, "percent": "\x1b[31m1.00%\x1b[0m"},
             # yellow
             {"category": "3.5", "downloads": 10, "percent": "\x1b[33m10.00%\x1b[0m"},
             # green
             {"category": "3.10", "downloads": 89, "percent": "\x1b[32m89.00%\x1b[0m"},
             {"category": "Total", "downloads": 100},
         ]
-        data = pypistats._percent(data)
-        data = pypistats._grand_total(data)
+        percent_data = pypistats._percent(data)
+        total_data = pypistats._grand_total(percent_data)
         monkeypatch.setenv("FORCE_COLOR", "1")
 
         # Act
-        output = pypistats._colourify(data)
+        output = pypistats._colourify(total_data)
 
         # Assert
         assert output == expected_output
 
     def test__tabulate_noarg(self) -> None:
         # Arrange
         data = copy.deepcopy(SAMPLE_DATA)
@@ -237,17 +240,18 @@
             pytest.param("html", EXPECTED_TABULATED_HTML, id="html"),
             pytest.param("markdown", EXPECTED_TABULATED_MD, id="markdown"),
             pytest.param("pretty", EXPECTED_TABULATED_PRETTY, id="pretty"),
             pytest.param("rst", EXPECTED_TABULATED_RST, id="rst"),
             pytest.param("tsv", EXPECTED_TABULATED_TSV, id="tsv"),
         ],
     )
-    def test__tabulate(self, test_input: str, expected: str) -> None:
+    def test__tabulate(self, test_input: str, expected: str, monkeypatch) -> None:
         # Arrange
         data = copy.deepcopy(SAMPLE_DATA)
+        monkeypatch.setenv("NO_COLOR", "1")
 
         # Act
         output = pypistats._tabulate(data, format_=test_input)
 
         # Assert
         assert output.strip() == expected.strip()
 
@@ -448,15 +452,15 @@
     @pytest.mark.parametrize(
         "test_format, expected_output",
         [
             pytest.param(
                 "markdown",
                 """
 |  last_day | last_month |  last_week |
-|----------:|-----------:|-----------:|
+|---------: |----------: |----------: |
 | 2,295,765 | 67,759,913 | 15,706,750 |
 """,
                 id="markdown",
             ),
             pytest.param(
                 "tsv",
                 """
@@ -481,53 +485,55 @@
         respx.get(mocked_url).respond(content=mocked_response)
         output = pypistats.recent(package, format=test_format)
 
         # Assert
         assert output.strip() == expected_output.strip()
 
     @respx.mock
-    def test_overall_tabular_start_date(self) -> None:
+    def test_overall_tabular_start_date(self, monkeypatch) -> None:
         # Arrange
         package = "pip"
         mocked_url = "https://pypistats.org/api/packages/pip/overall?&mirrors=false"
         mocked_response = SAMPLE_RESPONSE_OVERALL
         expected_output = """
 | category        | percent | downloads |
-|:----------------|--------:|----------:|
+| :---------------|-------: |---------: |
 | with_mirrors    | 100.00% | 1,487,218 |
 | without_mirrors |  99.24% | 1,475,979 |
 | Total           |         | 1,487,218 |
 
 Date range: 2020-05-02 - 2020-05-02
 """
+        monkeypatch.setenv("NO_COLOR", "1")
 
         # Act
         respx.get(mocked_url).respond(content=mocked_response)
         output = pypistats.overall(
             package, mirrors=False, start_date="2020-05-02", format="md"
         )
 
         # Assert
         assert output.strip() == expected_output.strip()
 
     @respx.mock
-    def test_overall_tabular_end_date(self) -> None:
+    def test_overall_tabular_end_date(self, monkeypatch) -> None:
         # Arrange
         package = "pip"
         mocked_url = "https://pypistats.org/api/packages/pip/overall?&mirrors=false"
         mocked_response = SAMPLE_RESPONSE_OVERALL
         expected_output = """
 | category        | percent | downloads |
-|:----------------|--------:|----------:|
+| :---------------|-------: |---------: |
 | with_mirrors    | 100.00% | 2,100,139 |
 | without_mirrors |  99.21% | 2,083,472 |
 | Total           |         | 2,100,139 |
 
 Date range: 2020-05-01 - 2020-05-01
 """
+        monkeypatch.setenv("NO_COLOR", "1")
 
         # Act
         respx.get(mocked_url).respond(content=mocked_response)
         output = pypistats.overall(
             package, mirrors=False, end_date="2020-05-01", format="md"
         )
 
@@ -607,15 +613,15 @@
         respx.get(mocked_url).respond(content=mocked_response)
         output = pypistats.python_minor(package, format="json")
 
         # Assert
         assert json.loads(output) == json.loads(expected_output)
 
     @respx.mock
-    def test_system_tabular(self) -> None:
+    def test_system_tabular(self, monkeypatch) -> None:
         # Arrange
         package = "pip"
         mocked_url = "https://pypistats.org/api/packages/pip/system"
         mocked_response = """{
             "data": [
                 {"category": "Darwin", "downloads": 10734594},
                 {"category": "Linux", "downloads": 236502274},
@@ -624,22 +630,23 @@
                 {"category": "Windows", "downloads": 6527978}
             ],
             "package": "pip",
             "type": "system_downloads"
         }"""
         expected_output = """
 | category | percent |   downloads |
-|:---------|--------:|------------:|
+| :--------|-------: |-----------: |
 | Linux    |  83.14% | 236,502,274 |
 | null     |  10.75% |  30,579,325 |
 | Darwin   |   3.77% |  10,734,594 |
 | Windows  |   2.29% |   6,527,978 |
 | other    |   0.04% |     111,243 |
 | Total    |         | 284,455,414 |
 """
+        monkeypatch.setenv("NO_COLOR", "1")
 
         # Act
         respx.get(mocked_url).respond(content=mocked_response)
         output = pypistats.system(package, format="md")
 
         # Assert
         assert output.strip() == expected_output.strip()
@@ -683,15 +690,15 @@
 
     @respx.mock
     def test_versions_are_strings(self) -> None:
         # Arrange
         data = copy.deepcopy(SAMPLE_DATA_VERSION_STRINGS)
         expected_output = """
 | category |    date    | downloads |
-|:---------|:----------:|----------:|
+| :--------| :--------: |---------: |
 | 3.1      | 2018-08-15 |        10 |
 | 3.10     | 2018-08-15 |         1 |
 """
 
         # Act
         output = pypistats._tabulate(data, format_="markdown")
 
@@ -736,7 +743,26 @@
         # Act
         respx.get(mocked_url).respond(content=mocked_response)
         output = pypistats.overall(package, format="pandas")
 
         # Assert
         assert isinstance(output, pandas.DataFrame)
         assert str(output).strip() == expected_output.strip()
+
+    @respx.mock
+    def test_package_not_exist(self) -> None:
+        # Arrange
+        package = "a" * 100
+        mocked_response = f"""{{
+            "data":[],
+            "package":"{package}",
+            "type":"python_major_downloads"
+        }}"""
+        mocked_url = f"https://pypistats.org/api/packages/{package}/python_major"
+        expected_output = f"No data found for https://pypi.org/project/{package}/"
+
+        # Act
+        respx.get(mocked_url).respond(content=mocked_response)
+        output = pypistats.python_major(package)
+
+        # Assert
+        assert output == expected_output
```

### Comparing `pypistats-1.5.0/tests/test_pypistats_cache.py` & `pypistats-1.6.0/tests/test_pypistats_cache.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 """
 Unit tests for pypistats cache
 """
+
+from __future__ import annotations
+
 import tempfile
 from pathlib import Path
 
 import respx
 from freezegun import freeze_time
 
 import pypistats
@@ -93,15 +96,15 @@
             {"category": "without_mirrors", "date": "2018-11-01", "downloads": 2295765}
           ],
           "package": "pip",
           "type": "overall_downloads"
         }"""
         expected_output = """
 | category        | downloads |
-|:----------------|----------:|
+| :---------------|---------: |
 | without_mirrors | 2,295,765 |
 
 Date range: 2018-11-01 - 2018-11-01
 """
 
         # Act
         respx.get(mocked_url).respond(content=mocked_response)
```

### Comparing `pypistats-1.5.0/tests/data/expected_tabulated.py` & `pypistats-1.6.0/tests/data/expected_tabulated.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,255 +1,257 @@
-00000000: 4558 5045 4354 4544 5f54 4142 554c 4154  EXPECTED_TABULAT
-00000010: 4544 5f48 544d 4c20 3d20 2222 220a 3c74  ED_HTML = """.<t
-00000020: 6162 6c65 3e0a 2020 2020 3c74 6865 6164  able>.    <thead
-00000030: 3e0a 2020 2020 2020 2020 3c74 723e 0a20  >.        <tr>. 
-00000040: 2020 2020 2020 2020 2020 203c 7468 3e63             <th>c
-00000050: 6174 6567 6f72 793c 2f74 683e 0a20 2020  ategory</th>.   
-00000060: 2020 2020 2020 2020 203c 7468 3e64 6174           <th>dat
-00000070: 653c 2f74 683e 0a20 2020 2020 2020 2020  e</th>.         
-00000080: 2020 203c 7468 3e64 6f77 6e6c 6f61 6473     <th>downloads
-00000090: 3c2f 7468 3e0a 2020 2020 2020 2020 3c2f  </th>.        </
-000000a0: 7472 3e0a 2020 2020 3c2f 7468 6561 643e  tr>.    </thead>
-000000b0: 0a20 2020 203c 7462 6f64 793e 0a20 2020  .    <tbody>.   
-000000c0: 2020 2020 203c 7472 3e0a 2020 2020 2020       <tr>.      
-000000d0: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
-000000e0: 226c 6566 7422 3e32 2e36 3c2f 7464 3e0a  "left">2.6</td>.
-000000f0: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
-00000100: 616c 6967 6e3d 226c 6566 7422 3e32 3031  align="left">201
-00000110: 382d 3038 2d31 353c 2f74 643e 0a20 2020  8-08-15</td>.   
-00000120: 2020 2020 2020 2020 203c 7464 2061 6c69           <td ali
-00000130: 676e 3d22 7269 6768 7422 3e35 313c 2f74  gn="right">51</t
-00000140: 643e 0a20 2020 2020 2020 203c 2f74 723e  d>.        </tr>
-00000150: 0a20 2020 2020 2020 203c 7472 3e0a 2020  .        <tr>.  
-00000160: 2020 2020 2020 2020 2020 3c74 6420 616c            <td al
-00000170: 6967 6e3d 226c 6566 7422 3e32 2e37 3c2f  ign="left">2.7</
-00000180: 7464 3e0a 2020 2020 2020 2020 2020 2020  td>.            
-00000190: 3c74 6420 616c 6967 6e3d 226c 6566 7422  <td align="left"
-000001a0: 3e32 3031 382d 3038 2d31 353c 2f74 643e  >2018-08-15</td>
-000001b0: 0a20 2020 2020 2020 2020 2020 203c 7464  .            <td
-000001c0: 2061 6c69 676e 3d22 7269 6768 7422 3e36   align="right">6
-000001d0: 332c 3734 393c 2f74 643e 0a20 2020 2020  3,749</td>.     
-000001e0: 2020 203c 2f74 723e 0a20 2020 2020 2020     </tr>.       
-000001f0: 203c 7472 3e0a 2020 2020 2020 2020 2020   <tr>.          
-00000200: 2020 3c74 6420 616c 6967 6e3d 226c 6566    <td align="lef
-00000210: 7422 3e33 2e32 3c2f 7464 3e0a 2020 2020  t">3.2</td>.    
-00000220: 2020 2020 2020 2020 3c74 6420 616c 6967          <td alig
-00000230: 6e3d 226c 6566 7422 3e32 3031 382d 3038  n="left">2018-08
-00000240: 2d31 353c 2f74 643e 0a20 2020 2020 2020  -15</td>.       
-00000250: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
-00000260: 7269 6768 7422 3e32 3c2f 7464 3e0a 2020  right">2</td>.  
-00000270: 2020 2020 2020 3c2f 7472 3e0a 2020 2020        </tr>.    
-00000280: 2020 2020 3c74 723e 0a20 2020 2020 2020      <tr>.       
-00000290: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
-000002a0: 6c65 6674 223e 332e 333c 2f74 643e 0a20  left">3.3</td>. 
-000002b0: 2020 2020 2020 2020 2020 203c 7464 2061             <td a
-000002c0: 6c69 676e 3d22 6c65 6674 223e 3230 3138  lign="left">2018
-000002d0: 2d30 382d 3135 3c2f 7464 3e0a 2020 2020  -08-15</td>.    
-000002e0: 2020 2020 2020 2020 3c74 6420 616c 6967          <td alig
-000002f0: 6e3d 2272 6967 6874 223e 3430 3c2f 7464  n="right">40</td
-00000300: 3e0a 2020 2020 2020 2020 3c2f 7472 3e0a  >.        </tr>.
-00000310: 2020 2020 2020 2020 3c74 723e 0a20 2020          <tr>.   
-00000320: 2020 2020 2020 2020 203c 7464 2061 6c69           <td ali
-00000330: 676e 3d22 6c65 6674 223e 332e 343c 2f74  gn="left">3.4</t
-00000340: 643e 0a20 2020 2020 2020 2020 2020 203c  d>.            <
-00000350: 7464 2061 6c69 676e 3d22 6c65 6674 223e  td align="left">
-00000360: 3230 3138 2d30 382d 3135 3c2f 7464 3e0a  2018-08-15</td>.
-00000370: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
-00000380: 616c 6967 6e3d 2272 6967 6874 223e 362c  align="right">6,
-00000390: 3039 353c 2f74 643e 0a20 2020 2020 2020  095</td>.       
-000003a0: 203c 2f74 723e 0a20 2020 2020 2020 203c   </tr>.        <
-000003b0: 7472 3e0a 2020 2020 2020 2020 2020 2020  tr>.            
-000003c0: 3c74 6420 616c 6967 6e3d 226c 6566 7422  <td align="left"
-000003d0: 3e33 2e35 3c2f 7464 3e0a 2020 2020 2020  >3.5</td>.      
-000003e0: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
-000003f0: 226c 6566 7422 3e32 3031 382d 3038 2d31  "left">2018-08-1
-00000400: 353c 2f74 643e 0a20 2020 2020 2020 2020  5</td>.         
-00000410: 2020 203c 7464 2061 6c69 676e 3d22 7269     <td align="ri
-00000420: 6768 7422 3e32 302c 3335 383c 2f74 643e  ght">20,358</td>
-00000430: 0a20 2020 2020 2020 203c 2f74 723e 0a20  .        </tr>. 
-00000440: 2020 2020 2020 203c 7472 3e0a 2020 2020         <tr>.    
-00000450: 2020 2020 2020 2020 3c74 6420 616c 6967          <td alig
-00000460: 6e3d 226c 6566 7422 3e33 2e36 3c2f 7464  n="left">3.6</td
-00000470: 3e0a 2020 2020 2020 2020 2020 2020 3c74  >.            <t
-00000480: 6420 616c 6967 6e3d 226c 6566 7422 3e32  d align="left">2
-00000490: 3031 382d 3038 2d31 353c 2f74 643e 0a20  018-08-15</td>. 
-000004a0: 2020 2020 2020 2020 2020 203c 7464 2061             <td a
-000004b0: 6c69 676e 3d22 7269 6768 7422 3e33 352c  lign="right">35,
-000004c0: 3237 343c 2f74 643e 0a20 2020 2020 2020  274</td>.       
-000004d0: 203c 2f74 723e 0a20 2020 2020 2020 203c   </tr>.        <
-000004e0: 7472 3e0a 2020 2020 2020 2020 2020 2020  tr>.            
-000004f0: 3c74 6420 616c 6967 6e3d 226c 6566 7422  <td align="left"
-00000500: 3e33 2e37 3c2f 7464 3e0a 2020 2020 2020  >3.7</td>.      
-00000510: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
-00000520: 226c 6566 7422 3e32 3031 382d 3038 2d31  "left">2018-08-1
-00000530: 353c 2f74 643e 0a20 2020 2020 2020 2020  5</td>.         
-00000540: 2020 203c 7464 2061 6c69 676e 3d22 7269     <td align="ri
-00000550: 6768 7422 3e36 2c35 3935 3c2f 7464 3e0a  ght">6,595</td>.
-00000560: 2020 2020 2020 2020 3c2f 7472 3e0a 2020          </tr>.  
-00000570: 2020 2020 2020 3c74 723e 0a20 2020 2020        <tr>.     
-00000580: 2020 2020 2020 203c 7464 2061 6c69 676e         <td align
-00000590: 3d22 6c65 6674 223e 332e 383c 2f74 643e  ="left">3.8</td>
-000005a0: 0a20 2020 2020 2020 2020 2020 203c 7464  .            <td
-000005b0: 2061 6c69 676e 3d22 6c65 6674 223e 3230   align="left">20
-000005c0: 3138 2d30 382d 3135 3c2f 7464 3e0a 2020  18-08-15</td>.  
-000005d0: 2020 2020 2020 2020 2020 3c74 6420 616c            <td al
-000005e0: 6967 6e3d 2272 6967 6874 223e 333c 2f74  ign="right">3</t
-000005f0: 643e 0a20 2020 2020 2020 203c 2f74 723e  d>.        </tr>
-00000600: 0a20 2020 2020 2020 203c 7472 3e0a 2020  .        <tr>.  
-00000610: 2020 2020 2020 2020 2020 3c74 6420 616c            <td al
-00000620: 6967 6e3d 226c 6566 7422 3e6e 756c 6c3c  ign="left">null<
-00000630: 2f74 643e 0a20 2020 2020 2020 2020 2020  /td>.           
-00000640: 203c 7464 2061 6c69 676e 3d22 6c65 6674   <td align="left
-00000650: 223e 3230 3138 2d30 382d 3135 3c2f 7464  ">2018-08-15</td
-00000660: 3e0a 2020 2020 2020 2020 2020 2020 3c74  >.            <t
-00000670: 6420 616c 6967 6e3d 2272 6967 6874 223e  d align="right">
-00000680: 312c 3031 393c 2f74 643e 0a20 2020 2020  1,019</td>.     
-00000690: 2020 203c 2f74 723e 0a20 2020 203c 2f74     </tr>.    </t
-000006a0: 626f 6479 3e0a 3c2f 7461 626c 653e 0a20  body>.</table>. 
-000006b0: 2020 2020 2020 2022 2222 0a0a 4558 5045         """..EXPE
-000006c0: 4354 4544 5f54 4142 554c 4154 4544 5f50  CTED_TABULATED_P
-000006d0: 5245 5454 5920 3d20 2222 220a e294 8ce2  RETTY = """.....
-000006e0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000006f0: 80e2 9480 e294 80e2 9480 e294 80e2 94ac  ................
-00000700: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
+00000000: 6672 6f6d 205f 5f66 7574 7572 655f 5f20  from __future__ 
+00000010: 696d 706f 7274 2061 6e6e 6f74 6174 696f  import annotatio
+00000020: 6e73 0a0a 4558 5045 4354 4544 5f54 4142  ns..EXPECTED_TAB
+00000030: 554c 4154 4544 5f48 544d 4c20 3d20 2222  ULATED_HTML = ""
+00000040: 220a 3c74 6162 6c65 3e0a 2020 2020 3c74  ".<table>.    <t
+00000050: 6865 6164 3e0a 2020 2020 2020 2020 3c74  head>.        <t
+00000060: 723e 0a20 2020 2020 2020 2020 2020 203c  r>.            <
+00000070: 7468 3e63 6174 6567 6f72 793c 2f74 683e  th>category</th>
+00000080: 0a20 2020 2020 2020 2020 2020 203c 7468  .            <th
+00000090: 3e64 6174 653c 2f74 683e 0a20 2020 2020  >date</th>.     
+000000a0: 2020 2020 2020 203c 7468 3e64 6f77 6e6c         <th>downl
+000000b0: 6f61 6473 3c2f 7468 3e0a 2020 2020 2020  oads</th>.      
+000000c0: 2020 3c2f 7472 3e0a 2020 2020 3c2f 7468    </tr>.    </th
+000000d0: 6561 643e 0a20 2020 203c 7462 6f64 793e  ead>.    <tbody>
+000000e0: 0a20 2020 2020 2020 203c 7472 3e0a 2020  .        <tr>.  
+000000f0: 2020 2020 2020 2020 2020 3c74 6420 616c            <td al
+00000100: 6967 6e3d 226c 6566 7422 3e32 2e36 3c2f  ign="left">2.6</
+00000110: 7464 3e0a 2020 2020 2020 2020 2020 2020  td>.            
+00000120: 3c74 6420 616c 6967 6e3d 226c 6566 7422  <td align="left"
+00000130: 3e32 3031 382d 3038 2d31 353c 2f74 643e  >2018-08-15</td>
+00000140: 0a20 2020 2020 2020 2020 2020 203c 7464  .            <td
+00000150: 2061 6c69 676e 3d22 7269 6768 7422 3e35   align="right">5
+00000160: 313c 2f74 643e 0a20 2020 2020 2020 203c  1</td>.        <
+00000170: 2f74 723e 0a20 2020 2020 2020 203c 7472  /tr>.        <tr
+00000180: 3e0a 2020 2020 2020 2020 2020 2020 3c74  >.            <t
+00000190: 6420 616c 6967 6e3d 226c 6566 7422 3e32  d align="left">2
+000001a0: 2e37 3c2f 7464 3e0a 2020 2020 2020 2020  .7</td>.        
+000001b0: 2020 2020 3c74 6420 616c 6967 6e3d 226c      <td align="l
+000001c0: 6566 7422 3e32 3031 382d 3038 2d31 353c  eft">2018-08-15<
+000001d0: 2f74 643e 0a20 2020 2020 2020 2020 2020  /td>.           
+000001e0: 203c 7464 2061 6c69 676e 3d22 7269 6768   <td align="righ
+000001f0: 7422 3e36 332c 3734 393c 2f74 643e 0a20  t">63,749</td>. 
+00000200: 2020 2020 2020 203c 2f74 723e 0a20 2020         </tr>.   
+00000210: 2020 2020 203c 7472 3e0a 2020 2020 2020       <tr>.      
+00000220: 2020 2020 2020 3c74 6420 616c 6967 6e3d        <td align=
+00000230: 226c 6566 7422 3e33 2e32 3c2f 7464 3e0a  "left">3.2</td>.
+00000240: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
+00000250: 616c 6967 6e3d 226c 6566 7422 3e32 3031  align="left">201
+00000260: 382d 3038 2d31 353c 2f74 643e 0a20 2020  8-08-15</td>.   
+00000270: 2020 2020 2020 2020 203c 7464 2061 6c69           <td ali
+00000280: 676e 3d22 7269 6768 7422 3e32 3c2f 7464  gn="right">2</td
+00000290: 3e0a 2020 2020 2020 2020 3c2f 7472 3e0a  >.        </tr>.
+000002a0: 2020 2020 2020 2020 3c74 723e 0a20 2020          <tr>.   
+000002b0: 2020 2020 2020 2020 203c 7464 2061 6c69           <td ali
+000002c0: 676e 3d22 6c65 6674 223e 332e 333c 2f74  gn="left">3.3</t
+000002d0: 643e 0a20 2020 2020 2020 2020 2020 203c  d>.            <
+000002e0: 7464 2061 6c69 676e 3d22 6c65 6674 223e  td align="left">
+000002f0: 3230 3138 2d30 382d 3135 3c2f 7464 3e0a  2018-08-15</td>.
+00000300: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
+00000310: 616c 6967 6e3d 2272 6967 6874 223e 3430  align="right">40
+00000320: 3c2f 7464 3e0a 2020 2020 2020 2020 3c2f  </td>.        </
+00000330: 7472 3e0a 2020 2020 2020 2020 3c74 723e  tr>.        <tr>
+00000340: 0a20 2020 2020 2020 2020 2020 203c 7464  .            <td
+00000350: 2061 6c69 676e 3d22 6c65 6674 223e 332e   align="left">3.
+00000360: 343c 2f74 643e 0a20 2020 2020 2020 2020  4</td>.         
+00000370: 2020 203c 7464 2061 6c69 676e 3d22 6c65     <td align="le
+00000380: 6674 223e 3230 3138 2d30 382d 3135 3c2f  ft">2018-08-15</
+00000390: 7464 3e0a 2020 2020 2020 2020 2020 2020  td>.            
+000003a0: 3c74 6420 616c 6967 6e3d 2272 6967 6874  <td align="right
+000003b0: 223e 362c 3039 353c 2f74 643e 0a20 2020  ">6,095</td>.   
+000003c0: 2020 2020 203c 2f74 723e 0a20 2020 2020       </tr>.     
+000003d0: 2020 203c 7472 3e0a 2020 2020 2020 2020     <tr>.        
+000003e0: 2020 2020 3c74 6420 616c 6967 6e3d 226c      <td align="l
+000003f0: 6566 7422 3e33 2e35 3c2f 7464 3e0a 2020  eft">3.5</td>.  
+00000400: 2020 2020 2020 2020 2020 3c74 6420 616c            <td al
+00000410: 6967 6e3d 226c 6566 7422 3e32 3031 382d  ign="left">2018-
+00000420: 3038 2d31 353c 2f74 643e 0a20 2020 2020  08-15</td>.     
+00000430: 2020 2020 2020 203c 7464 2061 6c69 676e         <td align
+00000440: 3d22 7269 6768 7422 3e32 302c 3335 383c  ="right">20,358<
+00000450: 2f74 643e 0a20 2020 2020 2020 203c 2f74  /td>.        </t
+00000460: 723e 0a20 2020 2020 2020 203c 7472 3e0a  r>.        <tr>.
+00000470: 2020 2020 2020 2020 2020 2020 3c74 6420              <td 
+00000480: 616c 6967 6e3d 226c 6566 7422 3e33 2e36  align="left">3.6
+00000490: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
+000004a0: 2020 3c74 6420 616c 6967 6e3d 226c 6566    <td align="lef
+000004b0: 7422 3e32 3031 382d 3038 2d31 353c 2f74  t">2018-08-15</t
+000004c0: 643e 0a20 2020 2020 2020 2020 2020 203c  d>.            <
+000004d0: 7464 2061 6c69 676e 3d22 7269 6768 7422  td align="right"
+000004e0: 3e33 352c 3237 343c 2f74 643e 0a20 2020  >35,274</td>.   
+000004f0: 2020 2020 203c 2f74 723e 0a20 2020 2020       </tr>.     
+00000500: 2020 203c 7472 3e0a 2020 2020 2020 2020     <tr>.        
+00000510: 2020 2020 3c74 6420 616c 6967 6e3d 226c      <td align="l
+00000520: 6566 7422 3e33 2e37 3c2f 7464 3e0a 2020  eft">3.7</td>.  
+00000530: 2020 2020 2020 2020 2020 3c74 6420 616c            <td al
+00000540: 6967 6e3d 226c 6566 7422 3e32 3031 382d  ign="left">2018-
+00000550: 3038 2d31 353c 2f74 643e 0a20 2020 2020  08-15</td>.     
+00000560: 2020 2020 2020 203c 7464 2061 6c69 676e         <td align
+00000570: 3d22 7269 6768 7422 3e36 2c35 3935 3c2f  ="right">6,595</
+00000580: 7464 3e0a 2020 2020 2020 2020 3c2f 7472  td>.        </tr
+00000590: 3e0a 2020 2020 2020 2020 3c74 723e 0a20  >.        <tr>. 
+000005a0: 2020 2020 2020 2020 2020 203c 7464 2061             <td a
+000005b0: 6c69 676e 3d22 6c65 6674 223e 332e 383c  lign="left">3.8<
+000005c0: 2f74 643e 0a20 2020 2020 2020 2020 2020  /td>.           
+000005d0: 203c 7464 2061 6c69 676e 3d22 6c65 6674   <td align="left
+000005e0: 223e 3230 3138 2d30 382d 3135 3c2f 7464  ">2018-08-15</td
+000005f0: 3e0a 2020 2020 2020 2020 2020 2020 3c74  >.            <t
+00000600: 6420 616c 6967 6e3d 2272 6967 6874 223e  d align="right">
+00000610: 333c 2f74 643e 0a20 2020 2020 2020 203c  3</td>.        <
+00000620: 2f74 723e 0a20 2020 2020 2020 203c 7472  /tr>.        <tr
+00000630: 3e0a 2020 2020 2020 2020 2020 2020 3c74  >.            <t
+00000640: 6420 616c 6967 6e3d 226c 6566 7422 3e6e  d align="left">n
+00000650: 756c 6c3c 2f74 643e 0a20 2020 2020 2020  ull</td>.       
+00000660: 2020 2020 203c 7464 2061 6c69 676e 3d22       <td align="
+00000670: 6c65 6674 223e 3230 3138 2d30 382d 3135  left">2018-08-15
+00000680: 3c2f 7464 3e0a 2020 2020 2020 2020 2020  </td>.          
+00000690: 2020 3c74 6420 616c 6967 6e3d 2272 6967    <td align="rig
+000006a0: 6874 223e 312c 3031 393c 2f74 643e 0a20  ht">1,019</td>. 
+000006b0: 2020 2020 2020 203c 2f74 723e 0a20 2020         </tr>.   
+000006c0: 203c 2f74 626f 6479 3e0a 3c2f 7461 626c   </tbody>.</tabl
+000006d0: 653e 0a20 2020 2020 2020 2022 2222 0a0a  e>.        """..
+000006e0: 4558 5045 4354 4544 5f54 4142 554c 4154  EXPECTED_TABULAT
+000006f0: 4544 5f50 5245 5454 5920 3d20 2222 220a  ED_PRETTY = """.
+00000700: e294 8ce2 9480 e294 80e2 9480 e294 80e2  ................
 00000710: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000720: 80e2 9480 e294 ace2 9480 e294 80e2 9480  ................
+00000720: 80e2 94ac e294 80e2 9480 e294 80e2 9480  ................
 00000730: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000740: 9480 e294 80e2 9480 e294 900a e294 8220  ............... 
-00000750: 6361 7465 676f 7279 20e2 9482 2020 2020  category ...    
-00000760: 6461 7465 2020 2020 e294 8220 646f 776e  date    ... down
-00000770: 6c6f 6164 7320 e294 820a e294 9ce2 9480  loads ..........
-00000780: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000790: 9480 e294 80e2 9480 e294 80e2 94bc e294  ................
-000007a0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000740: 9480 e294 80e2 9480 e294 ace2 9480 e294  ................
+00000750: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000760: e294 80e2 9480 e294 80e2 9480 e294 900a  ................
+00000770: e294 8220 6361 7465 676f 7279 20e2 9482  ... category ...
+00000780: 2020 2020 6461 7465 2020 2020 e294 8220      date    ... 
+00000790: 646f 776e 6c6f 6164 7320 e294 820a e294  downloads ......
+000007a0: 9ce2 9480 e294 80e2 9480 e294 80e2 9480  ................
 000007b0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000007c0: 9480 e294 bce2 9480 e294 80e2 9480 e294  ................
+000007c0: 94bc e294 80e2 9480 e294 80e2 9480 e294  ................
 000007d0: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
-000007e0: e294 80e2 9480 e294 a40a e294 8220 322e  ............. 2.
-000007f0: 3620 2020 2020 20e2 9482 2032 3031 382d  6      ... 2018-
-00000800: 3038 2d31 3520 e294 8220 2020 2020 2020  08-15 ...       
-00000810: 2035 3120 e294 820a e294 8220 322e 3720   51 ....... 2.7 
-00000820: 2020 2020 20e2 9482 2032 3031 382d 3038       ... 2018-08
-00000830: 2d31 3520 e294 8220 2020 2036 332c 3734  -15 ...    63,74
-00000840: 3920 e294 820a e294 8220 332e 3220 2020  9 ....... 3.2   
-00000850: 2020 20e2 9482 2032 3031 382d 3038 2d31     ... 2018-08-1
-00000860: 3520 e294 8220 2020 2020 2020 2020 3220  5 ...         2 
-00000870: e294 820a e294 8220 332e 3320 2020 2020  ....... 3.3     
-00000880: 20e2 9482 2032 3031 382d 3038 2d31 3520   ... 2018-08-15 
-00000890: e294 8220 2020 2020 2020 2034 3020 e294  ...        40 ..
-000008a0: 820a e294 8220 332e 3420 2020 2020 20e2  ..... 3.4      .
-000008b0: 9482 2032 3031 382d 3038 2d31 3520 e294  .. 2018-08-15 ..
-000008c0: 8220 2020 2020 362c 3039 3520 e294 820a  .     6,095 ....
-000008d0: e294 8220 332e 3520 2020 2020 20e2 9482  ... 3.5      ...
-000008e0: 2032 3031 382d 3038 2d31 3520 e294 8220   2018-08-15 ... 
-000008f0: 2020 2032 302c 3335 3820 e294 820a e294     20,358 ......
-00000900: 8220 332e 3620 2020 2020 20e2 9482 2032  . 3.6      ... 2
-00000910: 3031 382d 3038 2d31 3520 e294 8220 2020  018-08-15 ...   
-00000920: 2033 352c 3237 3420 e294 820a e294 8220   35,274 ....... 
-00000930: 332e 3720 2020 2020 20e2 9482 2032 3031  3.7      ... 201
-00000940: 382d 3038 2d31 3520 e294 8220 2020 2020  8-08-15 ...     
-00000950: 362c 3539 3520 e294 820a e294 8220 332e  6,595 ....... 3.
-00000960: 3820 2020 2020 20e2 9482 2032 3031 382d  8      ... 2018-
-00000970: 3038 2d31 3520 e294 8220 2020 2020 2020  08-15 ...       
-00000980: 2020 3320 e294 820a e294 8220 6e75 6c6c    3 ....... null
-00000990: 2020 2020 20e2 9482 2032 3031 382d 3038       ... 2018-08
-000009a0: 2d31 3520 e294 8220 2020 2020 312c 3031  -15 ...     1,01
-000009b0: 3920 e294 820a e294 94e2 9480 e294 80e2  9 ..............
-000009c0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-000009d0: 80e2 9480 e294 80e2 94b4 e294 80e2 9480  ................
+000007e0: e294 80e2 9480 e294 bce2 9480 e294 80e2  ................
+000007f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
+00000800: 80e2 9480 e294 80e2 9480 e294 a40a e294  ................
+00000810: 8220 322e 3620 2020 2020 20e2 9482 2032  . 2.6      ... 2
+00000820: 3031 382d 3038 2d31 3520 e294 8220 2020  018-08-15 ...   
+00000830: 2020 2020 2035 3120 e294 820a e294 8220       51 ....... 
+00000840: 322e 3720 2020 2020 20e2 9482 2032 3031  2.7      ... 201
+00000850: 382d 3038 2d31 3520 e294 8220 2020 2036  8-08-15 ...    6
+00000860: 332c 3734 3920 e294 820a e294 8220 332e  3,749 ....... 3.
+00000870: 3220 2020 2020 20e2 9482 2032 3031 382d  2      ... 2018-
+00000880: 3038 2d31 3520 e294 8220 2020 2020 2020  08-15 ...       
+00000890: 2020 3220 e294 820a e294 8220 332e 3320    2 ....... 3.3 
+000008a0: 2020 2020 20e2 9482 2032 3031 382d 3038       ... 2018-08
+000008b0: 2d31 3520 e294 8220 2020 2020 2020 2034  -15 ...        4
+000008c0: 3020 e294 820a e294 8220 332e 3420 2020  0 ....... 3.4   
+000008d0: 2020 20e2 9482 2032 3031 382d 3038 2d31     ... 2018-08-1
+000008e0: 3520 e294 8220 2020 2020 362c 3039 3520  5 ...     6,095 
+000008f0: e294 820a e294 8220 332e 3520 2020 2020  ....... 3.5     
+00000900: 20e2 9482 2032 3031 382d 3038 2d31 3520   ... 2018-08-15 
+00000910: e294 8220 2020 2032 302c 3335 3820 e294  ...    20,358 ..
+00000920: 820a e294 8220 332e 3620 2020 2020 20e2  ..... 3.6      .
+00000930: 9482 2032 3031 382d 3038 2d31 3520 e294  .. 2018-08-15 ..
+00000940: 8220 2020 2033 352c 3237 3420 e294 820a  .    35,274 ....
+00000950: e294 8220 332e 3720 2020 2020 20e2 9482  ... 3.7      ...
+00000960: 2032 3031 382d 3038 2d31 3520 e294 8220   2018-08-15 ... 
+00000970: 2020 2020 362c 3539 3520 e294 820a e294      6,595 ......
+00000980: 8220 332e 3820 2020 2020 20e2 9482 2032  . 3.8      ... 2
+00000990: 3031 382d 3038 2d31 3520 e294 8220 2020  018-08-15 ...   
+000009a0: 2020 2020 2020 3320 e294 820a e294 8220        3 ....... 
+000009b0: 6e75 6c6c 2020 2020 20e2 9482 2032 3031  null     ... 201
+000009c0: 382d 3038 2d31 3520 e294 8220 2020 2020  8-08-15 ...     
+000009d0: 312c 3031 3920 e294 820a e294 94e2 9480  1,019 ..........
 000009e0: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-000009f0: 9480 e294 80e2 9480 e294 80e2 9480 e294  ................
-00000a00: b4e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+000009f0: 9480 e294 80e2 9480 e294 80e2 94b4 e294  ................
+00000a00: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
 00000a10: e294 80e2 9480 e294 80e2 9480 e294 80e2  ................
-00000a20: 9480 e294 980a 2222 220a 0a45 5850 4543  ......"""..EXPEC
-00000a30: 5445 445f 5441 4255 4c41 5445 445f 4d44  TED_TABULATED_MD
-00000a40: 203d 2022 2222 0a7c 2063 6174 6567 6f72   = """.| categor
-00000a50: 7920 7c20 2020 2064 6174 6520 2020 207c  y |    date    |
-00000a60: 2064 6f77 6e6c 6f61 6473 207c 0a7c 3a2d   downloads |.|:-
-00000a70: 2d2d 2d2d 2d2d 2d2d 7c3a 2d2d 2d2d 2d2d  --------|:------
-00000a80: 2d2d 2d2d 3a7c 2d2d 2d2d 2d2d 2d2d 2d2d  ----:|----------
-00000a90: 3a7c 0a7c 2032 2e36 2020 2020 2020 7c20  :|.| 2.6      | 
-00000aa0: 3230 3138 2d30 382d 3135 207c 2020 2020  2018-08-15 |    
-00000ab0: 2020 2020 3531 207c 0a7c 2032 2e37 2020      51 |.| 2.7  
-00000ac0: 2020 2020 7c20 3230 3138 2d30 382d 3135      | 2018-08-15
-00000ad0: 207c 2020 2020 3633 2c37 3439 207c 0a7c   |    63,749 |.|
-00000ae0: 2033 2e32 2020 2020 2020 7c20 3230 3138   3.2      | 2018
-00000af0: 2d30 382d 3135 207c 2020 2020 2020 2020  -08-15 |        
-00000b00: 2032 207c 0a7c 2033 2e33 2020 2020 2020   2 |.| 3.3      
-00000b10: 7c20 3230 3138 2d30 382d 3135 207c 2020  | 2018-08-15 |  
-00000b20: 2020 2020 2020 3430 207c 0a7c 2033 2e34        40 |.| 3.4
-00000b30: 2020 2020 2020 7c20 3230 3138 2d30 382d        | 2018-08-
-00000b40: 3135 207c 2020 2020 2036 2c30 3935 207c  15 |     6,095 |
-00000b50: 0a7c 2033 2e35 2020 2020 2020 7c20 3230  .| 3.5      | 20
-00000b60: 3138 2d30 382d 3135 207c 2020 2020 3230  18-08-15 |    20
-00000b70: 2c33 3538 207c 0a7c 2033 2e36 2020 2020  ,358 |.| 3.6    
-00000b80: 2020 7c20 3230 3138 2d30 382d 3135 207c    | 2018-08-15 |
-00000b90: 2020 2020 3335 2c32 3734 207c 0a7c 2033      35,274 |.| 3
-00000ba0: 2e37 2020 2020 2020 7c20 3230 3138 2d30  .7      | 2018-0
-00000bb0: 382d 3135 207c 2020 2020 2036 2c35 3935  8-15 |     6,595
-00000bc0: 207c 0a7c 2033 2e38 2020 2020 2020 7c20   |.| 3.8      | 
-00000bd0: 3230 3138 2d30 382d 3135 207c 2020 2020  2018-08-15 |    
-00000be0: 2020 2020 2033 207c 0a7c 206e 756c 6c20       3 |.| null 
-00000bf0: 2020 2020 7c20 3230 3138 2d30 382d 3135      | 2018-08-15
-00000c00: 207c 2020 2020 2031 2c30 3139 207c 0a22   |     1,019 |."
-00000c10: 2222 0a0a 0a45 5850 4543 5445 445f 5441  ""...EXPECTED_TA
-00000c20: 4255 4c41 5445 445f 5253 5420 3d20 2222  BULATED_RST = ""
-00000c30: 220a 2e2e 2074 6162 6c65 3a3a 0a0a 2020  "... table::..  
-00000c40: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 2020 3d3d    ==========  ==
-00000c50: 3d3d 3d3d 3d3d 3d3d 3d3d 2020 3d3d 3d3d  ==========  ====
-00000c60: 3d3d 3d3d 3d3d 3d0a 2020 2020 2063 6174  =======.     cat
-00000c70: 6567 6f72 7920 2020 2020 2020 6461 7465  egory       date
-00000c80: 2020 2020 2020 2064 6f77 6e6c 6f61 6473         downloads
-00000c90: 200a 2020 2020 3d3d 3d3d 3d3d 3d3d 3d3d   .    ==========
-00000ca0: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2020    ============  
-00000cb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020  ===========.    
-00000cc0: 2032 2e36 2020 2020 2020 2020 2032 3031   2.6         201
-00000cd0: 382d 3038 2d31 3520 2020 2020 2020 2020  8-08-15         
-00000ce0: 2020 3531 200a 2020 2020 2032 2e37 2020    51 .     2.7  
-00000cf0: 2020 2020 2020 2032 3031 382d 3038 2d31         2018-08-1
-00000d00: 3520 2020 2020 2020 3633 2c37 3439 200a  5       63,749 .
-00000d10: 2020 2020 2033 2e32 2020 2020 2020 2020       3.2        
-00000d20: 2032 3031 382d 3038 2d31 3520 2020 2020   2018-08-15     
-00000d30: 2020 2020 2020 2032 200a 2020 2020 2033         2 .     3
-00000d40: 2e33 2020 2020 2020 2020 2032 3031 382d  .3         2018-
-00000d50: 3038 2d31 3520 2020 2020 2020 2020 2020  08-15           
-00000d60: 3430 200a 2020 2020 2033 2e34 2020 2020  40 .     3.4    
-00000d70: 2020 2020 2032 3031 382d 3038 2d31 3520       2018-08-15 
-00000d80: 2020 2020 2020 2036 2c30 3935 200a 2020         6,095 .  
-00000d90: 2020 2033 2e35 2020 2020 2020 2020 2032     3.5         2
-00000da0: 3031 382d 3038 2d31 3520 2020 2020 2020  018-08-15       
-00000db0: 3230 2c33 3538 200a 2020 2020 2033 2e36  20,358 .     3.6
-00000dc0: 2020 2020 2020 2020 2032 3031 382d 3038           2018-08
-00000dd0: 2d31 3520 2020 2020 2020 3335 2c32 3734  -15       35,274
-00000de0: 200a 2020 2020 2033 2e37 2020 2020 2020   .     3.7      
-00000df0: 2020 2032 3031 382d 3038 2d31 3520 2020     2018-08-15   
-00000e00: 2020 2020 2036 2c35 3935 200a 2020 2020       6,595 .    
-00000e10: 2033 2e38 2020 2020 2020 2020 2032 3031   3.8         201
-00000e20: 382d 3038 2d31 3520 2020 2020 2020 2020  8-08-15         
-00000e30: 2020 2033 200a 2020 2020 206e 756c 6c20     3 .     null 
-00000e40: 2020 2020 2020 2032 3031 382d 3038 2d31         2018-08-1
-00000e50: 3520 2020 2020 2020 2031 2c30 3139 200a  5        1,019 .
-00000e60: 2020 2020 3d3d 3d3d 3d3d 3d3d 3d3d 2020      ==========  
-00000e70: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2020 3d3d  ============  ==
-00000e80: 3d3d 3d3d 3d3d 3d3d 3d0a 2222 2220 2023  =========."""  #
-00000e90: 206e 6f71 613a 2057 3239 310a 0a45 5850   noqa: W291..EXP
-00000ea0: 4543 5445 445f 5441 4255 4c41 5445 445f  ECTED_TABULATED_
-00000eb0: 5453 5620 3d20 2222 220a 2263 6174 6567  TSV = """."categ
-00000ec0: 6f72 7922 5c74 2264 6174 6522 5c74 2264  ory"\t"date"\t"d
-00000ed0: 6f77 6e6c 6f61 6473 220a 2232 2e36 225c  ownloads"."2.6"\
-00000ee0: 7422 3230 3138 2d30 382d 3135 225c 7435  t"2018-08-15"\t5
-00000ef0: 310a 2232 2e37 225c 7422 3230 3138 2d30  1."2.7"\t"2018-0
-00000f00: 382d 3135 225c 7436 332c 3734 390a 2233  8-15"\t63,749."3
-00000f10: 2e32 225c 7422 3230 3138 2d30 382d 3135  .2"\t"2018-08-15
-00000f20: 225c 7432 0a22 332e 3322 5c74 2232 3031  "\t2."3.3"\t"201
-00000f30: 382d 3038 2d31 3522 5c74 3430 0a22 332e  8-08-15"\t40."3.
-00000f40: 3422 5c74 2232 3031 382d 3038 2d31 3522  4"\t"2018-08-15"
-00000f50: 5c74 362c 3039 350a 2233 2e35 225c 7422  \t6,095."3.5"\t"
-00000f60: 3230 3138 2d30 382d 3135 225c 7432 302c  2018-08-15"\t20,
-00000f70: 3335 380a 2233 2e36 225c 7422 3230 3138  358."3.6"\t"2018
-00000f80: 2d30 382d 3135 225c 7433 352c 3237 340a  -08-15"\t35,274.
-00000f90: 2233 2e37 225c 7422 3230 3138 2d30 382d  "3.7"\t"2018-08-
-00000fa0: 3135 225c 7436 2c35 3935 0a22 332e 3822  15"\t6,595."3.8"
-00000fb0: 5c74 2232 3031 382d 3038 2d31 3522 5c74  \t"2018-08-15"\t
-00000fc0: 330a 226e 756c 6c22 5c74 2232 3031 382d  3."null"\t"2018-
-00000fd0: 3038 2d31 3522 5c74 312c 3031 390a 2222  08-15"\t1,019.""
-00000fe0: 2220 2023 206e 6f71 613a 2057 3239 310a  "  # noqa: W291.
+00000a20: 9480 e294 b4e2 9480 e294 80e2 9480 e294  ................
+00000a30: 80e2 9480 e294 80e2 9480 e294 80e2 9480  ................
+00000a40: e294 80e2 9480 e294 980a 2222 220a 0a45  .........."""..E
+00000a50: 5850 4543 5445 445f 5441 4255 4c41 5445  XPECTED_TABULATE
+00000a60: 445f 4d44 203d 2022 2222 0a7c 2063 6174  D_MD = """.| cat
+00000a70: 6567 6f72 7920 7c20 2020 2064 6174 6520  egory |    date 
+00000a80: 2020 207c 2064 6f77 6e6c 6f61 6473 207c     | downloads |
+00000a90: 0a7c 203a 2d2d 2d2d 2d2d 2d2d 7c20 3a2d  .| :--------| :-
+00000aa0: 2d2d 2d2d 2d2d 2d3a 207c 2d2d 2d2d 2d2d  -------: |------
+00000ab0: 2d2d 2d3a 207c 0a7c 2032 2e36 2020 2020  ---: |.| 2.6    
+00000ac0: 2020 7c20 3230 3138 2d30 382d 3135 207c    | 2018-08-15 |
+00000ad0: 2020 2020 2020 2020 3531 207c 0a7c 2032          51 |.| 2
+00000ae0: 2e37 2020 2020 2020 7c20 3230 3138 2d30  .7      | 2018-0
+00000af0: 382d 3135 207c 2020 2020 3633 2c37 3439  8-15 |    63,749
+00000b00: 207c 0a7c 2033 2e32 2020 2020 2020 7c20   |.| 3.2      | 
+00000b10: 3230 3138 2d30 382d 3135 207c 2020 2020  2018-08-15 |    
+00000b20: 2020 2020 2032 207c 0a7c 2033 2e33 2020       2 |.| 3.3  
+00000b30: 2020 2020 7c20 3230 3138 2d30 382d 3135      | 2018-08-15
+00000b40: 207c 2020 2020 2020 2020 3430 207c 0a7c   |        40 |.|
+00000b50: 2033 2e34 2020 2020 2020 7c20 3230 3138   3.4      | 2018
+00000b60: 2d30 382d 3135 207c 2020 2020 2036 2c30  -08-15 |     6,0
+00000b70: 3935 207c 0a7c 2033 2e35 2020 2020 2020  95 |.| 3.5      
+00000b80: 7c20 3230 3138 2d30 382d 3135 207c 2020  | 2018-08-15 |  
+00000b90: 2020 3230 2c33 3538 207c 0a7c 2033 2e36    20,358 |.| 3.6
+00000ba0: 2020 2020 2020 7c20 3230 3138 2d30 382d        | 2018-08-
+00000bb0: 3135 207c 2020 2020 3335 2c32 3734 207c  15 |    35,274 |
+00000bc0: 0a7c 2033 2e37 2020 2020 2020 7c20 3230  .| 3.7      | 20
+00000bd0: 3138 2d30 382d 3135 207c 2020 2020 2036  18-08-15 |     6
+00000be0: 2c35 3935 207c 0a7c 2033 2e38 2020 2020  ,595 |.| 3.8    
+00000bf0: 2020 7c20 3230 3138 2d30 382d 3135 207c    | 2018-08-15 |
+00000c00: 2020 2020 2020 2020 2033 207c 0a7c 206e           3 |.| n
+00000c10: 756c 6c20 2020 2020 7c20 3230 3138 2d30  ull     | 2018-0
+00000c20: 382d 3135 207c 2020 2020 2031 2c30 3139  8-15 |     1,019
+00000c30: 207c 0a22 2222 0a0a 0a45 5850 4543 5445   |."""...EXPECTE
+00000c40: 445f 5441 4255 4c41 5445 445f 5253 5420  D_TABULATED_RST 
+00000c50: 3d20 2222 220a 2e2e 2074 6162 6c65 3a3a  = """... table::
+00000c60: 0a0a 2020 2020 3d3d 3d3d 3d3d 3d3d 3d3d  ..    ==========
+00000c70: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 2020    ============  
+00000c80: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2020 2020  ===========.    
+00000c90: 2063 6174 6567 6f72 7920 2020 2020 2020   category       
+00000ca0: 6461 7465 2020 2020 2020 2064 6f77 6e6c  date       downl
+00000cb0: 6f61 6473 200a 2020 2020 3d3d 3d3d 3d3d  oads .    ======
+00000cc0: 3d3d 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d  ====  ==========
+00000cd0: 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ==  ===========.
+00000ce0: 2020 2020 2032 2e36 2020 2020 2020 2020       2.6        
+00000cf0: 2032 3031 382d 3038 2d31 3520 2020 2020   2018-08-15     
+00000d00: 2020 2020 2020 3531 200a 2020 2020 2032        51 .     2
+00000d10: 2e37 2020 2020 2020 2020 2032 3031 382d  .7         2018-
+00000d20: 3038 2d31 3520 2020 2020 2020 3633 2c37  08-15       63,7
+00000d30: 3439 200a 2020 2020 2033 2e32 2020 2020  49 .     3.2    
+00000d40: 2020 2020 2032 3031 382d 3038 2d31 3520       2018-08-15 
+00000d50: 2020 2020 2020 2020 2020 2032 200a 2020             2 .  
+00000d60: 2020 2033 2e33 2020 2020 2020 2020 2032     3.3         2
+00000d70: 3031 382d 3038 2d31 3520 2020 2020 2020  018-08-15       
+00000d80: 2020 2020 3430 200a 2020 2020 2033 2e34      40 .     3.4
+00000d90: 2020 2020 2020 2020 2032 3031 382d 3038           2018-08
+00000da0: 2d31 3520 2020 2020 2020 2036 2c30 3935  -15        6,095
+00000db0: 200a 2020 2020 2033 2e35 2020 2020 2020   .     3.5      
+00000dc0: 2020 2032 3031 382d 3038 2d31 3520 2020     2018-08-15   
+00000dd0: 2020 2020 3230 2c33 3538 200a 2020 2020      20,358 .    
+00000de0: 2033 2e36 2020 2020 2020 2020 2032 3031   3.6         201
+00000df0: 382d 3038 2d31 3520 2020 2020 2020 3335  8-08-15       35
+00000e00: 2c32 3734 200a 2020 2020 2033 2e37 2020  ,274 .     3.7  
+00000e10: 2020 2020 2020 2032 3031 382d 3038 2d31         2018-08-1
+00000e20: 3520 2020 2020 2020 2036 2c35 3935 200a  5        6,595 .
+00000e30: 2020 2020 2033 2e38 2020 2020 2020 2020       3.8        
+00000e40: 2032 3031 382d 3038 2d31 3520 2020 2020   2018-08-15     
+00000e50: 2020 2020 2020 2033 200a 2020 2020 206e         3 .     n
+00000e60: 756c 6c20 2020 2020 2020 2032 3031 382d  ull        2018-
+00000e70: 3038 2d31 3520 2020 2020 2020 2031 2c30  08-15        1,0
+00000e80: 3139 200a 2020 2020 3d3d 3d3d 3d3d 3d3d  19 .    ========
+00000e90: 3d3d 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ==  ============
+00000ea0: 2020 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 2222    ===========.""
+00000eb0: 2220 2023 206e 6f71 613a 2057 3239 310a  "  # noqa: W291.
+00000ec0: 0a45 5850 4543 5445 445f 5441 4255 4c41  .EXPECTED_TABULA
+00000ed0: 5445 445f 5453 5620 3d20 2222 220a 2263  TED_TSV = """."c
+00000ee0: 6174 6567 6f72 7922 5c74 2264 6174 6522  ategory"\t"date"
+00000ef0: 5c74 2264 6f77 6e6c 6f61 6473 220a 2232  \t"downloads"."2
+00000f00: 2e36 225c 7422 3230 3138 2d30 382d 3135  .6"\t"2018-08-15
+00000f10: 225c 7435 310a 2232 2e37 225c 7422 3230  "\t51."2.7"\t"20
+00000f20: 3138 2d30 382d 3135 225c 7436 332c 3734  18-08-15"\t63,74
+00000f30: 390a 2233 2e32 225c 7422 3230 3138 2d30  9."3.2"\t"2018-0
+00000f40: 382d 3135 225c 7432 0a22 332e 3322 5c74  8-15"\t2."3.3"\t
+00000f50: 2232 3031 382d 3038 2d31 3522 5c74 3430  "2018-08-15"\t40
+00000f60: 0a22 332e 3422 5c74 2232 3031 382d 3038  ."3.4"\t"2018-08
+00000f70: 2d31 3522 5c74 362c 3039 350a 2233 2e35  -15"\t6,095."3.5
+00000f80: 225c 7422 3230 3138 2d30 382d 3135 225c  "\t"2018-08-15"\
+00000f90: 7432 302c 3335 380a 2233 2e36 225c 7422  t20,358."3.6"\t"
+00000fa0: 3230 3138 2d30 382d 3135 225c 7433 352c  2018-08-15"\t35,
+00000fb0: 3237 340a 2233 2e37 225c 7422 3230 3138  274."3.7"\t"2018
+00000fc0: 2d30 382d 3135 225c 7436 2c35 3935 0a22  -08-15"\t6,595."
+00000fd0: 332e 3822 5c74 2232 3031 382d 3038 2d31  3.8"\t"2018-08-1
+00000fe0: 3522 5c74 330a 226e 756c 6c22 5c74 2232  5"\t3."null"\t"2
+00000ff0: 3031 382d 3038 2d31 3522 5c74 312c 3031  018-08-15"\t1,01
+00001000: 390a 2222 220a                           9.""".
```

### Comparing `pypistats-1.5.0/tests/data/python_minor.py` & `pypistats-1.6.0/tests/data/python_minor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from __future__ import annotations
+
 DATA = [
     {"category": "2.4", "date": "2018-04-28", "downloads": 1},
     {"category": "2.4", "date": "2018-06-08", "downloads": 1},
     {"category": "2.4", "date": "2018-09-02", "downloads": 1},
     {"category": "2.4", "date": "2018-09-03", "downloads": 3},
     {"category": "2.4", "date": "2018-09-11", "downloads": 1},
     {"category": "2.4", "date": "2018-09-19", "downloads": 1},
```

### Comparing `pypistats-1.5.0/.gitignore` & `pypistats-1.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pypistats-1.5.0/LICENSE.txt` & `pypistats-1.6.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pypistats-1.5.0/README.md` & `pypistats-1.6.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -94,15 +94,15 @@
 <!-- [[[cog run("pypistats recent pillow") ]]] -->
 
 ```console
 $ pypistats recent pillow
 ┌───────────┬────────────┬────────────┐
 │  last_day │ last_month │  last_week │
 ├───────────┼────────────┼────────────┤
-│ 1,740,674 │ 50,722,906 │ 11,471,253 │
+│ 3,419,597 │ 91,237,125 │ 21,259,217 │
 └───────────┴────────────┴────────────┘
 ```
 
 <!-- [[[end]]] -->
 
 Help for another subcommand:
 
@@ -153,59 +153,61 @@
 <!-- [[[cog run("pypistats python_minor pillow --last-month") ]]] -->
 
 ```console
 $ pypistats python_minor pillow --last-month
 ┌──────────┬─────────┬────────────┐
 │ category │ percent │  downloads │
 ├──────────┼─────────┼────────────┤
-│ 3.7      │  36.58% │ 18,620,128 │
-│ 3.8      │  22.17% │ 11,285,248 │
-│ 3.9      │  13.83% │  7,041,419 │
-│ 3.6      │  10.72% │  5,454,315 │
-│ null     │   7.39% │  3,761,767 │
-│ 3.10     │   6.41% │  3,263,885 │
-│ 3.11     │   1.16% │    589,792 │
-│ 2.7      │   0.89% │    451,041 │
-│ 3.5      │   0.83% │    422,741 │
-│ 3.12     │   0.01% │      3,089 │
-│ 3.4      │   0.00% │      2,483 │
-│ 3.3      │   0.00% │        251 │
-│ 3.2      │   0.00% │         95 │
-│ 2.6      │   0.00% │          1 │
-│ Total    │         │ 50,896,255 │
+│ 3.8      │  18.37% │ 16,161,117 │
+│ 3.10     │  17.47% │ 15,373,666 │
+│ 3.7      │  16.70% │ 14,691,371 │
+│ 3.11     │  15.49% │ 13,630,259 │
+│ 3.9      │  13.19% │ 11,605,389 │
+│ 3.6      │   9.68% │  8,519,789 │
+│ null     │   4.64% │  4,085,994 │
+│ 3.12     │   3.26% │  2,871,386 │
+│ 2.7      │   0.95% │    837,638 │
+│ 3.5      │   0.25% │    216,308 │
+│ 3.13     │   0.00% │      2,830 │
+│ 3.4      │   0.00% │      1,237 │
+│ 3.3      │   0.00% │        109 │
+│ 3.1      │   0.00% │          3 │
+│ 3.2      │   0.00% │          2 │
+│ Total    │         │ 87,997,098 │
 └──────────┴─────────┴────────────┘
 
-Date range: 2022-11-01 - 2022-11-30
+Date range: 2024-02-01 - 2024-02-29
 ```
 
 <!-- [[[end]]] -->
 
 You can format in Markdown, ready for pasting in GitHub issues and PRs:
 
 <!-- [[[cog run("pypistats python_minor pillow --last-month --format md", with_console=False) ]]] -->
 
 | category | percent |  downloads |
 | :------- | ------: | ---------: |
-| 3.7      |  36.58% | 18,620,128 |
-| 3.8      |  22.17% | 11,285,248 |
-| 3.9      |  13.83% |  7,041,419 |
-| 3.6      |  10.72% |  5,454,315 |
-| null     |   7.39% |  3,761,767 |
-| 3.10     |   6.41% |  3,263,885 |
-| 3.11     |   1.16% |    589,792 |
-| 2.7      |   0.89% |    451,041 |
-| 3.5      |   0.83% |    422,741 |
-| 3.12     |   0.01% |      3,089 |
-| 3.4      |   0.00% |      2,483 |
-| 3.3      |   0.00% |        251 |
-| 3.2      |   0.00% |         95 |
-| 2.6      |   0.00% |          1 |
-| Total    |         | 50,896,255 |
+| 3.8      |  18.37% | 16,161,117 |
+| 3.10     |  17.47% | 15,373,666 |
+| 3.7      |  16.70% | 14,691,371 |
+| 3.11     |  15.49% | 13,630,259 |
+| 3.9      |  13.19% | 11,605,389 |
+| 3.6      |   9.68% |  8,519,789 |
+| null     |   4.64% |  4,085,994 |
+| 3.12     |   3.26% |  2,871,386 |
+| 2.7      |   0.95% |    837,638 |
+| 3.5      |   0.25% |    216,308 |
+| 3.13     |   0.00% |      2,830 |
+| 3.4      |   0.00% |      1,237 |
+| 3.3      |   0.00% |        109 |
+| 3.1      |   0.00% |          3 |
+| 3.2      |   0.00% |          2 |
+| Total    |         | 87,997,098 |
 
-Date range: 2022-11-01 - 2022-11-30
+Date range: 2024-02-01 - 2024-02-29
 
 <!-- [[[end]]] -->
 
 These are equivalent (in May 2019):
 
 ```sh
 pypistats python_major pip --last-month
```

### Comparing `pypistats-1.5.0/pyproject.toml` & `pypistats-1.6.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -27,14 +27,15 @@
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3 :: Only",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
+  "Programming Language :: Python :: 3.13",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dynamic = [
   "version",
 ]
 dependencies = [
@@ -68,12 +69,43 @@
 
 [tool.hatch]
 version.source = "vcs"
 
 [tool.hatch.version.raw-options]
 local_scheme = "no-local-version"
 
-[tool.isort]
-profile = "black"
+[tool.ruff]
+fix = true
+
+[tool.ruff.lint]
+select = [
+  "C4", # flake8-comprehensions
+  "E", # pycodestyle errors
+  "EM", # flake8-errmsg
+  "F", # pyflakes errors
+  "I", # isort
+  "ISC", # flake8-implicit-str-concat
+  "LOG", # flake8-logging
+  "PGH", # pygrep-hooks
+  "RUF100", # unused noqa (yesqa)
+  "UP", # pyupgrade
+  "W", # pycodestyle warnings
+  "YTT", # flake8-2020
+]
+extend-ignore = [
+  "E203", # Whitespace before ':'
+  "E221", # Multiple spaces before operator
+  "E226", # Missing whitespace around arithmetic operator
+  "E241", # Multiple spaces after ','
+]
+
+[tool.ruff.lint.isort]
+known-first-party = ["pypistats"]
+required-imports = ["from __future__ import annotations"]
 
 [tool.pytest.ini_options]
 addopts = "--color=yes"
+filterwarnings = [
+  # Python <= 3.11
+  "ignore:sys.monitoring isn't available, using default core:coverage.exceptions.CoverageWarning",
+]
+testpaths = ["tests"]
```

### Comparing `pypistats-1.5.0/PKG-INFO` & `pypistats-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pypistats
-Version: 1.5.0
+Version: 1.6.0
 Summary: Python interface to PyPI Stats API https://pypistats.org/api
 Project-URL: Changelog, https://github.com/hugovk/pypistats/releases
 Project-URL: Homepage, https://github.com/hugovk/pypistats
 Project-URL: Source, https://github.com/hugovk/pypistats
 Author: Hugo van Kemenade
 License: MIT
 License-File: LICENSE.txt
@@ -16,14 +16,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: 3.13
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: httpx>=0.19
 Requires-Dist: platformdirs
 Requires-Dist: prettytable>=2.4
 Requires-Dist: pytablewriter[html]>=0.63
@@ -137,15 +138,15 @@
 <!-- [[[cog run("pypistats recent pillow") ]]] -->
 
 ```console
 $ pypistats recent pillow
 ┌───────────┬────────────┬────────────┐
 │  last_day │ last_month │  last_week │
 ├───────────┼────────────┼────────────┤
-│ 1,740,674 │ 50,722,906 │ 11,471,253 │
+│ 3,419,597 │ 91,237,125 │ 21,259,217 │
 └───────────┴────────────┴────────────┘
 ```
 
 <!-- [[[end]]] -->
 
 Help for another subcommand:
 
@@ -196,59 +197,61 @@
 <!-- [[[cog run("pypistats python_minor pillow --last-month") ]]] -->
 
 ```console
 $ pypistats python_minor pillow --last-month
 ┌──────────┬─────────┬────────────┐
 │ category │ percent │  downloads │
 ├──────────┼─────────┼────────────┤
-│ 3.7      │  36.58% │ 18,620,128 │
-│ 3.8      │  22.17% │ 11,285,248 │
-│ 3.9      │  13.83% │  7,041,419 │
-│ 3.6      │  10.72% │  5,454,315 │
-│ null     │   7.39% │  3,761,767 │
-│ 3.10     │   6.41% │  3,263,885 │
-│ 3.11     │   1.16% │    589,792 │
-│ 2.7      │   0.89% │    451,041 │
-│ 3.5      │   0.83% │    422,741 │
-│ 3.12     │   0.01% │      3,089 │
-│ 3.4      │   0.00% │      2,483 │
-│ 3.3      │   0.00% │        251 │
-│ 3.2      │   0.00% │         95 │
-│ 2.6      │   0.00% │          1 │
-│ Total    │         │ 50,896,255 │
+│ 3.8      │  18.37% │ 16,161,117 │
+│ 3.10     │  17.47% │ 15,373,666 │
+│ 3.7      │  16.70% │ 14,691,371 │
+│ 3.11     │  15.49% │ 13,630,259 │
+│ 3.9      │  13.19% │ 11,605,389 │
+│ 3.6      │   9.68% │  8,519,789 │
+│ null     │   4.64% │  4,085,994 │
+│ 3.12     │   3.26% │  2,871,386 │
+│ 2.7      │   0.95% │    837,638 │
+│ 3.5      │   0.25% │    216,308 │
+│ 3.13     │   0.00% │      2,830 │
+│ 3.4      │   0.00% │      1,237 │
+│ 3.3      │   0.00% │        109 │
+│ 3.1      │   0.00% │          3 │
+│ 3.2      │   0.00% │          2 │
+│ Total    │         │ 87,997,098 │
 └──────────┴─────────┴────────────┘
 
-Date range: 2022-11-01 - 2022-11-30
+Date range: 2024-02-01 - 2024-02-29
 ```
 
 <!-- [[[end]]] -->
 
 You can format in Markdown, ready for pasting in GitHub issues and PRs:
 
 <!-- [[[cog run("pypistats python_minor pillow --last-month --format md", with_console=False) ]]] -->
 
 | category | percent |  downloads |
 | :------- | ------: | ---------: |
-| 3.7      |  36.58% | 18,620,128 |
-| 3.8      |  22.17% | 11,285,248 |
-| 3.9      |  13.83% |  7,041,419 |
-| 3.6      |  10.72% |  5,454,315 |
-| null     |   7.39% |  3,761,767 |
-| 3.10     |   6.41% |  3,263,885 |
-| 3.11     |   1.16% |    589,792 |
-| 2.7      |   0.89% |    451,041 |
-| 3.5      |   0.83% |    422,741 |
-| 3.12     |   0.01% |      3,089 |
-| 3.4      |   0.00% |      2,483 |
-| 3.3      |   0.00% |        251 |
-| 3.2      |   0.00% |         95 |
-| 2.6      |   0.00% |          1 |
-| Total    |         | 50,896,255 |
+| 3.8      |  18.37% | 16,161,117 |
+| 3.10     |  17.47% | 15,373,666 |
+| 3.7      |  16.70% | 14,691,371 |
+| 3.11     |  15.49% | 13,630,259 |
+| 3.9      |  13.19% | 11,605,389 |
+| 3.6      |   9.68% |  8,519,789 |
+| null     |   4.64% |  4,085,994 |
+| 3.12     |   3.26% |  2,871,386 |
+| 2.7      |   0.95% |    837,638 |
+| 3.5      |   0.25% |    216,308 |
+| 3.13     |   0.00% |      2,830 |
+| 3.4      |   0.00% |      1,237 |
+| 3.3      |   0.00% |        109 |
+| 3.1      |   0.00% |          3 |
+| 3.2      |   0.00% |          2 |
+| Total    |         | 87,997,098 |
 
-Date range: 2022-11-01 - 2022-11-30
+Date range: 2024-02-01 - 2024-02-29
 
 <!-- [[[end]]] -->
 
 These are equivalent (in May 2019):
 
 ```sh
 pypistats python_major pip --last-month
```

