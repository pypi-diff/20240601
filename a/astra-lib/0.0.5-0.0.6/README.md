# Comparing `tmp/astra-lib-0.0.5.tar.gz` & `tmp/astra_lib-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astra-lib-0.0.5.tar", last modified: Wed Nov 29 11:45:55 2023, max compression
+gzip compressed data, was "astra_lib-0.0.6.tar", last modified: Sat Jun  1 16:54:33 2024, max compression
```

## Comparing `astra-lib-0.0.5.tar` & `astra_lib-0.0.6.tar`

### file list

```diff
@@ -1,78 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.754283 astra-lib-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-11-29 11:45:43.000000 astra-lib-0.0.5/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.742283 astra-lib-0.0.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.746283 astra-lib-0.0.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     3272 2023-11-29 11:45:43.000000 astra-lib-0.0.5/.github/ISSUE_TEMPLATE/bug-report.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.746283 astra-lib-0.0.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2023-11-29 11:45:43.000000 astra-lib-0.0.5/.github/workflows/CI.template
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2023-11-29 11:45:43.000000 astra-lib-0.0.5/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2023-11-29 11:45:43.000000 astra-lib-0.0.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)      184 2023-11-29 11:45:43.000000 astra-lib-0.0.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2023-11-29 11:45:43.000000 astra-lib-0.0.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11318 2023-11-29 11:45:55.754283 astra-lib-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10848 2023-11-29 11:45:43.000000 astra-lib-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2023-11-29 11:45:43.000000 astra-lib-0.0.5/README_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3599 2023-11-29 11:45:43.000000 astra-lib-0.0.5/README_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.746283 astra-lib-0.0.5/astra/
--rw-r--r--   0 runner    (1001) docker     (127)       52 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2023-11-29 11:45:55.000000 astra-lib-0.0.5/astra/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.746283 astra-lib-0.0.5/astra/torch/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.750283 astra-lib-0.0.5/astra/torch/al/
--rw-r--r--   0 runner    (1001) docker     (127)     2443 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/al/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      703 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/al/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.750283 astra-lib-0.0.5/astra/torch/al/acquisitions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/al/acquisitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/al/acquisitions/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      269 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/al/acquisitions/uniform_random.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/al/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.750283 astra-lib-0.0.5/astra/torch/al/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/al/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/al/strategies/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2747 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/al/strategies/deterministic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3854 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/al/strategies/diversity.py
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/al/strategies/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (127)     3121 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/al/strategies/mc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2182 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/al/strategies/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    27823 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5791 2023-11-29 11:45:43.000000 astra-lib-0.0.5/astra/torch/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.754283 astra-lib-0.0.5/astra_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    11318 2023-11-29 11:45:55.000000 astra-lib-0.0.5/astra_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-11-29 11:45:55.000000 astra-lib-0.0.5/astra_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-29 11:45:55.000000 astra-lib-0.0.5/astra_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-29 11:45:55.000000 astra-lib-0.0.5/astra_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-11-29 11:45:55.000000 astra-lib-0.0.5/astra_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2424 2023-11-29 11:45:43.000000 astra-lib-0.0.5/customize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.742283 astra-lib-0.0.5/notebooks/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.750283 astra-lib-0.0.5/notebooks/al/
--rw-r--r--   0 runner    (1001) docker     (127)   185118 2023-11-29 11:45:43.000000 astra-lib-0.0.5/notebooks/al/basic_example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      215 2023-11-29 11:45:43.000000 astra-lib-0.0.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.754283 astra-lib-0.0.5/quick_examples/
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2023-11-29 11:45:43.000000 astra-lib-0.0.5/quick_examples/advanced_train.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2023-11-29 11:45:43.000000 astra-lib-0.0.5/quick_examples/cnn.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2023-11-29 11:45:43.000000 astra-lib-0.0.5/quick_examples/count_params.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2023-11-29 11:45:43.000000 astra-lib-0.0.5/quick_examples/efficientnet.py
--rw-r--r--   0 runner    (1001) docker     (127)       91 2023-11-29 11:45:43.000000 astra-lib-0.0.5/quick_examples/load_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      160 2023-11-29 11:45:43.000000 astra-lib-0.0.5/quick_examples/mlp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2023-11-29 11:45:43.000000 astra-lib-0.0.5/quick_examples/quick_train.py
--rw-r--r--   0 runner    (1001) docker     (127)      799 2023-11-29 11:45:43.000000 astra-lib-0.0.5/quick_examples/train_with_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-11-29 11:45:43.000000 astra-lib-0.0.5/quick_examples/vit.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-11-29 11:45:43.000000 astra-lib-0.0.5/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       72 2023-11-29 11:45:43.000000 astra-lib-0.0.5/requirements-ml.txt
--rw-r--r--   0 runner    (1001) docker     (127)      238 2023-11-29 11:45:43.000000 astra-lib-0.0.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.754283 astra-lib-0.0.5/sandbox/
--rw-r--r--   0 runner    (1001) docker     (127)    46864 2023-11-29 11:45:43.000000 astra-lib-0.0.5/sandbox/sandbox.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      349 2023-11-29 11:45:55.754283 astra-lib-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      275 2023-11-29 11:45:43.000000 astra-lib-0.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.754283 astra-lib-0.0.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:43.000000 astra-lib-0.0.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.754283 astra-lib-0.0.5/tests/torch/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-29 11:45:55.754283 astra-lib-0.0.5/tests/torch/acquisitions/
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2023-11-29 11:45:43.000000 astra-lib-0.0.5/tests/torch/acquisitions/test_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2023-11-29 11:45:43.000000 astra-lib-0.0.5/tests/torch/acquisitions/test_uniform_random.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-11-29 11:45:43.000000 astra-lib-0.0.5/tests/torch/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2023-11-29 11:45:43.000000 astra-lib-0.0.5/tests/torch/test_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)     6506 2023-11-29 11:45:43.000000 astra-lib-0.0.5/tests/torch/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4835 2023-11-29 11:45:43.000000 astra-lib-0.0.5/tests/torch/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.914823 astra_lib-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-01 16:54:25.000000 astra_lib-0.0.6/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.902823 astra_lib-0.0.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.906823 astra_lib-0.0.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     3272 2024-06-01 16:54:25.000000 astra_lib-0.0.6/.github/ISSUE_TEMPLATE/bug-report.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.906823 astra_lib-0.0.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-06-01 16:54:25.000000 astra_lib-0.0.6/.github/workflows/CI.template
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-06-01 16:54:25.000000 astra_lib-0.0.6/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-06-01 16:54:25.000000 astra_lib-0.0.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-06-01 16:54:25.000000 astra_lib-0.0.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-06-01 16:54:25.000000 astra_lib-0.0.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-06-01 16:54:33.914823 astra_lib-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10246 2024-06-01 16:54:25.000000 astra_lib-0.0.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-06-01 16:54:25.000000 astra_lib-0.0.6/README_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-06-01 16:54:25.000000 astra_lib-0.0.6/README_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.906823 astra_lib-0.0.6/astra/
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-06-01 16:54:33.000000 astra_lib-0.0.6/astra/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.906823 astra_lib-0.0.6/astra/plot/
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/plot/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.906823 astra_lib-0.0.6/astra/torch/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.910823 astra_lib-0.0.6/astra/torch/al/
+-rw-r--r--   0 runner    (1001) docker     (127)     2443 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/al/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/al/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.910823 astra_lib-0.0.6/astra/torch/al/acquisitions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/al/acquisitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/al/acquisitions/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/al/acquisitions/uniform_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/al/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.910823 astra_lib-0.0.6/astra/torch/al/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/al/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/al/strategies/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2747 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/al/strategies/deterministic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3854 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/al/strategies/diversity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/al/strategies/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/al/strategies/mc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2182 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/al/strategies/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1638 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28106 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5791 2024-06-01 16:54:25.000000 astra_lib-0.0.6/astra/torch/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.914823 astra_lib-0.0.6/astra_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10716 2024-06-01 16:54:33.000000 astra_lib-0.0.6/astra_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-06-01 16:54:33.000000 astra_lib-0.0.6/astra_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 16:54:33.000000 astra_lib-0.0.6/astra_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-01 16:54:33.000000 astra_lib-0.0.6/astra_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-06-01 16:54:33.000000 astra_lib-0.0.6/astra_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2424 2024-06-01 16:54:25.000000 astra_lib-0.0.6/customize.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-06-01 16:54:25.000000 astra_lib-0.0.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.914823 astra_lib-0.0.6/quick_examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-06-01 16:54:25.000000 astra_lib-0.0.6/quick_examples/advanced_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-06-01 16:54:25.000000 astra_lib-0.0.6/quick_examples/cnn.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-06-01 16:54:25.000000 astra_lib-0.0.6/quick_examples/count_params.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-06-01 16:54:25.000000 astra_lib-0.0.6/quick_examples/efficientnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-06-01 16:54:25.000000 astra_lib-0.0.6/quick_examples/load_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-01 16:54:25.000000 astra_lib-0.0.6/quick_examples/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-06-01 16:54:25.000000 astra_lib-0.0.6/quick_examples/quick_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-06-01 16:54:25.000000 astra_lib-0.0.6/quick_examples/train_with_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-06-01 16:54:25.000000 astra_lib-0.0.6/quick_examples/vit.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-01 16:54:25.000000 astra_lib-0.0.6/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       72 2024-06-01 16:54:25.000000 astra_lib-0.0.6/requirements-ml.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-06-01 16:54:25.000000 astra_lib-0.0.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.914823 astra_lib-0.0.6/sandbox/
+-rw-r--r--   0 runner    (1001) docker     (127)    46864 2024-06-01 16:54:25.000000 astra_lib-0.0.6/sandbox/sandbox.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-06-01 16:54:33.914823 astra_lib-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-06-01 16:54:25.000000 astra_lib-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.914823 astra_lib-0.0.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:25.000000 astra_lib-0.0.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.914823 astra_lib-0.0.6/tests/torch/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.914823 astra_lib-0.0.6/tests/torch/acquisitions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-06-01 16:54:25.000000 astra_lib-0.0.6/tests/torch/acquisitions/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-06-01 16:54:25.000000 astra_lib-0.0.6/tests/torch/acquisitions/test_uniform_random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-06-01 16:54:25.000000 astra_lib-0.0.6/tests/torch/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1977 2024-06-01 16:54:25.000000 astra_lib-0.0.6/tests/torch/test_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6506 2024-06-01 16:54:25.000000 astra_lib-0.0.6/tests/torch/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4835 2024-06-01 16:54:25.000000 astra_lib-0.0.6/tests/torch/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:54:33.914823 astra_lib-0.0.6/tutorials/
+-rw-r--r--   0 runner    (1001) docker     (127)   183918 2024-06-01 16:54:25.000000 astra_lib-0.0.6/tutorials/active_learning.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    71269 2024-06-01 16:54:25.000000 astra_lib-0.0.6/tutorials/classification.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)    36308 2024-06-01 16:54:25.000000 astra_lib-0.0.6/tutorials/latexify.ipynb
```

### Comparing `astra-lib-0.0.5/.github/ISSUE_TEMPLATE/bug-report.yml` & `astra_lib-0.0.6/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/.github/workflows/CI.template` & `astra_lib-0.0.6/.github/workflows/CI.template`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/.github/workflows/CI.yml` & `astra_lib-0.0.6/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/.github/workflows/publish.yml` & `astra_lib-0.0.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/CONTRIBUTING.md` & `astra_lib-0.0.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/PKG-INFO` & `astra_lib-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astra-lib
-Version: 0.0.5
+Version: 0.0.6
 Summary: A ML toolkit with code bits useful for our day to day research
 Home-page: https://github.com/sustainability-lab/ASTRA
 Author: Nipun Batra
 Author-email: nipun.batra@iitgn.ac.in
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -33,27 +33,20 @@
 "**A**I for **S**ustainability" **T**oolkit for **R**esearch and **A**nalysis. ASTRA (अस्त्र) means a "tool" or "a weapon" in Sanskrit.
 
 # Design Principles
 Since `astra` is developed for research purposes, we'd try to adhere to these principles:
 
 ## What we will try to do:
 1. Keep the API simple-to-use and standardized to enable quick prototyping via automated scripts.
-2. Keep the API transparent to expose as many details as possilbe. Explicit should be preferred over implicit.
+2. Keep the API transparent to expose as many details as possible. Explicit should be preferred over implicit.
 3. Keep the API flexible to allow users to stretch the limits of their experiments.
+4. Don't provide defaults at most places. This will force the user to think about the choices they are making.
 
 ## What we will try to avoid:
-4. We will try not to reduce code repeatation at expence of transparency, flexibility and performance. Too much abstraction often makes the API complex to understand and thus becomes hard to adapt for custom use cases.
-
-## Examples
-| Points | Example |
-| --- | --- |
-| 1 and 2 | We have exactly same arguments for all strategies in `astra.torch.al.strategies` to ease the automation but we explicitely mention in the docstrings if an argument is used or ignored for a strategy. |
-| 2 | predict functions in `astra` by default put the model on `eval` mode but also allow to set `eval_mode` to `False`. This can be useful for techniques like [MC dropout](https://arxiv.org/abs/1506.02142).
-| 3 | `train_fn` from `astra.torch.utils` works for all types of models and losses which may or may not be from `astra`.
-| 4 | Though F1 score can be computed from precision and recall, we explicitely use F1 score formula to allow transparency and to avoid computing `TP` multiple times.
+5. We will try not to reduce code repetition at the expense of transparency, flexibility and performance. Too much abstraction often makes the API complex to understand and thus becomes hard to adapt for custom use cases.                                        |
 
 # Install
 
 Stable version:
 ```bash
 pip install astra-lib
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astra-lib Version: 0.0.5 Summary: A ML toolkit with
+Metadata-Version: 2.1 Name: astra-lib Version: 0.0.6 Summary: A ML toolkit with
 code bits useful for our day to day research Home-page: https://github.com/
 sustainability-lab/ASTRA Author: Nipun Batra Author-email:
 nipun.batra@iitgn.ac.in License: MIT Requires-Python: >=3.9 Description-
 Content-Type: text/markdown Requires-Dist: numpy Requires-Dist: pandas
 Requires-Dist: matplotlib Requires-Dist: xarray Requires-Dist: tqdm Requires-
 Dist: optree Requires-Dist: wandb
   [https://github.com/sustainability-lab/ASTRA/assets/59758528/d6a8e7ed-5368-
@@ -11,63 +11,54 @@
      _s_u_s_t_a_i_n_a_b_i_l_i_t_y_-_l_a_b_/_A_S_T_R_A_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_C_I_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
    _c_o_v_e_r_a_l_l_s_._i_o_/_r_e_p_o_s_/_g_i_t_h_u_b_/_s_u_s_t_a_i_n_a_b_i_l_i_t_y_-_l_a_b_/_A_S_T_R_A_/_b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]
 "**A**I for **S**ustainability" **T**oolkit for **R**esearch and **A**nalysis.
 ASTRA (à¤à¤¸à¥à¤¤à¥à¤°) means a "tool" or "a weapon" in Sanskrit. # Design
 Principles Since `astra` is developed for research purposes, we'd try to adhere
 to these principles: ## What we will try to do: 1. Keep the API simple-to-use
 and standardized to enable quick prototyping via automated scripts. 2. Keep the
