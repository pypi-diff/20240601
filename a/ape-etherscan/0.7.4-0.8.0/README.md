# Comparing `tmp/ape-etherscan-0.7.4.tar.gz` & `tmp/ape-etherscan-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-etherscan-0.7.4.tar", last modified: Mon May 27 16:07:41 2024, max compression
+gzip compressed data, was "ape-etherscan-0.8.0.tar", last modified: Sat Jun  1 05:56:28 2024, max compression
```

## Comparing `ape-etherscan-0.7.4.tar` & `ape-etherscan-0.8.0.tar`

### file list

```diff
@@ -1,61 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:41.404014 ape-etherscan-0.7.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:41.396014 ape-etherscan-0.7.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:41.396014 ape-etherscan-0.7.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:41.400014 ape-etherscan-0.7.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      624 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/workflows/commit.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      554 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-27 16:07:41.404014 ape-etherscan-0.7.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:41.400014 ape-etherscan-0.7.4/ape_etherscan/
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15703 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4381 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/explorer.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5391 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18535 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/ape_etherscan/verify.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-27 16:07:41.000000 ape-etherscan-0.7.4/ape_etherscan/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:41.400014 ape-etherscan-0.7.4/ape_etherscan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-05-27 16:07:41.000000 ape-etherscan-0.7.4/ape_etherscan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1574 2024-05-27 16:07:41.000000 ape-etherscan-0.7.4/ape_etherscan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:07:41.000000 ape-etherscan-0.7.4/ape_etherscan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 16:07:41.000000 ape-etherscan-0.7.4/ape_etherscan.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-05-27 16:07:41.000000 ape-etherscan-0.7.4/ape_etherscan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-27 16:07:41.000000 ape-etherscan-0.7.4/ape_etherscan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1000 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-27 16:07:41.404014 ape-etherscan-0.7.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4443 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:41.400014 ape-etherscan-0.7.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    21852 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 16:07:41.404014 ape-etherscan-0.7.4/tests/mock_responses/
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/mock_responses/get_account_transactions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/mock_responses/get_account_transactions_with_ctor_args.json
--rw-r--r--   0 runner    (1001) docker     (127)    85182 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/mock_responses/get_contract_response_flattened.json
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/mock_responses/get_contract_response_json.json
--rw-r--r--   0 runner    (1001) docker     (127)    21603 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/mock_responses/get_contract_response_json_source_code.json
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/mock_responses/get_contract_response_not_verified.json
--rw-r--r--   0 runner    (1001) docker     (127)    93453 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/mock_responses/get_proxy_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (127)    93483 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/mock_responses/get_vyper_contract_response.json
--rw-r--r--   0 runner    (1001) docker     (127)     2945 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1690 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/test_dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-27 16:06:47.000000 ape-etherscan-0.7.4/tests/test_etherscan.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:56:28.237772 ape-etherscan-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:56:28.229772 ape-etherscan-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:56:28.233772 ape-etherscan-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:56:28.233772 ape-etherscan-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      624 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/.github/workflows/commit.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      554 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-06-01 05:56:28.237772 ape-etherscan-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5597 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:56:28.233772 ape-etherscan-0.8.0/ape_etherscan/
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/ape_etherscan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15718 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/ape_etherscan/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1459 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/ape_etherscan/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/ape_etherscan/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/ape_etherscan/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4593 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/ape_etherscan/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/ape_etherscan/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/ape_etherscan/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3458 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/ape_etherscan/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/ape_etherscan/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18477 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/ape_etherscan/verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-01 05:56:27.000000 ape-etherscan-0.8.0/ape_etherscan/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:56:28.233772 ape-etherscan-0.8.0/ape_etherscan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6588 2024-06-01 05:56:28.000000 ape-etherscan-0.8.0/ape_etherscan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-06-01 05:56:28.000000 ape-etherscan-0.8.0/ape_etherscan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 05:56:28.000000 ape-etherscan-0.8.0/ape_etherscan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 05:56:28.000000 ape-etherscan-0.8.0/ape_etherscan.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-06-01 05:56:28.000000 ape-etherscan-0.8.0/ape_etherscan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 05:56:28.000000 ape-etherscan-0.8.0/ape_etherscan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-01 05:56:28.237772 ape-etherscan-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4394 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:56:28.237772 ape-etherscan-0.8.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/tests/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20307 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:56:28.229772 ape-etherscan-0.8.0/tests/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:56:28.237772 ape-etherscan-0.8.0/tests/contracts/subcontracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/tests/contracts/subcontracts/foo.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:56:28.229772 ape-etherscan-0.8.0/tests/dependency/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:56:28.237772 ape-etherscan-0.8.0/tests/dependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/tests/dependency/contracts/bar.sol
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:56:28.237772 ape-etherscan-0.8.0/tests/mock_responses/
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/tests/mock_responses/get_account_transactions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/tests/mock_responses/get_account_transactions_with_ctor_args.json
+-rw-r--r--   0 runner    (1001) docker     (127)    85182 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/tests/mock_responses/get_contract_response_flattened.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/tests/mock_responses/get_contract_response_json.json
+-rw-r--r--   0 runner    (1001) docker     (127)    21603 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/tests/mock_responses/get_contract_response_json_source_code.json
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/tests/mock_responses/get_contract_response_not_verified.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93453 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/tests/mock_responses/get_proxy_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)    93483 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/tests/mock_responses/get_vyper_contract_response.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2633 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/tests/test_dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10193 2024-06-01 05:55:37.000000 ape-etherscan-0.8.0/tests/test_etherscan.py
```

### Comparing `ape-etherscan-0.7.4/.github/ISSUE_TEMPLATE/bug.md` & `ape-etherscan-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/.github/ISSUE_TEMPLATE/feature.md` & `ape-etherscan-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/.github/ISSUE_TEMPLATE/work-item.md` & `ape-etherscan-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/.github/release-drafter.yml` & `ape-etherscan-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/.github/workflows/codeql.yml` & `ape-etherscan-0.8.0/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/.github/workflows/commit.yaml` & `ape-etherscan-0.8.0/.github/workflows/commit.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/.github/workflows/prtitle.yaml` & `ape-etherscan-0.8.0/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/.github/workflows/publish.yaml` & `ape-etherscan-0.8.0/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/.github/workflows/stale-prs.yml` & `ape-etherscan-0.8.0/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/.github/workflows/test.yaml` & `ape-etherscan-0.8.0/.github/workflows/test.yaml`

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

### Comparing `ape-etherscan-0.7.4/.gitignore` & `ape-etherscan-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/.pre-commit-config.yaml` & `ape-etherscan-0.8.0/.pre-commit-config.yaml`

 * *Files 11% similar despite different names*

```diff
@@ -26,11 +26,11 @@
     -   id: mypy
         additional_dependencies: [types-PyYAML, types-requests, types-setuptools, pydantic]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
     -   id: mdformat
