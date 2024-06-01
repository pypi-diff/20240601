# Comparing `tmp/eth-ape-0.8.1.tar.gz` & `tmp/eth-ape-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-ape-0.8.1.tar", last modified: Fri May 31 18:45:26 2024, max compression
+gzip compressed data, was "eth-ape-0.8.2.tar", last modified: Sat Jun  1 04:04:20 2024, max compression
```

## Comparing `eth-ape-0.8.1.tar` & `eth-ape-0.8.2.tar`

### file list

```diff
@@ -1,529 +1,529 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.552713 eth-ape-0.8.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.552713 eth-ape-0.8.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.552713 eth-ape-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.github/workflows/docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      405 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.github/workflows/stale-prs.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-31 18:44:32.000000 eth-ape-0.8.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-31 18:44:32.000000 eth-ape-0.8.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-31 18:44:32.000000 eth-ape-0.8.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-05-31 18:44:32.000000 eth-ape-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-05-31 18:45:26.612713 eth-ape-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-31 18:44:32.000000 eth-ape-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-05-31 18:44:32.000000 eth-ape-0.8.1/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-05-31 18:44:32.000000 eth-ape-0.8.1/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-31 18:44:32.000000 eth-ape-0.8.1/codeql-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-31 18:44:32.000000 eth-ape-0.8.1/cz-requirement.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.552713 eth-ape-0.8.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.552713 eth-ape-0.8.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/_static/custom.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.552713 eth-ape-0.8.1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/_templates/layout.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.556713 eth-ape-0.8.1/docs/commands/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/commands/accounts.rst
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/commands/compile.rst
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/commands/console.rst
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/commands/init.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/commands/networks.rst
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/commands/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/commands/pm.rst
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/commands/run.rst
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/commands/test.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/logo.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.556713 eth-ape-0.8.1/docs/methoddocs/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/methoddocs/ape.md
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/methoddocs/ape_accounts.md
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/methoddocs/ape_compile.md
--rw-r--r--   0 runner    (1001) docker     (127)      220 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/methoddocs/ape_ethereum.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/methoddocs/ape_node.md
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/methoddocs/ape_pm.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/methoddocs/ape_test.md
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/methoddocs/api.md
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/methoddocs/cli.md
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/methoddocs/contracts.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/methoddocs/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/methoddocs/managers.md
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/methoddocs/plugins.md
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/methoddocs/types.md
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/methoddocs/utils.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.560713 eth-ape-0.8.1/docs/userguides/
--rw-r--r--   0 runner    (1001) docker     (127)    13411 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/accounts.md
--rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/clis.md
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/compile.md
--rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/config.md
--rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/console.md
--rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/contracts.md
--rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/data.md
--rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/dependencies.md
--rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/developing_plugins.md
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/forking_networks.md
--rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/installing_plugins.md
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/logging.md
--rw-r--r--   0 runner    (1001) docker     (127)    21459 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/networks.md
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/projects.md
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/proxy.md
--rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/publishing.md
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/quickstart.md
--rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/scripts.md
--rw-r--r--   0 runner    (1001) docker     (127)    25002 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/testing.md
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/trace.md
--rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-05-31 18:44:32.000000 eth-ape-0.8.1/docs/userguides/transactions.md
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-05-31 18:44:32.000000 eth-ape-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-31 18:44:32.000000 eth-ape-0.8.1/recommended-plugins.txt
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-31 18:45:26.616713 eth-ape-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-31 18:44:32.000000 eth-ape-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.540713 eth-ape-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.560713 eth-ape-0.8.1/src/ape/
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.564713 eth-ape-0.8.1/src/ape/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23416 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/api/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/api/address.py
--rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/api/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    15543 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/api/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/api/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/api/explorers.py
--rw-r--r--   0 runner    (1001) docker     (127)    43420 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/api/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/api/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)    39205 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/api/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     8089 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/api/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/api/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    19353 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/api/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.564713 eth-ape-0.8.1/src/ape/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/cli/arguments.py
--rw-r--r--   0 runner    (1001) docker     (127)    13618 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/cli/choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/cli/commands.py
--rw-r--r--   0 runner    (1001) docker     (127)    16844 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/cli/options.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/cli/paramtype.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.564713 eth-ape-0.8.1/src/ape/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      230 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55095 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/contracts/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26911 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/harambe.py
--rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.568713 eth-ape-0.8.1/src/ape/managers/
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/managers/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/managers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    61607 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/managers/chain.py
--rw-r--r--   0 runner    (1001) docker     (127)    14025 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/managers/compilers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/managers/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15741 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/managers/converters.py
--rw-r--r--   0 runner    (1001) docker     (127)    23385 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/managers/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/managers/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    81435 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/managers/project.py
--rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/managers/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.568713 eth-ape-0.8.1/src/ape/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    20704 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/plugins/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/plugins/account.py
--rw-r--r--   0 runner    (1001) docker     (127)      884 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/plugins/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/plugins/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/plugins/converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/plugins/network.py
--rw-r--r--   0 runner    (1001) docker     (127)      779 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/plugins/pluggy_patch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/plugins/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/plugins/query.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.568713 eth-ape-0.8.1/src/ape/pytest/
--rw-r--r--   0 runner    (1001) docker     (127)      550 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/pytest/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/pytest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/pytest/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/pytest/contextmanagers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12038 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/pytest/coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/pytest/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/pytest/gas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/pytest/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/pytest/runners.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.568713 eth-ape-0.8.1/src/ape/types/
--rw-r--r--   0 runner    (1001) docker     (127)    15857 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/types/address.py
--rw-r--r--   0 runner    (1001) docker     (127)    36405 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/types/coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/types/signatures.py
--rw-r--r--   0 runner    (1001) docker     (127)    17389 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/types/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.572713 eth-ape-0.8.1/src/ape/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/utils/_github.py
--rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/utils/abi.py
--rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/utils/basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)    16057 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8645 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/utils/os.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/utils/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/utils/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape/utils/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-31 18:45:26.000000 eth-ape-0.8.1/src/ape/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.572713 eth-ape-0.8.1/src/ape_accounts/
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_accounts/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_accounts/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_accounts/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.572713 eth-ape-0.8.1/src/ape_cache/
--rw-r--r--   0 runner    (1001) docker     (127)      375 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_cache/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_cache/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    17976 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_cache/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.572713 eth-ape-0.8.1/src/ape_compile/
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_compile/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_compile/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_compile/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.572713 eth-ape-0.8.1/src/ape_console/
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_console/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_console/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_console/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_console/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.576713 eth-ape-0.8.1/src/ape_ethereum/
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_ethereum/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   152476 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_ethereum/_console_log_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_ethereum/_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_ethereum/_print.py
--rw-r--r--   0 runner    (1001) docker     (127)    51598 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_ethereum/ecosystem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.576713 eth-ape-0.8.1/src/ape_ethereum/multicall/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_ethereum/multicall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_ethereum/multicall/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_ethereum/multicall/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_ethereum/multicall/handlers.py
--rw-r--r--   0 runner    (1001) docker     (127)    51957 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_ethereum/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_ethereum/proxies.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_ethereum/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_ethereum/query.py
--rw-r--r--   0 runner    (1001) docker     (127)    23875 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_ethereum/trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_ethereum/transactions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.576713 eth-ape-0.8.1/src/ape_init/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_init/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.576713 eth-ape-0.8.1/src/ape_networks/
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_networks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_networks/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.576713 eth-ape-0.8.1/src/ape_node/
--rw-r--r--   0 runner    (1001) docker     (127)      792 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_node/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_node/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_node/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.576713 eth-ape-0.8.1/src/ape_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_plugins/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.580713 eth-ape-0.8.1/src/ape_pm/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_pm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_pm/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_pm/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_pm/dependency.py
--rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_pm/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_pm/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.580713 eth-ape-0.8.1/src/ape_run/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_run/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_run/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.580713 eth-ape-0.8.1/src/ape_test/
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_test/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_test/accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_test/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/src/ape_test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.580713 eth-ape-0.8.1/src/eth_ape.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-05-31 18:45:26.000000 eth-ape-0.8.1/src/eth_ape.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    16815 2024-05-31 18:45:26.000000 eth-ape-0.8.1/src/eth_ape.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:45:26.000000 eth-ape-0.8.1/src/eth_ape.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-31 18:45:26.000000 eth-ape-0.8.1/src/eth_ape.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:45:26.000000 eth-ape-0.8.1/src/eth_ape.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-31 18:45:26.000000 eth-ape-0.8.1/src/eth_ape.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-31 18:45:26.000000 eth-ape-0.8.1/src/eth_ape.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.580713 eth-ape-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17283 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.588713 eth-ape-0.8.1/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28183 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.588713 eth-ape-0.8.1/tests/functional/conversion/
--rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/conversion/test_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/conversion/test_decimal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/conversion/test_encode_structs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/conversion/test_ether.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/conversion/test_hex.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/conversion/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/conversion/test_timestamp.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.588713 eth-ape-0.8.1/tests/functional/data/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.544713 eth-ape-0.8.1/tests/functional/data/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.544713 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.588713 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/abi/
--rw-r--r--   0 runner    (1001) docker     (127)    13727 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/abi/contract_abi.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.592713 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/
--rw-r--r--   0 runner    (1001) docker     (127)    26703 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/BeaconProxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    77599 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/ContractA.json
--rw-r--r--   0 runner    (1001) docker     (127)    75147 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/ContractB.json
--rw-r--r--   0 runner    (1001) docker     (127)    32313 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/ContractC.json
--rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/DsNoteTest.json
--rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/HasError.json
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/Interface.json
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/InterfaceImplementation.json
--rw-r--r--   0 runner    (1001) docker     (127)    46986 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/RevertsContract.json
--rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/SolFallbackAndReceive.json
--rw-r--r--   0 runner    (1001) docker     (127)   240439 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/SolidityContract.json
--rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/SubReverts.json
--rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/VyDefault.json
--rw-r--r--   0 runner    (1001) docker     (127)   251475 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/VyperContract.json
--rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/VyperFactory.json
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/beacon.json
--rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/eip1967.json
--rw-r--r--   0 runner    (1001) docker     (127)    13901 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/printing.json
--rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/proxy.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.544713 eth-ape-0.8.1/tests/functional/data/manifests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.544713 eth-ape-0.8.1/tests/functional/data/manifests/openzeppelin/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.592713 eth-ape-0.8.1/tests/functional/data/manifests/openzeppelin/3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)  1733602 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/manifests/openzeppelin/3.1.0/openzeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.592713 eth-ape-0.8.1/tests/functional/data/manifests/openzeppelin/4.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)  1733602 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/manifests/openzeppelin/4.4.2/openzeppelin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.544713 eth-ape-0.8.1/tests/functional/data/projects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.596713 eth-ape-0.8.1/tests/functional/data/projects/ApeProject/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/projects/ApeProject/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.596713 eth-ape-0.8.1/tests/functional/data/projects/ApeProject/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/projects/ApeProject/contracts/ApeContract0.json
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/projects/ApeProject/contracts/ApeContract1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/projects/ApeProject/contracts/Contract.json
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/projects/ApeProject/contracts/Exclude.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.596713 eth-ape-0.8.1/tests/functional/data/projects/ApeProject/contracts/subdir/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/projects/ApeProject/contracts/subdir/ApeContractNested.json
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/projects/ApeProject/contracts/subdir/ExcludeNested.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.596713 eth-ape-0.8.1/tests/functional/data/projects/BrownieProject/
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/projects/BrownieProject/brownie-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.596713 eth-ape-0.8.1/tests/functional/data/projects/BrownieProject/contractsrenamed/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/projects/BrownieProject/contractsrenamed/brownie.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.544713 eth-ape-0.8.1/tests/functional/data/projects/LongContractsFolder/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.544713 eth-ape-0.8.1/tests/functional/data/projects/LongContractsFolder/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.596713 eth-ape-0.8.1/tests/functional/data/projects/LongContractsFolder/source/v0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/projects/LongContractsFolder/source/v0.1/long_contracts_folder.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.596713 eth-ape-0.8.1/tests/functional/data/python/
--rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/python/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.600713 eth-ape-0.8.1/tests/functional/data/sources/
--rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/sources/ContractA.sol
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/sources/ContractB.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/sources/ContractC.sol
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/sources/HasError.sol
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/sources/Proxy.sol
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/sources/RevertsContract.vy
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/sources/SolFallbackAndReceive.sol
--rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/sources/SolidityContract.sol
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/sources/SubRevertsVy.vy
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/sources/VyDefault.vy
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/sources/VyperContract.vy
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/sources/VyperFactory.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.600713 eth-ape-0.8.1/tests/functional/data/sources/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/data/sources/interfaces/ISubReverts.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.600713 eth-ape-0.8.1/tests/functional/geth/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/geth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/geth/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/geth/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/geth/test_contract_event.py
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/geth/test_ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (127)      863 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/geth/test_gas_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/geth/test_network_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    18683 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/geth/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/geth/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/geth/test_receipt.py
--rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/geth/test_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/geth/text_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)    32503 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      751 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_base_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_block.py
--rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_block_container.py
--rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_chain.py
--rw-r--r--   0 runner    (1001) docker     (127)    27423 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6201 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_compilers.py
--rw-r--r--   0 runner    (1001) docker     (127)    10216 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_console.py
--rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_contract_call_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_contract_container.py
--rw-r--r--   0 runner    (1001) docker     (127)    13366 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_contract_event.py
--rw-r--r--   0 runner    (1001) docker     (127)    32749 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_contract_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_contract_method_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)    14951 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_contracts_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     5738 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_coverage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_default_sender_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    17404 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    65316 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_ecosystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_gas_tracker.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_multicall.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_network_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_network_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_project.py
--rw-r--r--   0 runner    (1001) docker     (127)    17323 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_proxy.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_receipt.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_receipt_capture.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_reverts_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_trace.py
--rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/test_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.600713 eth-ape-0.8.1/tests/functional/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/utils/test_abi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/utils/test_basemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/utils/test_github.py
--rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/functional/utils/test_os.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.600713 eth-ape-0.8.1/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.604713 eth-ape-0.8.1/tests/integration/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.548713 eth-ape-0.8.1/tests/integration/cli/projects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.544713 eth-ape-0.8.1/tests/integration/cli/projects/bad-contracts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.604713 eth-ape-0.8.1/tests/integration/cli/projects/bad-contracts/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/bad-contracts/contracts/Contract.test
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/bad-contracts/contracts/Contract2.foo
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/bad-contracts/contracts/doc.md
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/bad-contracts/contracts/file_without_ext
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/bad-contracts/contracts/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.604713 eth-ape-0.8.1/tests/integration/cli/projects/bad-contracts/contracts/subdir/
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/bad-contracts/contracts/subdir/tsconfig.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.604713 eth-ape-0.8.1/tests/integration/cli/projects/bad-contracts/contracts/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/bad-contracts/contracts/tests/TestContract.foobar
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.604713 eth-ape-0.8.1/tests/integration/cli/projects/empty-config/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/empty-config/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.604713 eth-ape-0.8.1/tests/integration/cli/projects/geth/
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/geth/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.604713 eth-ape-0.8.1/tests/integration/cli/projects/geth/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/geth/contracts/TokenA.json
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/geth/contracts/TokenB.json
--rw-r--r--   0 runner    (1001) docker     (127)    28131 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/geth/contracts/VyperContract.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.604713 eth-ape-0.8.1/tests/integration/cli/projects/geth/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/geth/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/geth/tests/test_using_local_geth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.544713 eth-ape-0.8.1/tests/integration/cli/projects/multiple-interfaces/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.608713 eth-ape-0.8.1/tests/integration/cli/projects/multiple-interfaces/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/multiple-interfaces/contracts/Interface-with-hyphens.json
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/multiple-interfaces/contracts/Interface.exclude.json
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/multiple-interfaces/contracts/Interface.json
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/multiple-interfaces/contracts/InterfaceWithNumber123.json
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/multiple-interfaces/contracts/Interface_with_underscores.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.608713 eth-ape-0.8.1/tests/integration/cli/projects/no-config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/no-config/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.608713 eth-ape-0.8.1/tests/integration/cli/projects/only-dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/only-dependencies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/only-dependencies/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.608713 eth-ape-0.8.1/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/importme.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.608713 eth-ape-0.8.1/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/sources/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/sources/DependencyInProjectOnly.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.544713 eth-ape-0.8.1/tests/integration/cli/projects/only-script-subdirs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.544713 eth-ape-0.8.1/tests/integration/cli/projects/only-script-subdirs/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.608713 eth-ape-0.8.1/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/subdirectory_click_print.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/subdirectory_main_print.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.544713 eth-ape-0.8.1/tests/integration/cli/projects/script/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.608713 eth-ape-0.8.1/tests/integration/cli/projects/script/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)    28131 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/script/contracts/VyperContract.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.608713 eth-ape-0.8.1/tests/integration/cli/projects/script/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/script/scripts/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/script/scripts/click.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/script/scripts/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/script/scripts/error_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/script/scripts/error_forgot_click.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/script/scripts/error_main.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/script/scripts/error_no_def.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/script/scripts/output_contract_view_methods.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/script/scripts/site.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.608713 eth-ape-0.8.1/tests/integration/cli/projects/script/scripts/subdirectory/
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/script/scripts/subdirectory/subdirectory_click_print.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/script/scripts/subdirectory/subdirectory_main_print.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.608713 eth-ape-0.8.1/tests/integration/cli/projects/test/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/test/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.608713 eth-ape-0.8.1/tests/integration/cli/projects/test/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/test/tests/test_fixture_isolation.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/test/tests/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/test/tests/test_networks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.608713 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/contracts/ContractA.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/contracts/DirectoryWithJSONExtension.json/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/contracts/DirectoryWithJSONExtension.json/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/contracts/Exclude.json
--rw-r--r--   0 runner    (1001) docker     (127)    41634 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/contracts/RawSolidityOutput.json
--rw-r--r--   0 runner    (1001) docker     (127)    64327 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/contracts/RawVyperOutput.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/contracts/exclude_dir/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/contracts/exclude_dir/UnwantedContract.json
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/contracts/hyphen-Contract.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.548713 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/dep/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/dep/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)    64326 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/dep/contracts/RawVyperOutputDep.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/dep_contracts_folder_root/
--rw-r--r--   0 runner    (1001) docker     (127)    64326 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/dep_contracts_folder_root/RawVyperOutputDepNoContractsFolder.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/scripts/txerr.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/tests/test_contract.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/contracts/containing_sub_dependencies.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.548713 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/contracts/sub-dependency.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/contracts/Other.json
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/contracts/Project.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.548713 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/default/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/default/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/default/contracts/default.json
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/default/contracts/hyphen-DependencyContract.json
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/manifest_dependency.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.548713 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.548713 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.548713 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/v0.1/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/v0.1/renamed_complex_contracts_folder.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.548713 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/sources/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/sources/renamed_contracts_folder.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:45:26.612713 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/my_contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/my_contracts/renamed_contracts_folder_specified_in_config.json
--rw-r--r--   0 runner    (1001) docker     (127)    12497 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/test_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)    13398 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/test_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/test_console.py
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/test_init.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/test_networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/test_pm.py
--rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/test_run.py
--rw-r--r--   0 runner    (1001) docker     (127)    13531 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/test_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-05-31 18:44:32.000000 eth-ape-0.8.1/tests/integration/cli/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.440991 eth-ape-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.380990 eth-ape-0.8.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.380990 eth-ape-0.8.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      526 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.380990 eth-ape-0.8.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.github/workflows/docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.github/workflows/stale-prs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3007 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2121 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-06-01 04:03:21.000000 eth-ape-0.8.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-06-01 04:03:21.000000 eth-ape-0.8.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-06-01 04:03:21.000000 eth-ape-0.8.2/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-06-01 04:03:21.000000 eth-ape-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-06-01 04:04:20.440991 eth-ape-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-06-01 04:03:21.000000 eth-ape-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-06-01 04:03:21.000000 eth-ape-0.8.2/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2515 2024-06-01 04:03:21.000000 eth-ape-0.8.2/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-01 04:03:21.000000 eth-ape-0.8.2/codeql-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-06-01 04:03:21.000000 eth-ape-0.8.2/cz-requirement.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.380990 eth-ape-0.8.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.380990 eth-ape-0.8.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/_static/custom.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.380990 eth-ape-0.8.2/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    10136 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/_templates/layout.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.384991 eth-ape-0.8.2/docs/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/commands/accounts.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/commands/compile.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/commands/console.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/commands/init.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/commands/networks.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/commands/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/commands/pm.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/commands/run.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/commands/test.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4432 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20915 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11889 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/logo.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.384991 eth-ape-0.8.2/docs/methoddocs/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/methoddocs/ape.md
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/methoddocs/ape_accounts.md
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/methoddocs/ape_compile.md
+-rw-r--r--   0 runner    (1001) docker     (127)      220 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/methoddocs/ape_ethereum.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/methoddocs/ape_node.md
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/methoddocs/ape_pm.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/methoddocs/ape_test.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/methoddocs/api.md
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/methoddocs/cli.md
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/methoddocs/contracts.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/methoddocs/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/methoddocs/managers.md
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/methoddocs/plugins.md
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/methoddocs/types.md
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/methoddocs/utils.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.388990 eth-ape-0.8.2/docs/userguides/
+-rw-r--r--   0 runner    (1001) docker     (127)    13411 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/accounts.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8866 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/clis.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/compile.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4671 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/config.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5938 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/console.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16302 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/contracts.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/data.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10220 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/dependencies.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6944 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/developing_plugins.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/forking_networks.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2845 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/installing_plugins.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/logging.md
+-rw-r--r--   0 runner    (1001) docker     (127)    21459 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/networks.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/projects.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/proxy.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2132 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/publishing.md
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/quickstart.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5251 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/scripts.md
+-rw-r--r--   0 runner    (1001) docker     (127)    25002 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/testing.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/trace.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-06-01 04:03:21.000000 eth-ape-0.8.2/docs/userguides/transactions.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-06-01 04:03:21.000000 eth-ape-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-06-01 04:03:21.000000 eth-ape-0.8.2/recommended-plugins.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-06-01 04:04:20.440991 eth-ape-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-06-01 04:03:21.000000 eth-ape-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.372990 eth-ape-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.388990 eth-ape-0.8.2/src/ape/
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5640 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.388990 eth-ape-0.8.2/src/ape/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23416 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/api/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6501 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/api/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10519 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/api/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15710 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/api/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/api/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/api/explorers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43420 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/api/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39205 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/api/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8089 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/api/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/api/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19353 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/api/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.392991 eth-ape-0.8.2/src/ape/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6107 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/cli/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13618 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/cli/choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5014 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/cli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16844 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/cli/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/cli/paramtype.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.392991 eth-ape-0.8.2/src/ape/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55095 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/contracts/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26911 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/harambe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9254 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.392991 eth-ape-0.8.2/src/ape/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13025 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/managers/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/managers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61607 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/managers/chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14025 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/managers/compilers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5130 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/managers/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15741 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/managers/converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23385 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/managers/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5636 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/managers/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81435 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/managers/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7596 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/managers/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.396991 eth-ape-0.8.2/src/ape/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20704 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/plugins/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/plugins/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      884 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/plugins/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/plugins/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/plugins/converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/plugins/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)      779 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/plugins/pluggy_patch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/plugins/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/plugins/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.396991 eth-ape-0.8.2/src/ape/pytest/
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/pytest/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/pytest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/pytest/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/pytest/contextmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12517 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/pytest/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8163 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/pytest/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/pytest/gas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4586 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/pytest/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10697 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/pytest/runners.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.396991 eth-ape-0.8.2/src/ape/types/
+-rw-r--r--   0 runner    (1001) docker     (127)    15857 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/types/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36405 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/types/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/types/signatures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17389 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/types/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.396991 eth-ape-0.8.2/src/ape/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     3367 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7947 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/utils/_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18563 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/utils/abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16143 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/utils/basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16057 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8645 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/utils/os.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/utils/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8187 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/utils/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape/utils/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-01 04:04:19.000000 eth-ape-0.8.2/src/ape/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.400991 eth-ape-0.8.2/src/ape_accounts/
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_accounts/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13258 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_accounts/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_accounts/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.400991 eth-ape-0.8.2/src/ape_cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      375 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_cache/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_cache/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17976 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_cache/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.400991 eth-ape-0.8.2/src/ape_compile/
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_compile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3914 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_compile/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_compile/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.400991 eth-ape-0.8.2/src/ape_console/
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_console/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5515 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_console/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_console/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_console/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.400991 eth-ape-0.8.2/src/ape_ethereum/
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_ethereum/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   152476 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_ethereum/_console_log_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_ethereum/_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3917 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_ethereum/_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51598 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_ethereum/ecosystem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.404991 eth-ape-0.8.2/src/ape_ethereum/multicall/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_ethereum/multicall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10277 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_ethereum/multicall/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_ethereum/multicall/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10396 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_ethereum/multicall/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51957 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_ethereum/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_ethereum/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_ethereum/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_ethereum/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23875 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_ethereum/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15635 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_ethereum/transactions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.404991 eth-ape-0.8.2/src/ape_init/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_init/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.404991 eth-ape-0.8.2/src/ape_networks/
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_networks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_networks/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.404991 eth-ape-0.8.2/src/ape_node/
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_node/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13503 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_node/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_node/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_node/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.404991 eth-ape-0.8.2/src/ape_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9386 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_plugins/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.404991 eth-ape-0.8.2/src/ape_pm/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_pm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10087 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_pm/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5639 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_pm/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10239 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_pm/dependency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3861 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_pm/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_pm/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.404991 eth-ape-0.8.2/src/ape_run/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9853 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_run/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_run/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.404991 eth-ape-0.8.2/src/ape_test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3647 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_test/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_test/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_test/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/src/ape_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.408991 eth-ape-0.8.2/src/eth_ape.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6563 2024-06-01 04:04:20.000000 eth-ape-0.8.2/src/eth_ape.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    16815 2024-06-01 04:04:20.000000 eth-ape-0.8.2/src/eth_ape.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 04:04:20.000000 eth-ape-0.8.2/src/eth_ape.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-06-01 04:04:20.000000 eth-ape-0.8.2/src/eth_ape.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 04:04:20.000000 eth-ape-0.8.2/src/eth_ape.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-06-01 04:04:20.000000 eth-ape-0.8.2/src/eth_ape.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-06-01 04:04:20.000000 eth-ape-0.8.2/src/eth_ape.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.408991 eth-ape-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17283 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.412991 eth-ape-0.8.2/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28387 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.416991 eth-ape-0.8.2/tests/functional/conversion/
+-rw-r--r--   0 runner    (1001) docker     (127)     2058 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/conversion/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/conversion/test_decimal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3162 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/conversion/test_encode_structs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/conversion/test_ether.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/conversion/test_hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/conversion/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/conversion/test_timestamp.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.416991 eth-ape-0.8.2/tests/functional/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.372990 eth-ape-0.8.2/tests/functional/data/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.372990 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.416991 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/abi/
+-rw-r--r--   0 runner    (1001) docker     (127)    13727 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/abi/contract_abi.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.420991 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/
+-rw-r--r--   0 runner    (1001) docker     (127)    26703 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/BeaconProxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    77599 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/ContractA.json
+-rw-r--r--   0 runner    (1001) docker     (127)    75147 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/ContractB.json
+-rw-r--r--   0 runner    (1001) docker     (127)    32313 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/ContractC.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6348 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/DsNoteTest.json
+-rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/HasError.json
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/Interface.json
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/InterfaceImplementation.json
+-rw-r--r--   0 runner    (1001) docker     (127)    46986 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/RevertsContract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5312 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/SolFallbackAndReceive.json
+-rw-r--r--   0 runner    (1001) docker     (127)   240439 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/SolidityContract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3735 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/SubReverts.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/VyDefault.json
+-rw-r--r--   0 runner    (1001) docker     (127)   251475 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/VyperContract.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7393 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/VyperFactory.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/beacon.json
+-rw-r--r--   0 runner    (1001) docker     (127)    19007 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/eip1967.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13901 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/printing.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8101 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/proxy.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.372990 eth-ape-0.8.2/tests/functional/data/manifests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.372990 eth-ape-0.8.2/tests/functional/data/manifests/openzeppelin/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.420991 eth-ape-0.8.2/tests/functional/data/manifests/openzeppelin/3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)  1733602 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/manifests/openzeppelin/3.1.0/openzeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.420991 eth-ape-0.8.2/tests/functional/data/manifests/openzeppelin/4.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)  1733602 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/manifests/openzeppelin/4.4.2/openzeppelin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.372990 eth-ape-0.8.2/tests/functional/data/projects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.424991 eth-ape-0.8.2/tests/functional/data/projects/ApeProject/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/projects/ApeProject/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.424991 eth-ape-0.8.2/tests/functional/data/projects/ApeProject/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/projects/ApeProject/contracts/ApeContract0.json
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/projects/ApeProject/contracts/ApeContract1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/projects/ApeProject/contracts/Contract.json
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/projects/ApeProject/contracts/Exclude.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.424991 eth-ape-0.8.2/tests/functional/data/projects/ApeProject/contracts/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/projects/ApeProject/contracts/subdir/ApeContractNested.json
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/projects/ApeProject/contracts/subdir/ExcludeNested.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.424991 eth-ape-0.8.2/tests/functional/data/projects/BrownieProject/
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/projects/BrownieProject/brownie-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.424991 eth-ape-0.8.2/tests/functional/data/projects/BrownieProject/contractsrenamed/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/projects/BrownieProject/contractsrenamed/brownie.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.372990 eth-ape-0.8.2/tests/functional/data/projects/LongContractsFolder/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.372990 eth-ape-0.8.2/tests/functional/data/projects/LongContractsFolder/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.424991 eth-ape-0.8.2/tests/functional/data/projects/LongContractsFolder/source/v0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/projects/LongContractsFolder/source/v0.1/long_contracts_folder.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.424991 eth-ape-0.8.2/tests/functional/data/python/
+-rw-r--r--   0 runner    (1001) docker     (127)    22650 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/python/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.424991 eth-ape-0.8.2/tests/functional/data/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2687 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/sources/ContractA.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/sources/ContractB.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1128 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/sources/ContractC.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/sources/HasError.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/sources/Proxy.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/sources/RevertsContract.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/sources/SolFallbackAndReceive.sol
+-rw-r--r--   0 runner    (1001) docker     (127)     8822 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/sources/SolidityContract.sol
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/sources/SubRevertsVy.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/sources/VyDefault.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/sources/VyperContract.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/sources/VyperFactory.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.424991 eth-ape-0.8.2/tests/functional/data/sources/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/data/sources/interfaces/ISubReverts.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.428991 eth-ape-0.8.2/tests/functional/geth/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/geth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/geth/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3327 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/geth/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/geth/test_contract_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/geth/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      863 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/geth/test_gas_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/geth/test_network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18683 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/geth/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/geth/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/geth/test_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10931 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/geth/test_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/geth/text_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32503 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      751 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_base_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6664 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_block_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4957 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_chain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27423 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6201 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_compilers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11196 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_contract_call_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6183 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_contract_container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13366 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_contract_event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32749 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_contract_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_contract_method_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14951 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_contracts_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8645 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_coverage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_default_sender_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17404 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65936 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_ecosystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2919 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_gas_tracker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2746 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_multicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_network_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_network_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14409 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28114 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17323 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3265 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8257 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_receipt_capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_reverts_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6987 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15166 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5275 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/test_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.428991 eth-ape-0.8.2/tests/functional/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/utils/test_abi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/utils/test_basemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3080 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/utils/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4738 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6141 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/functional/utils/test_os.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.428991 eth-ape-0.8.2/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.432991 eth-ape-0.8.2/tests/integration/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.376990 eth-ape-0.8.2/tests/integration/cli/projects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.372990 eth-ape-0.8.2/tests/integration/cli/projects/bad-contracts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.432991 eth-ape-0.8.2/tests/integration/cli/projects/bad-contracts/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/bad-contracts/contracts/Contract.test
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/bad-contracts/contracts/Contract2.foo
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/bad-contracts/contracts/doc.md
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/bad-contracts/contracts/file_without_ext
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/bad-contracts/contracts/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.432991 eth-ape-0.8.2/tests/integration/cli/projects/bad-contracts/contracts/subdir/
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/bad-contracts/contracts/subdir/tsconfig.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.432991 eth-ape-0.8.2/tests/integration/cli/projects/bad-contracts/contracts/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/bad-contracts/contracts/tests/TestContract.foobar
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.432991 eth-ape-0.8.2/tests/integration/cli/projects/empty-config/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/empty-config/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.432991 eth-ape-0.8.2/tests/integration/cli/projects/geth/
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/geth/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.432991 eth-ape-0.8.2/tests/integration/cli/projects/geth/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/geth/contracts/TokenA.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/geth/contracts/TokenB.json
+-rw-r--r--   0 runner    (1001) docker     (127)    28131 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/geth/contracts/VyperContract.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.432991 eth-ape-0.8.2/tests/integration/cli/projects/geth/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/geth/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/geth/tests/test_using_local_geth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.372990 eth-ape-0.8.2/tests/integration/cli/projects/multiple-interfaces/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.432991 eth-ape-0.8.2/tests/integration/cli/projects/multiple-interfaces/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/multiple-interfaces/contracts/Interface-with-hyphens.json
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/multiple-interfaces/contracts/Interface.exclude.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/multiple-interfaces/contracts/Interface.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/multiple-interfaces/contracts/InterfaceWithNumber123.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/multiple-interfaces/contracts/Interface_with_underscores.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.432991 eth-ape-0.8.2/tests/integration/cli/projects/no-config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/no-config/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.432991 eth-ape-0.8.2/tests/integration/cli/projects/only-dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/only-dependencies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/only-dependencies/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.432991 eth-ape-0.8.2/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       75 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/importme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.432991 eth-ape-0.8.2/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/only-dependencies/dependency_in_project_only/sources/DependencyInProjectOnly.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.372990 eth-ape-0.8.2/tests/integration/cli/projects/only-script-subdirs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.372990 eth-ape-0.8.2/tests/integration/cli/projects/only-script-subdirs/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.432991 eth-ape-0.8.2/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/subdirectory_click_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/only-script-subdirs/scripts/subdirectory/subdirectory_main_print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.376990 eth-ape-0.8.2/tests/integration/cli/projects/script/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.436991 eth-ape-0.8.2/tests/integration/cli/projects/script/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)    28131 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/script/contracts/VyperContract.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.436991 eth-ape-0.8.2/tests/integration/cli/projects/script/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/script/scripts/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/script/scripts/click.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/script/scripts/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/script/scripts/error_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/script/scripts/error_forgot_click.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/script/scripts/error_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/script/scripts/error_no_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/script/scripts/output_contract_view_methods.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/script/scripts/site.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.436991 eth-ape-0.8.2/tests/integration/cli/projects/script/scripts/subdirectory/
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/script/scripts/subdirectory/subdirectory_click_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/script/scripts/subdirectory/subdirectory_main_print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.436991 eth-ape-0.8.2/tests/integration/cli/projects/test/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/test/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.436991 eth-ape-0.8.2/tests/integration/cli/projects/test/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/test/tests/test_fixture_isolation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/test/tests/test_fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/test/tests/test_networks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.436991 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.436991 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2727 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/contracts/ContractA.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.436991 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/contracts/DirectoryWithJSONExtension.json/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/contracts/DirectoryWithJSONExtension.json/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/contracts/Exclude.json
+-rw-r--r--   0 runner    (1001) docker     (127)    41634 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/contracts/RawSolidityOutput.json
+-rw-r--r--   0 runner    (1001) docker     (127)    64327 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/contracts/RawVyperOutput.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.436991 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/contracts/exclude_dir/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/contracts/exclude_dir/UnwantedContract.json
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/contracts/hyphen-Contract.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.376990 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/dep/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.436991 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/dep/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)    64326 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/dep/contracts/RawVyperOutputDep.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.436991 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/dep_contracts_folder_root/
+-rw-r--r--   0 runner    (1001) docker     (127)    64326 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/dep_contracts_folder_root/RawVyperOutputDepNoContractsFolder.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.436991 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/scripts/txerr.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.440991 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/tests/test_contract.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.440991 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.440991 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.440991 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/contracts/containing_sub_dependencies.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.376990 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.440991 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/containing_sub_dependencies/sub_dependency/contracts/sub-dependency.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.440991 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/contracts/Other.json
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/contracts/Project.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.376990 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.440991 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/default/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/default/contracts/default.json
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/default/contracts/hyphen-DependencyContract.json
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/manifest_dependency.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.376990 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.376990 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.376990 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.440991 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/v0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/renamed_complex_contracts_folder/contracts/src/v0.1/renamed_complex_contracts_folder.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.376990 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.440991 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/sources/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder/sources/renamed_contracts_folder.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.440991 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:04:20.440991 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/my_contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/renamed_contracts_folder_specified_in_config/my_contracts/renamed_contracts_folder_specified_in_config.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12497 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/test_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13398 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/test_compile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8233 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/test_console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/test_networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5849 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/test_pm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7734 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13531 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/test_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4230 2024-06-01 04:03:21.000000 eth-ape-0.8.2/tests/integration/cli/utils.py
```

### Comparing `eth-ape-0.8.1/.github/ISSUE_TEMPLATE/bug.md` & `eth-ape-0.8.2/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/.github/ISSUE_TEMPLATE/feature.md` & `eth-ape-0.8.2/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/.github/ISSUE_TEMPLATE/work-item.md` & `eth-ape-0.8.2/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/.github/PULL_REQUEST_TEMPLATE.md` & `eth-ape-0.8.2/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/.github/release-drafter.yml` & `eth-ape-0.8.2/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/.github/workflows/codeql.yml` & `eth-ape-0.8.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/.github/workflows/commitlint.yaml` & `eth-ape-0.8.2/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/.github/workflows/docs.yaml` & `eth-ape-0.8.2/.github/workflows/docs.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/.github/workflows/prtitle.yaml` & `eth-ape-0.8.2/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/.github/workflows/publish.yaml` & `eth-ape-0.8.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/.github/workflows/stale-prs.yml` & `eth-ape-0.8.2/.github/workflows/stale-prs.yml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/.github/workflows/test.yaml` & `eth-ape-0.8.2/.github/workflows/test.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/.gitignore` & `eth-ape-0.8.2/.gitignore`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/.pre-commit-config.yaml` & `eth-ape-0.8.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/CONTRIBUTING.md` & `eth-ape-0.8.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/Dockerfile` & `eth-ape-0.8.2/Dockerfile`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/LICENSE` & `eth-ape-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/PKG-INFO` & `eth-ape-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-ape
-Version: 0.8.1
+Version: 0.8.2
 Summary: Ape Ethereum Framework
 Home-page: https://apeworx.io
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Project-URL: Documentation, https://docs.apeworx.io/ape/
 Project-URL: Funding, https://gitcoin.co/grants/5958/ape-maintenance-fund
