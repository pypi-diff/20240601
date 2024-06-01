# Comparing `tmp/ape-vyper-0.7.1.tar.gz` & `tmp/ape-vyper-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-vyper-0.7.1.tar", last modified: Fri Mar 22 18:45:51 2024, max compression
+gzip compressed data, was "ape-vyper-0.8.0.tar", last modified: Sat Jun  1 05:10:56 2024, max compression
```

## Comparing `ape-vyper-0.7.1.tar` & `ape-vyper-0.8.0.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.943903 ape-vyper-0.7.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.935903 ape-vyper-0.7.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.935903 ape-vyper-0.7.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.935903 ape-vyper-0.7.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      366 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3828 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-03-22 18:45:51.943903 ape-vyper-0.7.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.935903 ape-vyper-0.7.1/ape_vyper/
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/ape_vyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/ape_vyper/_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/ape_vyper/ast.py
--rw-r--r--   0 runner    (1001) docker     (127)    59902 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/ape_vyper/compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5194 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/ape_vyper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4227 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/ape_vyper/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-22 18:45:51.000000 ape-vyper-0.7.1/ape_vyper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.935903 ape-vyper-0.7.1/ape_vyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-03-22 18:45:51.000000 ape-vyper-0.7.1/ape_vyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-03-22 18:45:51.000000 ape-vyper-0.7.1/ape_vyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 18:45:51.000000 ape-vyper-0.7.1/ape_vyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-22 18:45:51.000000 ape-vyper-0.7.1/ape_vyper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 18:45:51.000000 ape-vyper-0.7.1/ape_vyper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-03-22 18:45:51.000000 ape-vyper-0.7.1/ape_vyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-22 18:45:51.000000 ape-vyper-0.7.1/ape_vyper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-03-22 18:45:51.943903 ape-vyper-0.7.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3252 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.939903 ape-vyper-0.7.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.931903 ape-vyper-0.7.1/tests/ExampleDependency/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.939903 ape-vyper-0.7.1/tests/ExampleDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/ExampleDependency/contracts/Dependency.vy
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.931903 ape-vyper-0.7.1/tests/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.939903 ape-vyper-0.7.1/tests/contracts/failing_contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       83 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/failing_contracts/contract_undeclared_variable.vy
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/failing_contracts/contract_unknown_pragma.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.939903 ape-vyper-0.7.1/tests/contracts/passing_contracts/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.939903 ape-vyper-0.7.1/tests/contracts/passing_contracts/DirectoryWithExtension.vy/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/contract_no_pragma.vy
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/contract_with_dev_messages.vy
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/empty.vy
--rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/erc20.vy
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/evm_pragma.vy
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/flatten_me.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.939903 ape-vyper-0.7.1/tests/contracts/passing_contracts/interfaces/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/interfaces/IFace.vy
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/interfaces/IFace2.vy
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/interfaces/IRegistry.vy
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/interfaces/ISubReverts.vy
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/non_payable_default.vy
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/older_version.vy
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/optimize_codesize.vy
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/payable_default.vy
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/pragma_with_space.vy
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/use_iface.vy
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/passing_contracts/use_iface2.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.939903 ape-vyper-0.7.1/tests/contracts/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/templates/contract.template
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/templates/registry.template
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/templates/reverts.template
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/templates/sub_reverts.template
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/contracts/templates/traceback_contract.template
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.931903 ape-vyper-0.7.1/tests/projects/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.943903 ape-vyper-0.7.1/tests/projects/coverage_project/
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/projects/coverage_project/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/projects/coverage_project/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.943903 ape-vyper-0.7.1/tests/projects/coverage_project/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)      426 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/projects/coverage_project/contracts/coverage_test.vy
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/projects/coverage_project/contracts/exclude_part_of_contract.vy
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/projects/coverage_project/contracts/exclude_whole_contract.vy
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.943903 ape-vyper-0.7.1/tests/projects/coverage_project/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/projects/coverage_project/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/projects/coverage_project/tests/test_coverage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.943903 ape-vyper-0.7.1/tests/projects/version_in_config/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/projects/version_in_config/ape-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:45:51.943903 ape-vyper-0.7.1/tests/projects/version_in_config/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/projects/version_in_config/contracts/v_contract.vy
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/test_ape_reverts.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    19955 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/test_compiler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5773 2024-03-22 18:44:52.000000 ape-vyper-0.7.1/tests/test_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.239219 ape-vyper-0.8.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.231219 ape-vyper-0.8.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.231219 ape-vyper-0.8.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.231219 ape-vyper-0.8.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3966 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11342 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-06-01 05:10:56.239219 ape-vyper-0.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3630 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.231219 ape-vyper-0.8.0/ape_vyper/
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/ape_vyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/ape_vyper/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3357 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/ape_vyper/ast.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65294 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/ape_vyper/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/ape_vyper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4208 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/ape_vyper/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-01 05:10:55.000000 ape-vyper-0.8.0/ape_vyper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.235219 ape-vyper-0.8.0/ape_vyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4588 2024-06-01 05:10:56.000000 ape-vyper-0.8.0/ape_vyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2842 2024-06-01 05:10:56.000000 ape-vyper-0.8.0/ape_vyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 05:10:56.000000 ape-vyper-0.8.0/ape_vyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-01 05:10:56.000000 ape-vyper-0.8.0/ape_vyper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 05:10:56.000000 ape-vyper-0.8.0/ape_vyper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-06-01 05:10:56.000000 ape-vyper-0.8.0/ape_vyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 05:10:56.000000 ape-vyper-0.8.0/ape_vyper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-06-01 05:10:56.239219 ape-vyper-0.8.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3308 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.235219 ape-vyper-0.8.0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.227219 ape-vyper-0.8.0/tests/ExampleDependency/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.235219 ape-vyper-0.8.0/tests/ExampleDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/ExampleDependency/contracts/Dependency.vy
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5507 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.227219 ape-vyper-0.8.0/tests/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.235219 ape-vyper-0.8.0/tests/contracts/failing_contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/failing_contracts/contract_undeclared_variable.vy
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/failing_contracts/contract_unknown_pragma.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.235219 ape-vyper-0.8.0/tests/contracts/passing_contracts/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.235219 ape-vyper-0.8.0/tests/contracts/passing_contracts/DirectoryWithExtension.vy/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/contract_no_pragma.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/contract_with_dev_messages.vy
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/empty.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     5231 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/erc20.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/evm_pragma.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/flatten_me.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.239219 ape-vyper-0.8.0/tests/contracts/passing_contracts/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/interfaces/IFace.vy
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/interfaces/IFace2.vy
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/interfaces/IRegistry.vy
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/interfaces/ISubReverts.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/non_payable_default.vy
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/older_version.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/optimize_codesize.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/payable_default.vy
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/pragma_with_space.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/use_iface.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/passing_contracts/use_iface2.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.239219 ape-vyper-0.8.0/tests/contracts/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/templates/contract.template
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/templates/registry.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/templates/reverts.template
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/templates/sub_reverts.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/contracts/templates/traceback_contract.template
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.227219 ape-vyper-0.8.0/tests/projects/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.239219 ape-vyper-0.8.0/tests/projects/coverage_project/
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/projects/coverage_project/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/projects/coverage_project/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.239219 ape-vyper-0.8.0/tests/projects/coverage_project/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)      426 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/projects/coverage_project/contracts/coverage_test.vy
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/projects/coverage_project/contracts/exclude_part_of_contract.vy
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/projects/coverage_project/contracts/exclude_whole_contract.vy
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.239219 ape-vyper-0.8.0/tests/projects/coverage_project/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/projects/coverage_project/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/projects/coverage_project/tests/test_coverage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.239219 ape-vyper-0.8.0/tests/projects/version_in_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/projects/version_in_config/ape-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 05:10:56.239219 ape-vyper-0.8.0/tests/projects/version_in_config/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/projects/version_in_config/contracts/v_contract.vy
+-rw-r--r--   0 runner    (1001) docker     (127)     4694 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/test_ape_reverts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20634 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/test_compiler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6513 2024-06-01 05:09:50.000000 ape-vyper-0.8.0/tests/test_coverage.py
```

### Comparing `ape-vyper-0.7.1/.github/ISSUE_TEMPLATE/bug.md` & `ape-vyper-0.8.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.7.1/.github/ISSUE_TEMPLATE/feature.md` & `ape-vyper-0.8.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.7.1/.github/ISSUE_TEMPLATE/work-item.md` & `ape-vyper-0.8.0/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.7.1/.github/release-drafter.yml` & `ape-vyper-0.8.0/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.7.1/.github/workflows/commitlint.yaml` & `ape-vyper-0.8.0/.github/workflows/commitlint.yaml`

 * *Files 2% similar despite different names*

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
             pip install commitizen
```

### Comparing `ape-vyper-0.7.1/.github/workflows/prtitle.yaml` & `ape-vyper-0.8.0/.github/workflows/prtitle.yaml`

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
           run: |
             python -m pip install --upgrade pip
             pip install commitizen
```

### Comparing `ape-vyper-0.7.1/.github/workflows/publish.yaml` & `ape-vyper-0.8.0/.github/workflows/publish.yaml`

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

### Comparing `ape-vyper-0.7.1/.github/workflows/test.yaml` & `ape-vyper-0.8.0/.github/workflows/test.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,18 @@
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
@@ -41,18 +41,18 @@
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
             pip install .[lint,test]  # Might need test deps
@@ -61,25 +61,27 @@
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
 
         env:
           GETH_VERSION: 1.12.0
 
         steps:
-        - uses: actions/checkout@v3
+        - uses: actions/checkout@v4
 
         - name: Setup Python
-          uses: actions/setup-python@v4
+          uses: actions/setup-python@v5
           with:
               python-version: ${{ matrix.python-version }}
 
         - name: Setup Go
           uses: actions/setup-go@v4
           with:
             go-version: '^1.20.1'
@@ -105,15 +107,15 @@
         - name: Install Dependencies
           run: |
             python -m pip install --upgrade pip
             pip install .[test]
 
         - name: Run Tests
           run: |
-            pytest tests/test_compiler.py -m "not fuzzing" -n 0 -s \
+            pytest -k "not test_coverage" -m "not fuzzing" -n 0 -s \
               --cov=ape_vyper \
               --cov-branch \
               --cov-report term \
               --cov-report html \
               --cov-report xml
 
         # Since --cov does not play nicely with --coverage (low-level tracer issues),
@@ -126,18 +128,18 @@
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
 #          run: |
 #             python -m pip install --upgrade pip
 #             pip install .[test]
```

### Comparing `ape-vyper-0.7.1/.gitignore` & `ape-vyper-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.7.1/.pre-commit-config.yaml` & `ape-vyper-0.8.0/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

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
         additional_dependencies: [types-setuptools, pydantic==1.10.4]
 
 -   repo: https://github.com/executablebooks/mdformat
     rev: 0.7.17
     hooks:
     -   id: mdformat
-        additional_dependencies: [mdformat-gfm, mdformat-frontmatter]
+        additional_dependencies: [mdformat-gfm, mdformat-frontmatter, mdformat-pyproject]
 
 default_language_version:
     python: python3