-        additional_dependencies: [mdformat-gfm, mdformat-frontmatter]
+        additional_dependencies: [mdformat-gfm, mdformat-frontmatter, mdformat-pyproject]
 
 default_language_version:
     python: python3
```

### Comparing `ape-etherscan-0.7.4/CONTRIBUTING.md` & `ape-etherscan-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/LICENSE` & `ape-etherscan-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/PKG-INFO` & `ape-etherscan-0.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: ape-etherscan
-Version: 0.7.4
+Version: 0.8.0
 Summary: ape-etherscan: Etherscan Explorer Plugin for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-etherscan
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
@@ -41,15 +40,15 @@
 - [Snowtrace](https://snowtrace.io) for Avalanche networks.
 - [Basescan](https://basescan.org) for Base networks.
 - [Bscscan](https://bscscan.com) for Binance-Smart-Chain networks.
 - [Blastscan](https://blastscan.io) for Blast networks.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-etherscan-0.7.4/README.md` & `ape-etherscan-0.8.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 - [Snowtrace](https://snowtrace.io) for Avalanche networks.
 - [Basescan](https://basescan.org) for Base networks.
 - [Bscscan](https://bscscan.com) for Binance-Smart-Chain networks.
 - [Blastscan](https://blastscan.io) for Blast networks.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-etherscan-0.7.4/ape_etherscan/__init__.py` & `ape-etherscan-0.8.0/ape_etherscan/__init__.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/ape_etherscan/client.py` & `ape-etherscan-0.8.0/ape_etherscan/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 import os
 import random
 import time
+from collections.abc import Iterator
 from io import StringIO
-from typing import Dict, Iterator, List, Optional
+from typing import Optional
 
 from ape.api import PluginConfig
 from ape.logging import logger
 from ape.utils import USER_AGENT, ManagerAccessMixin
 from requests import Session
 from yarl import URL
 
@@ -197,15 +198,15 @@
         self._last_call = 0.0
 
     @property
     def base_uri(self) -> str:
         return self._instance.api_uri
 
     @property
-    def base_params(self) -> Dict:
+    def base_params(self) -> dict:
         return {"module": self._module_name}
 
     @property
     def _rate_limit(self) -> int:
         config = self.config_manager.get_config("etherscan")
         return getattr(config, self.network_manager.ecosystem.name.lower()).rate_limit
 
@@ -221,16 +222,16 @@
     @property
     def _clean_uri(self) -> str:
         url = URL(self.base_uri).with_user(None).with_password(None)
         return f"{url.with_path('')}/[hidden]" if url.path else f"{url}"
 
     def _get(
         self,
-        params: Optional[Dict] = None,
-        headers: Optional[Dict[str, str]] = None,
+        params: Optional[dict] = None,
+        headers: Optional[dict[str, str]] = None,
         raise_on_exceptions: bool = True,
     ) -> EtherscanResponse:
         params = self.__authorize(params)
 
         # Rate limit
         if time.time() - self._last_call < self._min_time_between_calls:
             time_to_sleep = self._min_time_between_calls - (time.time() - self._last_call)
@@ -244,26 +245,26 @@
             "GET",
             params=params,
             headers=headers,
             raise_on_exceptions=raise_on_exceptions,
         )
 
     def _post(
-        self, json_dict: Optional[Dict] = None, headers: Optional[Dict[str, str]] = None
+        self, json_dict: Optional[dict] = None, headers: Optional[dict[str, str]] = None
     ) -> EtherscanResponse:
         data = self.__authorize(json_dict)
         return self._request("POST", data=data, headers=headers)
 
     def _request(
         self,
         method: str,
         raise_on_exceptions: bool = True,
-        headers: Optional[Dict] = None,
-        params: Optional[Dict] = None,
-        data: Optional[Dict] = None,
+        headers: Optional[dict] = None,
+        params: Optional[dict] = None,
+        data: Optional[dict] = None,
     ) -> EtherscanResponse:
         headers = headers or self.DEFAULT_HEADERS
         for i in range(self._retries):
             logger.debug(f"Request sent to {self._clean_uri}.")
             response = self.session.request(
                 method.upper(),
                 self.base_uri,
@@ -284,15 +285,15 @@
             elif not 200 <= response.status_code < 300:
                 logger.error(f"Response was not successful: {response.text}")
 
             break
 
         return EtherscanResponse(response, self._instance.ecosystem_name, raise_on_exceptions)
 
-    def __authorize(self, params_or_data: Optional[Dict] = None) -> Optional[Dict]:
+    def __authorize(self, params_or_data: Optional[dict] = None) -> Optional[dict]:
         env_var_key = API_KEY_ENV_KEY_MAP.get(self._instance.ecosystem_name)
         if not env_var_key:
             return params_or_data
 
         api_key = os.environ.get(env_var_key)
         if api_key and (not params_or_data or "apikey" not in params_or_data):
             params_or_data = params_or_data or {}
@@ -328,23 +329,23 @@
         if data.get("ABI") == "Contract source code not verified":
             raise ContractNotVerifiedError(result, self._address)
 
         return SourceCodeResponse.model_validate(data)
 
     def verify_source_code(
         self,
-        standard_json_output: Dict,
+        standard_json_output: dict,
         compiler_version: str,
         contract_name: Optional[str] = None,
         optimization_used: bool = False,
         optimization_runs: Optional[int] = 200,
         constructor_arguments: Optional[str] = None,
         evm_version: Optional[str] = None,
         license_type: Optional[int] = None,
-        libraries: Optional[Dict[str, str]] = None,
+        libraries: Optional[dict[str, str]] = None,
     ) -> str:
         libraries = libraries or {}
         if len(libraries) > 10:
             raise ValueError(f"Can only have up to 10 libraries (received {len(libraries)}).")
 
         if not compiler_version.startswith("v"):
             compiler_version = f"v{compiler_version}"
@@ -380,15 +381,15 @@
         return str(self._post(json_dict=json_dict, headers=headers).value)
 
     def check_verify_status(self, guid: str) -> str:
         json_dict = {**self.base_params, "action": "checkverifystatus", "guid": guid}
         response = self._get(params=json_dict, raise_on_exceptions=False)
         return str(response.value)
 
-    def get_creation_data(self) -> List[ContractCreationResponse]:
+    def get_creation_data(self) -> list[ContractCreationResponse]:
         params = {
             **self.base_params,
             "action": "getcontractcreation",
             "contractaddresses": [self._address],
         }
         result = self._get(params=params)
         items = result.value or []
@@ -405,15 +406,15 @@
 
     def get_all_normal_transactions(
         self,
         start_block: Optional[int] = None,
         end_block: Optional[int] = None,
         offset: int = 100,
         sort: str = "asc",
-    ) -> Iterator[Dict]:
+    ) -> Iterator[dict]:
         page_num = 1
         last_page_results = offset  # Start at offset to trigger iteration
         while last_page_results == offset:
             page = self._get_page_of_normal_transactions(
                 page_num, start_block, end_block, offset=offset, sort=sort
             )
 
@@ -426,15 +427,15 @@
     def _get_page_of_normal_transactions(
         self,
         page: int,
         start_block: Optional[int] = None,
         end_block: Optional[int] = None,
         offset: int = 100,
         sort: str = "asc",
-    ) -> List[Dict]:
+    ) -> list[dict]:
         params = {
             **self.base_params,
             "action": "txlist",
             "address": self._address,
             "startblock": start_block,
             "endblock": end_block,
             "page": page,
```

### Comparing `ape-etherscan-0.7.4/ape_etherscan/config.py` & `ape-etherscan-0.8.0/ape_etherscan/config.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/ape_etherscan/dependency.py` & `ape-etherscan-0.8.0/ape_etherscan/dependency.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+from pathlib import Path
+
 from ape.api.projects import DependencyAPI
 from ape.exceptions import ProjectError
 from ape.types import AddressType
 from ethpm_types import PackageManifest
 from hexbytes import HexBytes
-from pydantic import AnyUrl, HttpUrl, field_validator
+from pydantic import field_validator
 
 from .explorer import Etherscan
 
 
 class EtherscanDependency(DependencyAPI):
     etherscan: str
     ecosystem: str = "ethereum"
@@ -23,31 +25,39 @@
         return f"{self.ecosystem}_{self.network}"
 
     @property
     def address(self) -> AddressType:
         return self.network_manager.ethereum.decode_address(self.etherscan)
 
     @property
-    def uri(self) -> AnyUrl:
-        return HttpUrl(f"{self.explorer.get_address_url(self.address)}#code")
+    def package_id(self) -> str:
+        return self.address
+
+    @property
+    def uri(self) -> str:
+        return f"{self.explorer.get_address_url(self.address)}#code"
 
     @property
     def explorer(self) -> Etherscan:
         if self.network_manager.active_provider:
             explorer = self.provider.network.explorer
             if isinstance(explorer, Etherscan):
                 # Could be using a different network.
                 return explorer
             else:
                 return self.network_manager.ethereum.mainnet.explorer
 
         # Assume Ethereum
         return self.network_manager.ethereum.mainnet.explorer
 
-    def extract_manifest(self, use_cache: bool = True) -> PackageManifest:
+    def fetch(self, destination: Path):
+        manifest = self._get_manifest()
+        manifest.unpack_sources(destination)
+
+    def _get_manifest(self) -> PackageManifest:
         ecosystem = self.network_manager.get_ecosystem(self.ecosystem)
         network = ecosystem.get_network(self.network)
 
         ctx = None
         if self.network_manager.active_provider is None:
             ctx = network.use_default_provider()
             ctx.__enter__()
```

### Comparing `ape-etherscan-0.7.4/ape_etherscan/exceptions.py` & `ape-etherscan-0.8.0/ape_etherscan/exceptions.py`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/ape_etherscan/explorer.py` & `ape-etherscan-0.8.0/ape_etherscan/explorer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import json
 from typing import Optional
 
 from ape.api import ExplorerAPI, PluginConfig
 from ape.contracts import ContractInstance
 from ape.exceptions import ProviderNotConnectedError
+from ape.managers.project import ProjectManager
 from ape.types import AddressType, ContractType
 from ethpm_types import Compiler, PackageManifest
 from ethpm_types.source import Source
 
 from ape_etherscan.client import (
     ClientFactory,
     SourceCodeResponse,
@@ -116,9 +117,12 @@
                 contract_type.name = contract.symbol() or contract_type.name
             except ProviderNotConnectedError:
                 pass
 
         return contract_type
 
     def publish_contract(self, address: AddressType):
-        verifier = SourceVerifier(address, self._client_factory)
+        return self._publish_contract(address)
+
+    def _publish_contract(self, address: AddressType, project: Optional["ProjectManager"] = None):
+        verifier = SourceVerifier(address, self._client_factory, project=project)
         return verifier.attempt_verification()
```

### Comparing `ape-etherscan-0.7.4/ape_etherscan/query.py` & `ape-etherscan-0.8.0/ape_etherscan/query.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from typing import Iterator, Optional
+from collections.abc import Iterator
+from typing import Optional
 
 from ape.api import PluginConfig, QueryAPI, QueryType, ReceiptAPI
 from ape.api.query import AccountTransactionQuery, ContractCreationQuery
 from ape.exceptions import QueryEngineError
 from ape.utils import singledispatchmethod
 
 from ape_etherscan.client import ClientFactory, get_etherscan_api_uri, get_etherscan_uri
```

### Comparing `ape-etherscan-0.7.4/ape_etherscan/types.py` & `ape-etherscan-0.8.0/ape_etherscan/types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import re
 from dataclasses import dataclass
-from typing import Dict, List, Union
+from typing import Union
 
 from ape.utils import cached_property
 from ethpm_types import BaseModel
 from pydantic import Field, field_validator
 
 from ape_etherscan.exceptions import EtherscanResponseError, get_request_error
 
@@ -17,15 +17,15 @@
     ecosystem_name: str
     network_name: str  # normalized (e.g. no -fork)
     uri: str
     api_uri: str
 
 
 class SourceCodeResponse(BaseModel):
-    abi: List = Field([], alias="ABI")
+    abi: list = Field([], alias="ABI")
     name: str = Field("unknown", alias="ContractName")
     source_code: str = Field("", alias="SourceCode")
     compiler_version: str = Field("", alias="CompilerVersion")
     optimization_used: bool = Field(True, alias="OptimizationUsed")
     optimization_runs: int = Field(200, alias="Runs")
     evm_version: str = Field("Default", alias="EVMVersion")
     library: str = Field("", alias="Library")
@@ -63,15 +63,15 @@
 @dataclass
 class ContractCreationResponse:
     contractAddress: str
     contractCreator: str
     txHash: str
 
 
-ResponseValue = Union[List, Dict, str]
+ResponseValue = Union[list, dict, str]
 
 
 class EtherscanResponse:
     def __init__(self, response, ecosystem: str, raise_on_exceptions: bool):
         self.response = response
         self.ecosystem = ecosystem
         self.raise_on_exceptions = raise_on_exceptions
```

### Comparing `ape-etherscan-0.7.4/ape_etherscan/utils.py` & `ape-etherscan-0.8.0/ape_etherscan/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     ],
     "bsc": [
         "mainnet",
         "testnet",
     ],
     "ethereum": [
         "mainnet",
+        "holesky",
         "sepolia",
     ],
     "fantom": [
         "opera",
         "testnet",
     ],
     "gnosis": ["mainnet"],
```

### Comparing `ape-etherscan-0.7.4/ape_etherscan/verify.py` & `ape-etherscan-0.8.0/ape_etherscan/verify.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import json
 import time
 from enum import Enum
 from pathlib import Path
-from typing import Dict, Optional
+from typing import Optional
 
 from ape.api import CompilerAPI
 from ape.contracts import ContractInstance
 from ape.logging import LogLevel, logger
+from ape.managers.project import ProjectManager
 from ape.types import AddressType
 from ape.utils import ManagerAccessMixin, cached_property
 from ethpm_types import Compiler, ContractType
 
 from ape_etherscan.client import AccountClient, ClientFactory, ContractClient
 from ape_etherscan.exceptions import ContractVerificationError, EtherscanResponseError
 
@@ -165,17 +166,23 @@
             return cls(_SPDX_ID_TO_API_CODE[license_id])
 
         logger.warning(f"Unsupported license type '{license_id}'.")
         return cls.NO_LICENSE
 
 
 class SourceVerifier(ManagerAccessMixin):
-    def __init__(self, address: AddressType, client_factory: ClientFactory):
+    def __init__(
+        self,
+        address: AddressType,
+        client_factory: ClientFactory,
+        project: Optional[ProjectManager] = None,
+    ):
         self.address = address
         self.client_factory = client_factory
+        self.project = project or self.local_project
 
     @cached_property
     def account_client(self) -> AccountClient:
         return self.client_factory.get_account_client(str(self.address))
 
     @cached_property
     def contract_client(self) -> ContractClient:
@@ -190,20 +197,16 @@
         return self.contract.contract_type
 
     @property
     def contract_name(self) -> str:
         return self.contract.contract_type.name or ""
 
     @property
-    def _base_path(self) -> Path:
-        return self.project_manager.contracts_folder
-
-    @property
     def source_path(self) -> Path:
-        return self._base_path / (self.contract_type.source_id or "")
+        return self.project.path / (self.contract_type.source_id or "")
 
     @property
     def ext(self) -> str:
         return self.source_path.suffix
 
     @cached_property
     def constructor_arguments(self) -> str:
@@ -238,16 +241,15 @@
             raise ContractVerificationError("Failed to find runtime bytecode.")
 
     @cached_property
     def license_code(self) -> LicenseType:
         """
         The license type used in the code.
         """
-
-        spdx_id = self.source_path.read_text().split("\n")[0]
+        spdx_id = self.source_path.read_text().splitlines()[0]
         return LicenseType.from_spdx_id(spdx_id)
 
     @property
     def compiler_api(self) -> CompilerAPI:
         if compiler := self.compiler_manager.registered_compilers.get(self.ext):
             return compiler
 
@@ -258,25 +260,25 @@
     @cached_property
     def compiler_name(self) -> str:
         return self.compiler_api.name
 
     @property
     def compiler(self) -> Compiler:
         # Check the cached manifest for the compiler artifacts.
-        if manifest := self.project_manager.local_project.cached_manifest:
+        if manifest := self.local_project.manifest:
             if compiler := manifest.get_contract_compiler(self.contract_name):
                 return compiler
 
         # Look in the publishable manifest, as Ape includes these there.
-        manifest = self.project_manager.extract_manifest()
+        manifest = self.local_project.extract_manifest()
         if compiler := manifest.get_contract_compiler(self.contract_name):
             return compiler
 
         # Build a default one and hope for the best.
-        return Compiler(name=self.compiler_name, contractType=[self.contract_name], version=None)
+        return Compiler(name=self.compiler_name, contractType=[self.contract_name], version="")
 
     def attempt_verification(self):
         """
         Attempt to verify the source code.
         If the bytecode is already verified, Etherscan will use the existing bytecode
         and this method will still succeed.
 
@@ -310,16 +312,15 @@
         if not valid:
             settings = self._get_new_settings(version)
 
         optimizer = settings.get("optimizer", {})
         optimized = optimizer.get("enabled", False)
         runs = optimizer.get("runs", DEFAULT_OPTIMIZATION_RUNS)
         source_id = self.contract_type.source_id
-        base_folder = self.project_manager.contracts_folder
-        standard_input_json = self._get_standard_input_json(source_id, base_folder, **settings)
+        standard_input_json = self._get_standard_input_json(source_id, **settings)
         evm_version = settings.get("evmVersion")
         license_code = self.license_code
         license_code_value = license_code.value if license_code else None
 
         if logger.level == LogLevel.DEBUG:
             logger.debug("Dumping standard JSON output:\n")
             standard_json = json.dumps(standard_input_json, indent=2)
@@ -351,47 +352,43 @@
                 return
 
             else:
                 raise  # this error
 
         self._wait_for_verification(guid)
 
-    def _get_new_settings(self, version: str) -> Dict:
+    def _get_new_settings(self, version: str) -> dict:
         logger.warning(
             "Settings missing from cached manifest. " "Attempting to re-calculate find settings."
         )
 
         # Attempt to re-calculate settings.
         compiler_plugin = self.compiler_manager.registered_compilers[self.ext]
         all_settings = compiler_plugin.get_compiler_settings(
-            [self.source_path], base_path=self._base_path
+            [self.source_path], project=self.project
         )
 
         # Hack to allow any Version object work.
         return {str(v): s for v, s in all_settings.items() if str(v) == version}[version]
 
-    def _get_standard_input_json(
-        self, source_id: str, base_folder: Optional[Path] = None, **settings
-    ) -> Dict:
-        base_dir = base_folder or self.project_manager.contracts_folder
-        source_path = base_dir / source_id
+    def _get_standard_input_json(self, source_id: str, **settings) -> dict:
+        source_path = self.local_project.sources.lookup(source_id)
         compiler = self.compiler_manager.registered_compilers[source_path.suffix]
-        sources = {self.source_path.name: {"content": source_path.read_text()}}
+        sources = {source_id: {"content": source_path.read_text()}}
 
         def build_map(_source_id: str):
-            _source_path = base_dir / _source_id
+            _source_path = self.local_project.sources.lookup(_source_id)
             source_imports = compiler.get_imports([_source_path]).get(_source_id, [])
             for imported_source_id in source_imports:
-                sources[imported_source_id] = {
-                    "content": (base_dir / imported_source_id).read_text()
-                }
-                build_map(imported_source_id)
+                if imp_path := self.local_project.sources.lookup(imported_source_id):
+                    sources[imported_source_id] = {"content": imp_path.read_text()}
+                    build_map(imported_source_id)
 
         def flatten_source(_source_id: str) -> str:
-            _source_path = base_dir / _source_id
+            _source_path = self.local_project.sources.lookup(_source_id)
             flattened_source = str(compiler.flatten_contract(_source_path))
             return flattened_source
 
         build_map(source_id)
 
         # "libraries" field not allows in `settings` dict.
         if "libraries" in settings:
```

### Comparing `ape-etherscan-0.7.4/ape_etherscan.egg-info/PKG-INFO` & `ape-etherscan-0.8.0/ape_etherscan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: ape-etherscan
-Version: 0.7.4
+Version: 0.8.0
 Summary: ape-etherscan: Etherscan Explorer Plugin for Ethereum-based networks
 Home-page: https://github.com/ApeWorX/ape-etherscan
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
@@ -41,15 +40,15 @@
 - [Snowtrace](https://snowtrace.io) for Avalanche networks.
 - [Basescan](https://basescan.org) for Base networks.
 - [Bscscan](https://bscscan.com) for Binance-Smart-Chain networks.
 - [Blastscan](https://blastscan.io) for Blast networks.
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.12.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-etherscan-0.7.4/ape_etherscan.egg-info/SOURCES.txt` & `ape-etherscan-0.8.0/ape_etherscan.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 .pre-commit-config.yaml
 CONTRIBUTING.md
 LICENSE
 README.md
+ape-config.yaml
 pyproject.toml
 setup.cfg
 setup.py
 .github/PULL_REQUEST_TEMPLATE.md
 .github/release-drafter.yml
 .github/ISSUE_TEMPLATE/bug.md
 .github/ISSUE_TEMPLATE/feature.md
@@ -38,14 +39,16 @@
 ape_etherscan.egg-info/top_level.txt
 tests/__init__.py
 tests/_utils.py
 tests/conftest.py
 tests/test_config.py
 tests/test_dependency.py
 tests/test_etherscan.py
+tests/contracts/subcontracts/foo.sol
+tests/dependency/contracts/bar.sol
 tests/mock_responses/get_account_transactions.json
 tests/mock_responses/get_account_transactions_with_ctor_args.json
 tests/mock_responses/get_contract_response_flattened.json
 tests/mock_responses/get_contract_response_json.json
 tests/mock_responses/get_contract_response_json_source_code.json
 tests/mock_responses/get_contract_response_not_verified.json
 tests/mock_responses/get_proxy_contract_response.json
```

### Comparing `ape-etherscan-0.7.4/ape_etherscan.egg-info/requires.txt` & `ape-etherscan-0.8.0/ape_etherscan.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-eth-ape<0.8,>=0.7.6
+eth-ape<0.9,>=0.8.2
 ethpm_types
 requests
 yarl
 
 [dev]
 ape-arbitrum
 ape-base
```

### Comparing `ape-etherscan-0.7.4/pyproject.toml` & `ape-etherscan-0.8.0/pyproject.toml`

 * *Files 9% similar despite different names*

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

### Comparing `ape-etherscan-0.7.4/setup.py` & `ape-etherscan-0.8.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,20 +76,20 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-etherscan",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.7.6,<0.8",
+        "eth-ape>=0.8.2,<0.9",
         "ethpm_types",  # Use same version as eth-ape
         "requests",  # Use same version as eth-ape
         "yarl",  # Use same version as eth-ape
     ],
-    python_requires=">=3.8,<4",
+    python_requires=">=3.9,<4",
     extras_require=extras_require,
     py_modules=["ape_etherscan"],
     license="Apache-2.0",
     zip_safe=False,
     keywords="ethereum",
     packages=find_packages(exclude=["tests", "tests.*"]),
     package_data={"ape_etherscan": ["py.typed"]},
@@ -97,14 +97,13 @@
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

### Comparing `ape-etherscan-0.7.4/tests/conftest.py` & `ape-etherscan-0.8.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,97 +1,68 @@
 import json
 import os
-import tempfile
+import shutil
+from collections.abc import Callable
 from contextlib import contextmanager
 from io import StringIO
 from json import JSONDecodeError
 from pathlib import Path
 from tempfile import mkdtemp
-from typing import IO, Any, Callable, Dict, Optional, Union
+from typing import IO, Any, Optional, Union
 from unittest.mock import MagicMock
 
 import _io  # type: ignore
 import ape
 import pytest
-import yaml
 from ape.api import ExplorerAPI
 from ape.exceptions import NetworkError
 from ape.logging import logger
-from ape.managers.config import CONFIG_FILE_NAME
 from ape.types import AddressType
 from ape.utils import cached_property
 from ape_solidity._utils import OUTPUT_SELECTION
 from requests import Response
 
 from ape_etherscan import Etherscan
 from ape_etherscan.client import _APIClient
 from ape_etherscan.types import EtherscanResponse
+from ape_etherscan.verify import LicenseType
 
-ape.config.DATA_FOLDER = Path(mkdtemp()).resolve()
-ape.config.PROJECT_FOLDER = Path(mkdtemp()).resolve()
+DATA_FOLDER = Path(mkdtemp()).resolve()
+ape.config.DATA_FOLDER = DATA_FOLDER
 
-MOCK_RESPONSES_PATH = Path(__file__).parent / "mock_responses"
-FOO_SOURCE_CODE = """
-// SPDX-License-Identifier: AGPL-3.0
-pragma solidity ^0.8.20;
-
-import "@bar/bar.sol";
-
-library MyLib {
-    function insert(uint value) public returns (bool) {
-        return true;
-    }
-}
+HERE = Path(__file__).parent
+MOCK_RESPONSES_PATH = HERE / "mock_responses"
+FOO_SOURCE_CODE = (HERE / "contracts" / "subcontracts" / "foo.sol").read_text()
+BAR_SOURCE_CODE = (HERE / "dependency" / "contracts" / "bar.sol").read_text()
 
-contract foo {
-    function register(uint value) public {
-        require(MyLib.insert(value));
-    }
-}
 
-contract fooWithConstructor {
-    uint public value;
-    constructor(uint _value) {
-        value = _value;
-    }
-}
-"""
-BAR_SOURCE_CODE = r"""
-// SPDX-License-Identifier: AGPL-3.0
-pragma solidity ^0.8.20;
-
-contract bar {
-}
-"""
-APE_CONFIG_FILE = r"""
-dependencies:
-  - name: bar
-    local: ./bar
-
-solidity:
-  import_remapping:
-    - "@bar=bar"
-"""
+@pytest.fixture(scope="session", autouse=True)
+def clean_datafolder():
+    yield  # Run all collected tests.
+    shutil.rmtree(DATA_FOLDER, ignore_errors=True)
 
 
 @pytest.fixture(scope="session")
 def standard_input_json(library):
     return {
         "language": "Solidity",
         "sources": {
-            "foo.sol": {"content": FOO_SOURCE_CODE},
-            ".cache/bar/local/bar.sol": {"content": BAR_SOURCE_CODE},
+            "tests/contracts/.cache/bar/local/contracts/bar.sol": {"content": BAR_SOURCE_CODE},
+            "tests/contracts/subcontracts/foo.sol": {"content": FOO_SOURCE_CODE},
         },
         "settings": {
             "optimizer": {"enabled": True, "runs": 200},
             "outputSelection": {
-                ".cache/bar/local/bar.sol": {"": ["ast"], "*": OUTPUT_SELECTION},
-                "subcontracts/foo.sol": {"": ["ast"], "*": OUTPUT_SELECTION},
+                "tests/contracts/.cache/bar/local/contracts/bar.sol": {
+                    "": ["ast"],
+                    "*": OUTPUT_SELECTION,
+                },
+                "tests/contracts/subcontracts/foo.sol": {"": ["ast"], "*": OUTPUT_SELECTION},
             },
-            "remappings": ["@bar=.cache/bar/local"],
+            "remappings": ["@bar=tests/contracts/.cache/bar/local"],
         },
         "libraryname1": "MyLib",
         "libraryaddress1": library.address,
     }
 
 
 @pytest.fixture(autouse=True)
@@ -125,32 +96,17 @@
 
 def make_source(base_dir: Path, name: str, content: str):
     source_file = base_dir / f"{name}.sol"
     source_file.touch()
     source_file.write_text(content)
 
 
-@pytest.fixture(scope="session", autouse=True)
+@pytest.fixture(scope="session")
 def project():
-    base_dir = ape.config.PROJECT_FOLDER
-    contracts_dir = base_dir / "contracts"
-    dependency_contracts_dir = base_dir / "bar" / "contracts"
-    sub_contracts_dir = contracts_dir / "subcontracts"
-    sub_contracts_dir.mkdir(exist_ok=True, parents=True)
-    dependency_contracts_dir.mkdir(exist_ok=True, parents=True)
-
-    make_source(sub_contracts_dir, "foo", FOO_SOURCE_CODE)
-    make_source(dependency_contracts_dir, "bar", BAR_SOURCE_CODE)
-
-    config_file = base_dir / "ape-config.yaml"
-    config_file.unlink(missing_ok=True)
-    config_file.write_text(APE_CONFIG_FILE)
-
-    with ape.config.using_project(base_dir) as project:
-        yield project
+    return ape.project
 
 
 @pytest.fixture(scope="session")
 def address(contract_to_verify):
     return contract_to_verify.address
 
 
@@ -261,29 +217,30 @@
         self.handlers = {"get": {}, "post": {}}
         self.get_expected_account_txns_params = get_expected_account_txns_params
         self.contract_address_map = contract_address_map
 
     @cached_property
     def expected_uri_map(
         self,
-    ) -> Dict[str, Dict[str, str]]:
+    ) -> dict[str, dict[str, str]]:
         def get_url_f(testnet: bool = False, tld: str = "io"):
             f_str = f"https://api-{{}}.{{}}.{tld}/api" if testnet else f"https://api.{{}}.{tld}/api"
             return f_str.format
 
         url = get_url_f()
         testnet_url = get_url_f(testnet=True)
         com_url = get_url_f(tld="com")
         org_url = get_url_f(tld="org")
         com_testnet_url = get_url_f(testnet=True, tld="com")
         org_testnet_url = get_url_f(testnet=True, tld="org")
 
         return {
             "ethereum": {
                 "mainnet": url("etherscan"),
+                "holesky": testnet_url("holesky", "etherscan"),
                 "sepolia": testnet_url("sepolia", "etherscan"),
             },
             "arbitrum": {
                 "mainnet": url("arbiscan"),
                 "sepolia": testnet_url("sepolia", "arbiscan"),
             },
             "fantom": {
@@ -323,15 +280,15 @@
     def set_network(self, ecosystem: str, network: str):
         self.expected_base_uri = self.expected_uri_map[ecosystem][network.replace("-fork", "")]
 
     def add_handler(
         self,
         method: str,
         module: str,
-        expected_params: Dict,
+        expected_params: dict,
         return_value: Optional[Any] = None,
         side_effect: Optional[Callable] = None,
     ):
         if isinstance(return_value, (str, dict)):
             return_value = self.get_mock_response(return_value)
 
         def handler(self, method, base_uri, params=None, data=None, headers=None):
@@ -439,15 +396,15 @@
             content = (
                 MOCK_RESPONSES_PATH / "get_contract_response_json_source_code.json"
             ).read_text()
             data = json.loads(test_data_path.read_text())
             data["SourceCode"] = content
             return self.get_mock_response(data, file_name=file_name)
 
-    def _expected_get_ct_params(self, address: str) -> Dict:
+    def _expected_get_ct_params(self, address: str) -> dict:
         return {"module": "contract", "action": "getsourcecode", "address": address}
 
     def setup_mock_account_transactions_response(self, address: AddressType, **overrides):
         file_name = "get_account_transactions.json"
         test_data_path = MOCK_RESPONSES_PATH / file_name
         params = self.get_expected_account_txns_params(address)
         params["address"] = address
@@ -476,15 +433,15 @@
 
     def _setup_account_response(self, params, response):
         self.add_handler("GET", "account", params, return_value=response)
         self.set_network("ethereum", "mainnet")
         return response
 
     def get_mock_response(
-        self, response_data: Optional[Union[IO, Dict, str, MagicMock]] = None, **kwargs
+        self, response_data: Optional[Union[IO, dict, str, MagicMock]] = None, **kwargs
     ):
         if isinstance(response_data, str):
             return self.get_mock_response({"result": response_data, **kwargs})
 
         elif isinstance(response_data, _io.TextIOWrapper):
             return self.get_mock_response(json.load(response_data), **kwargs)
 
@@ -493,23 +450,23 @@
             response_data = {**kwargs}
 
         assert isinstance(response_data, dict)
         return self._get_mock_response(response_data=response_data, **kwargs)
 
     def _get_mock_response(
         self,
-        response_data: Optional[Dict] = None,
+        response_data: Optional[dict] = None,
         response_text: Optional[str] = None,
         *args,
         **kwargs,
     ):
         response = self.mocker.MagicMock(spec=Response)
         if response_data:
             assert isinstance(response_data, dict)  # For mypy
-            overrides: Dict = kwargs.get("response_overrides", {})
+            overrides: dict = kwargs.get("response_overrides", {})
             response.json.return_value = {**response_data, **overrides}
             if not response_text:
                 response_text = json.dumps(response_data or {})
 
         if response_text:
             response.text = response_text
 
@@ -527,15 +484,15 @@
     return {
         "action": "verifysourcecode",
         "codeformat": "solidity-standard-json-input",
         "constructorArguements": ctor_args,
         "contractaddress": address_to_verify,
         "contractname": "foo.sol:foo",
         "evmversion": None,
-        "licenseType": 1,
+        "licenseType": LicenseType.AGLP_3.value,
         "module": "contract",
         "optimizationUsed": 1,
         "runs": 200,
         "sourceCode": StringIO(json.dumps(standard_input_json)),
     }
 
 
@@ -555,15 +512,15 @@
     return {
         "action": "verifysourcecode",
         "codeformat": "solidity-standard-json-input",
         "constructorArguements": constructor_arguments,
         "contractaddress": address_to_verify_with_ctor_args,
         "contractname": "foo.sol:fooWithConstructor",
         "evmversion": None,
-        "licenseType": 1,
+        "licenseType": LicenseType.AGLP_3.value,
         "module": "contract",
         "optimizationUsed": 1,
         "runs": 200,
         "sourceCode": StringIO(json.dumps(json_data)),
     }
 
 
@@ -626,35 +583,7 @@
 
 @pytest.fixture(scope="session")
 def expected_verification_log_with_ctor_args(address_to_verify_with_ctor_args):
     return (
         "Contract verification successful!\n"
         f"https://etherscan.io/address/{address_to_verify_with_ctor_args}#code"
     )
-
-
-@pytest.fixture(scope="session")
-def temp_config():
-    config = ape.config
-
-    @contextmanager
-    def func(data: Dict, package_json: Optional[Dict] = None):
-        with tempfile.TemporaryDirectory() as temp_dir_str:
-            temp_dir = Path(temp_dir_str)
-
-            config._cached_configs = {}
-            config_file = temp_dir / CONFIG_FILE_NAME
-            config_file.touch()
-            config_file.write_text(yaml.dump(data))
-            config.load(force_reload=True)
-
-            if package_json:
-                package_json_file = temp_dir / "package.json"
-                package_json_file.write_text(json.dumps(package_json))
-
-            with config.using_project(temp_dir):
-                yield temp_dir
-
-            config_file.unlink()
-            config._cached_configs = {}
-
-    return func
```

### Comparing `ape-etherscan-0.7.4/tests/mock_responses/get_account_transactions.json` & `ape-etherscan-0.8.0/tests/mock_responses/get_account_transactions.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/tests/mock_responses/get_account_transactions_with_ctor_args.json` & `ape-etherscan-0.8.0/tests/mock_responses/get_account_transactions_with_ctor_args.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/tests/mock_responses/get_contract_response_flattened.json` & `ape-etherscan-0.8.0/tests/mock_responses/get_contract_response_flattened.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/tests/mock_responses/get_contract_response_json.json` & `ape-etherscan-0.8.0/tests/mock_responses/get_contract_response_json.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/tests/mock_responses/get_contract_response_json_source_code.json` & `ape-etherscan-0.8.0/tests/mock_responses/get_contract_response_json_source_code.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/tests/mock_responses/get_proxy_contract_response.json` & `ape-etherscan-0.8.0/tests/mock_responses/get_proxy_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/tests/mock_responses/get_vyper_contract_response.json` & `ape-etherscan-0.8.0/tests/mock_responses/get_vyper_contract_response.json`

 * *Files identical despite different names*

### Comparing `ape-etherscan-0.7.4/tests/test_config.py` & `ape-etherscan-0.8.0/tests/test_config.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,75 +3,61 @@
 from ._utils import ecosystems_and_networks
 
 network_ecosystems = pytest.mark.parametrize(
     "ecosystem,network",
     ecosystems_and_networks,
 )
 
-DEFAULT_CONFIG = {"name": "ape-etherscan-test"}
-
 
 @network_ecosystems
-def test_no_config(account, ecosystem, network, get_explorer, temp_config):
+def test_no_config(account, ecosystem, network, get_explorer, project):
     """Test default behavior"""
-    conf = DEFAULT_CONFIG
-    with temp_config(conf):
+    with project.temp_config(name="ape-etherscan-test"):
         explorer = get_explorer(ecosystem, network)
         assert explorer.network.name == network
         assert explorer.network.ecosystem.name == ecosystem
         assert account.query_manager.engines["etherscan"].rate_limit == 5
 
-        client = account.query_manager.engines["etherscan"]._client_factory.get_account_client(
-            account
-        )
+        engine = account.query_manager.engines["etherscan"]
+        client = engine._client_factory.get_account_client(account)
         assert client._retries == 5
 
 
-def test_config_rate_limit(account, get_explorer, temp_config):
+def test_config_rate_limit(account, project):
     """Test that rate limit config is set"""
-    conf = {**DEFAULT_CONFIG, **{"etherscan": {"ethereum": {"rate_limit": 123}}}}
-    with temp_config(conf):
-        assert account.query_manager.engines["etherscan"].rate_limit == 123
+    with project.temp_config(etherscan={"ethereum": {"rate_limit": 123}}):
+        engine = account.query_manager.engines["etherscan"]
+        assert engine.rate_limit == 123
 
 
-def test_config_retries(account, get_explorer, temp_config):
+def test_config_retries(account, project):
     """Test that rate limit config is set"""
-    conf = {**DEFAULT_CONFIG, **{"etherscan": {"ethereum": {"retries": 321}}}}
-    with temp_config(conf):
-        assert account.query_manager.engines["etherscan"].rate_limit == 5
-        client = account.query_manager.engines["etherscan"]._client_factory.get_account_client(
-            account
-        )
+    with project.temp_config(etherscan={"ethereum": {"retries": 321}}):
+        engine = account.query_manager.engines["etherscan"]
+        assert engine.rate_limit == 5
+        client = engine._client_factory.get_account_client(account)
         assert client._retries == 321
 
 
-def test_config_uri(account, get_explorer, mock_provider, temp_config):
+def test_config_uri(account, mock_provider, project):
     """
     Make sure URI parameter is used when configured
     """
     expected_uri = "https://monke.chain/"
     expected_api_uri = "https://api.monke.chain/api"
-    custon_network_name = "monkechain"
-    conf = {
-        **DEFAULT_CONFIG,
-        **{
-            "networks": {
-                "custom": [
-                    {"name": custon_network_name, "chain_id": 31337, "ecosystem": "ethereum"}
-                ]
-            },
-            "etherscan": {
-                "ethereum": {
-                    custon_network_name: {"uri": expected_uri, "api_uri": expected_api_uri}
-                }
-            },
-        },
+    custom_network_name = "monkechain"
+    networks_conf = (
+        {"custom": [{"name": custom_network_name, "chain_id": 31337, "ecosystem": "ethereum"}]},
+    )
+
+    explorer_confg = {
+        "ethereum": {custom_network_name: {"uri": expected_uri, "api_uri": expected_api_uri}}
     }
 
-    with temp_config(conf):
+    with project.temp_config(networks=networks_conf, etherscan=explorer_confg):
         with mock_provider("ethereum", "monkechain"):
             assert account.query_manager.engines["etherscan"].etherscan_uri == expected_uri
             assert account.query_manager.engines["etherscan"].etherscan_api_uri == expected_api_uri
             account_client = account.query_manager.engines[
                 "etherscan"
             ]._client_factory.get_account_client(account)
             assert account_client.base_uri == expected_api_uri
```

### Comparing `ape-etherscan-0.7.4/tests/test_etherscan.py` & `ape-etherscan-0.8.0/tests/test_etherscan.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable
+from collections.abc import Callable
 
 import pytest
 from ape.api.query import AccountTransactionQuery
 
 from ape_etherscan.exceptions import EtherscanResponseError, EtherscanTooManyRequestsError
 
 from ._utils import ecosystems_and_networks
@@ -21,14 +21,16 @@
 base_url_test = pytest.mark.parametrize(
     "ecosystem,network,url",
     [
         ("ethereum", "mainnet", "etherscan.io"),
         ("ethereum", "mainnet-fork", "etherscan.io"),
         ("ethereum", "sepolia", "sepolia.etherscan.io"),
         ("ethereum", "sepolia-fork", "sepolia.etherscan.io"),
+        ("ethereum", "holesky", "holesky.etherscan.io"),
+        ("ethereum", "holesky-fork", "holesky.etherscan.io"),
         ("fantom", "opera", "ftmscan.com"),
         ("fantom", "opera-fork", "ftmscan.com"),
         ("fantom", "testnet", "testnet.ftmscan.com"),
         ("fantom", "testnet-fork", "testnet.ftmscan.com"),
         ("arbitrum", "mainnet", "arbiscan.io"),
         ("arbitrum", "mainnet-fork", "arbiscan.io"),
         ("arbitrum", "sepolia", "sepolia.arbiscan.io"),
```