```

### Comparing `eth-ape-0.8.1/README.md` & `eth-ape-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/SECURITY.md` & `eth-ape-0.8.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/build_docs.py` & `eth-ape-0.8.2/build_docs.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/_static/custom.css` & `eth-ape-0.8.2/docs/_static/custom.css`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/_static/custom.js` & `eth-ape-0.8.2/docs/_static/custom.js`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/_templates/layout.html` & `eth-ape-0.8.2/docs/_templates/layout.html`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/conf.py` & `eth-ape-0.8.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/favicon.ico` & `eth-ape-0.8.2/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/index.md` & `eth-ape-0.8.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/logo.gif` & `eth-ape-0.8.2/docs/logo.gif`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/methoddocs/api.md` & `eth-ape-0.8.2/docs/methoddocs/api.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/methoddocs/cli.md` & `eth-ape-0.8.2/docs/methoddocs/cli.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/methoddocs/contracts.md` & `eth-ape-0.8.2/docs/methoddocs/contracts.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/methoddocs/managers.md` & `eth-ape-0.8.2/docs/methoddocs/managers.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/methoddocs/plugins.md` & `eth-ape-0.8.2/docs/methoddocs/plugins.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/methoddocs/types.md` & `eth-ape-0.8.2/docs/methoddocs/types.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/accounts.md` & `eth-ape-0.8.2/docs/userguides/accounts.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/clis.md` & `eth-ape-0.8.2/docs/userguides/clis.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/compile.md` & `eth-ape-0.8.2/docs/userguides/compile.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/config.md` & `eth-ape-0.8.2/docs/userguides/config.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/console.md` & `eth-ape-0.8.2/docs/userguides/console.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/contracts.md` & `eth-ape-0.8.2/docs/userguides/contracts.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/data.md` & `eth-ape-0.8.2/docs/userguides/data.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/dependencies.md` & `eth-ape-0.8.2/docs/userguides/dependencies.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/developing_plugins.md` & `eth-ape-0.8.2/docs/userguides/developing_plugins.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/forking_networks.md` & `eth-ape-0.8.2/docs/userguides/forking_networks.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/installing_plugins.md` & `eth-ape-0.8.2/docs/userguides/installing_plugins.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/logging.md` & `eth-ape-0.8.2/docs/userguides/logging.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/networks.md` & `eth-ape-0.8.2/docs/userguides/networks.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/projects.md` & `eth-ape-0.8.2/docs/userguides/projects.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/proxy.md` & `eth-ape-0.8.2/docs/userguides/proxy.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/publishing.md` & `eth-ape-0.8.2/docs/userguides/publishing.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/scripts.md` & `eth-ape-0.8.2/docs/userguides/scripts.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/testing.md` & `eth-ape-0.8.2/docs/userguides/testing.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/trace.md` & `eth-ape-0.8.2/docs/userguides/trace.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/docs/userguides/transactions.md` & `eth-ape-0.8.2/docs/userguides/transactions.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/pyproject.toml` & `eth-ape-0.8.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/setup.py` & `eth-ape-0.8.2/setup.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/__init__.py` & `eth-ape-0.8.2/src/ape/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/_cli.py` & `eth-ape-0.8.2/src/ape/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/api/__init__.py` & `eth-ape-0.8.2/src/ape/api/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/api/accounts.py` & `eth-ape-0.8.2/src/ape/api/accounts.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/api/address.py` & `eth-ape-0.8.2/src/ape/api/address.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/api/compiler.py` & `eth-ape-0.8.2/src/ape/api/compiler.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/api/config.py` & `eth-ape-0.8.2/src/ape/api/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,15 +217,15 @@
                 #  this is likely a dependency of a dependency.
 
                 fixed_deps.append(fixed_dep)
 
             if fixed_deps:
                 fixed_model["dependencies"] = fixed_deps
 