```

### Comparing `ape-vyper-0.7.1/CONTRIBUTING.md` & `ape-vyper-0.8.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.7.1/LICENSE` & `ape-vyper-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.7.1/PKG-INFO` & `ape-vyper-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: ape-vyper
-Version: 0.7.1
+Version: 0.8.0
 Summary: Plugin for Ape Ethereum Framework for compiling Vyper contracts
 Home-page: https://github.com/ApeWorX/ape-vyper
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
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 Ape compiler plugin around [VVM](https://github.com/vyperlang/vvm)
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-vyper-0.7.1/README.md` & `ape-vyper-0.8.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ape compiler plugin around [VVM](https://github.com/vyperlang/vvm)
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-vyper-0.7.1/ape_vyper/_cli.py` & `ape-vyper-0.8.0/ape_vyper/_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from pathlib import Path
 
 import ape
 import click
-from ape.cli import ape_cli_context
+from ape.cli import ape_cli_context, project_option
 
 
 @click.group
 def cli():
     """`vyper` command group"""
 
 
 @cli.command(short_help="Flatten select contract source files")
 @ape_cli_context()
+@project_option()
 @click.argument("CONTRACT", type=click.Path(exists=True, resolve_path=True))
 @click.argument("OUTFILE", type=click.Path(exists=False, resolve_path=True, writable=True))
-def flatten(cli_ctx, contract: Path, outfile: Path):
+def flatten(cli_ctx, project, contract: Path, outfile: Path):
     """
     Flatten a contract into a single file
     """
     with Path(outfile).open("w") as fout:
         content = ape.compilers.vyper.flatten_contract(
-            Path(contract), base_path=ape.project.contracts_folder
+            Path(contract),
+            base_path=ape.project.contracts_folder,
+            project=project,
         )
         fout.write(str(content))
```

### Comparing `ape-vyper-0.7.1/ape_vyper/ast.py` & `ape-vyper-0.8.0/ape_vyper/ast.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,58 +1,56 @@
 """Utilities for dealing with Vyper AST"""
 
-from typing import List
-
 from ethpm_types import ABI, MethodABI
 from ethpm_types.abi import ABIType
 from vyper.ast import parse_to_ast  # type: ignore
 from vyper.ast.nodes import FunctionDef, Module, Name, Subscript  # type: ignore
 
 DEFAULT_VYPER_MUTABILITY = "nonpayable"
 DECORATOR_MUTABILITY = {
     "pure",  # Function does not read contract state or environment variables
     "view",  # Function does not alter contract state
     "payable",  # Function is able to receive Ether and may alter state
     "nonpayable",  # Function may alter sate
 }
 
 
-def funcdef_decorators(funcdef: FunctionDef) -> List[str]:
+def funcdef_decorators(funcdef: FunctionDef) -> list[str]:
     return [d.id for d in funcdef.get("decorator_list") or []]
 
 
-def funcdef_inputs(funcdef: FunctionDef) -> List[ABIType]:
+def funcdef_inputs(funcdef: FunctionDef) -> list[ABIType]:
     """Get a FunctionDef's defined input args"""
     args = funcdef.get("args")
     # TODO: Does Vyper allow complex input types, like structs and arrays?
     return (
         [ABIType.model_validate({"name": arg.arg, "type": arg.annotation.id}) for arg in args.args]
         if args
         else []
     )
 
 
-def funcdef_outputs(funcdef: FunctionDef) -> List[ABIType]:
+def funcdef_outputs(funcdef: FunctionDef) -> list[ABIType]:
     """Get a FunctionDef's outputs, or return values"""
     returns = funcdef.get("returns")
 
     if not returns:
         return []
 
     if isinstance(returns, Name):
         # TODO: Structs fall in here. I think they're supposed to be a tuple of types in the ABI.
         #       Need to dig into that more.
         return [ABIType.model_validate({"type": returns.id})]
 
     elif isinstance(returns, Subscript):
         # An array type
         length = returns.slice.value.value
-        array_type = returns.value.id
-        # TOOD: Is this an acurrate way to define a fixed length array for ABI?
-        return [ABIType.model_validate({"type": f"{array_type}[{length}]"})]
+        if array_type := getattr(returns.value, "id", None):
+            # TOOD: Is this an accurate way to define a fixed length array for ABI?
+            return [ABIType.model_validate({"type": f"{array_type}[{length}]"})]
 
     raise NotImplementedError(f"Unhandled return type {type(returns)}")
 
 
 def funcdef_state_mutability(funcdef: FunctionDef) -> str:
     """Get a FunctionDef's declared state mutability"""
     for decorator in funcdef_decorators(funcdef):
@@ -77,25 +75,25 @@
             "inputs": funcdef_inputs(func),
             "outputs": funcdef_outputs(func),
             "stateMutability": funcdef_state_mutability(func),
         }
     )
 
 
-def module_to_abi(module: Module) -> List[ABI]:
+def module_to_abi(module: Module) -> list[ABI]:
     """
     Create a list of MethodABIs from a Vyper AST Module instance.
     """
     abi = []
     for child in module.get_children():
         if isinstance(child, FunctionDef):
             abi.append(funcdef_to_abi(child))
     return abi
 
 
-def source_to_abi(source: str) -> List[ABI]:
+def source_to_abi(source: str) -> list[ABI]:
     """
     Given Vyper source code, return a list of Ape ABI elements needed for an external interface.
     This currently does not include complex types or events.
     """
     module = parse_to_ast(source)
     return module_to_abi(module)
```

### Comparing `ape-vyper-0.7.1/ape_vyper/compiler.py` & `ape-vyper-0.8.0/ape_vyper/compiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,45 @@
 import os
 import re
 import shutil
 import time
 from base64 import b64encode
+from collections import defaultdict
+from collections.abc import Iterable, Iterator
 from fnmatch import fnmatch
 from importlib import import_module
 from pathlib import Path
-from typing import Any, Dict, Iterable, Iterator, List, Optional, Sequence, Set, Tuple, Union, cast
+from typing import Any, Optional, Union, cast
 
 import vvm  # type: ignore
-from ape.api import PluginConfig
+from ape.api import PluginConfig, TraceAPI
 from ape.api.compiler import CompilerAPI
 from ape.exceptions import ContractLogicError
 from ape.logging import logger
-from ape.types import ContractSourceCoverage, ContractType, SourceTraceback, TraceFrame
-from ape.utils import GithubClient, cached_property, get_relative_path, pragma_str_to_specifier_set
+from ape.managers.project import ProjectManager
+from ape.types import ContractSourceCoverage, ContractType, SourceTraceback
+from ape.utils import (
+    cached_property,
+    get_full_extension,
+    get_relative_path,
+    pragma_str_to_specifier_set,
+)
+from ape.utils._github import _GithubClient
 from eth_pydantic_types import HexBytes
 from eth_utils import is_0x_prefixed
 from ethpm_types import ASTNode, PackageManifest, PCMap, SourceMapItem
 from ethpm_types.ast import ASTClassification
 from ethpm_types.contract_type import SourceMap
 from ethpm_types.source import Compiler, Content, ContractSource, Function, SourceLocation
+from evm_trace import TraceFrame
 from evm_trace.enums import CALL_OPCODES
+from evm_trace.geth import create_call_node_data
 from packaging.specifiers import InvalidSpecifier, SpecifierSet
 from packaging.version import Version
-from pydantic import field_serializer, field_validator
+from pydantic import field_serializer, field_validator, model_validator
 from vvm import compile_standard as vvm_compile_standard
 from vvm.exceptions import VyperError  # type: ignore
 
 from ape_vyper.ast import source_to_abi
 from ape_vyper.exceptions import (
     RUNTIME_ERROR_MAP,
     IntegerBoundsCheck,
@@ -48,28 +59,75 @@
 _RETURN_OPCODES = ("RETURN", "REVERT", "STOP")
 _FUNCTION_DEF = "FunctionDef"
 _FUNCTION_AST_TYPES = (_FUNCTION_DEF, "Name", "arguments")
 _EMPTY_REVERT_OFFSET = 18
 _NON_PAYABLE_STR = f"dev: {RuntimeErrorType.NONPAYABLE_CHECK.value}"
 Optimization = Union[str, bool]
 
+EVM_VERSION_DEFAULT = {
+    "0.2.15": "berlin",
+    "0.2.16": "berlin",
+    "0.3.0": "berlin",
+    "0.3.1": "berlin",
+    "0.3.2": "berlin",
+    "0.3.3": "berlin",
+    "0.3.4": "berlin",
+    "0.3.6": "berlin",
+    "0.3.7": "paris",
+    "0.3.8": "shanghai",
+    "0.3.9": "shanghai",
+    "0.3.10": "shanghai",
+}
+
+
+class Remapping(PluginConfig):
+    key: str
+    dependency_name: str
+    dependency_version: Optional[None] = None
+
+    @model_validator(mode="before")
+    @classmethod
+    def validate_str(cls, value):
+        if isinstance(value, str):
+            parts = value.split("=")
+            key = parts[0].strip()
+            value = parts[1].strip()
+            if "@" in value:
+                value_parts = value.split("@")
+                dep_name = value_parts[0].strip()
+                dep_version = value_parts[1].strip()
+            else:
+                dep_name = value
+                dep_version = None
+
+            return {"key": key, "dependency_name": dep_name, "dependency_version": dep_version}
+
+        return value
+
+    def __str__(self) -> str:
+        value = self.dependency_name
+        if _version := self.dependency_version:
+            value = f"{value}@{_version}"
+
+        return f"{self.key}={value}"
+
 
 class VyperConfig(PluginConfig):
     version: Optional[SpecifierSet] = None
     """
     Configure a version to use for all files,
     regardless of pragma.
     """
 
     evm_version: Optional[str] = None
     """
     The evm-version or hard-fork name.
     """
 
-    import_remapping: List[str] = []
+    import_remapping: list[Remapping] = []
     """
     Configuration of an import name mapped to a dependency listing.
     To use a specific version of a dependency, specify using ``@`` symbol.
 
     Usage example::
 
         vyper:
@@ -106,15 +164,15 @@
 
     Args:
         source (str): Vyper source code
 
     Returns:
         ``packaging.specifiers.SpecifierSet``, or None if no valid pragma is found.
     """
-    _version_pragma_patterns: Tuple[str, str] = (
+    _version_pragma_patterns: tuple[str, str] = (
         r"(?:\n|^)\s*#\s*@version\s*([^\n]*)",
         r"(?:\n|^)\s*#\s*pragma\s+version\s*([^\n]*)",
     )
 
     source_str = source if isinstance(source, str) else source.read_text()
     for pattern in _version_pragma_patterns:
         for match in re.finditer(pattern, source_str):
@@ -166,30 +224,30 @@
     ):
         return pragma_match.groups()[0]
 
     return None
 
 
 def get_optimization_pragma_map(
-    contract_filepaths: Sequence[Path], base_path: Path
-) -> Dict[str, Optimization]:
-    pragma_map: Dict[str, Optimization] = {}
+    contract_filepaths: Iterable[Path], base_path: Path
+) -> dict[str, Optimization]:
+    pragma_map: dict[str, Optimization] = {}
 
     for path in contract_filepaths:
         pragma = get_optimization_pragma(path) or True
         source_id = str(get_relative_path(path.absolute(), base_path.absolute()))
         pragma_map[source_id] = pragma
 
     return pragma_map
 
 
 def get_evm_version_pragma_map(
-    contract_filepaths: Sequence[Path], base_path: Path
-) -> Dict[str, str]:
-    pragmas: Dict[str, str] = {}
+    contract_filepaths: Iterable[Path], base_path: Path
+) -> dict[str, str]:
+    pragmas: dict[str, str] = {}
     for path in contract_filepaths:
         pragma = get_evmversion_pragma(path)
         if not pragma:
             continue
 
         source_id = str(get_relative_path(path.absolute(), base_path.absolute()))
         pragmas[source_id] = pragma
@@ -198,30 +256,25 @@
 
 
 class VyperCompiler(CompilerAPI):
     @property
     def name(self) -> str:
         return "vyper"
 
-    @property
-    def settings(self) -> VyperConfig:
-        return cast(VyperConfig, super().settings)
-
-    @property
-    def evm_version(self) -> Optional[str]:
-        return self.settings.evm_version
-
     def get_imports(
-        self, contract_filepaths: Sequence[Path], base_path: Optional[Path] = None
-    ) -> Dict[str, List[str]]:
-        base_path = (base_path or self.project_manager.contracts_folder).absolute()
-        import_map = {}
+        self,
+        contract_filepaths: Iterable[Path],
+        project: Optional[ProjectManager] = None,
+    ) -> dict[str, list[str]]:
+        pm = project or self.local_project
+        import_map: defaultdict = defaultdict(list)
+        dependencies = self.get_dependencies(project=pm)
         for path in contract_filepaths:
             content = path.read_text().splitlines()
-            source_id = str(get_relative_path(path.absolute(), base_path.absolute()))
+            source_id = str(get_relative_path(path.absolute(), pm.path.absolute()))
             for line in content:
                 if line.startswith("import "):
                     import_line_parts = line.replace("import ", "").split(" ")
                     suffix = import_line_parts[0].strip().replace(".", os.path.sep)
 
                 elif line.startswith("from ") and " import " in line:
                     import_line_parts = line.replace("from ", "").split(" ")
@@ -230,25 +283,52 @@
 
                 else:
                     # Not an import line
                     continue
 
                 # NOTE: Defaults to JSON (assuming from input JSON or a local JSON),
                 #  unless a Vyper file exists.
