# Comparing `tmp/syngen-0.8.5.tar.gz` & `tmp/syngen-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.8.5.tar", last modified: Mon May 27 07:23:05 2024, max compression
+gzip compressed data, was "syngen-0.9.0.tar", last modified: Sat Jun  1 04:06:37 2024, max compression
```

## Comparing `syngen-0.8.5.tar` & `syngen-0.9.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.399691 syngen-0.8.5/
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-27 07:21:45.000000 syngen-0.8.5/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-27 07:21:45.000000 syngen-0.8.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-27 07:21:45.000000 syngen-0.8.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    27084 2024-05-27 07:23:05.399691 syngen-0.8.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25181 2024-05-27 07:21:45.000000 syngen-0.8.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-27 07:21:45.000000 syngen-0.8.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-27 07:23:05.399691 syngen-0.8.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.379691 syngen-0.8.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.387691 syngen-0.8.5/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.387691 syngen-0.8.5/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.387691 syngen-0.8.5/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/config/configurations.py
--rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/config/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.387691 syngen-0.8.5/src/syngen/ml/context/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/context/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.387691 syngen-0.8.5/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.387691 syngen-0.8.5/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17252 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.387691 syngen-0.8.5/src/syngen/ml/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18411 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/handlers/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.387691 syngen-0.8.5/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/metrics/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.391691 syngen-0.8.5/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   723510 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.391691 syngen-0.8.5/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.391691 syngen-0.8.5/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)   528976 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.391691 syngen-0.8.5/src/syngen/ml/metrics/accuracy_test/src/img/
--rw-r--r--   0 runner    (1001) docker     (127)      983 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg
--rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/metrics/accuracy_test/src/main.css
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/metrics/accuracy_test/src/script.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.391691 syngen-0.8.5/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46709 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.391691 syngen-0.8.5/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   708975 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.391691 syngen-0.8.5/src/syngen/ml/mlflow_tracker/
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/mlflow_tracker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6929 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/mlflow_tracker/mlflow_tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.391691 syngen-0.8.5/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (127)      137 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9796 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.391691 syngen-0.8.5/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8243 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.391691 syngen-0.8.5/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12235 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.391691 syngen-0.8.5/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/vae/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.395691 syngen-0.8.5/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/vae/models/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (127)    46231 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    24260 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.395691 syngen-0.8.5/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13916 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.395691 syngen-0.8.5/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.395691 syngen-0.8.5/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15659 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/ml/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.395691 syngen-0.8.5/src/syngen/streamlit_app/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.395691 syngen-0.8.5/src/syngen/streamlit_app/.streamlit/
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/streamlit_app/.streamlit/config.toml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/streamlit_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.395691 syngen-0.8.5/src/syngen/streamlit_app/css/
--rw-r--r--   0 runner    (1001) docker     (127)   707122 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/streamlit_app/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.395691 syngen-0.8.5/src/syngen/streamlit_app/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/streamlit_app/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/streamlit_app/handlers/handlers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.395691 syngen-0.8.5/src/syngen/streamlit_app/img/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/streamlit_app/img/favicon.svg
--rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/streamlit_app/img/logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/streamlit_app/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/streamlit_app/start.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.395691 syngen-0.8.5/src/syngen/streamlit_app/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/streamlit_app/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/streamlit_app/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-05-27 07:21:45.000000 syngen-0.8.5/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 07:23:05.395691 syngen-0.8.5/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    27084 2024-05-27 07:23:05.000000 syngen-0.8.5/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-05-27 07:23:05.000000 syngen-0.8.5/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 07:23:05.000000 syngen-0.8.5/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-27 07:23:05.000000 syngen-0.8.5/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-27 07:23:05.000000 syngen-0.8.5/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-27 07:23:05.000000 syngen-0.8.5/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.321091 syngen-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      400 2024-06-01 04:05:15.000000 syngen-0.9.0/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 04:05:15.000000 syngen-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-01 04:05:15.000000 syngen-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    29861 2024-06-01 04:06:37.321091 syngen-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27936 2024-06-01 04:05:15.000000 syngen-0.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-06-01 04:05:15.000000 syngen-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-06-01 04:06:37.321091 syngen-0.9.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.305091 syngen-0.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.309091 syngen-0.9.0/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.309091 syngen-0.9.0/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.309091 syngen-0.9.0/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11758 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/config/configurations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13290 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/config/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.309091 syngen-0.9.0/src/syngen/ml/context/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/context/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.309091 syngen-0.9.0/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3589 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.309091 syngen-0.9.0/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17252 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.309091 syngen-0.9.0/src/syngen/ml/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18510 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/handlers/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.309091 syngen-0.9.0/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/metrics/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.313091 syngen-0.9.0/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   723510 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (127)     9558 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.313091 syngen-0.9.0/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.313091 syngen-0.9.0/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)   528976 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.313091 syngen-0.9.0/src/syngen/ml/metrics/accuracy_test/src/img/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     3988 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/metrics/accuracy_test/src/main.css
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/metrics/accuracy_test/src/script.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.313091 syngen-0.9.0/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46709 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.313091 syngen-0.9.0/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   708975 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.313091 syngen-0.9.0/src/syngen/ml/mlflow_tracker/
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/mlflow_tracker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9520 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/mlflow_tracker/mlflow_tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.313091 syngen-0.9.0/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (127)      137 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9683 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.313091 syngen-0.9.0/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8414 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.313091 syngen-0.9.0/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12414 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.313091 syngen-0.9.0/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/vae/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.317091 syngen-0.9.0/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/vae/models/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46231 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24260 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10457 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.317091 syngen-0.9.0/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14141 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.317091 syngen-0.9.0/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8055 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.317091 syngen-0.9.0/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19173 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/ml/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.317091 syngen-0.9.0/src/syngen/streamlit_app/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.317091 syngen-0.9.0/src/syngen/streamlit_app/.streamlit/
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/streamlit_app/.streamlit/config.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/streamlit_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.317091 syngen-0.9.0/src/syngen/streamlit_app/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   707122 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/streamlit_app/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.317091 syngen-0.9.0/src/syngen/streamlit_app/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/streamlit_app/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/streamlit_app/handlers/handlers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.317091 syngen-0.9.0/src/syngen/streamlit_app/img/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/streamlit_app/img/favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     7417 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/streamlit_app/img/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     5883 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/streamlit_app/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/streamlit_app/start.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.317091 syngen-0.9.0/src/syngen/streamlit_app/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/streamlit_app/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/streamlit_app/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5633 2024-06-01 04:05:15.000000 syngen-0.9.0/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:06:37.317091 syngen-0.9.0/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29861 2024-06-01 04:06:37.000000 syngen-0.9.0/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-06-01 04:06:37.000000 syngen-0.9.0/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 04:06:37.000000 syngen-0.9.0/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-06-01 04:06:37.000000 syngen-0.9.0/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-06-01 04:06:37.000000 syngen-0.9.0/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-06-01 04:06:37.000000 syngen-0.9.0/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.8.5/LICENSE` & `syngen-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/PKG-INFO` & `syngen-0.9.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.8.5
+Version: 0.9.0
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,14 +33,15 @@
 Requires-Dist: mlflow==2.13.*
 Requires-Dist: numpy==1.23.*
 Requires-Dist: openpyxl
 Requires-Dist: pandas==1.3.*
 Requires-Dist: pandavro==1.7.2
 Requires-Dist: pathos==0.2.*
 Requires-Dist: pillow==10.3.*