-        # field: contracs_folder: Handle if given Path object.
+        # field: contracts_folder: Handle if given Path object.
         if "contracts_folder" in fixed_model and isinstance(fixed_model["contracts_folder"], Path):
             fixed_model["contracts_folder"] = str(fixed_model["contracts_folder"])
 
         return fixed_model
 
     @cached_property
     def deployments(self) -> dict[str, dict[str, list[DeploymentConfig]]]:
@@ -326,31 +326,35 @@
     def get_plugin_config(self, name: str) -> Optional[PluginConfig]:
         name = name.replace("-", "_")
         cfg = self._plugin_configs.get(name, {})
         if cfg and not isinstance(cfg, dict):
             # Already decoded.
             return cfg
 
-        for plugin_name, config_class in self.plugin_manager.config_class:
+        for plugin_name, config_class in self._get_config_plugin_classes():
             cls: type[PluginConfig] = config_class  # type: ignore
-            if plugin_name != name:
+            if plugin_name.replace("-", "_") != name:
                 continue
 
             if cls != ConfigDict:
                 # NOTE: Will raise if improperly provided keys
                 config = cls.from_overrides(cfg)
             else:
                 # NOTE: Just use it directly as a dict if `ConfigDict` is passed
                 config = cfg
 
             self._plugin_configs[name] = config
             return config
 
         return None
 