-                ext = "vy" if (base_path / f"{suffix}.vy").is_file() else "json"
+                import_source_id = None
+                if (pm.interfaces_folder.parent / f"{suffix}.vy").is_file():
+                    import_source_id = f"{suffix}.vy"
+
+                elif (pm.interfaces_folder.parent / f"{suffix}.json").is_file():
+                    import_source_id = f"{suffix}.json"
+
+                elif suffix.startswith(f"vyper{os.path.sep}"):
+                    # Vyper built-ins.
+                    import_source_id = f"{suffix}.json"
+
+                elif suffix.split(os.path.sep)[0] in dependencies:
+                    dependency_name = suffix.split(os.path.sep)[0]
+                    filestem = suffix.replace(f"{dependency_name}{os.path.sep}", "")
+                    for version_str, dep_project in pm.dependencies[dependency_name].items():
+                        dependency = pm.dependencies.get_dependency(dependency_name, version_str)
+                        path_id = dependency.package_id.replace("/", "_")
+                        dependency_source_prefix = (
+                            f"{get_relative_path(dep_project.contracts_folder, dep_project.path)}"
+                        )
+                        source_id_stem = f"{dependency_source_prefix}{os.path.sep}{filestem}"
+                        for ext in (".vy", ".json"):
+                            if f"{source_id_stem}{ext}" in dep_project.sources:
+                                import_source_id = os.path.sep.join(
+                                    (path_id, version_str, f"{source_id_stem}{ext}")
+                                )
+                                break
+
+                else:
+                    logger.error(f"Unable to find dependency {suffix}")
+                    continue
 
-                import_source_id = f"{suffix}.{ext}"
-                if source_id not in import_map:
-                    import_map[source_id] = [import_source_id]
-                elif import_source_id not in import_map[source_id]:
+                if import_source_id and import_source_id not in import_map[source_id]:
                     import_map[source_id].append(import_source_id)
 
-        return import_map
+        return dict(import_map)
 
-    def get_versions(self, all_paths: Sequence[Path]) -> Set[str]:
+    def get_versions(self, all_paths: Iterable[Path]) -> set[str]:
         versions = set()
         for path in all_paths:
             if version_spec := get_version_pragma_spec(path):
                 try:
                     # Make sure we have the best compiler available to compile this
                     version_iter = version_spec.filter(self.available_versions)
 
@@ -274,22 +354,22 @@
         except ModuleNotFoundError:
             return None
 
         version_str = getattr(vyper, "__version__", None)
         return Version(version_str) if version_str else None
 
     @cached_property
-    def available_versions(self) -> List[Version]:
+    def available_versions(self) -> list[Version]:
         # NOTE: Package version should already be included in available versions
         max_retries = 10
         buffer = 1
         times_tried = 0
         result = []
         headers = None
-        if token := os.environ.get(GithubClient.TOKEN_KEY):
+        if token := os.environ.get(_GithubClient.TOKEN_KEY):
             auth = b64encode(token.encode()).decode()
             headers = {"Authorization": f"Basic {auth}"}
 
         while times_tried < max_retries:
             try:
                 result = vvm.get_installable_vyper_versions(headers=headers)
             except ConnectionError as err:
@@ -313,15 +393,15 @@
 
             # Succeeded.
             break
 
         return result
 
     @property
-    def installed_versions(self) -> List[Version]:
+    def installed_versions(self) -> list[Version]:
         # Doing this so it prefers package version
         package_version = self.package_version
         versions = [package_version] if package_version else []
         # currently package version is [] this should be ok
         return versions + vvm.get_installed_vyper_versions()
 
     @cached_property
@@ -329,121 +409,154 @@
         try:
             from vyper.cli import vyper_json  # type: ignore
 
             return vyper_json
         except ImportError:
             return None
 
-    @property
-    def config_version_pragma(self) -> Optional[SpecifierSet]:
-        if version := self.settings.version:
-            return version
+    def get_dependencies(
+        self, project: Optional[ProjectManager] = None
+    ) -> dict[str, ProjectManager]:
+        pm = project or self.local_project
+        config = self.get_config(pm)
+        dependencies: dict[str, ProjectManager] = {}
+        handled: set[str] = set()
+
+        # Add remappings from config.
+        for remapping in config.import_remapping:
+            name = remapping.dependency_name
+            if not (_version := remapping.dependency_version):
+                versions = pm.dependencies[name]
+                if len(versions) == 1:
+                    _version = versions[0]
+                else:
+                    continue
 
-        return None
+            dependency = pm.dependencies.get_dependency(name, _version)
+            dep_id = f"{dependency.name}_{dependency.version}"
+            if dep_id in handled:
+                continue
 
-    @property
-    def remapped_manifests(self) -> Dict[str, PackageManifest]:
-        """
-        Interface import manifests.
-        """
+            handled.add(dep_id)
 
-        dependencies: Dict[str, PackageManifest] = {}
+            try:
+                dependency.compile()
+            except Exception as err:
+                logger.warning(
+                    f"Failed to compile dependency '{dependency.name}' @ '{dependency.version}'.\n"
+                    f"Reason: {err}"
+                )
+                continue
 
-        for remapping in self.settings.import_remapping:
-            key, value = remapping.split("=")
+            dependencies[remapping.key] = dependency.project
 
-            if remapping in dependencies:
-                dependency = dependencies[remapping]
-            else:
-                parts = value.split("@")
-                dep_name = parts[0]
-                dependency_versions = self.project_manager.dependencies[dep_name]
-                if not dependency_versions:
-                    raise VyperCompileError(f"Missing dependency '{dep_name}'.")
-
-                elif len(parts) == 1 and len(dependency_versions) < 2:
-                    # Use only version.
-                    version = list(dependency_versions.keys())[0]
+        # Add auto-remapped dependencies.
+        for dependency in pm.dependencies.specified:
+            dep_id = f"{dependency.name}_{dependency.version}"
+            if dep_id in handled:
+                continue
 
-                elif parts[1] not in dependency_versions:
-                    raise VyperCompileError(f"Missing dependency '{dep_name}'.")
+            handled.add(dep_id)
 
-                else:
-                    version = parts[1]
+            try:
+                dependency.compile()
+            except Exception as err:
+                logger.warning(
+                    f"Failed to compile dependency '{dependency.name}' @ '{dependency.version}'.\n"
+                    f"Reason: {err}"
+                )
+                continue
 
-                dependency = dependency_versions[version].compile()
-                dependencies[remapping] = dependency
+            dependencies[dependency.name] = dependency.project
 
         return dependencies
 
-    @property
-    def import_remapping(self) -> Dict[str, Dict]:
+    def get_import_remapping(self, project: Optional[ProjectManager] = None) -> dict[str, dict]:
         """
         Configured interface imports from dependencies.
         """
-
-        interfaces = {}
-
-        for remapping in self.settings.import_remapping:
-            key, _ = remapping.split("=")
-            for name, ct in (self.remapped_manifests[remapping].contract_types or {}).items():
-                interfaces[f"{key}/{name}.json"] = {
-                    "abi": [x.model_dump(mode="json", by_alias=True) for x in ct.abi]
-                }
+        pm = project or self.local_project
+        dependencies = self.get_dependencies(project=pm)
+        interfaces: dict[str, dict] = {}
+        for key, dependency_project in dependencies.items():
+            manifest = dependency_project.manifest
+            for name, ct in (manifest.contract_types or {}).items():
+                filename = f"{key}/{name}.json"
+                abi_list = [x.model_dump(mode="json", by_alias=True) for x in ct.abi]
+                interfaces[filename] = {"abi": abi_list}
 
         return interfaces
 
     def classify_ast(self, _node: ASTNode):
         if _node.ast_type in _FUNCTION_AST_TYPES:
             _node.classification = ASTClassification.FUNCTION
 
         for child in _node.children:
             self.classify_ast(child)
 
     def compile(
-        self, contract_filepaths: Sequence[Path], base_path: Optional[Path] = None
-    ) -> List[ContractType]:
-        contract_types = []
-        base_path = base_path or self.config_manager.contracts_folder
+        self,
+        contract_filepaths: Iterable[Path],
+        project: Optional[ProjectManager] = None,
+        settings: Optional[dict] = None,
+    ) -> Iterator[ContractType]:
+        pm = project or self.local_project
+        settings = settings or {}
         sources = [p for p in contract_filepaths if p.parent.name != "interfaces"]
-        version_map = self.get_version_map(sources)
-        compiler_data = self._get_compiler_arguments(version_map, base_path)
-        all_settings = self.get_compiler_settings(sources, base_path=base_path)
-        contract_versions: Dict[str, Tuple[Version, str]] = {}
+        contract_types: list[ContractType] = []
+        if version := settings.get("version", None):
+            version_map = {Version(version): set(sources)}
+        else:
+            version_map = self.get_version_map(sources, project=project)
+
+        compiler_data = self._get_compiler_arguments(version_map, project=pm)
+        all_settings: dict = self.get_compiler_settings(
+            sources, project=project, **(settings or {})
+        )
+        contract_versions: dict[str, tuple[Version, str]] = {}
+        import_remapping = self.get_import_remapping(project=pm)
 
         for vyper_version, version_settings in all_settings.items():
-            for settings_key, settings in version_settings.items():
-                source_ids = settings["outputSelection"]
-                optimization_paths = {p: base_path / p for p in source_ids}
-                input_json = {
+            for settings_key, settings_set in version_settings.items():
+                source_ids = settings_set["outputSelection"]
+                optimization_paths = {p: pm.path / p for p in source_ids}
+                input_json: dict = {
                     "language": "Vyper",
-                    "settings": settings,
+                    "settings": settings_set,
                     "sources": {
                         s: {"content": p.read_text()} for s, p in optimization_paths.items()
                     },
                 }
 
-                if interfaces := self.import_remapping:
+                if interfaces := import_remapping:
                     input_json["interfaces"] = interfaces
 
+                # Output compiler details.
+                keys = (
+                    "\n\t".join(sorted([x for x in input_json.get("sources", {}).keys()]))
+                    or "No input."
+                )
+                log_str = f"Compiling using Vyper compiler '{vyper_version}'.\nInput:\n\t{keys}"
+                logger.info(log_str)
+
                 vyper_binary = compiler_data[vyper_version]["vyper_binary"]
                 try:
                     result = vvm_compile_standard(
                         input_json,
-                        base_path=base_path,
+                        base_path=pm.path,
                         vyper_version=vyper_version,
                         vyper_binary=vyper_binary,
                     )
                 except VyperError as err:
                     raise VyperCompileError(err) from err
 
                 for source_id, output_items in result["contracts"].items():
                     content = {
                         i + 1: ln
-                        for i, ln in enumerate((base_path / source_id).read_text().splitlines())
+                        for i, ln in enumerate((pm.path / source_id).read_text().splitlines())
                     }
                     for name, output in output_items.items():
                         # De-compress source map to get PC POS map.
                         ast = ASTNode.model_validate(result["sources"][source_id]["ast"])
                         self.classify_ast(ast)
 
                         # Track function offsets.
@@ -486,17 +599,18 @@
                             pcmap=pcmap,
                             userdoc=output["userdoc"],
                             devdoc=output["devdoc"],
                             dev_messages=dev_messages,
                         )
                         contract_types.append(contract_type)
                         contract_versions[name] = (vyper_version, settings_key)
+                        yield contract_type
 
         # Output compiler data used.
-        compilers_used: Dict[Version, Dict[str, Compiler]] = {}
+        compilers_used: dict[Version, dict[str, Compiler]] = {}
         for ct in contract_types:
             if not ct.name:
                 # Won't happen, but just for mypy.
                 continue
 
             ct_version, ct_settings_key = contract_versions[ct.name]
             settings = all_settings[ct_version][ct_settings_key]
@@ -527,28 +641,28 @@
             compiler
             for optimization_settings in compilers_used.values()
             for compiler in optimization_settings.values()
         ]
 
         # NOTE: This method handles merging contractTypes and filtered out
         #   no longer used Compilers.
-        self.project_manager.local_project.add_compiler_data(compilers_ls)
-
-        return contract_types
+        pm.add_compiler_data(compilers_ls)
 