-API transparent to expose as many details as possilbe. Explicit should be
+API transparent to expose as many details as possible. Explicit should be
 preferred over implicit. 3. Keep the API flexible to allow users to stretch the
-limits of their experiments. ## What we will try to avoid: 4. We will try not
-to reduce code repeatation at expence of transparency, flexibility and
-performance. Too much abstraction often makes the API complex to understand and
-thus becomes hard to adapt for custom use cases. ## Examples | Points | Example
-| | --- | --- | | 1 and 2 | We have exactly same arguments for all strategies
-in `astra.torch.al.strategies` to ease the automation but we explicitely
-mention in the docstrings if an argument is used or ignored for a strategy. | |
-2 | predict functions in `astra` by default put the model on `eval` mode but
-also allow to set `eval_mode` to `False`. This can be useful for techniques
-like [MC dropout](https://arxiv.org/abs/1506.02142). | 3 | `train_fn` from
-`astra.torch.utils` works for all types of models and losses which may or may
-not be from `astra`. | 4 | Though F1 score can be computed from precision and
-recall, we explicitely use F1 score formula to allow transparency and to avoid
-computing `TP` multiple times. # Install Stable version: ```bash pip install
-astra-lib ``` Latest version: ```bash pip install git+https://github.com/
-sustainability-lab/ASTRA ``` # Contributing Please go through the [contributing
-guidelines](CONTRIBUTING.md) before making a contribution. # Useful Code
-Snippets ## Data ### Load Data ```python from astra.torch.data import
-load_mnist, load_cifar_10 data = load_cifar_10() print(data) ``` ````python
-Files already downloaded and verified Files already downloaded and verified
-CIFAR-10 Dataset length of dataset: 60000 shape of images: torch.Size([3, 32,
-32]) len of classes: 10 classes: ['airplane', 'automobile', 'bird', 'cat',
-'deer', 'dog', 'frog', 'horse', 'ship', 'truck'] dtype of images: torch.float32
-dtype of labels: torch.int64 range of image values: min=0.0, max=1.0 ```` ##
-Models ### MLPs ```python from astra.torch.models import MLPRegressor mlp =
-MLPRegressor(input_dim=100, hidden_dims=[128, 64], output_dim=10,
-activation="relu", dropout=0.1) print(mlp) ``` ```python MLPRegressor(
-(featurizer): MLP( (dropout): Dropout(p=0.1, inplace=False) (input_layer):
-Linear(in_features=100, out_features=128, bias=True) (hidden_layer_1): Linear
-(in_features=128, out_features=64, bias=True) ) (regressor): Linear
-(in_features=64, out_features=10, bias=True) ) ``` ### CNNs ```python from
-astra.torch.models import CNNClassifier cnn = CNNClassifier( image_dims=(32,
-32), kernel_size=5, input_channels=3, conv_hidden_dims=[32, 64],
-dense_hidden_dims=[128, 64], n_classes=10, ) print(cnn) ``` ```python
-CNNClassifier( (featurizer): CNN( (activation): ReLU() (max_pool): MaxPool2d
-(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-(input_layer): Conv2d(3, 32, kernel_size=(5, 5), stride=(1, 1), padding=(2, 2))
-(hidden_layer_1): Conv2d(32, 64, kernel_size=(5, 5), stride=(1, 1), padding=(2,
-2)) (aggregator): Identity() (flatten): Flatten(start_dim=1, end_dim=-1) )
-(classifier): MLPClassifier( (featurizer): MLP( (activation): ReLU() (dropout):
-Dropout(p=0.0, inplace=False) (input_layer): Linear(in_features=4096,
+limits of their experiments. 4. Don't provide defaults at most places. This
+will force the user to think about the choices they are making. ## What we will
+try to avoid: 5. We will try not to reduce code repetition at the expense of
+transparency, flexibility and performance. Too much abstraction often makes the
+API complex to understand and thus becomes hard to adapt for custom use cases.
+| # Install Stable version: ```bash pip install astra-lib ``` Latest version:
+```bash pip install git+https://github.com/sustainability-lab/ASTRA ``` #
+Contributing Please go through the [contributing guidelines](CONTRIBUTING.md)
+before making a contribution. # Useful Code Snippets ## Data ### Load Data
+```python from astra.torch.data import load_mnist, load_cifar_10 data =
+load_cifar_10() print(data) ``` ````python Files already downloaded and
+verified Files already downloaded and verified CIFAR-10 Dataset length of
+dataset: 60000 shape of images: torch.Size([3, 32, 32]) len of classes: 10
+classes: ['airplane', 'automobile', 'bird', 'cat', 'deer', 'dog', 'frog',
+'horse', 'ship', 'truck'] dtype of images: torch.float32 dtype of labels:
+torch.int64 range of image values: min=0.0, max=1.0 ```` ## Models ### MLPs
+```python from astra.torch.models import MLPRegressor mlp = MLPRegressor
+(input_dim=100, hidden_dims=[128, 64], output_dim=10, activation="relu",
+dropout=0.1) print(mlp) ``` ```python MLPRegressor( (featurizer): MLP(
+(dropout): Dropout(p=0.1, inplace=False) (input_layer): Linear(in_features=100,
 out_features=128, bias=True) (hidden_layer_1): Linear(in_features=128,
-out_features=64, bias=True) ) (classifier): Linear(in_features=64,
-out_features=10, bias=True) ) ) ``` ### EfficientNets ```python import torch
-from torchvision.models import efficientnet_b0, EfficientNet_B0_Weights from
-astra.torch.models import EfficientNetClassifier # Pretrained model model =
-EfficientNetClassifier(model=efficientnet_b0,
+out_features=64, bias=True) ) (regressor): Linear(in_features=64,
+out_features=10, bias=True) ) ``` ### CNNs ```python from astra.torch.models
+import CNNClassifier cnn = CNNClassifier( image_dims=(32, 32), kernel_size=5,
+input_channels=3, conv_hidden_dims=[32, 64], dense_hidden_dims=[128, 64],
+n_classes=10, ) print(cnn) ``` ```python CNNClassifier( (featurizer): CNN(
+(activation): ReLU() (max_pool): MaxPool2d(kernel_size=2, stride=2, padding=0,
+dilation=1, ceil_mode=False) (input_layer): Conv2d(3, 32, kernel_size=(5, 5),
+stride=(1, 1), padding=(2, 2)) (hidden_layer_1): Conv2d(32, 64, kernel_size=(5,
+5), stride=(1, 1), padding=(2, 2)) (aggregator): Identity() (flatten): Flatten
+(start_dim=1, end_dim=-1) ) (classifier): MLPClassifier( (featurizer): MLP(
+(activation): ReLU() (dropout): Dropout(p=0.0, inplace=False) (input_layer):
+Linear(in_features=4096, out_features=128, bias=True) (hidden_layer_1): Linear
+(in_features=128, out_features=64, bias=True) ) (classifier): Linear
+(in_features=64, out_features=10, bias=True) ) ) ``` ### EfficientNets
+```python import torch from torchvision.models import efficientnet_b0,
+EfficientNet_B0_Weights from astra.torch.models import EfficientNetClassifier #
+Pretrained model model = EfficientNetClassifier(model=efficientnet_b0,
 weights=EfficientNet_B0_Weights.DEFAULT, n_classes=10) # OR without pretrained
 weights # model = EfficientNetClassifier(model=efficientnet_b0, weights=None,
 n_classes=10) x = torch.rand(10, 3, 224, 224) out = model(x) print(out.shape)
 ``` ```python torch.Size([10, 10]) ``` ### ViT ```python import torch from
 torchvision.models import vit_b_16, ViT_B_16_Weights from astra.torch.models
 import ViTClassifier model = ViTClassifier(vit_b_16, ViT_B_16_Weights.DEFAULT,
 n_classes=10) x = torch.rand(10, 3, 224, 224) # (batch_size, channels, h, w)
```

### Comparing `astra-lib-0.0.5/README.md` & `astra_lib-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -15,27 +15,20 @@
 "**A**I for **S**ustainability" **T**oolkit for **R**esearch and **A**nalysis. ASTRA (अस्त्र) means a "tool" or "a weapon" in Sanskrit.
 
 # Design Principles
 Since `astra` is developed for research purposes, we'd try to adhere to these principles:
 
 ## What we will try to do:
 1. Keep the API simple-to-use and standardized to enable quick prototyping via automated scripts.
-2. Keep the API transparent to expose as many details as possilbe. Explicit should be preferred over implicit.
+2. Keep the API transparent to expose as many details as possible. Explicit should be preferred over implicit.
 3. Keep the API flexible to allow users to stretch the limits of their experiments.
+4. Don't provide defaults at most places. This will force the user to think about the choices they are making.
 
 ## What we will try to avoid:
-4. We will try not to reduce code repeatation at expence of transparency, flexibility and performance. Too much abstraction often makes the API complex to understand and thus becomes hard to adapt for custom use cases.
-
-## Examples
-| Points | Example |
-| --- | --- |
-| 1 and 2 | We have exactly same arguments for all strategies in `astra.torch.al.strategies` to ease the automation but we explicitely mention in the docstrings if an argument is used or ignored for a strategy. |
-| 2 | predict functions in `astra` by default put the model on `eval` mode but also allow to set `eval_mode` to `False`. This can be useful for techniques like [MC dropout](https://arxiv.org/abs/1506.02142).
-| 3 | `train_fn` from `astra.torch.utils` works for all types of models and losses which may or may not be from `astra`.
-| 4 | Though F1 score can be computed from precision and recall, we explicitely use F1 score formula to allow transparency and to avoid computing `TP` multiple times.
+5. We will try not to reduce code repetition at the expense of transparency, flexibility and performance. Too much abstraction often makes the API complex to understand and thus becomes hard to adapt for custom use cases.                                        |
 
 # Install
 
 Stable version:
 ```bash
 pip install astra-lib
 ```
@@ -276,15 +269,27 @@
 )
 print(np.array(epoch_losses).round(2))
 
 ```
 ```python
 [3.01 0.79 0.77 0.8  0.64]
 
-  0%|          | 0/5 [00:00<?, ?it/s]Loss: 3.00609981:   0%|          | 0/5 [00:00<?, ?it/s]Loss: 3.00609981:  20%|██        | 1/5 [00:00<00:02,  1.97it/s]Loss: 0.78690718:  20%|██        | 1/5 [00:00<00:02,  1.97it/s]Loss: 0.78690718:  40%|████      | 2/5 [00:00<00:00,  3.64it/s]Loss: 0.77431746:  40%|████      | 2/5 [00:00<00:00,  3.64it/s]Loss: 0.77431746:  60%|██████    | 3/5 [00:00<00:00,  4.79it/s]Loss: 0.79909155:  60%|██████    | 3/5 [00:00<00:00,  4.79it/s]Loss: 0.79909155:  80%|████████  | 4/5 [00:00<00:00,  5.12it/s]Loss: 0.64411481:  80%|████████  | 4/5 [00:01<00:00,  5.12it/s]Loss: 0.64411481: 100%|██████████| 5/5 [00:01<00:00,  5.76it/s]Loss: 0.64411481: 100%|██████████| 5/5 [00:01<00:00,  4.72it/s]
+
+  0%|          | 0/5 [00:00<?, ?it/s]
+Loss: 3.00609981:   0%|          | 0/5 [00:00<?, ?it/s]
+Loss: 3.00609981:  20%|██        | 1/5 [00:00<00:02,  1.97it/s]
+Loss: 0.78690718:  20%|██        | 1/5 [00:00<00:02,  1.97it/s]
+Loss: 0.78690718:  40%|████      | 2/5 [00:00<00:00,  3.64it/s]
+Loss: 0.77431746:  40%|████      | 2/5 [00:00<00:00,  3.64it/s]
+Loss: 0.77431746:  60%|██████    | 3/5 [00:00<00:00,  4.79it/s]
+Loss: 0.79909155:  60%|██████    | 3/5 [00:00<00:00,  4.79it/s]
+Loss: 0.79909155:  80%|████████  | 4/5 [00:00<00:00,  5.12it/s]
+Loss: 0.64411481:  80%|████████  | 4/5 [00:01<00:00,  5.12it/s]
+Loss: 0.64411481: 100%|██████████| 5/5 [00:01<00:00,  5.76it/s]
+Loss: 0.64411481: 100%|██████████| 5/5 [00:01<00:00,  4.72it/s]
 
 ```
 
 
 ### Advanced Usage
 ```python
 import torch
@@ -335,15 +340,23 @@
 
 print("Epoch_losses", np.array(epoch_losses).round(2))
 
 ```
 ```python
 Epoch_losses [9.63 7.52 6.59 4.98 4.11]
 
-  0%|          | 0/5 [00:00<?, ?it/s]Loss: 9.63069725:   0%|          | 0/5 [00:00<?, ?it/s]Loss: 9.63069725:  20%|██        | 1/5 [00:00<00:00,  6.42it/s]Loss: 7.51600790:  20%|██        | 1/5 [00:00<00:00,  6.42it/s]Loss: 6.59280062:  20%|██        | 1/5 [00:00<00:00,  6.42it/s]Loss: 4.97779894:  20%|██        | 1/5 [00:00<00:00,  6.42it/s]Loss: 4.11271286:  20%|██        | 1/5 [00:00<00:00,  6.42it/s]Loss: 4.11271286: 100%|██████████| 5/5 [00:00<00:00, 31.35it/s]
+
+  0%|          | 0/5 [00:00<?, ?it/s]
+Loss: 9.63069725:   0%|          | 0/5 [00:00<?, ?it/s]
+Loss: 9.63069725:  20%|██        | 1/5 [00:00<00:00,  6.42it/s]
+Loss: 7.51600790:  20%|██        | 1/5 [00:00<00:00,  6.42it/s]
+Loss: 6.59280062:  20%|██        | 1/5 [00:00<00:00,  6.42it/s]
+Loss: 4.97779894:  20%|██        | 1/5 [00:00<00:00,  6.42it/s]
+Loss: 4.11271286:  20%|██        | 1/5 [00:00<00:00,  6.42it/s]
+Loss: 4.11271286: 100%|██████████| 5/5 [00:00<00:00, 31.35it/s]
 
 ```
 
 
 ## Others
 ### Count number of parameters in a model
 ```python
```

#### html2text {}

```diff
@@ -4,63 +4,54 @@
      _s_u_s_t_a_i_n_a_b_i_l_i_t_y_-_l_a_b_/_A_S_T_R_A_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_C_I_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
    _c_o_v_e_r_a_l_l_s_._i_o_/_r_e_p_o_s_/_g_i_t_h_u_b_/_s_u_s_t_a_i_n_a_b_i_l_i_t_y_-_l_a_b_/_A_S_T_R_A_/_b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]
 "**A**I for **S**ustainability" **T**oolkit for **R**esearch and **A**nalysis.
 ASTRA (à¤à¤¸à¥à¤¤à¥à¤°) means a "tool" or "a weapon" in Sanskrit. # Design
 Principles Since `astra` is developed for research purposes, we'd try to adhere
 to these principles: ## What we will try to do: 1. Keep the API simple-to-use
 and standardized to enable quick prototyping via automated scripts. 2. Keep the
-API transparent to expose as many details as possilbe. Explicit should be
+API transparent to expose as many details as possible. Explicit should be
 preferred over implicit. 3. Keep the API flexible to allow users to stretch the
-limits of their experiments. ## What we will try to avoid: 4. We will try not
-to reduce code repeatation at expence of transparency, flexibility and
-performance. Too much abstraction often makes the API complex to understand and
-thus becomes hard to adapt for custom use cases. ## Examples | Points | Example
-| | --- | --- | | 1 and 2 | We have exactly same arguments for all strategies
-in `astra.torch.al.strategies` to ease the automation but we explicitely
-mention in the docstrings if an argument is used or ignored for a strategy. | |
-2 | predict functions in `astra` by default put the model on `eval` mode but
-also allow to set `eval_mode` to `False`. This can be useful for techniques
-like [MC dropout](https://arxiv.org/abs/1506.02142). | 3 | `train_fn` from
-`astra.torch.utils` works for all types of models and losses which may or may
-not be from `astra`. | 4 | Though F1 score can be computed from precision and
-recall, we explicitely use F1 score formula to allow transparency and to avoid
-computing `TP` multiple times. # Install Stable version: ```bash pip install
-astra-lib ``` Latest version: ```bash pip install git+https://github.com/
-sustainability-lab/ASTRA ``` # Contributing Please go through the [contributing
-guidelines](CONTRIBUTING.md) before making a contribution. # Useful Code
-Snippets ## Data ### Load Data ```python from astra.torch.data import
-load_mnist, load_cifar_10 data = load_cifar_10() print(data) ``` ````python
-Files already downloaded and verified Files already downloaded and verified
-CIFAR-10 Dataset length of dataset: 60000 shape of images: torch.Size([3, 32,
-32]) len of classes: 10 classes: ['airplane', 'automobile', 'bird', 'cat',
-'deer', 'dog', 'frog', 'horse', 'ship', 'truck'] dtype of images: torch.float32
-dtype of labels: torch.int64 range of image values: min=0.0, max=1.0 ```` ##
-Models ### MLPs ```python from astra.torch.models import MLPRegressor mlp =
-MLPRegressor(input_dim=100, hidden_dims=[128, 64], output_dim=10,
-activation="relu", dropout=0.1) print(mlp) ``` ```python MLPRegressor(
-(featurizer): MLP( (dropout): Dropout(p=0.1, inplace=False) (input_layer):
-Linear(in_features=100, out_features=128, bias=True) (hidden_layer_1): Linear
-(in_features=128, out_features=64, bias=True) ) (regressor): Linear
-(in_features=64, out_features=10, bias=True) ) ``` ### CNNs ```python from
-astra.torch.models import CNNClassifier cnn = CNNClassifier( image_dims=(32,
-32), kernel_size=5, input_channels=3, conv_hidden_dims=[32, 64],
-dense_hidden_dims=[128, 64], n_classes=10, ) print(cnn) ``` ```python
-CNNClassifier( (featurizer): CNN( (activation): ReLU() (max_pool): MaxPool2d
-(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-(input_layer): Conv2d(3, 32, kernel_size=(5, 5), stride=(1, 1), padding=(2, 2))
-(hidden_layer_1): Conv2d(32, 64, kernel_size=(5, 5), stride=(1, 1), padding=(2,
-2)) (aggregator): Identity() (flatten): Flatten(start_dim=1, end_dim=-1) )
-(classifier): MLPClassifier( (featurizer): MLP( (activation): ReLU() (dropout):
-Dropout(p=0.0, inplace=False) (input_layer): Linear(in_features=4096,
+limits of their experiments. 4. Don't provide defaults at most places. This
+will force the user to think about the choices they are making. ## What we will
+try to avoid: 5. We will try not to reduce code repetition at the expense of
+transparency, flexibility and performance. Too much abstraction often makes the
+API complex to understand and thus becomes hard to adapt for custom use cases.
+| # Install Stable version: ```bash pip install astra-lib ``` Latest version:
+```bash pip install git+https://github.com/sustainability-lab/ASTRA ``` #
+Contributing Please go through the [contributing guidelines](CONTRIBUTING.md)
+before making a contribution. # Useful Code Snippets ## Data ### Load Data
+```python from astra.torch.data import load_mnist, load_cifar_10 data =
+load_cifar_10() print(data) ``` ````python Files already downloaded and
+verified Files already downloaded and verified CIFAR-10 Dataset length of
+dataset: 60000 shape of images: torch.Size([3, 32, 32]) len of classes: 10
+classes: ['airplane', 'automobile', 'bird', 'cat', 'deer', 'dog', 'frog',
+'horse', 'ship', 'truck'] dtype of images: torch.float32 dtype of labels:
+torch.int64 range of image values: min=0.0, max=1.0 ```` ## Models ### MLPs
+```python from astra.torch.models import MLPRegressor mlp = MLPRegressor
+(input_dim=100, hidden_dims=[128, 64], output_dim=10, activation="relu",
+dropout=0.1) print(mlp) ``` ```python MLPRegressor( (featurizer): MLP(
+(dropout): Dropout(p=0.1, inplace=False) (input_layer): Linear(in_features=100,
 out_features=128, bias=True) (hidden_layer_1): Linear(in_features=128,
-out_features=64, bias=True) ) (classifier): Linear(in_features=64,
-out_features=10, bias=True) ) ) ``` ### EfficientNets ```python import torch
-from torchvision.models import efficientnet_b0, EfficientNet_B0_Weights from
-astra.torch.models import EfficientNetClassifier # Pretrained model model =
-EfficientNetClassifier(model=efficientnet_b0,
+out_features=64, bias=True) ) (regressor): Linear(in_features=64,
+out_features=10, bias=True) ) ``` ### CNNs ```python from astra.torch.models
+import CNNClassifier cnn = CNNClassifier( image_dims=(32, 32), kernel_size=5,
+input_channels=3, conv_hidden_dims=[32, 64], dense_hidden_dims=[128, 64],
+n_classes=10, ) print(cnn) ``` ```python CNNClassifier( (featurizer): CNN(
+(activation): ReLU() (max_pool): MaxPool2d(kernel_size=2, stride=2, padding=0,
+dilation=1, ceil_mode=False) (input_layer): Conv2d(3, 32, kernel_size=(5, 5),
+stride=(1, 1), padding=(2, 2)) (hidden_layer_1): Conv2d(32, 64, kernel_size=(5,
+5), stride=(1, 1), padding=(2, 2)) (aggregator): Identity() (flatten): Flatten
+(start_dim=1, end_dim=-1) ) (classifier): MLPClassifier( (featurizer): MLP(
+(activation): ReLU() (dropout): Dropout(p=0.0, inplace=False) (input_layer):
+Linear(in_features=4096, out_features=128, bias=True) (hidden_layer_1): Linear
+(in_features=128, out_features=64, bias=True) ) (classifier): Linear
+(in_features=64, out_features=10, bias=True) ) ) ``` ### EfficientNets
+```python import torch from torchvision.models import efficientnet_b0,
+EfficientNet_B0_Weights from astra.torch.models import EfficientNetClassifier #
+Pretrained model model = EfficientNetClassifier(model=efficientnet_b0,
 weights=EfficientNet_B0_Weights.DEFAULT, n_classes=10) # OR without pretrained
 weights # model = EfficientNetClassifier(model=efficientnet_b0, weights=None,
 n_classes=10) x = torch.rand(10, 3, 224, 224) out = model(x) print(out.shape)
 ``` ```python torch.Size([10, 10]) ``` ### ViT ```python import torch from
 torchvision.models import vit_b_16, ViT_B_16_Weights from astra.torch.models
 import ViTClassifier model = ViTClassifier(vit_b_16, ViT_B_16_Weights.DEFAULT,
 n_classes=10) x = torch.rand(10, 3, 224, 224) # (batch_size, channels, h, w)
@@ -90,24 +81,24 @@
 ( image_dims=(28, 28), kernel_size=5, input_channels=3, conv_hidden_dims=[4],
 dense_hidden_dims=[2], n_classes=2 ) dataset = TensorDataset(X, y) dataloader =
 DataLoader(dataset, batch_size=32, shuffle=True, num_workers=2) # Let train_fn
 do the optimization for you iter_losses, epoch_losses = train_fn( model,
 dataloader=dataloader, loss_fn=nn.CrossEntropyLoss(), lr=0.1, epochs=5, ) print
 (np.array(epoch_losses).round(2)) ``` ```python [3.01 0.79 0.77 0.8 0.64] 0%| |
 0/5 [00:00
- ?it/s]Loss: 3.00609981: 0%| | 0/5 [00:00
- ?it/s]Loss: 3.00609981: 20%|ââ | 1/5 [00:00<00:02, 1.97it/s]Loss:
-0.78690718: 20%|ââ | 1/5 [00:00<00:02, 1.97it/s]Loss: 0.78690718:
-40%|ââââ | 2/5 [00:00<00:00, 3.64it/s]Loss: 0.77431746:
-40%|ââââ | 2/5 [00:00<00:00, 3.64it/s]Loss: 0.77431746:
-60%|ââââââ | 3/5 [00:00<00:00, 4.79it/s]Loss: 0.79909155:
-60%|ââââââ | 3/5 [00:00<00:00, 4.79it/s]Loss: 0.79909155:
-80%|ââââââââ | 4/5 [00:00<00:00, 5.12it/s]Loss: 0.64411481:
-80%|ââââââââ | 4/5 [00:01<00:00, 5.12it/s]Loss: 0.64411481:
-100%|ââââââââââ| 5/5 [00:01<00:00, 5.76it/s]Loss:
+ ?it/s] Loss: 3.00609981: 0%| | 0/5 [00:00
+ ?it/s] Loss: 3.00609981: 20%|ââ | 1/5 [00:00<00:02, 1.97it/s] Loss:
+0.78690718: 20%|ââ | 1/5 [00:00<00:02, 1.97it/s] Loss: 0.78690718:
+40%|ââââ | 2/5 [00:00<00:00, 3.64it/s] Loss: 0.77431746:
+40%|ââââ | 2/5 [00:00<00:00, 3.64it/s] Loss: 0.77431746:
+60%|ââââââ | 3/5 [00:00<00:00, 4.79it/s] Loss: 0.79909155:
+60%|ââââââ | 3/5 [00:00<00:00, 4.79it/s] Loss: 0.79909155:
+80%|ââââââââ | 4/5 [00:00<00:00, 5.12it/s] Loss: 0.64411481:
+80%|ââââââââ | 4/5 [00:01<00:00, 5.12it/s] Loss: 0.64411481:
+100%|ââââââââââ| 5/5 [00:01<00:00, 5.76it/s] Loss:
 0.64411481: 100%|ââââââââââ| 5/5 [00:01<00:00, 4.72it/s]
 ``` ### Advanced Usage ```python import torch import torch.nn as nn import
 numpy as np from astra.torch.utils import train_fn from astra.torch.models
 import AstraModel class CustomModel(AstraModel): def __init__(self): super
 ().__init__() self.linear = nn.Linear(2, 1) self.inp1_linear = nn.Linear(2, 1)
 def forward(self, x, inp1, fixed_bias): return self.linear(x) +
 self.inp1_linear(inp1) + fixed_bias def custom_loss_fn(model_output, output,
@@ -118,18 +109,18 @@
 (iter_losses, epoch_losses), state_dict_history = train_fn( model, input=X, #
 Can be None if model.forward() does not require input model_kwargs={"inp1":
 inp1, "fixed_bias": bias}, output=y, # Can be None if loss_fn does not require
 output loss_fn=custom_loss_fn, loss_fn_kwargs={"norm_factor": norm_factor},
 optimizer=optimizer, epochs=5, shuffle=True, verbose=True,
 return_state_dict=True, ) print("Epoch_losses", np.array(epoch_losses).round
 (2)) ``` ```python Epoch_losses [9.63 7.52 6.59 4.98 4.11] 0%| | 0/5 [00:00
- ?it/s]Loss: 9.63069725: 0%| | 0/5 [00:00
- ?it/s]Loss: 9.63069725: 20%|ââ | 1/5 [00:00<00:00, 6.42it/s]Loss:
-7.51600790: 20%|ââ | 1/5 [00:00<00:00, 6.42it/s]Loss: 6.59280062:
-20%|ââ | 1/5 [00:00<00:00, 6.42it/s]Loss: 4.97779894: 20%|ââ | 1/5 [00:
-00<00:00, 6.42it/s]Loss: 4.11271286: 20%|ââ | 1/5 [00:00<00:00, 6.42it/
-s]Loss: 4.11271286: 100%|ââââââââââ| 5/5 [00:00<00:00,
-31.35it/s] ``` ## Others ### Count number of parameters in a model ```python
-from astra.torch.utils import count_params from astra.torch.models import
-MLPRegressor mlp = MLPRegressor(input_dim=2, hidden_dims=[5, 6], output_dim=1)
-n_params = count_params(mlp) print(n_params) ``` ```python {'total_params': 58,
-'trainable_params': 58, 'non_trainable_params': 0} ```
+ ?it/s] Loss: 9.63069725: 0%| | 0/5 [00:00
+ ?it/s] Loss: 9.63069725: 20%|ââ | 1/5 [00:00<00:00, 6.42it/s] Loss:
+7.51600790: 20%|ââ | 1/5 [00:00<00:00, 6.42it/s] Loss: 6.59280062:
+20%|ââ | 1/5 [00:00<00:00, 6.42it/s] Loss: 4.97779894: 20%|ââ | 1/5
+[00:00<00:00, 6.42it/s] Loss: 4.11271286: 20%|ââ | 1/5 [00:00<00:00,
+6.42it/s] Loss: 4.11271286: 100%|ââââââââââ| 5/5 [00:00<00:
+00, 31.35it/s] ``` ## Others ### Count number of parameters in a model
+```python from astra.torch.utils import count_params from astra.torch.models
+import MLPRegressor mlp = MLPRegressor(input_dim=2, hidden_dims=[5, 6],
+output_dim=1) n_params = count_params(mlp) print(n_params) ``` ```python
+{'total_params': 58, 'trainable_params': 58, 'non_trainable_params': 0} ```
```

### Comparing `astra-lib-0.0.5/README_generator.py` & `astra_lib-0.0.6/README_generator.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/README_template.md` & `astra_lib-0.0.6/README_template.md`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/astra/torch/al/README.md` & `astra_lib-0.0.6/astra/torch/al/README.md`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/astra/torch/al/__init__.py` & `astra_lib-0.0.6/astra/torch/al/__init__.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/astra/torch/al/acquisitions/base.py` & `astra_lib-0.0.6/astra/torch/al/acquisitions/base.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/astra/torch/al/strategies/base.py` & `astra_lib-0.0.6/astra/torch/al/strategies/base.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/astra/torch/al/strategies/deterministic.py` & `astra_lib-0.0.6/astra/torch/al/strategies/deterministic.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/astra/torch/al/strategies/diversity.py` & `astra_lib-0.0.6/astra/torch/al/strategies/diversity.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/astra/torch/al/strategies/ensemble.py` & `astra_lib-0.0.6/astra/torch/al/strategies/ensemble.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/astra/torch/al/strategies/mc.py` & `astra_lib-0.0.6/astra/torch/al/strategies/mc.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/astra/torch/al/strategies/random.py` & `astra_lib-0.0.6/astra/torch/al/strategies/random.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/astra/torch/data.py` & `astra_lib-0.0.6/astra/torch/data.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/astra/torch/models.py` & `astra_lib-0.0.6/astra/torch/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from torchvision.models import efficientnet_b0, EfficientNet_B0_Weights
 from torchvision.models import vit_b_16, ViT_B_16_Weights
 from torchvision.models import resnet18, ResNet18_Weights
 from torchvision.models import densenet121, DenseNet121_Weights
 from torchvision.models import alexnet, AlexNet_Weights
 
 ## Hotfix for https://github.com/pytorch/vision/issues/7744#issuecomment-1757321451
+## Hotfix Start ###################################################################
 from torchvision.models._api import WeightsEnum
 from torch.hub import load_state_dict_from_url
 
 from typing import Tuple, Literal
 
 from astra.torch.utils import get_model_device
 
@@ -32,15 +33,15 @@
 def get_state_dict(self, *args, **kwargs):
     if "check_hash" in kwargs:
         kwargs.pop("check_hash")
     return load_state_dict_from_url(self.url, *args, **kwargs)
 
 
 WeightsEnum.get_state_dict = get_state_dict
-################################################################################
+## Hotfix End #####################################################################
 
 
 # Base class for all ASTRA models
 class AstraModel(nn.Module):
     def predict(self, X=None, dataloader=None, batch_size=None, eval_mode: bool = True, verbose=True):
         device = get_model_device(self)
         if eval_mode:
@@ -75,15 +76,17 @@
                 pred = self(batch_input)
                 preds.append(pred)
             pred = torch.cat(preds)
 
             return pred
 
         else:
-            raise ValueError("Either X or dataloader should be provided. This should never happen. Contact Zeel.")
+            raise ValueError(
+                "Either X or dataloader should be provided. This should never happen. Please report this issue to the developers."
+            )
 
 
 # Classifier and regressor base classes
 class Classifier(AstraModel):
     def __init__(self, featurizer, classifier):
         super().__init__()
         self.featurizer = featurizer
@@ -745,7 +748,12 @@
             activation (nn.Module, optional): _description_. Defaults to nn.ReLU().
             output_dim (int, optional): _description_. Defaults to 1.
         """
         featurizer = ViT(model, weights, transform)
         # ViT uses fixed input size of 224 so output_dim is always 768
         regressor = MLPRegressor(768, dense_hidden_dims, output_dim, activation, dropout)
         super().__init__(featurizer, regressor)
+
+
+class NeuralPrcess(AstraModel):
+    def __init__(self, input_dim, output_dim, encoder_hidden_dims, decoder_hidden_dims):
+        pass
```

### Comparing `astra-lib-0.0.5/astra/torch/utils.py` & `astra_lib-0.0.6/astra/torch/utils.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/astra_lib.egg-info/PKG-INFO` & `astra_lib-0.0.6/astra_lib.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astra-lib
-Version: 0.0.5
+Version: 0.0.6
 Summary: A ML toolkit with code bits useful for our day to day research
 Home-page: https://github.com/sustainability-lab/ASTRA
 Author: Nipun Batra
 Author-email: nipun.batra@iitgn.ac.in
 License: MIT
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -33,27 +33,20 @@
 "**A**I for **S**ustainability" **T**oolkit for **R**esearch and **A**nalysis. ASTRA (अस्त्र) means a "tool" or "a weapon" in Sanskrit.
 
 # Design Principles
 Since `astra` is developed for research purposes, we'd try to adhere to these principles:
 
 ## What we will try to do:
 1. Keep the API simple-to-use and standardized to enable quick prototyping via automated scripts.
-2. Keep the API transparent to expose as many details as possilbe. Explicit should be preferred over implicit.
+2. Keep the API transparent to expose as many details as possible. Explicit should be preferred over implicit.
 3. Keep the API flexible to allow users to stretch the limits of their experiments.
+4. Don't provide defaults at most places. This will force the user to think about the choices they are making.
 
 ## What we will try to avoid:
-4. We will try not to reduce code repeatation at expence of transparency, flexibility and performance. Too much abstraction often makes the API complex to understand and thus becomes hard to adapt for custom use cases.
-
-## Examples
-| Points | Example |
-| --- | --- |
-| 1 and 2 | We have exactly same arguments for all strategies in `astra.torch.al.strategies` to ease the automation but we explicitely mention in the docstrings if an argument is used or ignored for a strategy. |
-| 2 | predict functions in `astra` by default put the model on `eval` mode but also allow to set `eval_mode` to `False`. This can be useful for techniques like [MC dropout](https://arxiv.org/abs/1506.02142).
-| 3 | `train_fn` from `astra.torch.utils` works for all types of models and losses which may or may not be from `astra`.
-| 4 | Though F1 score can be computed from precision and recall, we explicitely use F1 score formula to allow transparency and to avoid computing `TP` multiple times.
+5. We will try not to reduce code repetition at the expense of transparency, flexibility and performance. Too much abstraction often makes the API complex to understand and thus becomes hard to adapt for custom use cases.                                        |
 
 # Install
 
 Stable version:
 ```bash
 pip install astra-lib
 ```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: astra-lib Version: 0.0.5 Summary: A ML toolkit with
+Metadata-Version: 2.1 Name: astra-lib Version: 0.0.6 Summary: A ML toolkit with
 code bits useful for our day to day research Home-page: https://github.com/
 sustainability-lab/ASTRA Author: Nipun Batra Author-email:
 nipun.batra@iitgn.ac.in License: MIT Requires-Python: >=3.9 Description-
 Content-Type: text/markdown Requires-Dist: numpy Requires-Dist: pandas
 Requires-Dist: matplotlib Requires-Dist: xarray Requires-Dist: tqdm Requires-
 Dist: optree Requires-Dist: wandb
   [https://github.com/sustainability-lab/ASTRA/assets/59758528/d6a8e7ed-5368-
@@ -11,63 +11,54 @@
      _s_u_s_t_a_i_n_a_b_i_l_i_t_y_-_l_a_b_/_A_S_T_R_A_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_s_/_C_I_._y_m_l_/_b_a_d_g_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
    _c_o_v_e_r_a_l_l_s_._i_o_/_r_e_p_o_s_/_g_i_t_h_u_b_/_s_u_s_t_a_i_n_a_b_i_l_i_t_y_-_l_a_b_/_A_S_T_R_A_/_b_a_d_g_e_._s_v_g_?_b_r_a_n_c_h_=_m_a_i_n_]
 "**A**I for **S**ustainability" **T**oolkit for **R**esearch and **A**nalysis.
 ASTRA (à¤à¤¸à¥à¤¤à¥à¤°) means a "tool" or "a weapon" in Sanskrit. # Design
 Principles Since `astra` is developed for research purposes, we'd try to adhere
 to these principles: ## What we will try to do: 1. Keep the API simple-to-use
 and standardized to enable quick prototyping via automated scripts. 2. Keep the
-API transparent to expose as many details as possilbe. Explicit should be
+API transparent to expose as many details as possible. Explicit should be
 preferred over implicit. 3. Keep the API flexible to allow users to stretch the
-limits of their experiments. ## What we will try to avoid: 4. We will try not
-to reduce code repeatation at expence of transparency, flexibility and
-performance. Too much abstraction often makes the API complex to understand and
-thus becomes hard to adapt for custom use cases. ## Examples | Points | Example
-| | --- | --- | | 1 and 2 | We have exactly same arguments for all strategies
-in `astra.torch.al.strategies` to ease the automation but we explicitely
-mention in the docstrings if an argument is used or ignored for a strategy. | |
-2 | predict functions in `astra` by default put the model on `eval` mode but
-also allow to set `eval_mode` to `False`. This can be useful for techniques
-like [MC dropout](https://arxiv.org/abs/1506.02142). | 3 | `train_fn` from
-`astra.torch.utils` works for all types of models and losses which may or may
-not be from `astra`. | 4 | Though F1 score can be computed from precision and
-recall, we explicitely use F1 score formula to allow transparency and to avoid
-computing `TP` multiple times. # Install Stable version: ```bash pip install
-astra-lib ``` Latest version: ```bash pip install git+https://github.com/
-sustainability-lab/ASTRA ``` # Contributing Please go through the [contributing
-guidelines](CONTRIBUTING.md) before making a contribution. # Useful Code
-Snippets ## Data ### Load Data ```python from astra.torch.data import
-load_mnist, load_cifar_10 data = load_cifar_10() print(data) ``` ````python
-Files already downloaded and verified Files already downloaded and verified
-CIFAR-10 Dataset length of dataset: 60000 shape of images: torch.Size([3, 32,
-32]) len of classes: 10 classes: ['airplane', 'automobile', 'bird', 'cat',
-'deer', 'dog', 'frog', 'horse', 'ship', 'truck'] dtype of images: torch.float32
-dtype of labels: torch.int64 range of image values: min=0.0, max=1.0 ```` ##
-Models ### MLPs ```python from astra.torch.models import MLPRegressor mlp =
-MLPRegressor(input_dim=100, hidden_dims=[128, 64], output_dim=10,
-activation="relu", dropout=0.1) print(mlp) ``` ```python MLPRegressor(
-(featurizer): MLP( (dropout): Dropout(p=0.1, inplace=False) (input_layer):
-Linear(in_features=100, out_features=128, bias=True) (hidden_layer_1): Linear
-(in_features=128, out_features=64, bias=True) ) (regressor): Linear
-(in_features=64, out_features=10, bias=True) ) ``` ### CNNs ```python from
-astra.torch.models import CNNClassifier cnn = CNNClassifier( image_dims=(32,
-32), kernel_size=5, input_channels=3, conv_hidden_dims=[32, 64],
-dense_hidden_dims=[128, 64], n_classes=10, ) print(cnn) ``` ```python
-CNNClassifier( (featurizer): CNN( (activation): ReLU() (max_pool): MaxPool2d
-(kernel_size=2, stride=2, padding=0, dilation=1, ceil_mode=False)
-(input_layer): Conv2d(3, 32, kernel_size=(5, 5), stride=(1, 1), padding=(2, 2))
-(hidden_layer_1): Conv2d(32, 64, kernel_size=(5, 5), stride=(1, 1), padding=(2,
-2)) (aggregator): Identity() (flatten): Flatten(start_dim=1, end_dim=-1) )
-(classifier): MLPClassifier( (featurizer): MLP( (activation): ReLU() (dropout):
-Dropout(p=0.0, inplace=False) (input_layer): Linear(in_features=4096,
+limits of their experiments. 4. Don't provide defaults at most places. This
+will force the user to think about the choices they are making. ## What we will
+try to avoid: 5. We will try not to reduce code repetition at the expense of
+transparency, flexibility and performance. Too much abstraction often makes the
+API complex to understand and thus becomes hard to adapt for custom use cases.
+| # Install Stable version: ```bash pip install astra-lib ``` Latest version:
+```bash pip install git+https://github.com/sustainability-lab/ASTRA ``` #
+Contributing Please go through the [contributing guidelines](CONTRIBUTING.md)
+before making a contribution. # Useful Code Snippets ## Data ### Load Data
+```python from astra.torch.data import load_mnist, load_cifar_10 data =
+load_cifar_10() print(data) ``` ````python Files already downloaded and
+verified Files already downloaded and verified CIFAR-10 Dataset length of
+dataset: 60000 shape of images: torch.Size([3, 32, 32]) len of classes: 10
+classes: ['airplane', 'automobile', 'bird', 'cat', 'deer', 'dog', 'frog',
+'horse', 'ship', 'truck'] dtype of images: torch.float32 dtype of labels:
+torch.int64 range of image values: min=0.0, max=1.0 ```` ## Models ### MLPs
+```python from astra.torch.models import MLPRegressor mlp = MLPRegressor
+(input_dim=100, hidden_dims=[128, 64], output_dim=10, activation="relu",
+dropout=0.1) print(mlp) ``` ```python MLPRegressor( (featurizer): MLP(
+(dropout): Dropout(p=0.1, inplace=False) (input_layer): Linear(in_features=100,
 out_features=128, bias=True) (hidden_layer_1): Linear(in_features=128,
-out_features=64, bias=True) ) (classifier): Linear(in_features=64,
-out_features=10, bias=True) ) ) ``` ### EfficientNets ```python import torch
-from torchvision.models import efficientnet_b0, EfficientNet_B0_Weights from
-astra.torch.models import EfficientNetClassifier # Pretrained model model =
-EfficientNetClassifier(model=efficientnet_b0,
+out_features=64, bias=True) ) (regressor): Linear(in_features=64,
+out_features=10, bias=True) ) ``` ### CNNs ```python from astra.torch.models
+import CNNClassifier cnn = CNNClassifier( image_dims=(32, 32), kernel_size=5,
+input_channels=3, conv_hidden_dims=[32, 64], dense_hidden_dims=[128, 64],
+n_classes=10, ) print(cnn) ``` ```python CNNClassifier( (featurizer): CNN(
+(activation): ReLU() (max_pool): MaxPool2d(kernel_size=2, stride=2, padding=0,
+dilation=1, ceil_mode=False) (input_layer): Conv2d(3, 32, kernel_size=(5, 5),
+stride=(1, 1), padding=(2, 2)) (hidden_layer_1): Conv2d(32, 64, kernel_size=(5,
+5), stride=(1, 1), padding=(2, 2)) (aggregator): Identity() (flatten): Flatten
+(start_dim=1, end_dim=-1) ) (classifier): MLPClassifier( (featurizer): MLP(
+(activation): ReLU() (dropout): Dropout(p=0.0, inplace=False) (input_layer):
+Linear(in_features=4096, out_features=128, bias=True) (hidden_layer_1): Linear
+(in_features=128, out_features=64, bias=True) ) (classifier): Linear
+(in_features=64, out_features=10, bias=True) ) ) ``` ### EfficientNets
+```python import torch from torchvision.models import efficientnet_b0,
+EfficientNet_B0_Weights from astra.torch.models import EfficientNetClassifier #
+Pretrained model model = EfficientNetClassifier(model=efficientnet_b0,
 weights=EfficientNet_B0_Weights.DEFAULT, n_classes=10) # OR without pretrained
 weights # model = EfficientNetClassifier(model=efficientnet_b0, weights=None,
 n_classes=10) x = torch.rand(10, 3, 224, 224) out = model(x) print(out.shape)
 ``` ```python torch.Size([10, 10]) ``` ### ViT ```python import torch from
 torchvision.models import vit_b_16, ViT_B_16_Weights from astra.torch.models
 import ViTClassifier model = ViTClassifier(vit_b_16, ViT_B_16_Weights.DEFAULT,
 n_classes=10) x = torch.rand(10, 3, 224, 224) # (batch_size, channels, h, w)
```

### Comparing `astra-lib-0.0.5/astra_lib.egg-info/SOURCES.txt` & `astra_lib-0.0.6/astra_lib.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 setup.py
 .github/ISSUE_TEMPLATE/bug-report.yml
 .github/workflows/CI.template
 .github/workflows/CI.yml
 .github/workflows/publish.yml
 astra/__init__.py
 astra/_version.py
+astra/plot/utils.py
 astra/torch/__init__.py
 astra/torch/data.py
 astra/torch/metrics.py
 astra/torch/models.py
 astra/torch/utils.py
 astra/torch/al/README.md
 astra/torch/al/__init__.py
@@ -36,15 +37,14 @@
 astra/torch/al/strategies/mc.py
 astra/torch/al/strategies/random.py
 astra_lib.egg-info/PKG-INFO
 astra_lib.egg-info/SOURCES.txt
 astra_lib.egg-info/dependency_links.txt
 astra_lib.egg-info/requires.txt
 astra_lib.egg-info/top_level.txt
-notebooks/al/basic_example.ipynb
 quick_examples/advanced_train.py
 quick_examples/cnn.py
 quick_examples/count_params.py
 quick_examples/efficientnet.py
 quick_examples/load_data.py
 quick_examples/mlp.py
 quick_examples/quick_train.py
@@ -53,8 +53,11 @@
 sandbox/sandbox.ipynb
 tests/__init__.py
 tests/torch/test_data.py
 tests/torch/test_metrics.py
 tests/torch/test_models.py
 tests/torch/test_utils.py
 tests/torch/acquisitions/test_common.py
-tests/torch/acquisitions/test_uniform_random.py
+tests/torch/acquisitions/test_uniform_random.py
+tutorials/active_learning.ipynb
+tutorials/classification.ipynb
+tutorials/latexify.ipynb
```

### Comparing `astra-lib-0.0.5/customize.py` & `astra_lib-0.0.6/customize.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/notebooks/al/basic_example.ipynb` & `astra_lib-0.0.6/tutorials/active_learning.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9933159722222222%*

 * *Differences: {"'cells'": "{0: {'cell_type': 'markdown', 'source': ['# Active Learning'], delete: "*

 * *            "['execution_count', 'outputs']}, 1: {'source': {insert: [(0, 'import os\\n'), (2, "*

 * *            '\'os.environ["CUDA_VISIBLE_DEVICES"] = "3"\\n\'), (3, \'\\n\'), (4, \'import numpy as '*

 * *            "np\\n'), (5, '\\n'), (6, 'import torch\\n'), (7, 'import torch.nn as nn\\n'), (8, "*

 * *            "'\\n'), (9, 'from torchvision.models import efficientnet_b0, "*

 * *            "EfficientNet_B0_Weights\\n'), (10, 'from a […]*

```diff
@@ -1,58 +1,48 @@
 {
     "cells": [
         {
+            "cell_type": "markdown",
+            "metadata": {},
+            "source": [
+                "# Active Learning"
+            ]
+        },
+        {
             "cell_type": "code",
-            "execution_count": 1,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
                 "\n",
                 "os.environ[\"CUDA_VISIBLE_DEVICES\"] = \"3\"\n",
                 "\n",
                 "import numpy as np\n",
                 "\n",
                 "import torch\n",
                 "import torch.nn as nn\n",
-                "from torch.utils.data import DataLoader, TensorDataset\n",
                 "\n",
-                "from torchvision.datasets import CIFAR10\n",
-                "from torchvision.transforms import Normalize, Resize, Compose, CenterCrop, InterpolationMode\n",
                 "from torchvision.models import efficientnet_b0, EfficientNet_B0_Weights\n",
                 "from astra.torch.models import EfficientNet, CNN\n",
                 "from astra.torch.al import RandomAcquisition, RandomStrategy\n",
-                "from astra.torch.utils import train_fn, predict_class\n",
+                "from astra.torch.utils import train_fn\n",
                 "\n",
-                "from sklearn.metrics import accuracy_score\n",
+                "from astra.torch.metrics import accuracy_score\n",
                 "\n",
                 "import matplotlib.pyplot as plt\n",
                 "\n",
                 "device = \"cuda\"\n"
             ]
         },
         {
-            "cell_type": "code",
-            "execution_count": 2,
-            "metadata": {},
-            "outputs": [],
-            "source": [
-                "eff_transform = EfficientNet_B0_Weights.DEFAULT.transforms()\n",
-                "# print(eff_transform)\n",
-                "# transform = Compose([Resize(256, interpolation=InterpolationMode.BICUBIC), Normalize((0.485, 0.456, 0.406), (0.229, 0.224, 0.225))])\n",
-                "\n",
-                "# plt.imshow(transform(train_inputs[0:5])[0, 0].numpy())\n",
-                "# plt.imshow(transform(eff_transform(train_inputs[0:5]))[0, 0].numpy())"
-            ]
-        },
-        {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
-                "## Prepare the dataset"
+                "## Load the dataset"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 3,
             "metadata": {},
             "outputs": [
@@ -64,25 +54,15 @@
                         "Files already downloaded and verified\n",
                         "torch.Size([50000, 3, 32, 32]) <built-in method type of Tensor object at 0x7f8939963050>\n",
                         "torch.Size([50000]) <built-in method type of Tensor object at 0x7f8939960050>\n"
                     ]
                 }
             ],
             "source": [
-                "train_data = CIFAR10(root=\"./data\", train=True, download=True)\n",
-                "test_data = CIFAR10(root=\"./data\", train=False, download=True)\n",
-                "\n",
-                "train_inputs = torch.tensor(train_data.data).permute(0, 3, 1, 2).float() / 255\n",
-                "train_outputs = torch.tensor(train_data.targets).long()\n",
-                "\n",
-                "test_inputs = torch.tensor(test_data.data).permute(0, 3, 1, 2).float() / 255\n",
-                "test_outputs = torch.tensor(test_data.targets).long()\n",
-                "\n",
-                "print(train_inputs.shape, train_inputs.type)\n",
-                "print(train_outputs.shape, train_outputs.type)"
+                "dataset = load_cifar_10()"
             ]
         },
         {
             "cell_type": "markdown",
             "metadata": {},
             "source": [
                 "## Divide into train, test and pool"
```

### Comparing `astra-lib-0.0.5/quick_examples/advanced_train.py` & `astra_lib-0.0.6/quick_examples/advanced_train.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/quick_examples/quick_train.py` & `astra_lib-0.0.6/quick_examples/quick_train.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/quick_examples/train_with_dataloader.py` & `astra_lib-0.0.6/quick_examples/train_with_dataloader.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/sandbox/sandbox.ipynb` & `astra_lib-0.0.6/sandbox/sandbox.ipynb`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/tests/torch/acquisitions/test_common.py` & `astra_lib-0.0.6/tests/torch/acquisitions/test_common.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/tests/torch/acquisitions/test_uniform_random.py` & `astra_lib-0.0.6/tests/torch/acquisitions/test_uniform_random.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/tests/torch/test_data.py` & `astra_lib-0.0.6/tests/torch/test_data.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/tests/torch/test_models.py` & `astra_lib-0.0.6/tests/torch/test_models.py`

 * *Files identical despite different names*

### Comparing `astra-lib-0.0.5/tests/torch/test_utils.py` & `astra_lib-0.0.6/tests/torch/test_utils.py`

 * *Files identical despite different names*