+    def _get_config_plugin_classes(self):
+        # NOTE: Abstracted for easily mocking in tests.
+        return self.plugin_manager.config_class
+
     def get_custom_ecosystem_config(self, name: str) -> Optional[PluginConfig]:
         name = name.replace("-", "_")
         if not (networks := self.get_plugin_config("networks")):
             # Shouldn't happen.
             return None
 
         for network in networks.custom:
```

### Comparing `eth-ape-0.8.1/src/ape/api/convert.py` & `eth-ape-0.8.2/src/ape/api/convert.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/api/explorers.py` & `eth-ape-0.8.2/src/ape/api/explorers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/api/networks.py` & `eth-ape-0.8.2/src/ape/api/networks.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/api/projects.py` & `eth-ape-0.8.2/src/ape/api/projects.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/api/providers.py` & `eth-ape-0.8.2/src/ape/api/providers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/api/query.py` & `eth-ape-0.8.2/src/ape/api/query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/api/trace.py` & `eth-ape-0.8.2/src/ape/api/trace.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/api/transactions.py` & `eth-ape-0.8.2/src/ape/api/transactions.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/cli/__init__.py` & `eth-ape-0.8.2/src/ape/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/cli/arguments.py` & `eth-ape-0.8.2/src/ape/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/cli/choices.py` & `eth-ape-0.8.2/src/ape/cli/choices.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/cli/commands.py` & `eth-ape-0.8.2/src/ape/cli/commands.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/cli/options.py` & `eth-ape-0.8.2/src/ape/cli/options.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/cli/paramtype.py` & `eth-ape-0.8.2/src/ape/cli/paramtype.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/contracts/base.py` & `eth-ape-0.8.2/src/ape/contracts/base.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/exceptions.py` & `eth-ape-0.8.2/src/ape/exceptions.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/logging.py` & `eth-ape-0.8.2/src/ape/logging.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/managers/__init__.py` & `eth-ape-0.8.2/src/ape/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/managers/accounts.py` & `eth-ape-0.8.2/src/ape/managers/accounts.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/managers/base.py` & `eth-ape-0.8.2/src/ape/managers/base.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/managers/chain.py` & `eth-ape-0.8.2/src/ape/managers/chain.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/managers/compilers.py` & `eth-ape-0.8.2/src/ape/managers/compilers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/managers/config.py` & `eth-ape-0.8.2/src/ape/managers/config.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/managers/converters.py` & `eth-ape-0.8.2/src/ape/managers/converters.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/managers/networks.py` & `eth-ape-0.8.2/src/ape/managers/networks.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/managers/plugins.py` & `eth-ape-0.8.2/src/ape/managers/plugins.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/managers/project.py` & `eth-ape-0.8.2/src/ape/managers/project.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/managers/query.py` & `eth-ape-0.8.2/src/ape/managers/query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/plugins/__init__.py` & `eth-ape-0.8.2/src/ape/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/plugins/_utils.py` & `eth-ape-0.8.2/src/ape/plugins/_utils.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/plugins/account.py` & `eth-ape-0.8.2/src/ape/plugins/account.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/plugins/compiler.py` & `eth-ape-0.8.2/src/ape/plugins/compiler.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/plugins/config.py` & `eth-ape-0.8.2/src/ape/plugins/config.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/plugins/converter.py` & `eth-ape-0.8.2/src/ape/plugins/converter.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/plugins/network.py` & `eth-ape-0.8.2/src/ape/plugins/network.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/plugins/pluggy_patch.py` & `eth-ape-0.8.2/src/ape/plugins/pluggy_patch.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/plugins/project.py` & `eth-ape-0.8.2/src/ape/plugins/project.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/plugins/query.py` & `eth-ape-0.8.2/src/ape/plugins/query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/pytest/README.md` & `eth-ape-0.8.2/src/ape/pytest/README.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/pytest/config.py` & `eth-ape-0.8.2/src/ape/pytest/config.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/pytest/contextmanagers.py` & `eth-ape-0.8.2/src/ape/pytest/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/pytest/coverage.py` & `eth-ape-0.8.2/src/ape/pytest/coverage.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from typing import Optional
 
 import click
 from ethpm_types.abi import MethodABI
 from ethpm_types.source import ContractSource
 
 from ape.logging import logger