-    def compile_code(self, code: str, base_path: Optional[Path] = None, **kwargs) -> ContractType:
-        base_path = base_path or self.project_manager.contracts_folder
+    def compile_code(
+        self, code: str, project: Optional[ProjectManager] = None, **kwargs
+    ) -> ContractType:
+        pm = project or self.local_project
 
         # Figure out what compiler version we need for this contract...
         version = self._source_vyper_version(code)
         # ...and install it if necessary
         _install_vyper(version)
 
         try:
-            result = vvm.compile_source(code, base_path=base_path, vyper_version=version)
+            result = vvm.compile_source(code, base_path=pm.path, vyper_version=version)
         except Exception as err:
             raise VyperCompileError(str(err)) from err
 
         output = result.get("<stdin>", {})
         return ContractType(
             abi=output["abi"],
             deploymentBytecode={"bytecode": output["bytecode"]},
@@ -560,90 +674,97 @@
         """Given source code, figure out which Vyper version to use"""
         version_spec = get_version_pragma_spec(code)
 
         def first_full_release(versions: Iterable[Version]) -> Optional[Version]:
             for vers in versions:
                 if not vers.is_devrelease and not vers.is_postrelease and not vers.is_prerelease:
                     return vers
+
             return None
 
         if version_spec is None:
             if version := first_full_release(self.installed_versions + self.available_versions):
                 return version
+
             raise VyperInstallError("No available version.")
 
         return next(version_spec.filter(self.available_versions))
 
-    def _flatten_source(
-        self, path: Path, base_path: Optional[Path] = None, raw_import_name: Optional[str] = None
-    ) -> str:
-        base_path = base_path or self.config_manager.contracts_folder
+    def _flatten_source(self, path: Path, project: Optional[ProjectManager] = None) -> str:
+        pm = project or self.local_project
 
         # Get the non stdlib import paths for our contracts
         imports = list(
             filter(
                 lambda x: not x.startswith("vyper/"),
-                [y for x in self.get_imports([path], base_path).values() for y in x],
+                [y for x in self.get_imports((path,), project=pm).values() for y in x],
             )
         )
 
-        dependencies: Dict[str, PackageManifest] = {}
-        for key, manifest in self.remapped_manifests.items():
+        dependencies: dict[str, PackageManifest] = {}
+        dependency_projects = self.get_dependencies(project=pm)
+        for key, dependency_project in dependency_projects.items():
             package = key.split("=")[0]
-
+            base = dependency_project.path if hasattr(dependency_project, "path") else package
+            manifest = dependency_project.manifest
             if manifest.sources is None:
                 continue
 
             for source_id in manifest.sources.keys():
-                import_match = f"{package}/{source_id}"
+                import_match = f"{base}/{source_id}"
                 dependencies[import_match] = manifest
 
-        flattened_source = ""
         interfaces_source = ""
-        og_source = (base_path / path).read_text()
+        og_source = (pm.path / path).read_text()
 
         # Get info about imports and source meta
         aliases = extract_import_aliases(og_source)
         pragma, source_without_meta = extract_meta(og_source)
         stdlib_imports, _, source_without_imports = extract_imports(source_without_meta)
 
         for import_path in sorted(imports):
-            import_file = base_path / import_path
+            import_file = None
+            for base in (pm.path, pm.interfaces_folder):
+                for opt in {import_path, import_path.replace(f"interfaces{os.path.sep}", "")}:
+                    try_import_file = base / opt
+                    if try_import_file.is_file():
+                        import_file = try_import_file
+                        break
+
+            if import_file is None:
+                import_file = pm.path / import_path
 
             # Vyper imported interface names come from their file names
             file_name = iface_name_from_file(import_file)
             # If we have a known alias, ("import X as Y"), use the alias as interface name
             iface_name = aliases[file_name] if file_name in aliases else file_name
 
-            # We need to compare without extensions because sometimes they're made up for some
-            # reason.  TODO: Cleaner way to deal with this?
-            def _match_source(import_path: str) -> Optional[PackageManifest]:
-                import_path_name = ".".join(import_path.split(".")[:-1])
+            def _match_source(imp_path: str) -> Optional[PackageManifest]:
                 for source_path in dependencies.keys():
-                    if source_path.startswith(import_path_name):
+                    if source_path.endswith(imp_path):
                         return dependencies[source_path]
+
                 return None
 
             if matched_source := _match_source(import_path):
                 if not matched_source.contract_types:
                     continue
 
                 abis = [
                     el
                     for k in matched_source.contract_types.keys()
                     for el in matched_source.contract_types[k].abi
                 ]
                 interfaces_source += generate_interface(abis, iface_name)
                 continue
 
-            # Vyper imported interface names come from their file names
-            file_name = iface_name_from_file(import_file)
             # Generate an ABI from the source code
-            abis = source_to_abi(import_file.read_text())
-            interfaces_source += generate_interface(abis, iface_name)
+            elif import_file.is_file():
+                abis = source_to_abi(import_file.read_text())
+                interfaces_source += generate_interface(abis, iface_name)
 
         def no_nones(it: Iterable[Optional[str]]) -> Iterable[str]:
             # Type guard like generator to remove Nones and make mypy happy
             for el in it:
                 if el is not None:
                     yield el
 
@@ -656,31 +777,41 @@
         def format_source(source: str) -> str:
             while "\n\n\n\n" in source:
                 source = source.replace("\n\n\n\n", "\n\n\n")
             return source
 
         return format_source(flattened_source)
 
-    def flatten_contract(self, path: Path, base_path: Optional[Path] = None) -> Content:
+    def flatten_contract(
+        self,
+        path: Path,
+        project: Optional[ProjectManager] = None,
+        **kwargs,
+    ) -> Content:
         """
         Returns the flattened contract suitable for compilation or verification as a single file
         """
-        source = self._flatten_source(path, base_path, path.name)
-        return Content({i: ln for i, ln in enumerate(source.splitlines())})
+        pm = project or self.local_project
+        src = self._flatten_source(path, project=pm)
+        return Content({i: ln for i, ln in enumerate(src.splitlines())})
 
     def get_version_map(
-        self, contract_filepaths: Sequence[Path], base_path: Optional[Path] = None
-    ) -> Dict[Version, Set[Path]]:
-        version_map: Dict[Version, Set[Path]] = {}
-        source_path_by_version_spec: Dict[SpecifierSet, Set[Path]] = {}
+        self,
+        contract_filepaths: Iterable[Path],
+        project: Optional[ProjectManager] = None,
+    ) -> dict[Version, set[Path]]:
+        pm = project or self.local_project
+        config = self.get_config(pm)
+        version_map: dict[Version, set[Path]] = {}
+        source_path_by_version_spec: dict[SpecifierSet, set[Path]] = {}
         source_paths_without_pragma = set()
 
         # Sort contract_filepaths to promote consistent, reproduce-able behavior
         for path in sorted(contract_filepaths):
-            if config_spec := self.config_version_pragma:
+            if config_spec := config.version:
                 _safe_append(source_path_by_version_spec, config_spec, path)
             elif pragma := get_version_pragma_spec(path):
                 _safe_append(source_path_by_version_spec, pragma, path)
             else:
                 source_paths_without_pragma.add(path)
 
         # Install all requires versions *before* building map
@@ -719,51 +850,62 @@
             # If we have no installed versions by this point, we need to install one.
             # This happens when there are no pragmas in any sources and no vyper installations.
             _install_vyper(max(self.available_versions))
 
         # Handle no-pragma sources
         if source_paths_without_pragma:
             max_installed_vyper_version = (
-                max(version_map) if version_map else max(self.installed_versions)
+                max(version_map)
+                if version_map
+                else max(v for v in self.installed_versions if not v.pre)
             )
             _safe_append(version_map, max_installed_vyper_version, source_paths_without_pragma)
 
         return version_map
 
     def get_compiler_settings(
-        self, contract_filepaths: Sequence[Path], base_path: Optional[Path] = None
-    ) -> Dict[Version, Dict]:
+        self,
+        contract_filepaths: Iterable[Path],
+        project: Optional[ProjectManager] = None,
+        **kwargs,
+    ) -> dict[Version, dict]:
+        pm = project or self.local_project
         valid_paths = [p for p in contract_filepaths if p.suffix == ".vy"]
-        contracts_path = base_path or self.config_manager.contracts_folder
-        files_by_vyper_version = self.get_version_map(valid_paths, base_path=contracts_path)
+        if version := kwargs.pop("version", None):
+            files_by_vyper_version = {Version(version): set(valid_paths)}
+        else:
+            files_by_vyper_version = self.get_version_map(valid_paths, project=pm)
+
         if not files_by_vyper_version:
             return {}
 
-        compiler_data = self._get_compiler_arguments(files_by_vyper_version, contracts_path)
+        compiler_data = self._get_compiler_arguments(files_by_vyper_version, project=pm)
         settings = {}
         for version, data in compiler_data.items():
             source_paths = list(files_by_vyper_version.get(version, []))
             if not source_paths:
                 continue
 
-            output_selection: Dict[str, Set[str]] = {}
-            optimizations_map = get_optimization_pragma_map(source_paths, contracts_path)
-            evm_version_map = get_evm_version_pragma_map(source_paths, contracts_path)
-            default_evm_version = data.get("evm_version", data.get("evmVersion"))
+            output_selection: dict[str, set[str]] = {}
+            optimizations_map = get_optimization_pragma_map(source_paths, pm.path)
+            evm_version_map = get_evm_version_pragma_map(source_paths, pm.path)
+            default_evm_version = data.get(
+                "evm_version", data.get("evmVersion")
+            ) or EVM_VERSION_DEFAULT.get(version.base_version)
             for source_path in source_paths:
-                source_id = str(get_relative_path(source_path.absolute(), contracts_path))
+                source_id = str(get_relative_path(source_path.absolute(), pm.path))
                 optimization = optimizations_map.get(source_id, True)
                 evm_version = evm_version_map.get(source_id, default_evm_version)
                 settings_key = f"{optimization}%{evm_version}".lower()
                 if settings_key not in output_selection:
                     output_selection[settings_key] = {source_id}
                 else:
                     output_selection[settings_key].add(source_id)
 
-            version_settings: Dict[str, Dict] = {}
+            version_settings: dict[str, dict] = {}
             for settings_key, selection in output_selection.items():
                 optimization, evm_version = settings_key.split("%")
                 if optimization == "true":
                     optimization = True
                 elif optimization == "false":
                     optimization = False
 
@@ -821,15 +963,15 @@
                 else None
             )
             _function_coverage.profile_statement(pc_int, location=location, tag=tag)
 
         # Some statements are too difficult to know right away where they belong,
         # such as statement related to kwarg-default auto-generated implicit lookups.
         # function_name -> (pc, location)
-        pending_statements: Dict[str, List[Tuple[int, SourceLocation]]] = {}
+        pending_statements: dict[str, list[tuple[int, SourceLocation]]] = {}
 
         for pc, item in contract_source.pcmap.root.items():
             pc_int = int(pc)
             if pc_int < 0:
                 continue
 
             location: Optional[SourceLocation]
@@ -903,15 +1045,15 @@
                 ]
                 longest_abi = max(matching_abis, key=lambda x: len(x.inputs))
                 autogenerated_abis = [
                     abi for abi in matching_abis if abi.selector != longest_abi.selector
                 ]
                 # Sort the autogenerated ABIs so we can loop through them in the correct order.
                 autogenerated_abis.sort(key=lambda a: len(a.inputs))
