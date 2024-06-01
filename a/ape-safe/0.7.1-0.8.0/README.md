# Comparing `tmp/ape_safe-0.7.1.tar.gz` & `tmp/ape-safe-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape_safe-0.7.1.tar", max compression
+gzip compressed data, was "ape-safe-0.8.0.tar", last modified: Sat Jun  1 04:30:21 2024, max compression
```

## Comparing `ape_safe-0.7.1.tar` & `ape-safe-0.8.0.tar`

### file list

```diff
@@ -1,5 +1,76 @@
--rw-r--r--   0        0        0    17320 2023-02-05 05:06:40.885007 ape_safe-0.7.1/ape_safe.py
--rw-r--r--   0        0        0      503 2023-02-05 05:18:30.181629 ape_safe-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      809 2022-04-13 16:18:59.305099 ape_safe-0.7.1/readme.md
--rw-r--r--   0        0        0     1526 1970-01-01 00:00:00.000000 ape_safe-0.7.1/setup.py
--rw-r--r--   0        0        0     1543 1970-01-01 00:00:00.000000 ape_safe-0.7.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:30:21.551013 ape-safe-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:30:21.539013 ape-safe-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:30:21.543013 ape-safe-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-06-01 04:29:33.000000 ape-safe-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-06-01 04:29:33.000000 ape-safe-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-06-01 04:29:33.000000 ape-safe-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-06-01 04:29:33.000000 ape-safe-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-06-01 04:29:33.000000 ape-safe-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:30:21.543013 ape-safe-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 04:29:33.000000 ape-safe-0.8.0/.github/workflows/codeql.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-06-01 04:29:33.000000 ape-safe-0.8.0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-06-01 04:29:33.000000 ape-safe-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-01 04:29:33.000000 ape-safe-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-06-01 04:29:33.000000 ape-safe-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-06-01 04:29:33.000000 ape-safe-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-06-01 04:29:33.000000 ape-safe-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-06-01 04:29:33.000000 ape-safe-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-06-01 04:29:33.000000 ape-safe-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11360 2024-06-01 04:29:33.000000 ape-safe-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-06-01 04:30:21.551013 ape-safe-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4809 2024-06-01 04:29:33.000000 ape-safe-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-06-01 04:29:33.000000 ape-safe-0.8.0/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:30:21.543013 ape-safe-0.8.0/ape_safe/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 04:29:33.000000 ape-safe-0.8.0/ape_safe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:30:21.543013 ape-safe-0.8.0/ape_safe/_cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-06-01 04:29:33.000000 ape-safe-0.8.0/ape_safe/_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5123 2024-06-01 04:29:33.000000 ape-safe-0.8.0/ape_safe/_cli/click_ext.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13364 2024-06-01 04:29:33.000000 ape-safe-0.8.0/ape_safe/_cli/pending.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5068 2024-06-01 04:29:33.000000 ape-safe-0.8.0/ape_safe/_cli/safe_mgmt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29622 2024-06-01 04:29:33.000000 ape-safe-0.8.0/ape_safe/accounts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:30:21.547013 ape-safe-0.8.0/ape_safe/client/
+-rw-r--r--   0 runner    (1001) docker     (127)     6682 2024-06-01 04:29:33.000000 ape-safe-0.8.0/ape_safe/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-06-01 04:29:33.000000 ape-safe-0.8.0/ape_safe/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4452 2024-06-01 04:29:33.000000 ape-safe-0.8.0/ape_safe/client/mock.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4081 2024-06-01 04:29:33.000000 ape-safe-0.8.0/ape_safe/client/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4970 2024-06-01 04:29:33.000000 ape-safe-0.8.0/ape_safe/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10281 2024-06-01 04:29:33.000000 ape-safe-0.8.0/ape_safe/multisend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      713 2024-06-01 04:29:33.000000 ape-safe-0.8.0/ape_safe/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-01 04:30:21.000000 ape-safe-0.8.0/ape_safe/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:30:21.543013 ape-safe-0.8.0/ape_safe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5758 2024-06-01 04:30:21.000000 ape-safe-0.8.0/ape_safe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-06-01 04:30:21.000000 ape-safe-0.8.0/ape_safe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 04:30:21.000000 ape-safe-0.8.0/ape_safe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-01 04:30:21.000000 ape-safe-0.8.0/ape_safe.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 04:30:21.000000 ape-safe-0.8.0/ape_safe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-06-01 04:30:21.000000 ape-safe-0.8.0/ape_safe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 04:30:21.000000 ape-safe-0.8.0/ape_safe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:30:21.547013 ape-safe-0.8.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-06-01 04:29:33.000000 ape-safe-0.8.0/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-06-01 04:29:33.000000 ape-safe-0.8.0/docs/ape_safe.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-06-01 04:29:33.000000 ape-safe-0.8.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-06-01 04:29:33.000000 ape-safe-0.8.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-06-01 04:29:33.000000 ape-safe-0.8.0/docs/detailed.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-06-01 04:29:33.000000 ape-safe-0.8.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-06-01 04:29:33.000000 ape-safe-0.8.0/docs/install.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-06-01 04:29:33.000000 ape-safe-0.8.0/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-06-01 04:29:33.000000 ape-safe-0.8.0/docs/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-06-01 04:29:33.000000 ape-safe-0.8.0/docs/signing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-06-01 04:29:33.000000 ape-safe-0.8.0/docs/useful.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-06-01 04:29:33.000000 ape-safe-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-06-01 04:30:21.551013 ape-safe-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3363 2024-06-01 04:29:33.000000 ape-safe-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:30:21.547013 ape-safe-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3899 2024-06-01 04:29:33.000000 ape-safe-0.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:30:21.547013 ape-safe-0.8.0/tests/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)   227900 2024-06-01 04:29:33.000000 ape-safe-0.8.0/tests/contracts/Token.json
+-rw-r--r--   0 runner    (1001) docker     (127)   782533 2024-06-01 04:29:33.000000 ape-safe-0.8.0/tests/contracts/VyperVault.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:30:21.547013 ape-safe-0.8.0/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)     6322 2024-06-01 04:29:33.000000 ape-safe-0.8.0/tests/functional/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-06-01 04:29:33.000000 ape-safe-0.8.0/tests/functional/test_multisend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-06-01 04:29:33.000000 ape-safe-0.8.0/tests/functional/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:30:21.551013 ape-safe-0.8.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:29:33.000000 ape-safe-0.8.0/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-06-01 04:29:33.000000 ape-safe-0.8.0/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2024-06-01 04:29:33.000000 ape-safe-0.8.0/tests/integration/test_pending_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-06-01 04:29:33.000000 ape-safe-0.8.0/tests/integration/test_safe_mgmt_cli.py
```

### Comparing `ape_safe-0.7.1/readme.md` & `ape-safe-0.8.0/docs/quickstart.rst`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,24 @@
-# Ape Safe: Gnosis Safe tx builder
+Quickstart
+================
 
-Ape Safe allows you to iteratively build complex multi-step Gnosis Safe transactions and safely preview their side effects from the convenience of a locally forked mainnet environment.
+.. code-block:: bash
 
-## Installation
+    pip install -U ape-safe
+    brownie console --network mainnet-fork
 
-```
-pip install -U ape-safe
-```
 
-## Quickstart
+.. code-block:: python
 
-```bash
-brownie console --network mainnet-fork
-```
+    from ape_safe import ApeSafe
+    safe = ApeSafe('ychad.eth')
 
-```python
-from ape_safe import ApeSafe
-safe = ApeSafe('ychad.eth')
+    dai = safe.contract('0x6B175474E89094C44Da98b954EedeAC495271d0F')
+    vault = safe.contract('0x19D3364A399d251E894aC732651be8B0E4e85001')
 
-dai = safe.contract('0x6B175474E89094C44Da98b954EedeAC495271d0F')
-vault = safe.contract('0x19D3364A399d251E894aC732651be8B0E4e85001')
+    amount = dai.balanceOf(safe.account)
+    dai.approve(vault, amount)
+    vault.deposit(amount)
 
-amount = dai.balanceOf(safe.account)
-dai.approve(vault, amount)
-vault.deposit(amount)
-
-safe_tx = safe.multisend_from_receipts()
-safe.preview(safe_tx)
-safe.post_transaction(safe_tx)
-```
-
-See [Documentation](https://safe.ape.tax/) for more examples and full reference.
+    safe_tx = safe.multisend_from_receipts()
+    safe.preview(safe_tx)
+    safe.post_transaction(safe_tx)
```