+from ape.managers import ProjectManager
 from ape.pytest.config import ConfigWrapper
 from ape.types import (
     ContractFunctionPath,
     ControlFlow,
     CoverageProject,
     CoverageReport,
     SourceTraceback,
@@ -18,16 +19,16 @@
 from ape.utils.basemodel import ManagerAccessMixin
 from ape.utils.misc import get_current_timestamp_ms
 from ape.utils.os import get_full_extension, get_relative_path
 from ape.utils.trace import parse_coverage_tables
 
 
 class CoverageData(ManagerAccessMixin):
-    def __init__(self, base_path: Path, sources: Iterable[ContractSource]):
-        self.base_path = base_path
+    def __init__(self, project: ProjectManager, sources: Iterable[ContractSource]):
+        self.project = project
         self.sources = list(sources)
         self._report: Optional[CoverageReport] = None
         self._init_coverage_profile()  # Inits self._report.
 
     @property
     def report(self) -> CoverageReport:
         if self._report is None:
@@ -39,15 +40,15 @@
         self._report = None
         self._init_coverage_profile()
 
     def _init_coverage_profile(
         self,
     ) -> CoverageReport:
         # source_id -> pc(s) -> times hit
-        project_coverage = CoverageProject(name=self.config_manager.name or "__local__")
+        project_coverage = CoverageProject(name=self.project.name or "__local__")
 
         for src in self.sources:
             source_cov = project_coverage.include(src)
             ext = get_full_extension(Path(src.source_id))
             if ext not in self.compiler_manager.registered_compilers:
                 continue
 
@@ -56,29 +57,33 @@
                 compiler.init_coverage_profile(source_cov, src)
             except NotImplementedError:
                 continue
 
         timestamp = get_current_timestamp_ms()
         report = CoverageReport(
             projects=[project_coverage],
-            source_folders=[self.local_project.contracts_folder],
+            source_folders=[self.project.contracts_folder],
             timestamp=timestamp,
         )
 
-        # Remove emptys.
+        # Remove empties.
         for project in report.projects:
             project.sources = [x for x in project.sources if len(x.statements) > 0]
 
         self._report = report
         return report
 
     def cover(
         self, src_path: Path, pcs: Iterable[int], inc_fn_hits: bool = True
     ) -> tuple[set[int], list[str]]:
-        source_id = str(get_relative_path(src_path.absolute(), self.base_path))
+        if hasattr(self.project, "path"):
+            source_id = str(get_relative_path(src_path.absolute(), self.project.path))
+        else:
+            source_id = str(src_path)
+
         if source_id not in self.report.sources:
             # The source is not tracked for coverage.
             return set(), []
 
         handled_pcs = set()
         functions_incremented: list[str] = []
         for pc in pcs:
@@ -116,22 +121,35 @@
             # Maybe a bug in ape.
             logger.debug(f"Unhandled PCs: '{','.join([f'{x}' for x in unhandled_pcs])}'")
 
         return handled_pcs, functions_incremented
 
 
 class CoverageTracker(ManagerAccessMixin):
-    def __init__(self, config_wrapper: ConfigWrapper):
+    def __init__(
+        self,
+        config_wrapper: ConfigWrapper,
+        project: Optional[ProjectManager] = None,
+        output_path: Optional[Path] = None,
+    ):
         self.config_wrapper = config_wrapper
-        sources = self.local_project._contract_sources
+        self._project = project or self.local_project
+
+        if output_path:
+            self._output_path = output_path
+        elif hasattr(self._project, "manifest_path"):
+            # Local project.
+            self._output_path = self._project.manifest_path.parent
+        else:
+            self._output_path = Path.cwd()
+
+        sources = self._project._contract_sources
 
         self.data: Optional[CoverageData] = (
-            CoverageData(self.local_project.path, sources)
-            if self.config_wrapper.track_coverage
-            else None
+            CoverageData(self._project, sources) if self.config_wrapper.track_coverage else None
         )
 
     @property
     def enabled(self) -> bool:
         return self.config_wrapper.track_coverage
 
     @property
@@ -176,15 +194,15 @@
         elif contract and function:
             # Make sure it is the actual source.
             source_path = traceback[0].source_path if len(traceback) > 0 else None
             for project in self.data.report.projects:
                 for src in project.sources:
                     # NOTE: We will allow this check to skip if there is no source is the
                     # traceback. This helps increment methods that are missing from the source map.
-                    path = self.local_project.contracts_folder / src.source_id
+                    path = self._project.path / src.source_id
                     if source_path is not None and path != source_path:
                         continue
 
                     # Source containing the auto-getter found.
                     for con in src.contracts:
                         if con.name != contract:
                             continue
@@ -275,15 +293,14 @@
 
     def show_session_coverage(self) -> bool:
         if not self.data or not self.data.report or not self.data.report.sources:
             return False
 
         # Reports are set in ape-config.yaml.
         reports = self.config_wrapper.ape_test_config.coverage.reports
-        out_folder = self.local_project.manifest_path.parent
         if reports.terminal:
             verbose = (
                 reports.terminal.get("verbose", False)
                 if isinstance(reports.terminal, dict)
                 else False
             )
             if isinstance(verbose, str):
@@ -304,13 +321,13 @@
             for idx, table in enumerate(tables):
                 self.chain_manager._reports.echo(table)
 
                 if idx < len(tables) - 1:
                     click.echo()
 
         if self.config_wrapper.xml_coverage:
-            self.data.report.write_xml(out_folder)
+            self.data.report.write_xml(self._output_path)
         if value := self.config_wrapper.html_coverage:
             verbose = value.get("verbose", False) if isinstance(value, dict) else False
-            self.data.report.write_html(out_folder, verbose=verbose)
+            self.data.report.write_html(self._output_path, verbose=verbose)
 
         return True
```

### Comparing `eth-ape-0.8.1/src/ape/pytest/fixtures.py` & `eth-ape-0.8.2/src/ape/pytest/fixtures.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/pytest/gas.py` & `eth-ape-0.8.2/src/ape/pytest/gas.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/pytest/plugin.py` & `eth-ape-0.8.2/src/ape/pytest/plugin.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/pytest/runners.py` & `eth-ape-0.8.2/src/ape/pytest/runners.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/types/__init__.py` & `eth-ape-0.8.2/src/ape/types/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/types/address.py` & `eth-ape-0.8.2/src/ape/types/address.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/types/coverage.py` & `eth-ape-0.8.2/src/ape/types/coverage.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/types/signatures.py` & `eth-ape-0.8.2/src/ape/types/signatures.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/types/trace.py` & `eth-ape-0.8.2/src/ape/types/trace.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/utils/__init__.py` & `eth-ape-0.8.2/src/ape/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/utils/_github.py` & `eth-ape-0.8.2/src/ape/utils/_github.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/utils/abi.py` & `eth-ape-0.8.2/src/ape/utils/abi.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/utils/basemodel.py` & `eth-ape-0.8.2/src/ape/utils/basemodel.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/utils/misc.py` & `eth-ape-0.8.2/src/ape/utils/misc.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/utils/os.py` & `eth-ape-0.8.2/src/ape/utils/os.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/utils/process.py` & `eth-ape-0.8.2/src/ape/utils/process.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/utils/testing.py` & `eth-ape-0.8.2/src/ape/utils/testing.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/utils/trace.py` & `eth-ape-0.8.2/src/ape/utils/trace.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape/utils/validators.py` & `eth-ape-0.8.2/src/ape/utils/validators.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_accounts/_cli.py` & `eth-ape-0.8.2/src/ape_accounts/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_accounts/accounts.py` & `eth-ape-0.8.2/src/ape_accounts/accounts.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_cache/_cli.py` & `eth-ape-0.8.2/src/ape_cache/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_cache/models.py` & `eth-ape-0.8.2/src/ape_cache/models.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_cache/query.py` & `eth-ape-0.8.2/src/ape_cache/query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_compile/__init__.py` & `eth-ape-0.8.2/src/ape_compile/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_compile/_cli.py` & `eth-ape-0.8.2/src/ape_compile/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_console/_cli.py` & `eth-ape-0.8.2/src/ape_console/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_console/plugin.py` & `eth-ape-0.8.2/src/ape_console/plugin.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_ethereum/__init__.py` & `eth-ape-0.8.2/src/ape_ethereum/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_ethereum/_console_log_abi.py` & `eth-ape-0.8.2/src/ape_ethereum/_console_log_abi.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_ethereum/_converters.py` & `eth-ape-0.8.2/src/ape_ethereum/_converters.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_ethereum/_print.py` & `eth-ape-0.8.2/src/ape_ethereum/_print.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_ethereum/ecosystem.py` & `eth-ape-0.8.2/src/ape_ethereum/ecosystem.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_ethereum/multicall/constants.py` & `eth-ape-0.8.2/src/ape_ethereum/multicall/constants.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_ethereum/multicall/exceptions.py` & `eth-ape-0.8.2/src/ape_ethereum/multicall/exceptions.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_ethereum/multicall/handlers.py` & `eth-ape-0.8.2/src/ape_ethereum/multicall/handlers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_ethereum/provider.py` & `eth-ape-0.8.2/src/ape_ethereum/provider.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_ethereum/proxies.py` & `eth-ape-0.8.2/src/ape_ethereum/proxies.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_ethereum/query.py` & `eth-ape-0.8.2/src/ape_ethereum/query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_ethereum/trace.py` & `eth-ape-0.8.2/src/ape_ethereum/trace.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_ethereum/transactions.py` & `eth-ape-0.8.2/src/ape_ethereum/transactions.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_init/_cli.py` & `eth-ape-0.8.2/src/ape_init/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_networks/__init__.py` & `eth-ape-0.8.2/src/ape_networks/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_networks/_cli.py` & `eth-ape-0.8.2/src/ape_networks/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_node/__init__.py` & `eth-ape-0.8.2/src/ape_node/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_node/provider.py` & `eth-ape-0.8.2/src/ape_node/provider.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_node/query.py` & `eth-ape-0.8.2/src/ape_node/query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_plugins/_cli.py` & `eth-ape-0.8.2/src/ape_plugins/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_pm/__init__.py` & `eth-ape-0.8.2/src/ape_pm/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_pm/_cli.py` & `eth-ape-0.8.2/src/ape_pm/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_pm/compiler.py` & `eth-ape-0.8.2/src/ape_pm/compiler.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_pm/dependency.py` & `eth-ape-0.8.2/src/ape_pm/dependency.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_pm/projects.py` & `eth-ape-0.8.2/src/ape_pm/projects.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_run/_cli.py` & `eth-ape-0.8.2/src/ape_run/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_test/__init__.py` & `eth-ape-0.8.2/src/ape_test/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_test/_cli.py` & `eth-ape-0.8.2/src/ape_test/_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_test/accounts.py` & `eth-ape-0.8.2/src/ape_test/accounts.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/ape_test/provider.py` & `eth-ape-0.8.2/src/ape_test/provider.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/eth_ape.egg-info/PKG-INFO` & `eth-ape-0.8.2/src/eth_ape.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eth-ape
-Version: 0.8.1
+Version: 0.8.2
 Summary: Ape Ethereum Framework
 Home-page: https://apeworx.io
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Project-URL: Documentation, https://docs.apeworx.io/ape/
 Project-URL: Funding, https://gitcoin.co/grants/5958/ape-maintenance-fund
```

### Comparing `eth-ape-0.8.1/src/eth_ape.egg-info/SOURCES.txt` & `eth-ape-0.8.2/src/eth_ape.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/src/eth_ape.egg-info/requires.txt` & `eth-ape-0.8.2/src/eth_ape.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/README.md` & `eth-ape-0.8.2/tests/README.md`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/conftest.py` & `eth-ape-0.8.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/conftest.py` & `eth-ape-0.8.2/tests/functional/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -676,29 +676,35 @@
 
 @pytest.fixture
 def mock_compiler(mocker):
     mock = mocker.MagicMock()
     mock.name = "mock"
     mock.ext = ".__mock__"
     mock.tracked_settings = []
+    mock.ast = None
+    mock.pcmap = None
 
     def mock_compile(paths, project=None, settings=None):
         settings = settings or {}
         mock.tracked_settings.append(settings)
         result = []
         for path in paths:
             if path.suffix == mock.ext:
                 name = path.stem
                 code = HexBytes(123).hex()
                 data = {
                     "contractName": name,
-                    "abi": [],
+                    "abi": mock.abi,
                     "deploymentBytecode": code,
                     "sourceId": f"{project.contracts_folder.name}/{path.name}",
                 }
+                if ast := mock.ast:
+                    data["ast"] = ast
+                if pcmap := mock.pcmap:
+                    data["pcmap"] = pcmap
 
                 # Check for mocked overrides
                 overrides = mock.overrides
                 if isinstance(overrides, dict):
                     data = {**data, **overrides}
 
                 contract_type = ContractType.model_validate(data)
```

### Comparing `eth-ape-0.8.1/tests/functional/conversion/test_address.py` & `eth-ape-0.8.2/tests/functional/conversion/test_address.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/conversion/test_decimal.py` & `eth-ape-0.8.2/tests/functional/conversion/test_decimal.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/conversion/test_encode_structs.py` & `eth-ape-0.8.2/tests/functional/conversion/test_encode_structs.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/conversion/test_ether.py` & `eth-ape-0.8.2/tests/functional/conversion/test_ether.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/conversion/test_hex.py` & `eth-ape-0.8.2/tests/functional/conversion/test_hex.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/conversion/test_misc.py` & `eth-ape-0.8.2/tests/functional/conversion/test_misc.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/conversion/test_timestamp.py` & `eth-ape-0.8.2/tests/functional/conversion/test_timestamp.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/abi/contract_abi.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/abi/contract_abi.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/BeaconProxy.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/BeaconProxy.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/ContractA.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/ContractA.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/ContractB.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/ContractB.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/ContractC.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/ContractC.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/DsNoteTest.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/DsNoteTest.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/HasError.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/HasError.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/InterfaceImplementation.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/InterfaceImplementation.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/RevertsContract.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/RevertsContract.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/SolFallbackAndReceive.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/SolFallbackAndReceive.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/SolidityContract.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/SolidityContract.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/SubReverts.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/SubReverts.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/VyDefault.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/VyDefault.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/VyperContract.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/VyperContract.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/VyperFactory.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/VyperFactory.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/beacon.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/beacon.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/eip1967.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/eip1967.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/printing.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/printing.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/contracts/ethereum/local/proxy.json` & `eth-ape-0.8.2/tests/functional/data/contracts/ethereum/local/proxy.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/manifests/openzeppelin/3.1.0/openzeppelin.json` & `eth-ape-0.8.2/tests/functional/data/manifests/openzeppelin/3.1.0/openzeppelin.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/manifests/openzeppelin/4.4.2/openzeppelin.json` & `eth-ape-0.8.2/tests/functional/data/manifests/openzeppelin/4.4.2/openzeppelin.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/projects/ApeProject/contracts/Contract.json` & `eth-ape-0.8.2/tests/functional/data/projects/ApeProject/contracts/Contract.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/python/__init__.py` & `eth-ape-0.8.2/tests/functional/data/python/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/sources/ContractA.sol` & `eth-ape-0.8.2/tests/functional/data/sources/ContractA.sol`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/sources/ContractB.sol` & `eth-ape-0.8.2/tests/functional/data/sources/ContractB.sol`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/sources/ContractC.sol` & `eth-ape-0.8.2/tests/functional/data/sources/ContractC.sol`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/sources/HasError.sol` & `eth-ape-0.8.2/tests/functional/data/sources/HasError.sol`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/sources/RevertsContract.vy` & `eth-ape-0.8.2/tests/functional/data/sources/RevertsContract.vy`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/sources/SolidityContract.sol` & `eth-ape-0.8.2/tests/functional/data/sources/SolidityContract.sol`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/data/sources/VyperContract.vy` & `eth-ape-0.8.2/tests/functional/data/sources/VyperContract.vy`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/geth/conftest.py` & `eth-ape-0.8.2/tests/functional/geth/conftest.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/geth/test_contract.py` & `eth-ape-0.8.2/tests/functional/geth/test_contract.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/geth/test_gas_tracker.py` & `eth-ape-0.8.2/tests/functional/geth/test_gas_tracker.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/geth/test_network_manager.py` & `eth-ape-0.8.2/tests/functional/geth/test_network_manager.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/geth/test_provider.py` & `eth-ape-0.8.2/tests/functional/geth/test_provider.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/geth/test_query.py` & `eth-ape-0.8.2/tests/functional/geth/test_query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/geth/test_receipt.py` & `eth-ape-0.8.2/tests/functional/geth/test_receipt.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/geth/test_trace.py` & `eth-ape-0.8.2/tests/functional/geth/test_trace.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/geth/text_proxy.py` & `eth-ape-0.8.2/tests/functional/geth/text_proxy.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_accounts.py` & `eth-ape-0.8.2/tests/functional/test_accounts.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_address.py` & `eth-ape-0.8.2/tests/functional/test_address.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_base_manager.py` & `eth-ape-0.8.2/tests/functional/test_base_manager.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_block.py` & `eth-ape-0.8.2/tests/functional/test_block.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_block_container.py` & `eth-ape-0.8.2/tests/functional/test_block_container.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_chain.py` & `eth-ape-0.8.2/tests/functional/test_chain.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_cli.py` & `eth-ape-0.8.2/tests/functional/test_cli.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_compilers.py` & `eth-ape-0.8.2/tests/functional/test_compilers.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_config.py` & `eth-ape-0.8.2/tests/functional/test_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import pytest
 from pydantic_settings import SettingsConfigDict
 
 from ape.api.config import ApeConfig, ConfigEnum, PluginConfig
 from ape.exceptions import ConfigError
 from ape.managers.config import CONFIG_FILE_NAME, merge_configs
 from ape.types import GasLimit
-from ape_ethereum.ecosystem import NetworkConfig
+from ape_ethereum.ecosystem import EthereumConfig, NetworkConfig
 from ape_networks import CustomNetwork
 from tests.functional.conftest import PROJECT_WITH_LONG_CONTRACTS_FOLDER
 
 
 def test_model_validate_empty():
     data: dict = {}
     cfg = ApeConfig.model_validate(data)
@@ -310,7 +310,39 @@
         "chain_id": 11191919191991918223773,
         "ecosystem": "ethereum",
     }
     network = CustomNetwork.model_validate(data)
     assert network.name == "mytestnet"
     assert network.chain_id == chain_id
     assert network.ecosystem == "ethereum"