-                buckets: Dict[str, List[Tuple[int, SourceLocation]]] = {
+                buckets: dict[str, list[tuple[int, SourceLocation]]] = {
                     a.selector: [] for a in autogenerated_abis
                 }
                 selector_index = 0
                 selector = autogenerated_abis[0].selector
                 # Must loop through PCs from smallest to greatest for this to work.
                 pending_ls.sort()
                 jump_threshold = 10
@@ -952,22 +1094,26 @@
             if method.selector not in [fn.full_name for fn in contract_coverage.functions]:
                 if _exclude_fn(method.name):
                     return
 
                 # Auto-getter found. Profile function without statements.
                 contract_coverage.include(method.name, method.selector)
 
-    def _get_compiler_arguments(self, version_map: Dict, base_path: Path) -> Dict[Version, Dict]:
-        base_path = base_path or self.project_manager.contracts_folder
+    def _get_compiler_arguments(
+        self, version_map: dict, project: Optional[ProjectManager] = None
+    ) -> dict[Version, dict]:
+        pm = project or self.local_project
+        config = self.get_config(pm)
+        evm_version = config.evm_version
         arguments_map = {}
         for vyper_version, source_paths in version_map.items():
             bin_arg = self._get_vyper_bin(vyper_version)
             arguments_map[vyper_version] = {
-                "base_path": str(base_path),
-                "evm_version": self.evm_version,
+                "base_path": f"{pm.path}",
+                "evm_version": evm_version,
                 "vyper_version": str(vyper_version),
                 "vyper_binary": bin_arg,
             }
 
         return arguments_map
 
     def _get_vyper_bin(self, vyper_version: Version):
@@ -1000,135 +1146,133 @@
                     break
 
         if not error_type:
             # Not a builtin compiler error; cannot enrich.
             return err
 
         runtime_error_cls = RUNTIME_ERROR_MAP[error_type]
-        tx_kwargs: Dict = {
+        tx_kwargs: dict = {
             "contract_address": err.contract_address,
             "source_traceback": err.source_traceback,
             "trace": err.trace,
             "txn": err.txn,
         }
         return (
             runtime_error_cls(err_str.split(" ")[0], **tx_kwargs)
             if runtime_error_cls == IntegerBoundsCheck
             else runtime_error_cls(**tx_kwargs)
         )
 
     def trace_source(
-        self, contract_type: ContractType, trace: Iterator[TraceFrame], calldata: HexBytes
+        self, contract_source: ContractSource, trace: TraceAPI, calldata: HexBytes
     ) -> SourceTraceback:
-        if source_contract_type := self.project_manager._create_contract_source(contract_type):
-            return self._get_traceback(source_contract_type, trace, calldata)
-
-        return SourceTraceback.model_validate([])
+        frames = trace.get_raw_frames()
+        return self._get_traceback(contract_source, frames, calldata)
 
     def _get_traceback(
         self,
         contract_src: ContractSource,
-        trace: Iterator[TraceFrame],
+        frames: Iterator[dict],
         calldata: HexBytes,
         previous_depth: Optional[int] = None,
     ) -> SourceTraceback:
         traceback = SourceTraceback.model_validate([])
         method_id = HexBytes(calldata[:4])
         completed = False
         pcmap = PCMap.model_validate({})
 
-        for frame in trace:
-            if frame.op in CALL_OPCODES:
-                start_depth = frame.depth
+        for frame in frames:
+            if frame["op"] in CALL_OPCODES:
+                start_depth = frame["depth"]
                 called_contract, sub_calldata = self._create_contract_from_call(frame)
                 if called_contract:
-                    ext = Path(called_contract.source_id).suffix
+                    ext = get_full_extension(Path(called_contract.source_id))
                     if ext.endswith(".vy"):
                         # Called another Vyper contract.
                         sub_trace = self._get_traceback(
-                            called_contract, trace, sub_calldata, previous_depth=frame.depth
+                            called_contract, frames, sub_calldata, previous_depth=frame["depth"]
                         )
                         traceback.extend(sub_trace)
 
                     else:
                         # Not a Vyper contract!
                         compiler = self.compiler_manager.registered_compilers[ext]
                         try:
                             sub_trace = compiler.trace_source(
-                                called_contract.contract_type, trace, sub_calldata
+                                called_contract.contract_type, frames, sub_calldata
                             )
                             traceback.extend(sub_trace)
                         except NotImplementedError:
                             # Compiler not supported. Fast forward out of this call.
-                            for fr in trace:
-                                if fr.depth <= start_depth:
+                            for fr in frames:
+                                if fr["depth"] <= start_depth:
                                     break
 
                             continue
 
                 else:
                     # Contract not found. Fast forward out of this call.
-                    for fr in trace:
-                        if fr.depth <= start_depth:
+                    for fr in frames:
+                        if fr["depth"] <= start_depth:
                             break
 
                     continue
 
-            elif frame.op in _RETURN_OPCODES:
+            elif frame["op"] in _RETURN_OPCODES:
                 # For the base CALL, don't mark as completed until trace is gone.
                 # This helps in cases where we failed to detect a subcall properly.
                 completed = previous_depth is not None
 
             pcs_to_try_adding = set()
-            if "PUSH" in frame.op and frame.pc in contract_src.pcmap:
+            if "PUSH" in frame["op"] and frame["pc"] in contract_src.pcmap:
                 # Check if next op is SSTORE to properly use AST from push op.
-                next_frame: Optional[TraceFrame] = frame
-                loc = contract_src.pcmap[frame.pc]
-                pcs_to_try_adding.add(frame.pc)
-
-                while next_frame and "PUSH" in next_frame.op:
-                    next_frame = next(trace, None)
-                    if next_frame and "PUSH" in next_frame.op:
-                        pcs_to_try_adding.add(next_frame.pc)
+                next_frame: Optional[dict] = frame
+                loc = contract_src.pcmap[frame["pc"]]
+                pcs_to_try_adding.add(frame["pc"])
+
+                while next_frame and "PUSH" in next_frame["op"]:
+                    next_frame = next(frames, None)
+                    if next_frame and "PUSH" in next_frame["op"]:
+                        pcs_to_try_adding.add(next_frame["pc"])
 
                 is_non_payable_hit = False
-                if next_frame and next_frame.op == "SSTORE":
+                if next_frame and next_frame["op"] == "SSTORE":
                     push_location = tuple(loc["location"])  # type: ignore
-                    pcmap = PCMap.model_validate({next_frame.pc: {"location": push_location}})
+                    pcmap = PCMap.model_validate({next_frame["pc"]: {"location": push_location}})
 
-                elif next_frame and next_frame.op in _RETURN_OPCODES:
+                elif next_frame and next_frame["op"] in _RETURN_OPCODES:
                     completed = True
 
                 else:
                     pcmap = contract_src.pcmap
                     dev_val = str((loc.get("dev") or "")).replace("dev: ", "")
                     is_non_payable_hit = dev_val == RuntimeErrorType.NONPAYABLE_CHECK.value
 
                 if not is_non_payable_hit and next_frame:
                     frame = next_frame
 
             else:
                 pcmap = contract_src.pcmap
 
-            pcs_to_try_adding.add(frame.pc)
+            pcs_to_try_adding.add(frame["pc"])
             pcs_to_try_adding = {pc for pc in pcs_to_try_adding if pc in pcmap}
             if not pcs_to_try_adding:
                 if (
-                    frame.op == "REVERT"
-                    and frame.pc + 1 in pcmap
+                    frame["op"] == "REVERT"
+                    and frame["pc"] + 1 in pcmap
                     and RuntimeErrorType.USER_ASSERT.value
-                    in str(pcmap[frame.pc + 1].get("dev", ""))
+                    in str(pcmap[frame["pc"] + 1].get("dev", ""))
                 ):
                     # Not sure why this happens. Maybe an off-by-1 bug in Vyper.
-                    pcs_to_try_adding.add(frame.pc + 1)
+                    pcs_to_try_adding.add(frame["pc"] + 1)
 
-            pc_groups: List[List] = []
+            pc_groups: list[list] = []
             for pc in pcs_to_try_adding:
                 location = (
-                    cast(Tuple[int, int, int, int], tuple(pcmap[pc].get("location") or [])) or None
+                    cast(tuple[int, int, int, int], tuple(pcmap[pc].get("location") or [])) or None
                 )
                 dev_item = pcmap[pc].get("dev", "")
                 dev = str(dev_item).replace("dev: ", "")
 
                 done = False
                 for group in pc_groups:
                     if group[0] != location:
@@ -1195,17 +1339,17 @@
 
                 if (
                     not traceback.last
                     or traceback.last.closure.full_name != function.full_name
                     or not isinstance(traceback.last.closure, Function)
                 ):
                     depth = (
-                        frame.depth + 1
-                        if traceback.last and traceback.last.depth == frame.depth
-                        else frame.depth
+                        frame["depth"] + 1
+                        if traceback.last and traceback.last.depth == frame["depth"]
+                        else frame["depth"]
                     )
 
                     traceback.add_jump(
                         location,
                         function,
                         depth,
                         pcs=pcs,
@@ -1227,35 +1371,53 @@
                                 last_statement.type = dev_messages[lineno]
 
             if completed:
                 break
 
         return traceback
 
+    def _create_contract_from_call(self, frame: dict) -> tuple[Optional[ContractSource], HexBytes]:
+        evm_frame = TraceFrame(**frame)
+        data = create_call_node_data(evm_frame)
+        calldata = data.get("calldata", HexBytes(""))
+        if not (address := (data.get("address", evm_frame.contract_address) or None)):
+            return None, calldata
+
+        try:
+            address = self.provider.network.ecosystem.decode_address(address)
+        except Exception:
+            return None, calldata
+
+        if address not in self.chain_manager.contracts:
+            return None, calldata
 
-def _safe_append(data: Dict, version: Union[Version, SpecifierSet], paths: Union[Path, Set]):
+        called_contract = self.chain_manager.contracts[address]
+        return self.local_project._create_contract_source(called_contract), calldata
+
+
+def _safe_append(data: dict, version: Union[Version, SpecifierSet], paths: Union[Path, set]):
     if isinstance(paths, Path):
         paths = {paths}
     if version in data:
         data[version] = data[version].union(paths)
     else:
         data[version] = paths
 
 
 def _is_revert_jump(op: str, value: Optional[int], revert_pc: int) -> bool:
     return op == "JUMPI" and value is not None and value == revert_pc
 
 
-def _has_empty_revert(opcodes: List[str]) -> bool:
+def _has_empty_revert(opcodes: list[str]) -> bool:
     return (len(opcodes) > 12 and opcodes[-13] == "JUMPDEST" and opcodes[-9] == "REVERT") or (
         len(opcodes) > 4 and opcodes[-5] == "JUMPDEST" and opcodes[-1] == "REVERT"
     )
 
 
-def _get_pcmap(bytecode: Dict) -> PCMap:
+def _get_pcmap(bytecode: dict) -> PCMap:
     # Find the non payable value check.
     src_info = bytecode["sourceMapFull"]
     pc_data = {pc: {"location": ln} for pc, ln in src_info["pc_pos_map"].items()}
     if not pc_data:
         return PCMap.model_validate({})
 
     # Apply other errors.
@@ -1312,21 +1474,21 @@
             pc_data[err_pc]["dev"] = f"dev: {error_str}"
         else:
             pc_data[err_pc] = {"dev": f"dev: {error_str}", "location": location}
 
     return PCMap.model_validate(pc_data)
 
 
-def _get_legacy_pcmap(ast: ASTNode, src_map: List[SourceMapItem], opcodes: List[str]):
+def _get_legacy_pcmap(ast: ASTNode, src_map: list[SourceMapItem], opcodes: list[str]):
     """
     For Vyper versions <= 0.3.7, allows us to still get a PCMap.
     """
 
     pc = 0
-    pc_map_list: List[Tuple[int, Dict[str, Optional[Any]]]] = []
+    pc_map_list: list[tuple[int, dict[str, Optional[Any]]]] = []
     last_value = None
     revert_pc = -1
     if _has_empty_revert(opcodes):
         revert_pc = _get_revert_pc(opcodes)
 
     processed_opcodes = []
 
@@ -1353,15 +1515,15 @@
         # Also check for compiler runtime error handling.
         # Runtime error locations are marked in the PCMap for further analysis.
         if src.start is not None and src.length is not None:
             stmt = ast.get_node(src)
             if stmt:
                 # Add located item.
                 line_nos = list(stmt.line_numbers)
-                item: Dict = {"location": line_nos}
+                item: dict = {"location": line_nos}
                 is_revert_jump = _is_revert_jump(op, last_value, revert_pc)
                 if op == "REVERT" or is_revert_jump:
                     dev = None
                     if stmt.ast_type in ("AugAssign", "BinOp"):
                         # SafeMath
                         for node in stmt.children:
                             dev = RuntimeErrorType.from_operator(node.ast_type)
@@ -1403,15 +1565,15 @@
                     item["dev"] = f"dev: {RuntimeErrorType.USER_ASSERT.value}"
                     break
 
     pcmap_data = dict(pc_map_list)
     return PCMap.model_validate(pcmap_data)
 
 
-def _find_non_payable_check(src_map: List[SourceMapItem], opcodes: List[str]) -> Optional[int]:
+def _find_non_payable_check(src_map: list[SourceMapItem], opcodes: list[str]) -> Optional[int]:
     pc = 0
     revert_pc = -1
     if _has_empty_revert(opcodes):
         revert_pc = _get_revert_pc(opcodes)
 
     while src_map and opcodes:
         op = opcodes.pop(0)
@@ -1424,37 +1586,37 @@
 
         if _is_non_payable_check(opcodes, op, revert_pc):
             return pc
 
     return None
 
 
-def _is_non_payable_check(opcodes: List[str], op: str, revert_pc: int) -> bool:
+def _is_non_payable_check(opcodes: list[str], op: str, revert_pc: int) -> bool:
     return (
         len(opcodes) >= 3
         and op == "CALLVALUE"
         and "PUSH" in opcodes[0]
         and is_0x_prefixed(opcodes[1])
         and _is_revert_jump(opcodes[2], int(opcodes[1], 16), revert_pc)
     )
 
 
-def _get_revert_pc(opcodes: List[str]) -> int:
+def _get_revert_pc(opcodes: list[str]) -> int:
     """
     Starting in vyper 0.2.14, reverts without a reason string are optimized
     with a jump to the "end" of the bytecode.
     """
     return (
         len(opcodes)
         + sum(int(i[4:]) - 1 for i in opcodes if i.startswith("PUSH"))
         - _EMPTY_REVERT_OFFSET
     )
 
 
-def _is_immutable_member_load(opcodes: List[str]):
+def _is_immutable_member_load(opcodes: list[str]):
     is_code_copy = len(opcodes) > 5 and opcodes[5] == "CODECOPY"
     return not is_code_copy and opcodes and is_0x_prefixed(opcodes[0])
 
 
 def _extend_return(function: Function, traceback: SourceTraceback, last_pc: int, source_path: Path):
     return_ast_result = [x for x in function.ast.children if x.ast_type == "Return"]
     if not return_ast_result:
@@ -1476,23 +1638,15 @@
     if traceback.last:
         traceback.last.extend(location, pcs=last_pcs, ws_start=start)
     else:
         # Not sure if it ever gets here, but type-checks say it could.
         traceback.add_jump(location, function, 1, last_pcs, source_path=source_path)
 
 
-def _is_fallback_check(opcodes: List[str], op: str) -> bool:
+def _is_fallback_check(opcodes: list[str], op: str) -> bool:
     return (
         "JUMP" in op
         and len(opcodes) >= 7
         and opcodes[0] == "JUMPDEST"
         and opcodes[6] == "SHR"
         and opcodes[5] == "0xE0"
     )
-
-
-# def _version_to_specifier(version: str) -> str:
-#     pragma_str = " ".join(version.split()).replace("^", "~=")
-#     if pragma_str and pragma_str[0].isnumeric():
-#         return f"=={pragma_str}"
-#
-#     return pragma_str
```

### Comparing `ape-vyper-0.7.1/ape_vyper/exceptions.py` & `ape-vyper-0.8.0/ape_vyper/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from enum import Enum
-from typing import Dict, Optional, Type, Union
+from typing import Optional, Union
 
 from ape.exceptions import CompilerError, ContractLogicError
 from ape.utils import USER_ASSERT_TAG
 from vvm.exceptions import VyperError  # type: ignore
 
 
 class VyperCompilerPluginError(CompilerError):
@@ -153,15 +153,15 @@
     method defined in its ABI.
     """
 
     def __init__(self, **kwargs):
         super().__init__(RuntimeErrorType.FALLBACK_NOT_DEFINED, **kwargs)
 
 
-RUNTIME_ERROR_MAP: Dict[RuntimeErrorType, Type[ContractLogicError]] = {
+RUNTIME_ERROR_MAP: dict[RuntimeErrorType, type[ContractLogicError]] = {
     RuntimeErrorType.NONPAYABLE_CHECK: NonPayableError,
     RuntimeErrorType.INVALID_CALLDATA_OR_VALUE: InvalidCalldataOrValueError,
     RuntimeErrorType.INDEX_OUT_OF_RANGE: IndexOutOfRangeError,
     RuntimeErrorType.INTEGER_OVERFLOW: IntegerOverflowError,
     RuntimeErrorType.INTEGER_UNDERFLOW: IntegerUnderflowError,
     RuntimeErrorType.INTEGER_BOUNDS_CHECK: IntegerBoundsCheck,
     RuntimeErrorType.DIVISION_BY_ZERO: DivisionByZeroError,
```

### Comparing `ape-vyper-0.7.1/ape_vyper/interface.py` & `ape-vyper-0.8.0/ape_vyper/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Tools for working with ABI specs and Vyper interface source code
 """
 
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple, Union
+from typing import Any, Optional, Union
 
 from ethpm_types import ABI, MethodABI
 from ethpm_types.abi import ABIType
 
 INDENT_SPACES = 4
 INDENT = " " * INDENT_SPACES
 
@@ -18,34 +18,34 @@
 
 
 def iface_name_from_file(fpath: Path) -> str:
     """Get Interface name from file path"""
     return fpath.name.split(".")[0]
 
 
-def generate_inputs(inputs: List[ABIType]) -> str:
+def generate_inputs(inputs: list[ABIType]) -> str:
     """Generate the source code input args from ABI inputs"""
     return ", ".join(f"{i.name}: {i.type}" for i in inputs)
 
 
 def generate_method(abi: MethodABI) -> str:
     """Generate Vyper interface method definition"""
     inputs = generate_inputs(abi.inputs)
     return_maybe = f" -> {abi.outputs[0].type}" if abi.outputs else ""
     return f"def {abi.name}({inputs}){return_maybe}: {abi.stateMutability}\n"
 
 
-def abi_to_type(iface: Dict[str, Any]) -> Optional[ABI]:
+def abi_to_type(iface: dict[str, Any]) -> Optional[ABI]:
     """Convert a dict JSON-like interface to an ethpm-types ABI type"""
     if iface["type"] == "function":
         return MethodABI.model_validate(iface)
     return None
 
 
-def generate_interface(abi: Union[List[Dict[str, Any]], List[ABI]], iface_name: str) -> str:
+def generate_interface(abi: Union[list[dict[str, Any]], list[ABI]], iface_name: str) -> str:
     """
     Generate a Vyper interface source code from an ABI spec
 
     Args:
         abi (List[Union[Dict[str, Any], ABI]]): An ABI spec for a contract
         iface_name (str): The name of the interface
 
@@ -66,18 +66,18 @@
 
         if isinstance(iface, MethodABI):
             source += indent_line(generate_method(iface))
 
     return f"{source}\n"
 
 
-def extract_meta(source_code: str) -> Tuple[Optional[str], str]:
+def extract_meta(source_code: str) -> tuple[Optional[str], str]:
     """Extract version pragma, and returne cleaned source"""
     version_pragma: Optional[str] = None
-    cleaned_source_lines: List[str] = []
+    cleaned_source_lines: list[str] = []
 
     """
     Pragma format changed a bit.
 
     >= 3.10: #pragma version ^0.3.0
     < 3.10: # @version ^0.3.0
 
@@ -90,15 +90,15 @@
             version_pragma = line
         else:
             cleaned_source_lines.append(line)
 
     return (version_pragma, "\n".join(cleaned_source_lines))
 
 
-def extract_imports(source: str) -> Tuple[str, str, str]:
+def extract_imports(source: str) -> tuple[str, str, str]:
     """
     Extract import lines from the source, return them and the source without imports
 
     Returns:
      Tuple[str, str, str]: (stdlib_import_lines, interface_import_lines, cleaned_source)
     """
     interface_import_lines = []
@@ -117,15 +117,15 @@
     return (
         "\n".join(stdlib_import_lines),
         "\n".join(interface_import_lines),
         "\n".join(cleaned_source_lines),
     )
 
 
-def extract_import_aliases(source: str) -> Dict[str, str]:
+def extract_import_aliases(source: str) -> dict[str, str]:
     """
     Extract import aliases from import lines
 
     Returns:
         Dict[str, str]: {import: alias}
     """
     aliases = {}
```

### Comparing `ape-vyper-0.7.1/ape_vyper.egg-info/PKG-INFO` & `ape-vyper-0.8.0/ape_vyper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 Metadata-Version: 2.1
 Name: ape-vyper
-Version: 0.7.1
+Version: 0.8.0
 Summary: Plugin for Ape Ethereum Framework for compiling Vyper contracts
 Home-page: https://github.com/ApeWorX/ape-vyper
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
 Provides-Extra: release
 Provides-Extra: dev
 License-File: LICENSE
 
 # Quick Start
 
 Ape compiler plugin around [VVM](https://github.com/vyperlang/vvm)
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
+- [python3](https://www.python.org/downloads) version 3.9 up to 3.12.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
```

### Comparing `ape-vyper-0.7.1/ape_vyper.egg-info/SOURCES.txt` & `ape-vyper-0.8.0/ape_vyper.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 .gitignore
-.mdformat.toml
 .pre-commit-config.yaml
 CONTRIBUTING.md
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 .github/PULL_REQUEST_TEMPLATE.md
 .github/release-drafter.yml
 .github/ISSUE_TEMPLATE/bug.md
 .github/ISSUE_TEMPLATE/feature.md
 .github/ISSUE_TEMPLATE/work-item.md
+.github/workflows/codeql.yml
 .github/workflows/commitlint.yaml
 .github/workflows/draft.yaml
 .github/workflows/prtitle.yaml
 .github/workflows/publish.yaml
 .github/workflows/test.yaml
 ape_vyper/__init__.py
 ape_vyper/_cli.py
```

### Comparing `ape-vyper-0.7.1/pyproject.toml` & `ape-vyper-0.8.0/pyproject.toml`

 * *Files 19% similar despite different names*

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
 norecursedirs = "projects"
 addopts = """
     -p no:ape_test
 """
@@ -29,7 +29,10 @@
 
 [tool.isort]
 line_length = 100
 force_grid_wrap = 0
 include_trailing_comma = true
 multi_line_output = 3
 use_parentheses = true
+
+[tool.mdformat]
+number = true
```

### Comparing `ape-vyper-0.7.1/setup.py` & `ape-vyper-0.8.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 extras_require = {
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
         "pytest-mock",
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
-        "black>=23.12.0,<24",  # Auto-formatter and linter
-        "mypy>=1.7.1",  # Static type analyzer
+        "black>=24.4.2,<25",  # Auto-formatter and linter
+        "mypy>=1.10.0,<2",  # Static type analyzer
         "types-setuptools",  # Needed due to mypy typeshed
-        "flake8>=6.1.0,<7",  # Style linter
-        "isort>=5.10.1",  # Import sorting linter
+        "flake8>=7.0.0,<8",  # Style linter
+        "isort>=5.13.2",  # Import sorting linter
         "mdformat>=0.7.17",  # Auto-formatter for markdown
         "mdformat-gfm>=0.3.5",  # Needed for formatting GitHub-flavored markdown
         "mdformat-frontmatter>=0.4.1",  # Needed for frontmatters-style headers in issue templates
+        "mdformat-pyproject>=0.0.1",  # Allows configuring in pyproject.toml
     ],
     "release": [  # `release` GitHub Action job uses this
         "setuptools",  # Installation tool
         "wheel",  # Packaging tool
         "twine",  # Package upload tool
     ],
     "dev": [
@@ -54,21 +54,21 @@
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-vyper",
     include_package_data=True,
     install_requires=[
-        "eth-ape>=0.7.13,<0.8",
+        "eth-ape>=0.8.2,<0.9",
         "ethpm-types",  # Use same version as eth-ape
         "tqdm",  # Use same version as eth-ape
         "vvm>=0.2.0,<0.3",
         "vyper~=0.3.7",
     ],
-    python_requires=">=3.8,<4",
+    python_requires=">=3.9,<4",
     extras_require=extras_require,
     py_modules=["ape_vyper"],
     entry_points={
         "ape_cli_subcommands": [
             "ape_vyper=ape_vyper._cli:cli",
         ],
     },
@@ -81,13 +81,13 @@
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

### Comparing `ape-vyper-0.7.1/tests/conftest.py` & `ape-vyper-0.8.0/tests/conftest.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 import os
 import shutil
+import tempfile
 from contextlib import contextmanager
-from distutils.dir_util import copy_tree
 from pathlib import Path
 from tempfile import mkdtemp
-from typing import List
 
 import ape
 import pytest
 import vvm  # type: ignore
 from click.testing import CliRunner
 
-# NOTE: Ensure that we don't use local paths for these
-DATA_FOLDER = Path(mkdtemp()).resolve()
-PROJECT_FOLDER = Path(mkdtemp()).resolve()
-ape.config.DATA_FOLDER = DATA_FOLDER
-ape.config.PROJECT_FOLDER = PROJECT_FOLDER
-
 BASE_CONTRACTS_PATH = Path(__file__).parent / "contracts"
 TEMPLATES_PATH = BASE_CONTRACTS_PATH / "templates"
 FAILING_BASE = BASE_CONTRACTS_PATH / "failing_contracts"
 PASSING_BASE = BASE_CONTRACTS_PATH / "passing_contracts"
 ALL_VERSIONS = (
     "0.2.1",
     "0.2.2",
@@ -43,15 +36,40 @@
         "0.3.9",
         "0.3.10",
     ),
     "sub_reverts": ALL_VERSIONS,
 }
 
 
-def contract_test_cases(passing: bool) -> List[str]:
+@pytest.fixture(scope="session", autouse=True)
+def from_tests_dir():
+    # Makes default project correct.
+    here = Path(__file__).parent
+    orig = Path.cwd()
+    if orig != here:
+        os.chdir(f"{here}")
+
+    yield
+
+    if Path.cwd() != orig:
+        os.chdir(f"{orig}")
+
+
+@pytest.fixture(scope="session", autouse=True)
+def config():
+    cfg = ape.config
+
+    # Ensure we don't persist any .ape data.
+    with tempfile.TemporaryDirectory() as temp_dir:
+        path = Path(temp_dir).resolve()
+        cfg.DATA_FOLDER = path
+        yield cfg
+
+
+def contract_test_cases(passing: bool) -> list[str]:
     """
     Returns test-case names for outputting nicely with pytest.
     """
     suffix = "passing_contracts" if passing else "failing_contracts"
     return [p.name for p in (BASE_CONTRACTS_PATH / suffix).glob("*.vy") if p.is_file()]
 
 
@@ -124,62 +142,41 @@
     Creates a new, temporary installation path for vvm for a given test.
     """
     with _tmp_vvm_path(monkeypatch) as path:
         yield path
 
 
 @pytest.fixture
-def data_folder():
-    return DATA_FOLDER
-
-
-@pytest.fixture
-def project_folder():
-    return PROJECT_FOLDER
-
-
-@pytest.fixture
 def compiler_manager():
     return ape.compilers
 
 
 @pytest.fixture
 def compiler(compiler_manager):
     return compiler_manager.vyper
 
 
-@pytest.fixture
-def config():
-    return ape.config
-
-
-@pytest.fixture(autouse=True)
+@pytest.fixture(scope="session", autouse=True)
 def project(config):
     project_source_dir = Path(__file__).parent
-    project_dest_dir = config.PROJECT_FOLDER / project_source_dir.name
 
     # Delete build / .cache that may exist pre-copy
-    project_path = Path(__file__).parent
-    cache = project_path / ".build"
-
-    if cache.is_dir():
-        shutil.rmtree(cache)
+    cache = project_source_dir / ".build"
+    shutil.rmtree(cache, ignore_errors=True)
 
-    copy_tree(project_source_dir.as_posix(), project_dest_dir.as_posix())
-    with config.using_project(project_dest_dir) as project:
-        yield project
-        if project.local_project._cache_folder.is_dir():
-            shutil.rmtree(project.local_project._cache_folder)
+    root_project = ape.Project(project_source_dir)
+    with root_project.isolate_in_tempdir() as tmp_project:
+        yield tmp_project
 
 
 @pytest.fixture
 def geth_provider():
-    if not ape.networks.active_provider or ape.networks.provider.name != "geth":
+    if not ape.networks.active_provider or ape.networks.provider.name != "node":
         with ape.networks.ethereum.local.use_provider(
-            "geth", provider_settings={"uri": "http://127.0.0.1:5550"}
+            "node", provider_settings={"uri": "http://127.0.0.1:5550"}
         ) as provider:
             yield provider
     else:
         yield ape.networks.provider
 
 
 @pytest.fixture
```

### Comparing `ape-vyper-0.7.1/tests/contracts/passing_contracts/erc20.vy` & `ape-vyper-0.8.0/tests/contracts/passing_contracts/erc20.vy`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.7.1/tests/contracts/passing_contracts/flatten_me.vy` & `ape-vyper-0.8.0/tests/contracts/passing_contracts/flatten_me.vy`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # pragma version 0.3.10
 
 from vyper.interfaces import ERC20
 
 from interfaces import IFace2 as IFaceTwo
 import interfaces.IFace as IFace
-import exampledep.Dependency as Dep
+import exampledependency.Dependency as Dep
 
 
 @external
 @view
 def read_contract(some_address: address) -> uint256:
     myContract: IFace = IFace(some_address)
     return myContract.read_stuff()
```

### Comparing `ape-vyper-0.7.1/tests/contracts/templates/contract.template` & `ape-vyper-0.8.0/tests/contracts/templates/contract.template`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.7.1/tests/contracts/templates/reverts.template` & `ape-vyper-0.8.0/tests/contracts/templates/reverts.template`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.7.1/tests/contracts/templates/traceback_contract.template` & `ape-vyper-0.8.0/tests/contracts/templates/traceback_contract.template`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.7.1/tests/projects/coverage_project/ape-config.yaml` & `ape-vyper-0.8.0/tests/projects/coverage_project/ape-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ethereum:
   local:
-    default_provider: geth
+    default_provider: node
 
-geth:
+node:
   ethereum:
     local:
       # Connect to node running from other tests.
       uri: "http://127.0.0.1:5550"
 
 test:
   coverage:
```

### Comparing `ape-vyper-0.7.1/tests/projects/coverage_project/tests/test_coverage.py` & `ape-vyper-0.8.0/tests/projects/coverage_project/tests/test_coverage.py`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.7.1/tests/test_ape_reverts.py` & `ape-vyper-0.8.0/tests/test_ape_reverts.py`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.7.1/tests/test_cli.py` & `ape-vyper-0.8.0/tests/test_cli.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,9 @@
-from pathlib import Path
-from tempfile import NamedTemporaryFile
-
 import pytest
+from ape.utils import create_tempdir
 
 from ape_vyper._cli import cli
 
 
 @pytest.mark.parametrize(
     "contract_name,expected",
     [
@@ -19,13 +17,17 @@
                 "interface IFaceTwo:",
             ],
         ),
     ],
 )
 def test_cli_flatten(project, contract_name, expected, cli_runner):
     path = project.contracts_folder / contract_name
-    with NamedTemporaryFile() as tmpfile:
-        result = cli_runner.invoke(cli, ["flatten", str(path), tmpfile.name])
+    arguments = ["flatten", str(path)]
+    end = ("--project", str(project.path))
+    with create_tempdir() as tmpdir:
+        file = tmpdir / "flatten.vy"
+        arguments.extend([str(file), *end])
+        result = cli_runner.invoke(cli, arguments, catch_exceptions=False)
         assert result.exit_code == 0, result.stderr_bytes
-        output = Path(tmpfile.name).read_text()
+        output = file.read_text()
         for expect in expected:
             assert expect in output
```

### Comparing `ape-vyper-0.7.1/tests/test_compiler.py` & `ape-vyper-0.8.0/tests/test_compiler.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 import re
+from pathlib import Path
 
+import ape
 import pytest
 import vvm  # type: ignore
-from ape.exceptions import ContractLogicError
+from ape.exceptions import CompilerError, ContractLogicError
 from ethpm_types import ContractType
 from packaging.version import Version
 from vvm.exceptions import VyperError  # type: ignore
 
 from ape_vyper.compiler import RuntimeErrorType
 from ape_vyper.exceptions import (
     FallbackNotDefinedError,
@@ -44,47 +46,50 @@
 
 
 def test_compile_project(project):
     contracts = project.load_contracts()
     assert len(contracts) == len(
         [p.name for p in project.contracts_folder.glob("*.vy") if p.is_file()]
     )
-    assert contracts["contract_039"].source_id == "contract_039.vy"
-    assert contracts["contract_no_pragma"].source_id == "contract_no_pragma.vy"
-    assert contracts["older_version"].source_id == "older_version.vy"
+    prefix = "contracts/passing_contracts"
+    assert contracts["contract_039"].source_id == f"{prefix}/contract_039.vy"
+    assert contracts["contract_no_pragma"].source_id == f"{prefix}/contract_no_pragma.vy"
+    assert contracts["older_version"].source_id == f"{prefix}/older_version.vy"
 
 
 @pytest.mark.parametrize("contract_name", PASSING_CONTRACT_NAMES)
 def test_compile_individual_contracts(project, contract_name, compiler):
     path = project.contracts_folder / contract_name
-    assert compiler.compile([path])
+    assert list(compiler.compile((path,), project=project))
 
 
 @pytest.mark.parametrize(
     "contract_name", [n for n in FAILING_CONTRACT_NAMES if n != "contract_unknown_pragma.vy"]
 )
 def test_compile_failures(contract_name, compiler):
+    failing_project = ape.Project(FAILING_BASE)
     path = FAILING_BASE / contract_name
     with pytest.raises(VyperCompileError, match=EXPECTED_FAIL_PATTERNS[path.stem]) as err:
-        compiler.compile([path], base_path=FAILING_BASE)
+        list(compiler.compile((path,), project=failing_project))
 
     assert isinstance(err.value.base_err, VyperError)
 
 
 def test_install_failure(compiler):
+    failing_project = ape.Project(FAILING_BASE)
     path = FAILING_BASE / "contract_unknown_pragma.vy"
     with pytest.raises(VyperInstallError, match="No available version to install."):
-        compiler.compile([path])
+        list(compiler.compile((path,), project=failing_project))
 
 
 def test_get_version_map(project, compiler, all_versions):
     vyper_files = [
         x for x in project.contracts_folder.iterdir() if x.is_file() and x.suffix == ".vy"
     ]
-    actual = compiler.get_version_map(vyper_files)
+    actual = compiler.get_version_map(vyper_files, project=project)
     expected_versions = [Version(v) for v in all_versions]
 
     for version, sources in actual.items():
         if version in expected_versions:
             continue
 
         sources = ", ".join([p.name for p in actual[version]])
@@ -147,15 +152,18 @@
         ][0]
         vyper_028 = [
             c for c in manifest.compilers if str(c.version) == str(OLDER_VERSION_FROM_PRAGMA)
         ][0]
 
         for compiler in (vyper_028, codesize_latest, true_latest):
             assert compiler.name == "vyper"
-            assert compiler.settings["evmVersion"] == "istanbul"
+
+        assert vyper_028.settings["evmVersion"] == "berlin"
+        assert codesize_latest.settings["evmVersion"] == "shanghai"
+        assert true_latest.settings["evmVersion"] == "shanghai"
 
         # There is only one contract with codesize pragma.
         assert codesize_latest.contractTypes == ["optimize_codesize"]
         assert codesize_latest.settings["optimize"] == "codesize"
 
         # There is only one contract with evm-version pragma.
         assert evm_latest.contractTypes == ["evm_pragma"]
@@ -164,29 +172,29 @@
         assert len(true_latest.contractTypes) >= 9
         assert len(vyper_028.contractTypes) >= 1
         assert "contract_0310" in true_latest.contractTypes
         assert "older_version" in vyper_028.contractTypes
         for compiler in (true_latest, vyper_028):
             assert compiler.settings["optimize"] is True
 
-    project.local_project.update_manifest(compilers=[])
+    project.update_manifest(compilers=[])
     project.load_contracts(use_cache=False)
-    run_test(project.local_project.manifest)
+    run_test(project.manifest)
     man = project.extract_manifest()
     run_test(man)
 
 
 def test_compile_parse_dev_messages(compiler, dev_revert_source, project):
     """
     Test parsing of dev messages in a contract. These follow the form of "#dev: ...".
 
     The compiler will output a map that maps dev messages to line numbers.
     See contract_with_dev_messages.vy for more information.
     """
-    result = compiler.compile([dev_revert_source], base_path=project.contracts_folder)
+    result = list(compiler.compile((dev_revert_source,), project=project))
 
     assert len(result) == 1
 
     contract = result[0]
 
     assert contract.dev_messages is not None
     assert len(contract.dev_messages) == 4
@@ -197,44 +205,49 @@
     assert 23 not in contract.dev_messages
 
 
 def test_get_imports(compiler, project):
     vyper_files = [
         x for x in project.contracts_folder.iterdir() if x.is_file() and x.suffix == ".vy"
     ]
-    actual = compiler.get_imports(vyper_files)
+    actual = compiler.get_imports(vyper_files, project=project)
+    prefix = "contracts/passing_contracts"
     builtin_import = "vyper/interfaces/ERC20.json"
     local_import = "interfaces/IFace.vy"
     local_from_import = "interfaces/IFace2.vy"
-    dependency_import = "exampledep/Dependency.json"
-
-    assert len(actual["contract_037.vy"]) == 1
-    assert set(actual["contract_037.vy"]) == {builtin_import}
-    assert len(actual["use_iface.vy"]) == 3
-    assert set(actual["use_iface.vy"]) == {local_import, local_from_import, dependency_import}
-    assert len(actual["use_iface2.vy"]) == 1
-    assert set(actual["use_iface2.vy"]) == {local_import}
+    dep_key = project.dependencies.get_dependency("exampledependency", "local").package_id.replace(
+        "/", "_"
+    )
+    dependency_import = f"{dep_key}/local/contracts/Dependency.vy"
+    assert set(actual[f"{prefix}/contract_037.vy"]) == {builtin_import}
+    assert set(actual[f"{prefix}/use_iface.vy"]) == {
+        local_import,
+        local_from_import,
+        dependency_import,
+    }
+    assert set(actual[f"{prefix}/use_iface2.vy"]) == {local_import}
 
 
 @pytest.mark.parametrize("src,vers", [("contract_039", "0.3.9"), ("contract_037", "0.3.7")])
 def test_pc_map(compiler, project, src, vers):
     """
     Ensure we de-compress the source map correctly by comparing to the results
     from `compile_src()` which includes the uncompressed source map data.
     """
 
-    path = project.contracts_folder / f"{src}.vy"
-    result = compiler.compile([path], base_path=project.contracts_folder)[0]
+    path = project.sources.lookup(src)
+    result = list(compiler.compile((path,), project=project))[0]
     actual = result.pcmap.root
     code = path.read_text()
     vvm.install_vyper(vers)
-    compile_result = vvm.compile_source(code, vyper_version=vers, evm_version=compiler.evm_version)[
-        "<stdin>"
-    ]
-    src_map = compile_result["source_map"]
+    cfg = compiler.get_config(project=project)
+    evm_version = cfg.evm_version
+    compile_result = vvm.compile_source(code, vyper_version=vers, evm_version=evm_version)
+    std_result = compile_result["<stdin>"]
+    src_map = std_result["source_map"]
     lines = code.splitlines()
 
     # Use the old-fashioned way of gathering PCMap to ensure our creative way works
     expected = {pc: {"location": ln} for pc, ln in src_map["pc_pos_map"].items()}
     missing_pcs = []
     empty_locs = []
     wrong_locs = []
@@ -382,15 +395,15 @@
     assert isinstance(new_error, NonPayableError)
 
 
 @pytest.mark.parametrize("arguments", [(), (123,), (123, 321)])
 def test_trace_source(account, geth_provider, project, traceback_contract, arguments):
     receipt = traceback_contract.addBalance(*arguments, sender=account)
     actual = receipt.source_traceback
-    base_folder = project.contracts_folder
+    base_folder = Path(__file__).parent / "contracts" / "passing_contracts"
     contract_name = traceback_contract.contract_type.name
     expected = rf"""
 Traceback (most recent call last)
   File {base_folder}/{contract_name}.vy, in addBalance
        32         if i != num:
        33             continue
        34
@@ -430,15 +443,15 @@
     try:
         account.call(txn)
     except ContractLogicError:
         pass
 
     receipt = geth_provider.get_receipt(txn.txn_hash.hex())
     actual = receipt.source_traceback
-    base_folder = project.contracts_folder
+    base_folder = Path(__file__).parent / "contracts" / "passing_contracts"
     contract_name = traceback_contract.contract_type.name
     version_key = contract_name.split("traceback_contract_")[-1]
     expected = rf"""
 Traceback (most recent call last)
   File {base_folder}/{contract_name}.vy, in addBalance_f
        48         if i == num:
        49             break
@@ -471,44 +484,45 @@
     assert actual == expected
 
 
 def test_compile_with_version_set_in_config(config, projects_path, compiler, mocker):
     path = projects_path / "version_in_config"
     version_from_config = "0.3.7"
     spy = mocker.patch("ape_vyper.compiler.vvm_compile_standard")
-    with config.using_project(path) as project:
-        contract = project.contracts_folder / "v_contract.vy"
-        settings = compiler.get_compiler_settings((contract,))
-        assert str(list(settings.keys())[0]) == version_from_config
+    project = ape.Project(path)
 
-        # Show it uses this version in the compiler.
-        project.load_contracts(use_cache=False)
-        assert str(spy.call_args[1]["vyper_version"]) == version_from_config
+    contract = project.contracts_folder / "v_contract.vy"
+    settings = compiler.get_compiler_settings((contract,), project=project)
+    assert str(list(settings.keys())[0]) == version_from_config
+
+    # Show it uses this version in the compiler.
+    project.load_contracts(use_cache=False)
+    assert str(spy.call_args[1]["vyper_version"]) == version_from_config
 
 
-def test_compile_code(compiler, dev_revert_source):
+def test_compile_code(project, compiler, dev_revert_source):
     code = dev_revert_source.read_text()
-    actual = compiler.compile_code(code, contractName="MyContract")
+    actual = compiler.compile_code(code, project=project, contractName="MyContract")
     assert isinstance(actual, ContractType)
     assert actual.name == "MyContract"
     assert len(actual.abi) > 1
     assert len(actual.deployment_bytecode.bytecode) > 1
     assert len(actual.runtime_bytecode.bytecode) > 1
 
 
 def test_compile_with_version_set_in_settings_dict(config, compiler_manager, projects_path):
     path = projects_path / "version_in_config"
     contract = path / "contracts" / "v_contract.vy"
-
-    with config.using_project(path):
-        expected = (
-            '.*Version specification "0.3.10" is not compatible with compiler version "0.3.3"'
-        )
-        with pytest.raises(VyperCompileError, match=expected):
-            compiler_manager.compile([contract], settings={"version": "0.3.3"})
+    project = ape.Project(path)
+    expected = '.*Version specification "0.3.10" is not compatible with compiler version "0.3.3"'
+    iterator = compiler_manager.compile(
+        (contract,), project=project, settings={"vyper": {"version": "0.3.3"}}
+    )
+    with pytest.raises(CompilerError, match=expected):
+        _ = list(iterator)
 
 
 @pytest.mark.parametrize(
     "contract_name",
     [
         # This first one has most known edge cases
         "flatten_me.vy",
@@ -522,12 +536,12 @@
         "contract_no_pragma.vy",  # no pragma should compile with latest version
         "empty.vy",  # empty file still compiles with latest version
         "pragma_with_space.vy",
     ],
 )
 def test_flatten_contract(all_versions, project, contract_name, compiler):
     path = project.contracts_folder / contract_name
-    source = compiler.flatten_contract(path)
+    source = compiler.flatten_contract(path, project=project)
     source_code = str(source)
     version = compiler._source_vyper_version(source_code)
     vvm.install_vyper(str(version))
-    vvm.compile_source(source_code, base_path=project.contracts_folder, vyper_version=version)
+    vvm.compile_source(source_code, base_path=project.path, vyper_version=version)
```

### Comparing `ape-vyper-0.7.1/tests/test_coverage.py` & `ape-vyper-0.8.0/tests/test_coverage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import re
 import shutil
-import tempfile
 import xml.etree.ElementTree as ET
 from pathlib import Path
-from typing import List
+from typing import Optional
 
 import pytest
 
 LINES_VALID = 8
 MISSES = 0
 LINE_COV = "100.0".replace(".", r"\.")
 FUNC_COV = "100.0".replace(".", r"\.")
@@ -46,27 +45,45 @@
     return projects_path / "coverage_project"
 
 
 @pytest.fixture
 def coverage_project(config, coverage_project_path):
     build_dir = coverage_project_path / ".build"
     shutil.rmtree(build_dir, ignore_errors=True)
-    with tempfile.TemporaryDirectory() as base_dir:
-        # Copy Coverage project
-        project_dir = Path(base_dir) / "coverage_project"
-        shutil.copytree(coverage_project_path, project_dir)
-        with config.using_project(project_dir) as project:
-            yield project
+
+    with config.Project.create_temporary_project() as tmp_project:
+        shutil.copytree(coverage_project_path, tmp_project.path, dirs_exist_ok=True)
+        yield tmp_project
 
     shutil.rmtree(build_dir, ignore_errors=True)
 
 
 @pytest.fixture
-def setup_pytester(pytester, coverage_project_path):
-    tests_path = coverage_project_path / "tests"
+def setup_pytester(pytester, coverage_project):
+    tests_path = coverage_project.tests_folder
+
+    # Make other files
+    def _make_all_files(base: Path, prefix: Optional[Path] = None):
+        if not base.is_dir():
+            return
+
+        for file in base.iterdir():
+            if file.is_dir() and not file.name == "tests":
+                _make_all_files(file, prefix=Path(file.name))
+            elif file.is_file():
+                name = (prefix / file.name).as_posix() if prefix else file.name
+
+                if name == "ape-config.yaml":
+                    # Hack in in-memory overrides for testing purposes.
+                    text = str(coverage_project.config)
+                else:
+                    text = file.read_text()
+
+                src = {name: text.splitlines()}
+                pytester.makefile(file.suffix, **src)
 
     # Assume all tests should pass
     num_passes = 0
     num_failed = 0
     test_files = {}
     for file_path in tests_path.iterdir():
         if file_path.name.startswith("test_") and file_path.suffix == ".py":
@@ -78,44 +95,49 @@
                     for x in content.split("\n")
                     if x.startswith("def test_") and not x.startswith("def test_fail_")
                 ]
             )
             num_failed += len([x for x in content.split("\n") if x.startswith("def test_fail_")])
 
     pytester.makepyfile(**test_files)
+    _make_all_files(coverage_project.path)
 
     # Check for a conftest.py
     conftest = tests_path / "conftest.py"
     if conftest.is_file():
         pytester.makeconftest(conftest.read_text())
 
     # Returns expected number of passing tests.
     return num_passes, num_failed
 
 
 def test_coverage(geth_provider, setup_pytester, coverage_project, pytester):
     passed, failed = setup_pytester
-    result = pytester.runpytest("--coverage")
-    result.assert_outcomes(passed=passed, failed=failed)
+    result = pytester.runpytest_subprocess("--coverage")
+    try:
+        result.assert_outcomes(passed=passed, failed=failed)
+    except ValueError:
+        pytest.fail(str(result.stderr))
+
     actual = _get_coverage_report(result.outlines)
     expected = [x.strip() for x in EXPECTED_COVERAGE_REPORT.split("\n")]
     _assert_coverage(actual, expected)
 
     # Ensure XML was created.
-    base_dir = coverage_project.local_project._cache_folder
+    base_dir = pytester.path / ".build"
     xml_path = base_dir / "coverage.xml"
     _assert_xml(xml_path)
     html_path = base_dir / "htmlcov"
     assert html_path.is_dir()
     index = html_path / "index.html"
     assert index.is_file()
     _assert_html(index)
 
 
-def _get_coverage_report(lines: List[str]) -> List[str]:
+def _get_coverage_report(lines: list[str]) -> list[str]:
     ret = []
     started = False
     for line in lines:
         if not started:
             if COVERAGE_START_PATTERN.match(line):
                 # Started.
                 started = True
@@ -132,15 +154,15 @@
         else:
             # Line in between start and end.
             ret.append(line.strip())
 
     return ret
 
 
-def _assert_coverage(actual: List[str], expected: List[str]):
+def _assert_coverage(actual: list[str], expected: list[str]):
     for idx, (a_line, e_line) in enumerate(zip(actual, expected)):
         message = f"Failed at index {idx}. Expected={e_line}, Actual={a_line}"
         assert re.match(e_line, a_line), message
 
 
 def _assert_xml(xml_path: Path):
     assert xml_path.is_file()
```