+Requires-Dist: psutil
 Requires-Dist: py-ulid
 Requires-Dist: pytest
 Requires-Dist: pytest-reportportal
 Requires-Dist: python-slugify[unidecode]>=7.0.0
 Requires-Dist: PyYAML==6.*
 Requires-Dist: reportportal-client
 Requires-Dist: scikit_learn==1.1.*
@@ -459,40 +460,132 @@
 
 #### MLflow monitoring
 
 Set the `MLFLOW_TRACKING_URI` environment variable to the desired MLflow tracking server, for instance:
 http://localhost:5000/. You can also set the `MLFLOW_ARTIFACTS_DESTINATION` environment variable to your preferred path 
 (including the cloud path), where the artifacts should be stored. Additionally, set the `MLFLOW_EXPERIMENT_NAME` 
 environment variable to the name you prefer for the experiment. 
+To get the system metrics, please set the `MLFLOW_ENABLE_SYSTEM_METRICS_LOGGING` environment variable to `true`.
+By default, the metrics are logged every 10 seconds, but the interval may be changed by setting the environment variable 
+`MLFLOW_SYSTEM_METRICS_SAMPLING_INTERVAL` (for more detailed description look [here](https://mlflow.org/docs/latest/system-metrics/index.html))
+
 When using Docker, ensure the environmental variables are set before running the container.
 
 The provided environmental variables allow to track the training process, and the inference process, and store 
 the artifacts in the desired location.
 You can access the MLflow UI by navigating to the provided URL in your browser. If you store artifacts in remote storage,
 ensure that all necessary credentials are provided before using Mlflow.
 
 ```bash
 docker pull tdspora/syngen:latest
 docker run --rm -it \
   --user $(id -u):$(id -g) \
   -e MLFLOW_TRACKING_URI='http://localhost:5000' \
   -e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION \
   -e MLFLOW_EXPERIMENT_NAME=test_name \
+  -e MLFLOW_ENABLE_SYSTEM_METRICS_LOGGING=true \
+  -e MLFLOW_SYSTEM_METRICS_SAMPLING_INTERVAL 10 \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 
 docker run --rm -it \
   --user $(id -u):$(id -g) \
   -e MLFLOW_TRACKING_URI='http://localhost:5000' \
   -e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION \
   -e MLFLOW_EXPERIMENT_NAME=test_name \
+  -e MLFLOW_ENABLE_SYSTEM_METRICS_LOGGING=true \
+  -e MLFLOW_SYSTEM_METRICS_SAMPLING_INTERVAL 10 \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 ```
 
+## Syngen Installation Guide for MacOS ARM (M1/M2) with Python 3.10
+
+### Prerequisites
+
+Before you begin, make sure you have the following installed:
+
+- Python 3.10
+- Homebrew (optional but recommended for managing dependencies)
+
+### Installation Steps
+
+1. **Upgrade pip**: Ensure you have the latest version of `pip`.
+
+    ```sh
+    pip install --upgrade pip
+    ```
+
+2. **Install Setuptools, Wheel, and Cython**: These packages are necessary for building and installing other dependencies.
+
+    ```sh
+    pip install setuptools wheel 'Cython<3'
+    ```
+
+3. **Install Fastavro**: Install a specific version of `fastavro` to avoid build issues.
+
+    ```sh
+    pip install --no-build-isolation fastavro==1.5.1
+    ```
+
+4. **Install Syngen**: Now, you can install the Syngen package.
+
+    ```sh
+    pip install syngen
+    ```
+
+5. **Install TensorFlow Metal**: This package leverages the GPU capabilities of M1/M2 chips for TensorFlow.
+
+    ```sh
+    pip install tensorflow-metal
+    ```
+
+#### From source (development)
+
+Download repository from GitHub by cloning or zip file.
+Then install it in editable mode.
+
+```sh
+    pip install -e .
+```
+
+### Additional Information
+
+- **Homebrew**: If you do not have Homebrew installed, you can install it by running:
+
+    ```sh
+    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
+    ```
+
+- **Python 3.10**: Ensure you have Python 3.10 installed. You can use pyenv to manage different Python versions:
+
+    ```sh
+    brew install pyenv
+    pyenv install 3.10.0
+    pyenv global 3.10.0
+    ```
+
+### Verifying Installation
+
+To verify the installation, run the following command to check if Syngen is installed correctly:
+
+```sh
+python -c "import syngen; print(syngen.__version__)"
+```
+
+If the command prints the version of Syngen without errors, the installation was successful.
+
+### Troubleshooting
+
+If you encounter any issues during installation, consider the following steps:
+
+- Ensure all dependencies are up to date.
+- Check for any compatibility issues with other installed packages.
+- Consult the Syngen [documentation](https://github.com/tdspora/syngen) or raise an issue on GitHub.
+
 ## Contribution
 
 We welcome contributions from the community to help us improve and maintain our public GitHub repository. We appreciate any feedback, bug reports, or feature requests, and we encourage developers to submit fixes or new features using issues.
 
 If you have found a bug or have a feature request, please submit an issue to our GitHub repository. Please provide as much detail as possible, including steps to reproduce the issue or a clear description of the feature request. Our team will review the issue and work with you to address any problems or discuss any potential new features.
 
 If you would like to contribute a fix or a new feature, please submit a pull request to our GitHub repository. Please make sure your code follows our coding standards and best practices. Our team will review your pull request and work with you to ensure that it meets our standards and is ready for inclusion in our codebase.
```

### Comparing `syngen-0.8.5/README.md` & `syngen-0.9.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -401,40 +401,132 @@
 
 #### MLflow monitoring
 
 Set the `MLFLOW_TRACKING_URI` environment variable to the desired MLflow tracking server, for instance:
 http://localhost:5000/. You can also set the `MLFLOW_ARTIFACTS_DESTINATION` environment variable to your preferred path 
 (including the cloud path), where the artifacts should be stored. Additionally, set the `MLFLOW_EXPERIMENT_NAME` 
 environment variable to the name you prefer for the experiment. 
+To get the system metrics, please set the `MLFLOW_ENABLE_SYSTEM_METRICS_LOGGING` environment variable to `true`.
+By default, the metrics are logged every 10 seconds, but the interval may be changed by setting the environment variable 
+`MLFLOW_SYSTEM_METRICS_SAMPLING_INTERVAL` (for more detailed description look [here](https://mlflow.org/docs/latest/system-metrics/index.html))
+
 When using Docker, ensure the environmental variables are set before running the container.
 
 The provided environmental variables allow to track the training process, and the inference process, and store 
 the artifacts in the desired location.
 You can access the MLflow UI by navigating to the provided URL in your browser. If you store artifacts in remote storage,
 ensure that all necessary credentials are provided before using Mlflow.
 
 ```bash
 docker pull tdspora/syngen:latest
 docker run --rm -it \
   --user $(id -u):$(id -g) \
   -e MLFLOW_TRACKING_URI='http://localhost:5000' \
   -e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION \
   -e MLFLOW_EXPERIMENT_NAME=test_name \
+  -e MLFLOW_ENABLE_SYSTEM_METRICS_LOGGING=true \
+  -e MLFLOW_SYSTEM_METRICS_SAMPLING_INTERVAL 10 \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 
 docker run --rm -it \
   --user $(id -u):$(id -g) \
   -e MLFLOW_TRACKING_URI='http://localhost:5000' \
   -e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION \
   -e MLFLOW_EXPERIMENT_NAME=test_name \
+  -e MLFLOW_ENABLE_SYSTEM_METRICS_LOGGING=true \
+  -e MLFLOW_SYSTEM_METRICS_SAMPLING_INTERVAL 10 \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 ```
 
+## Syngen Installation Guide for MacOS ARM (M1/M2) with Python 3.10
+
+### Prerequisites
+
+Before you begin, make sure you have the following installed:
+
+- Python 3.10
+- Homebrew (optional but recommended for managing dependencies)
+
+### Installation Steps
+
+1. **Upgrade pip**: Ensure you have the latest version of `pip`.
+
+    ```sh
+    pip install --upgrade pip
+    ```
+
+2. **Install Setuptools, Wheel, and Cython**: These packages are necessary for building and installing other dependencies.
+
+    ```sh
+    pip install setuptools wheel 'Cython<3'
+    ```
+
+3. **Install Fastavro**: Install a specific version of `fastavro` to avoid build issues.
+
+    ```sh
+    pip install --no-build-isolation fastavro==1.5.1
+    ```
+
+4. **Install Syngen**: Now, you can install the Syngen package.
+
+    ```sh
+    pip install syngen
+    ```
+
+5. **Install TensorFlow Metal**: This package leverages the GPU capabilities of M1/M2 chips for TensorFlow.
+
+    ```sh
+    pip install tensorflow-metal
+    ```
+
+#### From source (development)
+
+Download repository from GitHub by cloning or zip file.
+Then install it in editable mode.
+
+```sh
+    pip install -e .
+```
+
+### Additional Information
+
+- **Homebrew**: If you do not have Homebrew installed, you can install it by running:
+
+    ```sh
+    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
+    ```
+
+- **Python 3.10**: Ensure you have Python 3.10 installed. You can use pyenv to manage different Python versions:
+
+    ```sh
+    brew install pyenv
+    pyenv install 3.10.0
+    pyenv global 3.10.0
+    ```
+
+### Verifying Installation
+
+To verify the installation, run the following command to check if Syngen is installed correctly:
+
+```sh
+python -c "import syngen; print(syngen.__version__)"
+```
+
+If the command prints the version of Syngen without errors, the installation was successful.
+
+### Troubleshooting
+
+If you encounter any issues during installation, consider the following steps:
+
+- Ensure all dependencies are up to date.
+- Check for any compatibility issues with other installed packages.
+- Consult the Syngen [documentation](https://github.com/tdspora/syngen) or raise an issue on GitHub.
+
 ## Contribution
 
 We welcome contributions from the community to help us improve and maintain our public GitHub repository. We appreciate any feedback, bug reports, or feature requests, and we encourage developers to submit fixes or new features using issues.
 
 If you have found a bug or have a feature request, please submit an issue to our GitHub repository. Please provide as much detail as possible, including steps to reproduce the issue or a clear description of the feature request. Our team will review the issue and work with you to address any problems or discuss any potential new features.
 
 If you would like to contribute a fix or a new feature, please submit a pull request to our GitHub repository. Please make sure your code follows our coding standards and best practices. Our team will review your pull request and work with you to ensure that it meets our standards and is ready for inclusion in our codebase.
```

#### html2text {}

```diff
@@ -258,38 +258,74 @@
 tdspora/syngen docker run -p 8501:8501 tdspora/syngen --webui ``` The UI will
 be available at
 localhost:8501>. #### MLflow monitoring Set the `MLFLOW_TRACKING_URI`
 environment variable to the desired MLflow tracking server, for instance: http:
 //localhost:5000/. You can also set the `MLFLOW_ARTIFACTS_DESTINATION`
 environment variable to your preferred path (including the cloud path), where
 the artifacts should be stored. Additionally, set the `MLFLOW_EXPERIMENT_NAME`
-environment variable to the name you prefer for the experiment. When using
+environment variable to the name you prefer for the experiment. To get the
+system metrics, please set the `MLFLOW_ENABLE_SYSTEM_METRICS_LOGGING`
+environment variable to `true`. By default, the metrics are logged every 10
+seconds, but the interval may be changed by setting the environment variable
+`MLFLOW_SYSTEM_METRICS_SAMPLING_INTERVAL` (for more detailed description look
+[here](https://mlflow.org/docs/latest/system-metrics/index.html)) When using
 Docker, ensure the environmental variables are set before running the
 container. The provided environmental variables allow to track the training
 process, and the inference process, and store the artifacts in the desired
 location. You can access the MLflow UI by navigating to the provided URL in
 your browser. If you store artifacts in remote storage, ensure that all
 necessary credentials are provided before using Mlflow. ```bash docker pull
 tdspora/syngen:latest docker run --rm -it \ --user $(id -u):$(id -g) \ -
 e MLFLOW_TRACKING_URI='http://localhost:5000' \ -
 e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION \ -
-e MLFLOW_EXPERIMENT_NAME=test_name \ -v PATH_TO_LOCAL_FOLDER:/src/
+e MLFLOW_EXPERIMENT_NAME=test_name \ -
+e MLFLOW_ENABLE_SYSTEM_METRICS_LOGGING=true \ -
+e MLFLOW_SYSTEM_METRICS_SAMPLING_INTERVAL 10 \ -v PATH_TO_LOCAL_FOLDER:/src/
 model_artifacts tdspora/syngen \ --metadata_path=./model_artifacts/
 PATH_TO_METADATA_YAML docker run --rm -it \ --user $(id -u):$(id -g) \ -
 e MLFLOW_TRACKING_URI='http://localhost:5000' \ -
 e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION \ -
-e MLFLOW_EXPERIMENT_NAME=test_name \ -v PATH_TO_LOCAL_FOLDER:/src/
+e MLFLOW_EXPERIMENT_NAME=test_name \ -
+e MLFLOW_ENABLE_SYSTEM_METRICS_LOGGING=true \ -
+e MLFLOW_SYSTEM_METRICS_SAMPLING_INTERVAL 10 \ -v PATH_TO_LOCAL_FOLDER:/src/
 model_artifacts tdspora/syngen \ --metadata_path=./model_artifacts/
-PATH_TO_METADATA_YAML ``` ## Contribution We welcome contributions from the
-community to help us improve and maintain our public GitHub repository. We
-appreciate any feedback, bug reports, or feature requests, and we encourage
-developers to submit fixes or new features using issues. If you have found a
-bug or have a feature request, please submit an issue to our GitHub repository.
-Please provide as much detail as possible, including steps to reproduce the
-issue or a clear description of the feature request. Our team will review the
-issue and work with you to address any problems or discuss any potential new
-features. If you would like to contribute a fix or a new feature, please submit
-a pull request to our GitHub repository. Please make sure your code follows our
-coding standards and best practices. Our team will review your pull request and
-work with you to ensure that it meets our standards and is ready for inclusion
-in our codebase. We appreciate your contributions, and thank you for your
-interest in helping us maintain and improve our public GitHub repository.
+PATH_TO_METADATA_YAML ``` ## Syngen Installation Guide for MacOS ARM (M1/M2)
+with Python 3.10 ### Prerequisites Before you begin, make sure you have the
+following installed: - Python 3.10 - Homebrew (optional but recommended for
+managing dependencies) ### Installation Steps 1. **Upgrade pip**: Ensure you
+have the latest version of `pip`. ```sh pip install --upgrade pip ``` 2.
+**Install Setuptools, Wheel, and Cython**: These packages are necessary for
+building and installing other dependencies. ```sh pip install setuptools wheel
+'Cython<3' ``` 3. **Install Fastavro**: Install a specific version of
+`fastavro` to avoid build issues. ```sh pip install --no-build-isolation
+fastavro==1.5.1 ``` 4. **Install Syngen**: Now, you can install the Syngen
+package. ```sh pip install syngen ``` 5. **Install TensorFlow Metal**: This
+package leverages the GPU capabilities of M1/M2 chips for TensorFlow. ```sh pip
+install tensorflow-metal ``` #### From source (development) Download repository
+from GitHub by cloning or zip file. Then install it in editable mode. ```sh pip
+install -e . ``` ### Additional Information - **Homebrew**: If you do not have
+Homebrew installed, you can install it by running: ```sh /bin/bash -c "$(curl -
+fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)" ``` -
+**Python 3.10**: Ensure you have Python 3.10 installed. You can use pyenv to
+manage different Python versions: ```sh brew install pyenv pyenv install 3.10.0
+pyenv global 3.10.0 ``` ### Verifying Installation To verify the installation,
+run the following command to check if Syngen is installed correctly: ```sh
+python -c "import syngen; print(syngen.__version__)" ``` If the command prints
+the version of Syngen without errors, the installation was successful. ###
+Troubleshooting If you encounter any issues during installation, consider the
+following steps: - Ensure all dependencies are up to date. - Check for any
+compatibility issues with other installed packages. - Consult the Syngen
+[documentation](https://github.com/tdspora/syngen) or raise an issue on GitHub.
+## Contribution We welcome contributions from the community to help us improve
+and maintain our public GitHub repository. We appreciate any feedback, bug
+reports, or feature requests, and we encourage developers to submit fixes or
+new features using issues. If you have found a bug or have a feature request,
+please submit an issue to our GitHub repository. Please provide as much detail
+as possible, including steps to reproduce the issue or a clear description of
+the feature request. Our team will review the issue and work with you to
+address any problems or discuss any potential new features. If you would like
+to contribute a fix or a new feature, please submit a pull request to our
+GitHub repository. Please make sure your code follows our coding standards and
+best practices. Our team will review your pull request and work with you to
+ensure that it meets our standards and is ready for inclusion in our codebase.
+We appreciate your contributions, and thank you for your interest in helping us
+maintain and improve our public GitHub repository.
```

### Comparing `syngen-0.8.5/setup.cfg` & `syngen-0.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 	mlflow==2.13.*
 	numpy==1.23.*
 	openpyxl
 	pandas==1.3.*
 	pandavro==1.7.2
 	pathos==0.2.*
 	pillow==10.3.*
+	psutil
 	py-ulid
 	pytest
 	pytest-reportportal
 	python-slugify[unidecode]>=7.0.0
 	PyYAML==6.*
 	reportportal-client
 	scikit_learn==1.1.*
```

### Comparing `syngen-0.8.5/src/syngen/infer.py` & `syngen-0.9.0/src/syngen/infer.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/config/configurations.py` & `syngen-0.9.0/src/syngen/ml/config/configurations.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/config/validation.py` & `syngen-0.9.0/src/syngen/ml/config/validation.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/context/context.py` & `syngen-0.9.0/src/syngen/ml/context/context.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/convertor/convertor.py` & `syngen-0.9.0/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.9.0/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/handlers/handlers.py` & `syngen-0.9.0/src/syngen/ml/handlers/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 from syngen.ml.vae import *  # noqa: F403
 from syngen.ml.data_loaders import DataLoader
 from syngen.ml.utils import (
     fetch_dataset,
     check_if_features_assigned,
     generate_uuid,
+    get_initial_table_name,
     ProgressBarHandler
 )
 from syngen.ml.context import get_context
 
 
 class AbstractHandler(ABC):
     @abstractmethod
@@ -376,18 +377,18 @@
             destination_to_pk_table = infer_settings.get("destination")
 
             if destination_to_pk_table is None:
                 destination_to_pk_table = (
                     f"model_artifacts/tmp_store/{slugify(pk_table)}/"
                     f"merged_infer_{slugify(pk_table)}.csv"
                 )
-
+        initial_table_name = get_initial_table_name(table_name)
         if self.type_of_process == "train":
             destination_to_pk_table = self.paths["path_to_merged_infer"].replace(
-                slugify(table_name), slugify(pk_table)
+                slugify(initial_table_name), slugify(pk_table)
             )
         if not os.path.exists(destination_to_pk_table):
             raise FileNotFoundError(
                 "The table with a primary key specified in the metadata file does not "
                 "exist or is not trained. Ensure that the metadata contains the "
                 "name of referenced table with a primary key in the foreign key "
                 "declaration section."
```

### Comparing `syngen-0.8.5/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.9.0/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.9.0/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.9.0/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg` & `syngen-0.9.0/src/syngen/ml/metrics/accuracy_test/src/img/linear-gradient.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/metrics/accuracy_test/src/main.css` & `syngen-0.9.0/src/syngen/ml/metrics/accuracy_test/src/main.css`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.9.0/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.9.0/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.9.0/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/metrics/utils.py` & `syngen-0.9.0/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/reporters/reporters.py` & `syngen-0.9.0/src/syngen/ml/reporters/reporters.py`

 * *Files 1% similar despite different names*

```diff
@@ -180,20 +180,18 @@
     def generate_report(cls, type_of_process: str):
         """
         Generate all needed reports
         """
         grouped_reporters = cls._group_reporters()
 
         for table_name, reporters in grouped_reporters.items():
-            MlflowTracker.reset_status(active_status=True)
-            run_id = MlflowTracker().search_run(
-                table_name=table_name, type_of_process=type_of_process
+            MlflowTracker().start_run(
+                run_name=f"{table_name}-REPORT",
+                tags={"table_name": table_name, "process": "report"},
             )
-            if run_id is not None:
-                MlflowTracker().start_run(run_id=run_id)
             delta = 0.25 / len(reporters)
             for reporter in reporters:
                 message = (f"The calculation of {reporter.__class__.report_type} metrics "
                            f"for the table - '{reporter.table_name}' has started")
                 ProgressBarHandler().set_progress(delta=delta, message=message)
                 reporter.report()
                 if reporter.config["print_report"]:
```

### Comparing `syngen-0.8.5/src/syngen/ml/strategies/strategies.py` & `syngen-0.9.0/src/syngen/ml/strategies/strategies.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from abc import ABC, abstractmethod
 import os
+import re
 import traceback
 from loguru import logger
 
 os.environ["TF_CPP_MIN_LOG_LEVEL"] = "2"
 
 from syngen.ml.handlers import RootHandler
 from syngen.ml.reporters import Report, AccuracyReporter, SampleAccuracyReporter
 from syngen.ml.config import TrainConfig, InferConfig
 from syngen.ml.handlers import LongTextsHandler, VaeTrainHandler, VaeInferHandler
 from syngen.ml.vae import VanillaVAEWrapper
 from syngen.ml.data_loaders import BinaryLoader
 from syngen.ml.mlflow_tracker.mlflow_tracker import MlflowTracker
+from syngen.ml.utils import get_initial_table_name
 
 
 class Strategy(ABC):
     """
     Abstract class for the strategies of training or infer process
     """
 
@@ -109,21 +111,22 @@
 
         root_handler.set_next(vae_handler).set_next(long_text_handler)
 
         self.handler = root_handler
         return self
 
     def add_reporters(self, **kwargs):
-        if self.config.print_report:
+        table_name = self.config.table_name
+        if not table_name.endswith("_fk") and self.config.print_report:
             sample_reporter = SampleAccuracyReporter(
-                table_name=self.config.table_name,
+                table_name=get_initial_table_name(table_name),
                 paths=self.config.paths,
                 config=self.config.to_dict(),
             )
-            Report().register_reporter(table=self.config.table_name, reporter=sample_reporter)
+            Report().register_reporter(table=table_name, reporter=sample_reporter)
 
         return self
 
     def run(self, **kwargs):
         """
         Launch the training process
         """
@@ -193,21 +196,23 @@
             get_infer_metrics=self.config.get_infer_metrics,
             log_level=self.config.log_level,
             type_of_process=type_of_process,
         )
         return self
 
     def add_reporters(self):
-        if self.config.print_report or self.config.get_infer_metrics:
-            accuracy_reporter = AccuracyReporter(
-                table_name=self.config.table_name,
-                paths=self.config.paths,
-                config=self.config.to_dict(),
-            )
-            Report().register_reporter(table=self.config.table_name, reporter=accuracy_reporter)
+        table_name = self.config.table_name
+        if not table_name.endswith("_fk") and \
+                (self.config.print_report or self.config.get_infer_metrics):
+                accuracy_reporter = AccuracyReporter(
+                    table_name=get_initial_table_name(table_name),
+                    paths=self.config.paths,
+                    config=self.config.to_dict(),
+                )
+                Report().register_reporter(table=table_name, reporter=accuracy_reporter)
 
         return self
 
     def run(self, **kwargs):
         """
         Launch the infer process
         """
@@ -222,20 +227,19 @@
                 batch_size=kwargs["batch_size"],
                 random_seed=kwargs["random_seed"],
                 print_report=kwargs["print_report"],
                 get_infer_metrics=kwargs["get_infer_metrics"],
                 log_level=kwargs["log_level"],
                 both_keys=kwargs["both_keys"],
             )
-            type_of_process = kwargs["type_of_process"]
-            if type_of_process == "infer":
-                MlflowTracker().log_params(self.config.to_dict())
+
+            MlflowTracker().log_params(self.config.to_dict())
 
             self.add_reporters().set_metadata(kwargs["metadata"]).add_handler(
-                type_of_process=type_of_process
+                type_of_process=kwargs["type_of_process"]
             )
             self.handler.handle()
         except Exception:
             logger.error(
                 f"Generation of the table - \"{kwargs['table_name']}\" failed on running stage.\n"
                 f"The traceback of the error - {traceback.format_exc()}"
             )
```

### Comparing `syngen-0.8.5/src/syngen/ml/utils/__init__.py` & `syngen-0.9.0/src/syngen/ml/utils/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -19,9 +19,10 @@
     timestamp_to_datetime,
     define_existent_columns,
     set_log_path,
     clean_up_metadata,
     fetch_log_message,
     file_sink,
     ProgressBarHandler,
-    check_if_logs_available
+    check_if_logs_available,
+    get_initial_table_name
 )
```

### Comparing `syngen-0.8.5/src/syngen/ml/utils/utils.py` & `syngen-0.9.0/src/syngen/ml/utils/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -407,7 +407,14 @@
     Check if the logs are available and
     write a message to the log file if not
     """
     path_to_logs = os.getenv("SUCCESS_LOG_FILE")
     if not os.path.exists(path_to_logs):
         with open(path_to_logs, "a") as file:
             file.write("No logs available\n")
+
+
+def get_initial_table_name(table_name) -> str:
+    """"
+    Get the initial table name without the suffix "_pk" or "_fk"
+    """
+    return re.sub(r"_pk$|_fk$", "", table_name)
```

### Comparing `syngen-0.8.5/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.9.0/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/vae/models/dataset.py` & `syngen-0.9.0/src/syngen/ml/vae/models/dataset.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/vae/models/features.py` & `syngen-0.9.0/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/vae/models/model.py` & `syngen-0.9.0/src/syngen/ml/vae/models/model.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.9.0/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import warnings
 import pickle
 import tensorflow as tf
 from tensorflow.python.data.experimental import AutoShardPolicy
 import matplotlib.pyplot as plt
 import time
 import tqdm
+import psutil
 import pandas as pd
 import numpy as np
 from loguru import logger
 
 from syngen.ml.vae.models.model import CVAE
 from syngen.ml.vae.models import Dataset
 from syngen.ml.mlflow_tracker import MlflowTracker
@@ -251,14 +252,20 @@
             tags={"table_name": self.table_name, "process": "train"},
         )
         config = fetch_training_config(self.paths["train_config_pickle_path"])
         MlflowTracker().log_params(config.to_dict())
 
         self._train(train_dataset, epochs)
 
+        MlflowTracker().end_run()
+
+        MlflowTracker().start_run(
+            run_name=f"{self.table_name}-POSTPROCESS",
+            tags={"table_name": self.table_name, "process": "postprocess"},
+        )
         self.model.model = self.vae
         self.fit_sampler(df)
 
     def _train(self, dataset, epochs: int):
         step = self._train_step
 
         self.feature_losses = defaultdict(list)
```

### Comparing `syngen-0.8.5/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.9.0/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/ml/worker/worker.py` & `syngen-0.9.0/src/syngen/ml/worker/worker.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from typing import Dict, List, Optional, Tuple, Any
+from typing import Dict, List, Optional, Any
 from attrs import define, field
 from copy import deepcopy
 from loguru import logger
 from slugify import slugify
 import os
+from itertools import product
 
 from syngen.ml.data_loaders import MetadataLoader
 from syngen.ml.strategies import TrainStrategy, InferStrategy
 from syngen.ml.reporters import Report
 from syngen.ml.config import Validator
 from syngen.ml.mlflow_tracker import MlflowTrackerFactory
 from syngen.ml.context.context import global_context
@@ -26,21 +27,25 @@
     settings: Dict = field(kw_only=True)
     log_level: str = field(kw_only=True)
     type_of_process: str = field(kw_only=True)
     train_strategy = TrainStrategy()
     infer_strategy = InferStrategy()
     metadata: Optional[Dict] = None
     divided: List = field(default=list())
+    initial_table_names: List = field(default=list())
     merged_metadata: Dict = field(default=dict())
+    train_stages: List = ["PREPROCESS", "TRAIN", "POSTPROCESS"]
+    infer_stages: List = ["INFER", "REPORT"]
 
     def __attrs_post_init__(self):
         os.makedirs("model_artifacts/metadata", exist_ok=True)
         self.metadata = self.__fetch_metadata()
         self._update_metadata()
         self.__validate_metadata()
+        self.initial_table_names = list(self.merged_metadata.keys())
         self._set_mlflow()
 
     def __validate_metadata(self):
         """
         Validate the metadata, set the merged metadata
         """
         validator = Validator(
@@ -190,168 +195,247 @@
         config_of_tables = {
             **self.metadata,
             **{k: v for k, v in config_of_tables.items() if k not in self.metadata},
         }
         chain_of_tables = [i for i in chain_of_tables for j in self.metadata if j in i]
         return chain_of_tables, config_of_tables
 
+    @staticmethod
+    def _split_keys(keys):
+        """
+        Split the keys into primary keys and unique keys, and foreign keys
+        """
+        pk_uq_keys = {k: v for k, v in keys.items() if v["type"] in ["PK", "UQ"]}
+        fk_keys = {k: v for k, v in keys.items() if v["type"] == "FK"}
+        return pk_uq_keys, fk_keys
+
+    @staticmethod
+    def _get_meta_copy(original_meta, new_keys):
+        """
+        Get updated metadata copy
+        """
+        meta_copy = original_meta.copy()
+        meta_copy["keys"] = new_keys
+        return meta_copy
+
     def _split_pk_fk_metadata(self, config, tables):
+        """
+        Split the metadata of tables into primary key and foreign key metadata
+        """
+
         for table in tables:
-            types_of_keys = [value["type"] for key, value in config[table].get("keys", {}).items()]
+            keys = config[table].get("keys", {})
+            types_of_keys = {k_type["type"] for k_type in keys.values()}
+
             if "PK" in types_of_keys and "FK" in types_of_keys:
-                self.divided += [table + "_pk", table + "_fk"]
-                pk_uq_part = {
-                    key: value
-                    for key, value in config[table]["keys"].items()
-                    if value["type"] in ["PK", "UQ"]
-                }
-                fk_part = {
-                    key: value
-                    for key, value in config[table]["keys"].items()
-                    if value["type"] == "FK"
-                }
+                self.divided.append(f"{table}_pk")
+                self.divided.append(f"{table}_fk")
 
-                # Do this to create a new object instead of a reference
-                as_pk_meta = {k: v for k, v in config[table].items()}
-                as_fk_meta = {k: v for k, v in config[table].items()}
+                pk_uq_keys, fk_keys = self._split_keys(keys)
 
-                as_pk_meta["keys"] = pk_uq_part
-                as_fk_meta["keys"] = fk_part
+                config[f"{table}_pk"] = self._get_meta_copy(config[table], pk_uq_keys)
+                config[f"{table}_fk"] = self._get_meta_copy(config[table], fk_keys)
 
-                config[table + "_pk"] = as_pk_meta
-                config[table + "_fk"] = as_fk_meta
                 config.pop(table)
+
         return config
 
+    @staticmethod
+    def _should_generate_report(config_of_tables: Dict, type_of_process: str):
+        """
+        Determine whether reports should be generated based
+        on the configurations of the tables
+        """
+        return any(
+            [
+                config.get(f"{type_of_process}_settings", {}).get("print_report", False)
+                for table, config in config_of_tables.items()
+            ]
+        )
+
+    def _collect_metrics_in_train(
+        self,
+        tables_for_training: List[str],
+        tables_for_inference: List[str],
+        generation_of_reports: bool
+    ):
+        """
+        Collect the integral metrics for the training process
+        """
+        MlflowTracker().start_run(
+            run_name="integral_metrics",
+            tags={"process": "bottleneck"}
+        )
+        self._collect_integral_metrics(tables=tables_for_training, type_of_process="train")
+        if generation_of_reports:
+            self._collect_integral_metrics(tables=tables_for_inference, type_of_process="infer")
+        MlflowTracker().end_run()
+
+    def _train_table(self, table, metadata, delta):
+        """"
+        Train process for a single table
+        """
+        config_of_table = metadata[table]
+        global_context(config_of_table.get("format", {}))
+        train_settings = config_of_table["train_settings"]
+        log_message = f"Training process of the table - '{table}' has started"
+        logger.info(log_message)
+        ProgressBarHandler().set_progress(delta=delta, message=log_message)
+
+        self.train_strategy.run(
+            metadata=metadata,
+            source=train_settings["source"],
+            epochs=train_settings["epochs"],
+            drop_null=train_settings["drop_null"],
+            row_limit=train_settings["row_limit"],
+            table_name=table,
+            metadata_path=self.metadata_path,
+            print_report=train_settings["print_report"],
+            batch_size=train_settings["batch_size"]
+        )
+        self._write_success_message(slugify(table))
+        self._save_metadata_file()
+        ProgressBarHandler().set_progress(
+            delta=delta,
+            message=f"Training of the table - {table} was completed"
+        )
+
     def __train_tables(
         self,
-        metadata_for_training: Tuple[List, Dict],
-        metadata_for_inference: Tuple[List, Dict],
+        tables_for_training: List,
+        tables_for_inference: List,
+        metadata_for_training: Dict,
+        metadata_for_inference: Dict,
+        generation_of_reports: bool
     ):
         """
         Run training process for the list of tables
         :param metadata_for_training:
         the tuple included the list of tables and metadata for training process
         :param metadata_for_inference:
         the tuple included the list of tables and metadata for inference process
         """
-        (
-            chain_for_tables_for_training,
-            config_of_metadata_for_training,
-        ) = metadata_for_training
-        (
-            chain_for_tables_for_inference,
-            config_of_metadata_for_inference,
-        ) = metadata_for_inference
+        delta = 0.49 / len(tables_for_training)
 
-        delta = 0.49 / len(chain_for_tables_for_training)
+        for table in tables_for_training:
+            self._train_table(table, metadata_for_training, delta)
 
-        for table in chain_for_tables_for_training:
-            config_of_table = config_of_metadata_for_training[table]
-            global_context(config_of_table.get("format", {}))
-            train_settings = config_of_table["train_settings"]
-            log_message = f"Training process of the table - '{table}' has started"
-            logger.info(log_message)
-            ProgressBarHandler().set_progress(delta=delta, message=log_message)
-
-            self.train_strategy.run(
-                metadata=config_of_metadata_for_training,
-                source=train_settings["source"],
-                epochs=train_settings["epochs"],
-                drop_null=train_settings["drop_null"],
-                row_limit=train_settings["row_limit"],
-                table_name=table,
-                metadata_path=self.metadata_path,
-                print_report=train_settings["print_report"],
-                batch_size=train_settings["batch_size"]
-            )
-            self._write_success_message(slugify(table))
-            self._save_metadata_file()
-            ProgressBarHandler().set_progress(
-                delta=delta,
-                message=f"Training of the table - {table} was completed"
+        if generation_of_reports:
+            self.__infer_tables(
+                tables_for_inference,
+                metadata_for_inference,
+                delta,
+                type_of_process="train"
             )
-        generation_of_reports = any(
-            [
-                config.get("train_settings", {}).get("print_report", False)
-                for table, config in config_of_metadata_for_training.items()
-            ]
+
+        self._generate_reports()
+
+    def _get_surrogate_tables_mapping(self):
+        """
+        Get the mapping of surrogate tables, which end with "_pk" and "_fk",
+        to the initial tables from which they were derived
+        """
+        return {
+            table: [t for t in self.divided if t.startswith(table)]
+            for table in self.initial_table_names
+            if any(t.startswith(table) for t in self.divided)
+        }
+
+    def _find_parent_table(self, table):
+        """
+        Find the initial table
+        from which the surrogate table was derived
+        """
+        return next(
+            (
+                parent
+                for parent, children in self._get_surrogate_tables_mapping().items()
+                if table in children
+            ), None
         )
-        if generation_of_reports:
-            for table in chain_for_tables_for_inference:
-                config_of_table = config_of_metadata_for_inference[table]
-                global_context(config_of_table.get("format", {}))
-                train_settings = config_of_table["train_settings"]
-                print_report = train_settings.get("print_report")
-                both_keys = table in self.divided
-
-                logger.info(f"Infer process of the table - {table} has started")
-
-                self.infer_strategy.run(
-                    destination=None,
-                    metadata=config_of_metadata_for_inference,
-                    size=None,
-                    table_name=table,
-                    metadata_path=self.metadata_path,
-                    run_parallel=False,
-                    batch_size=1000,
-                    random_seed=1,
-                    print_report=print_report,
-                    get_infer_metrics=False,
-                    log_level=self.log_level,
-                    both_keys=both_keys,
-                    type_of_process=self.type_of_process,
-                )
 
-    def __infer_tables(self, tables: List, config_of_tables: Dict):
+    def _infer_table(self, table, metadata, type_of_process, delta, is_nested=False):
+        """
+        Infer process for a single table
+        """
+        config_of_table = metadata[table]
+        global_context(config_of_table.get("format", {}))
+        log_message = f"Infer process of the table - '{table}' has started"
+        logger.info(log_message)
+        ProgressBarHandler().set_progress(delta=delta, message=log_message)
+        both_keys = table in self.divided
+        settings = config_of_table[f"{type_of_process}_settings"]
+
+        MlflowTracker().start_run(
+                run_name=f"{table}-INFER",
+                tags={"table_name": table, "process": type_of_process},
+                nested=is_nested,
+        )
+        self.infer_strategy.run(
+            destination=settings.get("destination") if type_of_process == "infer" else None,
+            metadata=metadata,
+            size=settings.get("size") if type_of_process == "infer" else None,
+            table_name=table,
+            metadata_path=self.metadata_path,
+            run_parallel=settings.get("run_parallel") if type_of_process == "infer" else False,
+            batch_size=settings.get("batch_size") if type_of_process == "infer" else 1000,
+            random_seed=settings.get("random_seed") if type_of_process == "infer" else 1,
+            print_report=settings["print_report"],
+            get_infer_metrics=settings.get("get_infer_metrics") if type_of_process == "infer" else False,
+            log_level=self.log_level,
+            both_keys=both_keys,
+            type_of_process=self.type_of_process,
+        )
+        ProgressBarHandler().set_progress(
+            delta=delta,
+            message=f"Infer process of the table - {table} was completed"
+        )
+        MlflowTracker().end_run()
+
+    def __infer_tables(self, tables: List, config_of_tables: Dict, delta: float, type_of_process: str):
         """
         Run infer process for the list of tables
         :param tables: the list of tables for infer process
         :param config_of_tables: configuration of tables declared in metadata file
         """
-        generation_of_reports = any(
-            [
-                config.get("infer_settings", {}).get("print_report", False)
-                for table, config in config_of_tables.items()
-            ]
-        )
-        delta = 0.25 / len(tables) if generation_of_reports else 0.5 / len(tables)
-        for table in tables:
-            config_of_table = config_of_tables[table]
-            global_context(config_of_table.get("format", {}))
-            log_message = f"Infer process of the table - '{table}' has started"
-            logger.info(log_message)
-            ProgressBarHandler().set_progress(delta=delta, message=log_message)
-            both_keys = table in self.divided
-            infer_settings = config_of_table["infer_settings"]
 
-            MlflowTracker().start_run(
-                run_name=f"{table}-INFER",
-                tags={"table_name": table, "process": "infer"},
-            )
-            self.infer_strategy.run(
-                destination=infer_settings.get("destination"),
+        non_surrogate_tables = [table for table in tables if table not in self.divided]
+        for table in non_surrogate_tables:
+            self._infer_table(
+                table=table,
                 metadata=config_of_tables,
-                size=infer_settings["size"],
-                table_name=table,
-                metadata_path=self.metadata_path,
-                run_parallel=infer_settings["run_parallel"],
-                batch_size=infer_settings["batch_size"],
-                random_seed=infer_settings["random_seed"],
-                print_report=infer_settings["print_report"],
-                get_infer_metrics=infer_settings["get_infer_metrics"],
-                log_level=self.log_level,
-                both_keys=both_keys,
-                type_of_process=self.type_of_process,
+                type_of_process=type_of_process,
+                delta=delta
             )
-            MlflowTracker().end_run()
-            ProgressBarHandler().set_progress(
-                delta=delta,
-                message=f"Infer process of the table - {table} was completed"
+
+        tables_mapping = self._get_surrogate_tables_mapping()
+        for table_root in tables_mapping.keys():
+            MlflowTracker().start_run(
+                run_name=f"{table_root}-INFER",
+                tags={"table_name": table_root, "process": type_of_process}
             )
+            for table in tables_mapping[table_root]:
+                self._infer_table(
+                    table=table,
+                    metadata=config_of_tables,
+                    type_of_process=type_of_process,
+                    delta=delta,
+                    is_nested=True
+                )
+            MlflowTracker().end_run()
+
+        self._generate_reports()
+
+    def _collect_integral_metrics(self, tables, type_of_process):
+        """
+        Collect the integral metrics depending on the type of process
+        """
+        stages = self.train_stages if type_of_process == "train" else self.infer_stages
+        for table, stage in product(tables, stages):
+            MlflowTracker().collect_metrics(table, stage)
 
     def _generate_reports(self):
         """
         Generate reports
         """
         Report().generate_report(type_of_process=self.type_of_process.upper())
         Report().clear_report()
@@ -372,21 +456,57 @@
                 f"model_artifacts/metadata/{metadata_file_name}", self.metadata
             )
 
     def launch_train(self):
         """
         Launch training process either for a single table or for several tables
         """
-        metadata_for_training = self._prepare_metadata_for_process()
+        metadata_for_training = self._prepare_metadata_for_process(type_of_process="train")
         metadata_for_inference = self._prepare_metadata_for_process(type_of_process="infer")
-        self.__train_tables(metadata_for_training, metadata_for_inference)
-        self._generate_reports()
+
+        (
+            tables_for_training,
+            metadata_for_training,
+        ) = metadata_for_training
+        (
+            tables_for_inference,
+            metadata_for_inference,
+        ) = metadata_for_inference
+
+        generation_of_reports = self._should_generate_report(metadata_for_training, "train")
+
+        self.__train_tables(
+            tables_for_training,
+            tables_for_inference,
+            metadata_for_training,
+            metadata_for_inference,
+            generation_of_reports
+        )
+
+        self._collect_metrics_in_train(
+            tables_for_training,
+            tables_for_inference,
+            generation_of_reports
+        )
+
+    def _collect_metrics_in_infer(self, tables):
+        """
+        Collect the integral metrics for the inference process
+        """
+        MlflowTracker().start_run(
+            run_name="integral_metrics",
+            tags={"process": "bottleneck"}
+        )
+        self._collect_integral_metrics(tables, type_of_process="infer")
+        MlflowTracker().end_run()
 
     def launch_infer(self):
         """
         Launch infer process either for a single table or for several tables
         """
-        chain_of_tables, config_of_tables = self._prepare_metadata_for_process(
-            type_of_process="infer"
-        )
-        self.__infer_tables(chain_of_tables, config_of_tables)
-        self._generate_reports()
+        tables, config_of_tables = self._prepare_metadata_for_process(type_of_process="infer")
+
+        generation_of_reports = self._should_generate_report(config_of_tables, "infer")
+        delta = 0.25 / len(tables) if generation_of_reports else 0.5 / len(tables)
+
+        self.__infer_tables(tables, config_of_tables, delta, type_of_process="infer")
+        self._collect_metrics_in_infer(tables)
```

### Comparing `syngen-0.8.5/src/syngen/streamlit_app/css/style.css` & `syngen-0.9.0/src/syngen/streamlit_app/css/style.css`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/streamlit_app/handlers/handlers.py` & `syngen-0.9.0/src/syngen/streamlit_app/handlers/handlers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/streamlit_app/img/favicon.svg` & `syngen-0.9.0/src/syngen/streamlit_app/img/favicon.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/streamlit_app/img/logo.svg` & `syngen-0.9.0/src/syngen/streamlit_app/img/logo.svg`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/streamlit_app/run.py` & `syngen-0.9.0/src/syngen/streamlit_app/run.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/streamlit_app/start.py` & `syngen-0.9.0/src/syngen/streamlit_app/start.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/streamlit_app/utils/utils.py` & `syngen-0.9.0/src/syngen/streamlit_app/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen/train.py` & `syngen-0.9.0/src/syngen/train.py`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen.egg-info/PKG-INFO` & `syngen-0.9.0/src/syngen.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.8.5
+Version: 0.9.0
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
@@ -33,14 +33,15 @@
 Requires-Dist: mlflow==2.13.*
 Requires-Dist: numpy==1.23.*
 Requires-Dist: openpyxl
 Requires-Dist: pandas==1.3.*
 Requires-Dist: pandavro==1.7.2
 Requires-Dist: pathos==0.2.*
 Requires-Dist: pillow==10.3.*
+Requires-Dist: psutil
 Requires-Dist: py-ulid
 Requires-Dist: pytest
 Requires-Dist: pytest-reportportal
 Requires-Dist: python-slugify[unidecode]>=7.0.0
 Requires-Dist: PyYAML==6.*
 Requires-Dist: reportportal-client
 Requires-Dist: scikit_learn==1.1.*
@@ -459,40 +460,132 @@
 
 #### MLflow monitoring
 
 Set the `MLFLOW_TRACKING_URI` environment variable to the desired MLflow tracking server, for instance:
 http://localhost:5000/. You can also set the `MLFLOW_ARTIFACTS_DESTINATION` environment variable to your preferred path 
 (including the cloud path), where the artifacts should be stored. Additionally, set the `MLFLOW_EXPERIMENT_NAME` 
 environment variable to the name you prefer for the experiment. 
+To get the system metrics, please set the `MLFLOW_ENABLE_SYSTEM_METRICS_LOGGING` environment variable to `true`.
+By default, the metrics are logged every 10 seconds, but the interval may be changed by setting the environment variable 
+`MLFLOW_SYSTEM_METRICS_SAMPLING_INTERVAL` (for more detailed description look [here](https://mlflow.org/docs/latest/system-metrics/index.html))
+
 When using Docker, ensure the environmental variables are set before running the container.
 
 The provided environmental variables allow to track the training process, and the inference process, and store 
 the artifacts in the desired location.
 You can access the MLflow UI by navigating to the provided URL in your browser. If you store artifacts in remote storage,
 ensure that all necessary credentials are provided before using Mlflow.
 
 ```bash
 docker pull tdspora/syngen:latest
 docker run --rm -it \
   --user $(id -u):$(id -g) \
   -e MLFLOW_TRACKING_URI='http://localhost:5000' \
   -e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION \
   -e MLFLOW_EXPERIMENT_NAME=test_name \
+  -e MLFLOW_ENABLE_SYSTEM_METRICS_LOGGING=true \
+  -e MLFLOW_SYSTEM_METRICS_SAMPLING_INTERVAL 10 \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 
 docker run --rm -it \
   --user $(id -u):$(id -g) \
   -e MLFLOW_TRACKING_URI='http://localhost:5000' \
   -e MLFLOW_ARTIFACTS_DESTINATION=MLFLOW_ARTIFACTS_DESTINATION \
   -e MLFLOW_EXPERIMENT_NAME=test_name \
+  -e MLFLOW_ENABLE_SYSTEM_METRICS_LOGGING=true \
+  -e MLFLOW_SYSTEM_METRICS_SAMPLING_INTERVAL 10 \
   -v PATH_TO_LOCAL_FOLDER:/src/model_artifacts tdspora/syngen \
   --metadata_path=./model_artifacts/PATH_TO_METADATA_YAML
 ```
 
+## Syngen Installation Guide for MacOS ARM (M1/M2) with Python 3.10
+
+### Prerequisites
+
+Before you begin, make sure you have the following installed:
+
+- Python 3.10
+- Homebrew (optional but recommended for managing dependencies)
+
+### Installation Steps
+
+1. **Upgrade pip**: Ensure you have the latest version of `pip`.
+
+    ```sh
+    pip install --upgrade pip
+    ```
+
+2. **Install Setuptools, Wheel, and Cython**: These packages are necessary for building and installing other dependencies.
+
+    ```sh
+    pip install setuptools wheel 'Cython<3'
+    ```
+
+3. **Install Fastavro**: Install a specific version of `fastavro` to avoid build issues.
+
+    ```sh
+    pip install --no-build-isolation fastavro==1.5.1
+    ```
+
+4. **Install Syngen**: Now, you can install the Syngen package.
+
+    ```sh
+    pip install syngen
+    ```
+
+5. **Install TensorFlow Metal**: This package leverages the GPU capabilities of M1/M2 chips for TensorFlow.
+
+    ```sh
+    pip install tensorflow-metal
+    ```
+
+#### From source (development)
+
+Download repository from GitHub by cloning or zip file.
+Then install it in editable mode.
+
+```sh
+    pip install -e .
+```
+
+### Additional Information
+
+- **Homebrew**: If you do not have Homebrew installed, you can install it by running:
+
+    ```sh
+    /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"
+    ```
+
+- **Python 3.10**: Ensure you have Python 3.10 installed. You can use pyenv to manage different Python versions:
+
+    ```sh
+    brew install pyenv
+    pyenv install 3.10.0
+    pyenv global 3.10.0
+    ```
+
+### Verifying Installation
+
+To verify the installation, run the following command to check if Syngen is installed correctly:
+
+```sh
+python -c "import syngen; print(syngen.__version__)"
+```
+
+If the command prints the version of Syngen without errors, the installation was successful.
+
+### Troubleshooting
+
+If you encounter any issues during installation, consider the following steps:
+
+- Ensure all dependencies are up to date.
+- Check for any compatibility issues with other installed packages.
+- Consult the Syngen [documentation](https://github.com/tdspora/syngen) or raise an issue on GitHub.
+
 ## Contribution
 
 We welcome contributions from the community to help us improve and maintain our public GitHub repository. We appreciate any feedback, bug reports, or feature requests, and we encourage developers to submit fixes or new features using issues.
 
 If you have found a bug or have a feature request, please submit an issue to our GitHub repository. Please provide as much detail as possible, including steps to reproduce the issue or a clear description of the feature request. Our team will review the issue and work with you to address any problems or discuss any potential new features.
 
 If you would like to contribute a fix or a new feature, please submit a pull request to our GitHub repository. Please make sure your code follows our coding standards and best practices. Our team will review your pull request and work with you to ensure that it meets our standards and is ready for inclusion in our codebase.
```

### Comparing `syngen-0.8.5/src/syngen.egg-info/SOURCES.txt` & `syngen-0.9.0/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `syngen-0.8.5/src/syngen.egg-info/requires.txt` & `syngen-0.9.0/src/syngen.egg-info/requires.txt`

 * *Files 24% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 mlflow==2.13.*
 numpy==1.23.*
 openpyxl
 pandas==1.3.*
 pandavro==1.7.2
 pathos==0.2.*
 pillow==10.3.*
+psutil
 py-ulid
 pytest
 pytest-reportportal
 python-slugify[unidecode]>=7.0.0
 PyYAML==6.*
 reportportal-client
 scikit_learn==1.1.*
```