+
+
+def test_get_config(config):
+    actual = config.get_config("ethereum")
+    assert isinstance(actual, EthereumConfig)
+
+
+def test_get_config_hyphen_in_plugin_name(config):
+    """
+    Tests against a bug noticed with ape-polygon-zkevm installed
+    on Ape 0.8.0 release where the config no longer worked.
+    """
+
+    class CustomConfig(PluginConfig):
+        x: int = 123
+
+    mock_cfg_with_hyphens = CustomConfig
+    original_method = config.local_project.config._get_config_plugin_classes
+
+    # Hack in the fake plugin to test the behavior.
+    def hacked_in_method():
+        yield from [*list(original_method()), ("mock-plugin", mock_cfg_with_hyphens)]
+
+    config.local_project.config._get_config_plugin_classes = hacked_in_method
+
+    try:
+        cfg = config.get_config("mock-plugin")
+        assert isinstance(cfg, CustomConfig)
+        assert cfg.x == 123
+
+    finally:
+        config.local_project.config._get_config_plugin_classes = original_method
```

### Comparing `eth-ape-0.8.1/tests/functional/test_console.py` & `eth-ape-0.8.2/tests/functional/test_console.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_contract.py` & `eth-ape-0.8.2/tests/functional/test_contract.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_contract_container.py` & `eth-ape-0.8.2/tests/functional/test_contract_container.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_contract_event.py` & `eth-ape-0.8.2/tests/functional/test_contract_event.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_contract_instance.py` & `eth-ape-0.8.2/tests/functional/test_contract_instance.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_contract_method_handler.py` & `eth-ape-0.8.2/tests/functional/test_contract_method_handler.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_contracts_cache.py` & `eth-ape-0.8.2/tests/functional/test_contracts_cache.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_default_sender_context_manager.py` & `eth-ape-0.8.2/tests/functional/test_default_sender_context_manager.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_dependencies.py` & `eth-ape-0.8.2/tests/functional/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_ecosystem.py` & `eth-ape-0.8.2/tests/functional/test_ecosystem.py`

 * *Files 0% similar despite different names*

```diff
@@ -970,15 +970,29 @@
     net["ecosystem"] = ecosystem_name
 
     only_network = "onlynet"  # More obvious name for test.
     net["name"] = only_network
 
     with project.temp_config(networks={"custom": [net]}):
         ecosystem = project.network_manager.get_ecosystem(ecosystem_name)
-        assert ecosystem.default_network_name == only_network
+        actual = ecosystem.default_network_name
+
+        if actual == LOCAL_NETWORK_NAME:
+            # For some reason, this test is flake-y. Offer more info
+            # to try and debug when this happens (intermittent CI failure).
+            all_nets = ", ".join([x.name for x in ecosystem.networks])
+            pytest.fail(
+                f"assert '{LOCAL_NETWORK_NAME}' == '{only_network}'. More info below:\n"
+                f"ecosystem_name={ecosystem.name}\n"
+                f"networks={all_nets}\n"
+                f"type={type(ecosystem)}"
+            )
+        else:
+            # This should pass.
+            assert ecosystem.default_network_name == only_network
 
 
 def test_decode_custom_error(chain, ethereum):
     data = HexBytes("0x6a12f104")
     abi = [ErrorABI(type="error", name="InsufficientETH", inputs=[])]
     contract_type = ContractType(abi=abi)
     addr = cast(AddressType, "0x3fC91A3afd70395Cd496C647d5a6CC9D4B2b7FAD")
```

### Comparing `eth-ape-0.8.1/tests/functional/test_exceptions.py` & `eth-ape-0.8.2/tests/functional/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_fixtures.py` & `eth-ape-0.8.2/tests/functional/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_gas_tracker.py` & `eth-ape-0.8.2/tests/functional/test_gas_tracker.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_history.py` & `eth-ape-0.8.2/tests/functional/test_history.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_logging.py` & `eth-ape-0.8.2/tests/functional/test_logging.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_multicall.py` & `eth-ape-0.8.2/tests/functional/test_multicall.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_network_api.py` & `eth-ape-0.8.2/tests/functional/test_network_api.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_network_manager.py` & `eth-ape-0.8.2/tests/functional/test_network_manager.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_plugins.py` & `eth-ape-0.8.2/tests/functional/test_plugins.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_project.py` & `eth-ape-0.8.2/tests/functional/test_project.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_provider.py` & `eth-ape-0.8.2/tests/functional/test_provider.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_query.py` & `eth-ape-0.8.2/tests/functional/test_query.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_receipt.py` & `eth-ape-0.8.2/tests/functional/test_receipt.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_reverts_context_manager.py` & `eth-ape-0.8.2/tests/functional/test_reverts_context_manager.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_trace.py` & `eth-ape-0.8.2/tests/functional/test_trace.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_transaction.py` & `eth-ape-0.8.2/tests/functional/test_transaction.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/test_types.py` & `eth-ape-0.8.2/tests/functional/test_types.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/utils/test_abi.py` & `eth-ape-0.8.2/tests/functional/utils/test_abi.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/utils/test_basemodel.py` & `eth-ape-0.8.2/tests/functional/utils/test_basemodel.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/utils/test_github.py` & `eth-ape-0.8.2/tests/functional/utils/test_github.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/utils/test_misc.py` & `eth-ape-0.8.2/tests/functional/utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/functional/utils/test_os.py` & `eth-ape-0.8.2/tests/functional/utils/test_os.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/conftest.py` & `eth-ape-0.8.2/tests/integration/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/projects/geth/ape-config.yaml` & `eth-ape-0.8.2/tests/integration/cli/projects/geth/ape-config.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/projects/geth/contracts/TokenA.json` & `eth-ape-0.8.2/tests/integration/cli/projects/geth/contracts/TokenA.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/projects/geth/contracts/TokenB.json` & `eth-ape-0.8.2/tests/integration/cli/projects/geth/contracts/TokenB.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/projects/geth/contracts/VyperContract.json` & `eth-ape-0.8.2/tests/integration/cli/projects/geth/contracts/VyperContract.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/projects/geth/tests/test_using_local_geth.py` & `eth-ape-0.8.2/tests/integration/cli/projects/geth/tests/test_using_local_geth.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/projects/script/contracts/VyperContract.json` & `eth-ape-0.8.2/tests/integration/cli/projects/script/contracts/VyperContract.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/projects/test/tests/test_fixture_isolation.py` & `eth-ape-0.8.2/tests/integration/cli/projects/test/tests/test_fixture_isolation.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/projects/test/tests/test_fixtures.py` & `eth-ape-0.8.2/tests/integration/cli/projects/test/tests/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/projects/test/tests/test_networks.py` & `eth-ape-0.8.2/tests/integration/cli/projects/test/tests/test_networks.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/contracts/ContractA.json` & `eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/contracts/ContractA.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/contracts/RawSolidityOutput.json` & `eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/contracts/RawSolidityOutput.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/contracts/RawVyperOutput.json` & `eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/contracts/RawVyperOutput.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/dep/contracts/RawVyperOutputDep.json` & `eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/dep/contracts/RawVyperOutputDep.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/dep_contracts_folder_root/RawVyperOutputDepNoContractsFolder.json` & `eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/dep_contracts_folder_root/RawVyperOutputDepNoContractsFolder.json`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/projects/with-contracts/tests/test_contract.py` & `eth-ape-0.8.2/tests/integration/cli/projects/with-contracts/tests/test_contract.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/projects/with-dependencies/ape-config.yaml` & `eth-ape-0.8.2/tests/integration/cli/projects/with-dependencies/ape-config.yaml`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/test_accounts.py` & `eth-ape-0.8.2/tests/integration/cli/test_accounts.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/test_compile.py` & `eth-ape-0.8.2/tests/integration/cli/test_compile.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/test_console.py` & `eth-ape-0.8.2/tests/integration/cli/test_console.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/test_init.py` & `eth-ape-0.8.2/tests/integration/cli/test_init.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/test_misc.py` & `eth-ape-0.8.2/tests/integration/cli/test_misc.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/test_networks.py` & `eth-ape-0.8.2/tests/integration/cli/test_networks.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/test_plugins.py` & `eth-ape-0.8.2/tests/integration/cli/test_plugins.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/test_pm.py` & `eth-ape-0.8.2/tests/integration/cli/test_pm.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/test_run.py` & `eth-ape-0.8.2/tests/integration/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/test_test.py` & `eth-ape-0.8.2/tests/integration/cli/test_test.py`

 * *Files identical despite different names*

### Comparing `eth-ape-0.8.1/tests/integration/cli/utils.py` & `eth-ape-0.8.2/tests/integration/cli/utils.py`

 * *Files identical despite different names*

