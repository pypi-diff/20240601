# Comparing `tmp/sageworks-0.6.8.tar.gz` & `tmp/sageworks-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sageworks-0.6.8.tar", last modified: Thu May 30 17:23:31 2024, max compression
+gzip compressed data, was "sageworks-0.6.9.tar", last modified: Fri May 31 23:16:54 2024, max compression
```

## Comparing `sageworks-0.6.8.tar` & `sageworks-0.6.9.tar`

### file list

```diff
@@ -1,569 +1,570 @@
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.104442 sageworks-0.6.8/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.999856 sageworks-0.6.8/.github/
--rw-r--r--   0 briford    (501) staff       (20)     1338 2024-03-28 17:23:43.000000 sageworks-0.6.8/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 briford    (501) staff       (20)      499 2023-12-24 17:18:24.000000 sageworks-0.6.8/.github/dependabot.yml
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.000306 sageworks-0.6.8/.github/workflows/
--rw-r--r--   0 briford    (501) staff       (20)      598 2024-01-10 18:45:51.000000 sageworks-0.6.8/.github/workflows/deploy-docs.yml
--rw-r--r--   0 briford    (501) staff       (20)      556 2024-01-23 15:36:53.000000 sageworks-0.6.8/.github/workflows/python-lint.yml
--rw-r--r--   0 briford    (501) staff       (20)     2037 2024-05-15 21:28:12.000000 sageworks-0.6.8/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)      791 2024-04-16 15:58:18.000000 sageworks-0.6.8/CONTRIBUTING.md
--rw-r--r--   0 briford    (501) staff       (20)      102 2024-03-28 17:23:43.000000 sageworks-0.6.8/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)     1080 2024-03-28 17:23:43.000000 sageworks-0.6.8/LICENSE
--rw-r--r--   0 briford    (501) staff       (20)     1426 2023-12-24 17:18:24.000000 sageworks-0.6.8/Makefile
--rw-r--r--   0 briford    (501) staff       (20)     4961 2024-05-30 17:23:31.104374 sageworks-0.6.8/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)     3510 2024-05-09 14:32:45.000000 sageworks-0.6.8/README.md
--rw-r--r--   0 briford    (501) staff       (20)      463 2023-12-24 17:18:24.000000 sageworks-0.6.8/SECURITY.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.988849 sageworks-0.6.8/applications/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.002147 sageworks-0.6.8/applications/aws_dashboard/
--rw-r--r--   0 briford    (501) staff       (20)     1071 2024-05-24 14:50:34.000000 sageworks-0.6.8/applications/aws_dashboard/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)      331 2024-03-28 17:23:43.000000 sageworks-0.6.8/applications/aws_dashboard/Dockerfile_plugins
--rw-r--r--   0 briford    (501) staff       (20)      841 2024-01-10 18:45:51.000000 sageworks-0.6.8/applications/aws_dashboard/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1526 2024-04-09 14:37:33.000000 sageworks-0.6.8/applications/aws_dashboard/app.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.003543 sageworks-0.6.8/applications/aws_dashboard/assets/
--rw-r--r--   0 briford    (501) staff       (20)   232839 2024-04-06 16:51:44.000000 sageworks-0.6.8/applications/aws_dashboard/assets/bootstrap_darkly.min.css
--rw-r--r--   0 briford    (501) staff       (20)    14995 2024-04-06 16:51:44.000000 sageworks-0.6.8/applications/aws_dashboard/assets/default.css
--rw-r--r--   0 briford    (501) staff       (20)    10375 2024-04-16 15:58:18.000000 sageworks-0.6.8/applications/aws_dashboard/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)      732 2023-12-24 17:18:24.000000 sageworks-0.6.8/applications/aws_dashboard/assets/trash.png
--rwxr-xr-x   0 briford    (501) staff       (20)      637 2024-04-26 21:03:22.000000 sageworks-0.6.8/applications/aws_dashboard/dashboard
--rw-r--r--   0 briford    (501) staff       (20)      205 2023-12-24 17:18:24.000000 sageworks-0.6.8/applications/aws_dashboard/nginx.conf
--rw-r--r--   0 briford    (501) staff       (20)      684 2024-03-28 17:23:43.000000 sageworks-0.6.8/applications/aws_dashboard/open_source_config.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.988772 sageworks-0.6.8/applications/aws_dashboard/pages/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.004298 sageworks-0.6.8/applications/aws_dashboard/pages/data_sources/
--rw-r--r--   0 briford    (501) staff       (20)    11700 2024-04-16 15:58:18.000000 sageworks-0.6.8/applications/aws_dashboard/pages/data_sources/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2756 2024-03-28 17:23:43.000000 sageworks-0.6.8/applications/aws_dashboard/pages/data_sources/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2555 2024-03-28 17:23:43.000000 sageworks-0.6.8/applications/aws_dashboard/pages/data_sources/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.005069 sageworks-0.6.8/applications/aws_dashboard/pages/endpoints/
--rw-r--r--   0 briford    (501) staff       (20)     4439 2024-05-28 15:10:23.000000 sageworks-0.6.8/applications/aws_dashboard/pages/endpoints/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2677 2024-04-16 15:58:18.000000 sageworks-0.6.8/applications/aws_dashboard/pages/endpoints/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2550 2024-05-28 15:10:23.000000 sageworks-0.6.8/applications/aws_dashboard/pages/endpoints/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.005777 sageworks-0.6.8/applications/aws_dashboard/pages/feature_sets/
--rw-r--r--   0 briford    (501) staff       (20)    11614 2024-04-16 15:58:18.000000 sageworks-0.6.8/applications/aws_dashboard/pages/feature_sets/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2438 2024-03-28 17:23:43.000000 sageworks-0.6.8/applications/aws_dashboard/pages/feature_sets/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.8/applications/aws_dashboard/pages/feature_sets/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.005940 sageworks-0.6.8/applications/aws_dashboard/pages/license/
--rw-r--r--   0 briford    (501) staff       (20)     1531 2024-05-19 19:25:10.000000 sageworks-0.6.8/applications/aws_dashboard/pages/license/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.006700 sageworks-0.6.8/applications/aws_dashboard/pages/main/
--rw-r--r--   0 briford    (501) staff       (20)     4899 2024-04-06 16:51:44.000000 sageworks-0.6.8/applications/aws_dashboard/pages/main/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     3307 2024-05-19 19:21:21.000000 sageworks-0.6.8/applications/aws_dashboard/pages/main/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1844 2024-03-28 17:23:43.000000 sageworks-0.6.8/applications/aws_dashboard/pages/main/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.007393 sageworks-0.6.8/applications/aws_dashboard/pages/models/
--rw-r--r--   0 briford    (501) staff       (20)     4195 2024-05-28 15:10:23.000000 sageworks-0.6.8/applications/aws_dashboard/pages/models/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2234 2024-04-27 20:59:25.000000 sageworks-0.6.8/applications/aws_dashboard/pages/models/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     2227 2024-05-28 15:10:23.000000 sageworks-0.6.8/applications/aws_dashboard/pages/models/page.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.008058 sageworks-0.6.8/applications/aws_dashboard/pages/pipelines/
--rw-r--r--   0 briford    (501) staff       (20)     1791 2024-04-26 21:07:33.000000 sageworks-0.6.8/applications/aws_dashboard/pages/pipelines/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2664 2024-04-26 20:07:24.000000 sageworks-0.6.8/applications/aws_dashboard/pages/pipelines/layout.py
--rw-r--r--   0 briford    (501) staff       (20)     1927 2024-04-26 21:04:41.000000 sageworks-0.6.8/applications/aws_dashboard/pages/pipelines/page.py
--rw-r--r--   0 briford    (501) staff       (20)      407 2024-05-19 21:33:27.000000 sageworks-0.6.8/applications/aws_dashboard/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)      457 2023-12-24 17:18:24.000000 sageworks-0.6.8/applications/aws_dashboard/supervisord.conf
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.988901 sageworks-0.6.8/applications/experiments/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.009674 sageworks-0.6.8/applications/experiments/compound_explorer/
--rw-r--r--   0 briford    (501) staff       (20)      181 2023-12-24 17:18:24.000000 sageworks-0.6.8/applications/experiments/compound_explorer/Dockerfile
--rw-r--r--   0 briford    (501) staff       (20)      360 2023-12-24 17:18:24.000000 sageworks-0.6.8/applications/experiments/compound_explorer/README.md
--rw-r--r--   0 briford    (501) staff       (20)     3082 2024-04-06 16:51:44.000000 sageworks-0.6.8/applications/experiments/compound_explorer/app.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.010176 sageworks-0.6.8/applications/experiments/compound_explorer/assets/
--rw-r--r--   0 briford    (501) staff       (20)    12861 2023-12-24 17:18:24.000000 sageworks-0.6.8/applications/experiments/compound_explorer/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.6.8/applications/experiments/compound_explorer/assets/favicon.ico
--rw-r--r--   0 briford    (501) staff       (20)     7678 2024-04-16 15:58:18.000000 sageworks-0.6.8/applications/experiments/compound_explorer/callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     4860 2024-03-28 17:23:43.000000 sageworks-0.6.8/applications/experiments/compound_explorer/layout.py
--rw-r--r--   0 briford    (501) staff       (20)       94 2023-12-24 17:18:24.000000 sageworks-0.6.8/applications/experiments/compound_explorer/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.010690 sageworks-0.6.8/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     3582 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/aws_account_check.py
--rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/aws_identity_check.py
--rw-r--r--   0 briford    (501) staff       (20)     2629 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/build_ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.010841 sageworks-0.6.8/aws_setup/event_bridge/
--rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/event_bridge/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.011595 sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/
--rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     1007 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/cdk.json
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.011838 sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/lambda/
--rw-r--r--   0 briford    (501) staff       (20)     1812 2024-01-10 18:45:51.000000 sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py
--rw-r--r--   0 briford    (501) staff       (20)     2599 2024-03-27 20:43:31.000000 sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.013062 sageworks-0.6.8/aws_setup/sageworks_core/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_core/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1028 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_core/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_core/app.py
--rw-r--r--   0 briford    (501) staff       (20)     1998 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_core/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_core/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       53 2024-01-10 18:45:51.000000 sageworks-0.6.8/aws_setup/sageworks_core/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.013432 sageworks-0.6.8/aws_setup/sageworks_core/sageworks_core/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/aws_setup/sageworks_core/sageworks_core/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    23575 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_core/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.013791 sageworks-0.6.8/aws_setup/sageworks_core/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_core/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.014019 sageworks-0.6.8/aws_setup/sageworks_core/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_core/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      720 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.015719 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/
--rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1907 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/requirements-dev.txt
--rw-r--r--   0 briford    (501) staff       (20)       47 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.016042 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7022 2024-04-24 21:53:47.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py
--rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/source.bat
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.016359 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/tests/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/tests/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.016562 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/tests/unit/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/tests/unit/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)      565 2023-12-24 17:18:24.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.017272 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/
--rw-r--r--   0 briford    (501) staff       (20)      119 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/.gitignore
--rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/README.md
--rw-r--r--   0 briford    (501) staff       (20)     1928 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/app.py
--rw-r--r--   0 briford    (501) staff       (20)     2567 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/cdk.json
--rw-r--r--   0 briford    (501) staff       (20)       47 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.017529 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-03-28 17:23:43.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     6849 2024-05-24 14:56:58.000000 sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.018776 sageworks-0.6.8/data/
--rw-r--r--   0 briford    (501) staff       (20)   191978 2023-12-24 17:18:24.000000 sageworks-0.6.8/data/abalone.csv
--rw-r--r--   0 briford    (501) staff       (20)     1515 2023-12-24 17:18:24.000000 sageworks-0.6.8/data/test_data.csv
--rw-r--r--   0 briford    (501) staff       (20)     2270 2023-12-24 17:18:24.000000 sageworks-0.6.8/data/test_data.json
--rw-r--r--   0 briford    (501) staff       (20)    12977 2024-01-10 18:45:51.000000 sageworks-0.6.8/data/wine_dataset.csv
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.019022 sageworks-0.6.8/docs/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.019512 sageworks-0.6.8/docs/admin/
--rw-r--r--   0 briford    (501) staff       (20)     2176 2024-04-16 15:58:18.000000 sageworks-0.6.8/docs/admin/docker_push.md
--rw-r--r--   0 briford    (501) staff       (20)     1594 2024-05-30 16:53:00.000000 sageworks-0.6.8/docs/admin/pypi_release.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.021416 sageworks-0.6.8/docs/api_classes/
--rw-r--r--   0 briford    (501) staff       (20)     3595 2024-01-23 15:36:53.000000 sageworks-0.6.8/docs/api_classes/data_source.md
--rw-r--r--   0 briford    (501) staff       (20)     5199 2024-05-28 20:18:51.000000 sageworks-0.6.8/docs/api_classes/endpoint.md
--rw-r--r--   0 briford    (501) staff       (20)     6299 2024-03-28 17:23:43.000000 sageworks-0.6.8/docs/api_classes/feature_set.md
--rw-r--r--   0 briford    (501) staff       (20)     5350 2024-04-06 16:51:44.000000 sageworks-0.6.8/docs/api_classes/meta.md
--rw-r--r--   0 briford    (501) staff       (20)     4356 2024-05-28 20:18:51.000000 sageworks-0.6.8/docs/api_classes/model.md
--rw-r--r--   0 briford    (501) staff       (20)     2218 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/api_classes/monitor.md
--rw-r--r--   0 briford    (501) staff       (20)     3549 2024-05-28 20:18:51.000000 sageworks-0.6.8/docs/api_classes/overview.md
--rw-r--r--   0 briford    (501) staff       (20)     4894 2024-04-19 15:50:50.000000 sageworks-0.6.8/docs/api_classes/pipelines.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.023124 sageworks-0.6.8/docs/aws_setup/
--rw-r--r--   0 briford    (501) staff       (20)     1121 2024-03-28 17:23:43.000000 sageworks-0.6.8/docs/aws_setup/aws_access_management.md
--rw-r--r--   0 briford    (501) staff       (20)     5610 2024-05-06 14:50:56.000000 sageworks-0.6.8/docs/aws_setup/aws_tips_and_tricks.md
--rw-r--r--   0 briford    (501) staff       (20)     4210 2024-05-09 14:32:45.000000 sageworks-0.6.8/docs/aws_setup/core_stack.md
--rw-r--r--   0 briford    (501) staff       (20)     2075 2024-03-28 17:23:43.000000 sageworks-0.6.8/docs/aws_setup/dashboard_stack.md
--rw-r--r--   0 briford    (501) staff       (20)     7313 2024-05-15 23:47:50.000000 sageworks-0.6.8/docs/aws_setup/domain_cert_setup.md
--rw-r--r--   0 briford    (501) staff       (20)     2540 2024-01-23 15:36:53.000000 sageworks-0.6.8/docs/aws_setup/full_pipeline.md
--rw-r--r--   0 briford    (501) staff       (20)     3438 2024-05-09 14:20:27.000000 sageworks-0.6.8/docs/aws_setup/sso_setup.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.023886 sageworks-0.6.8/docs/blogs_research/
--rw-r--r--   0 briford    (501) staff       (20)      912 2024-03-28 17:23:43.000000 sageworks-0.6.8/docs/blogs_research/eda.md
--rw-r--r--   0 briford    (501) staff       (20)     2017 2024-03-28 17:23:43.000000 sageworks-0.6.8/docs/blogs_research/htg.md
--rw-r--r--   0 briford    (501) staff       (20)      802 2024-05-21 22:30:34.000000 sageworks-0.6.8/docs/blogs_research/index.md
--rw-r--r--   0 briford    (501) staff       (20)     1245 2024-05-28 20:18:51.000000 sageworks-0.6.8/docs/blogs_research/residual_analysis.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.024101 sageworks-0.6.8/docs/concepts/
--rw-r--r--   0 briford    (501) staff       (20)      907 2024-05-28 20:18:51.000000 sageworks-0.6.8/docs/concepts/model_monitoring.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.024321 sageworks-0.6.8/docs/core_classes/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.025900 sageworks-0.6.8/docs/core_classes/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      464 2024-01-23 15:36:53.000000 sageworks-0.6.8/docs/core_classes/artifacts/artifact.md
--rw-r--r--   0 briford    (501) staff       (20)      290 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/artifacts/athena_source.md
--rw-r--r--   0 briford    (501) staff       (20)      479 2024-01-23 15:36:53.000000 sageworks-0.6.8/docs/core_classes/artifacts/data_source_abstract.md
--rw-r--r--   0 briford    (501) staff       (20)      292 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/artifacts/endpoint_core.md
--rw-r--r--   0 briford    (501) staff       (20)      294 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/artifacts/feature_set_core.md
--rw-r--r--   0 briford    (501) staff       (20)      281 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/artifacts/model_core.md
--rw-r--r--   0 briford    (501) staff       (20)      289 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/artifacts/monitor_core.md
--rw-r--r--   0 briford    (501) staff       (20)      861 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/artifacts/overview.md
--rw-r--r--   0 briford    (501) staff       (20)     2119 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/overview.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.027545 sageworks-0.6.8/docs/core_classes/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      352 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/transforms/data_loaders_heavy.md
--rw-r--r--   0 briford    (501) staff       (20)      396 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/transforms/data_loaders_light.md
--rw-r--r--   0 briford    (501) staff       (20)      349 2024-03-28 17:23:43.000000 sageworks-0.6.8/docs/core_classes/transforms/data_to_features.md
--rw-r--r--   0 briford    (501) staff       (20)      265 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/transforms/features_to_model.md
--rw-r--r--   0 briford    (501) staff       (20)      264 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/transforms/model_to_endpoint.md
--rw-r--r--   0 briford    (501) staff       (20)     1177 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/core_classes/transforms/overview.md
--rw-r--r--   0 briford    (501) staff       (20)      970 2024-01-23 15:36:53.000000 sageworks-0.6.8/docs/core_classes/transforms/pandas_transforms.md
--rw-r--r--   0 briford    (501) staff       (20)      521 2024-01-23 15:36:53.000000 sageworks-0.6.8/docs/core_classes/transforms/transform.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.028312 sageworks-0.6.8/docs/enterprise/
--rw-r--r--   0 briford    (501) staff       (20)     4075 2024-05-20 20:55:48.000000 sageworks-0.6.8/docs/enterprise/index.md
--rw-r--r--   0 briford    (501) staff       (20)      786 2024-04-28 17:52:09.000000 sageworks-0.6.8/docs/enterprise/project_branding.md
--rw-r--r--   0 briford    (501) staff       (20)      892 2024-04-28 18:00:11.000000 sageworks-0.6.8/docs/enterprise/themes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.028546 sageworks-0.6.8/docs/getting_started/
--rw-r--r--   0 briford    (501) staff       (20)     1975 2024-05-09 14:38:45.000000 sageworks-0.6.8/docs/getting_started/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.028772 sageworks-0.6.8/docs/glue/
--rw-r--r--   0 briford    (501) staff       (20)     4837 2024-03-28 17:23:43.000000 sageworks-0.6.8/docs/glue/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.033858 sageworks-0.6.8/docs/images/
--rw-r--r--   0 briford    (501) staff       (20)   605827 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/big_spider.png
--rw-r--r--   0 briford    (501) staff       (20)    32320 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/graph_representation.png
--rw-r--r--   0 briford    (501) staff       (20)    15549 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/powered_aws_dark_blue.png
--rw-r--r--   0 briford    (501) staff       (20)    10003 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/powered_aws_transparent.png
--rw-r--r--   0 briford    (501) staff       (20)     6435 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/powered_aws_white.png
--rw-r--r--   0 briford    (501) staff       (20)    21174 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/powered_aws_with_tm_grey.png
--rw-r--r--   0 briford    (501) staff       (20)    51137 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/sageworks.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)    30017 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/scp.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)   381209 2023-12-24 17:18:24.000000 sageworks-0.6.8/docs/images/small_spider.png
--rw-r--r--   0 briford    (501) staff       (20)     3443 2024-05-09 14:20:27.000000 sageworks-0.6.8/docs/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.035444 sageworks-0.6.8/docs/misc/
--rw-r--r--   0 briford    (501) staff       (20)     2791 2024-03-28 17:23:43.000000 sageworks-0.6.8/docs/misc/faq.md
--rw-r--r--   0 briford    (501) staff       (20)     5069 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/misc/general_info.md
--rw-r--r--   0 briford    (501) staff       (20)      667 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/misc/sageworks_classes_concepts.md
--rw-r--r--   0 briford    (501) staff       (20)     1873 2024-01-10 18:45:51.000000 sageworks-0.6.8/docs/misc/scp_consulting.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.035933 sageworks-0.6.8/docs/plugins/
--rw-r--r--   0 briford    (501) staff       (20)     3361 2024-04-16 15:58:18.000000 sageworks-0.6.8/docs/plugins/index.md
--rw-r--r--   0 briford    (501) staff       (20)      750 2024-04-06 16:51:44.000000 sageworks-0.6.8/docs/plugins/plugin_api_changes.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.036172 sageworks-0.6.8/docs/repl/
--rw-r--r--   0 briford    (501) staff       (20)     2080 2024-05-09 14:40:59.000000 sageworks-0.6.8/docs/repl/index.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.036428 sageworks-0.6.8/examples/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.036648 sageworks-0.6.8/examples/ag-grid/
--rw-r--r--   0 briford    (501) staff       (20)      496 2024-04-06 16:51:44.000000 sageworks-0.6.8/examples/ag-grid/hello_world.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.037759 sageworks-0.6.8/examples/datasource/
--rw-r--r--   0 briford    (501) staff       (20)      326 2024-01-10 18:45:51.000000 sageworks-0.6.8/examples/datasource/datasource_from_df.py
--rw-r--r--   0 briford    (501) staff       (20)      332 2024-01-10 18:45:51.000000 sageworks-0.6.8/examples/datasource/datasource_from_s3.py
--rw-r--r--   0 briford    (501) staff       (20)      536 2024-01-23 15:36:53.000000 sageworks-0.6.8/examples/datasource/datasource_query.py
--rw-r--r--   0 briford    (501) staff       (20)      680 2024-01-23 15:36:53.000000 sageworks-0.6.8/examples/datasource/datasource_stats.py
--rw-r--r--   0 briford    (501) staff       (20)      223 2024-01-10 18:45:51.000000 sageworks-0.6.8/examples/datasource/datasource_to_featureset.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.038282 sageworks-0.6.8/examples/endpoint/
--rw-r--r--   0 briford    (501) staff       (20)      199 2024-01-10 18:45:51.000000 sageworks-0.6.8/examples/endpoint/endpoint_details.py
--rw-r--r--   0 briford    (501) staff       (20)      834 2024-05-28 20:18:51.000000 sageworks-0.6.8/examples/endpoint/endpoint_inference.py
--rw-r--r--   0 briford    (501) staff       (20)      481 2024-01-10 18:45:51.000000 sageworks-0.6.8/examples/endpoint/endpoint_metrics.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.038786 sageworks-0.6.8/examples/featureset/
--rw-r--r--   0 briford    (501) staff       (20)      744 2024-01-10 18:45:51.000000 sageworks-0.6.8/examples/featureset/featureset_eda.py
--rw-r--r--   0 briford    (501) staff       (20)      560 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/featureset/featureset_query.py
--rw-r--r--   0 briford    (501) staff       (20)      421 2024-03-27 20:32:26.000000 sageworks-0.6.8/examples/featureset/featureset_to_model.py
--rw-r--r--   0 briford    (501) staff       (20)     1534 2024-05-28 20:18:51.000000 sageworks-0.6.8/examples/full_ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.039477 sageworks-0.6.8/examples/glue/
--rw-r--r--   0 briford    (501) staff       (20)      580 2024-01-23 15:36:53.000000 sageworks-0.6.8/examples/glue/glue_hello_world.py
--rw-r--r--   0 briford    (501) staff       (20)      942 2024-01-23 15:36:53.000000 sageworks-0.6.8/examples/glue/glue_hello_world_with_log.py
--rw-r--r--   0 briford    (501) staff       (20)      686 2024-01-23 15:36:53.000000 sageworks-0.6.8/examples/glue/glue_load_s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.040035 sageworks-0.6.8/examples/meta/
--rw-r--r--   0 briford    (501) staff       (20)      363 2024-04-06 16:51:44.000000 sageworks-0.6.8/examples/meta/meta_list_endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      328 2024-04-06 16:51:44.000000 sageworks-0.6.8/examples/meta/meta_list_models.py
--rw-r--r--   0 briford    (501) staff       (20)      659 2024-04-06 16:51:44.000000 sageworks-0.6.8/examples/meta/meta_model_metrics.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.040585 sageworks-0.6.8/examples/model/
--rw-r--r--   0 briford    (501) staff       (20)      564 2024-05-29 18:44:03.000000 sageworks-0.6.8/examples/model/model_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)      312 2024-03-27 20:32:26.000000 sageworks-0.6.8/examples/model/model_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)      705 2024-05-08 21:58:54.000000 sageworks-0.6.8/examples/model/onboard_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.040960 sageworks-0.6.8/examples/monitor/
--rw-r--r--   0 briford    (501) staff       (20)      400 2024-01-10 18:45:51.000000 sageworks-0.6.8/examples/monitor/monitor_setup.py
--rw-r--r--   0 briford    (501) staff       (20)      765 2024-01-10 18:45:51.000000 sageworks-0.6.8/examples/monitor/monitor_usage.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.042253 sageworks-0.6.8/examples/pipelines/
--rw-r--r--   0 briford    (501) staff       (20)     1000 2024-04-19 14:53:32.000000 sageworks-0.6.8/examples/pipelines/abalone_pipeline_v1.json
--rw-r--r--   0 briford    (501) staff       (20)     1073 2024-04-19 19:42:10.000000 sageworks-0.6.8/examples/pipelines/abalone_pipeline_v2.json
--rw-r--r--   0 briford    (501) staff       (20)     4435 2024-04-20 17:35:29.000000 sageworks-0.6.8/examples/pipelines/aqsol_pipeline_v1.json
--rw-r--r--   0 briford    (501) staff       (20)      142 2024-04-19 14:55:38.000000 sageworks-0.6.8/examples/pipelines/pipeline_details.py
--rw-r--r--   0 briford    (501) staff       (20)      324 2024-04-19 14:55:38.000000 sageworks-0.6.8/examples/pipelines/pipeline_execute.py
--rw-r--r--   0 briford    (501) staff       (20)      556 2024-04-19 14:51:51.000000 sageworks-0.6.8/examples/pipelines/pipeline_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.992177 sageworks-0.6.8/examples/plugins/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.043154 sageworks-0.6.8/examples/plugins/pages/
--rw-r--r--   0 briford    (501) staff       (20)     2467 2024-04-09 15:13:19.000000 sageworks-0.6.8/examples/plugins/pages/my_plugin_page.py
--rw-r--r--   0 briford    (501) staff       (20)     1635 2024-04-16 15:58:18.000000 sageworks-0.6.8/examples/plugins/pages/plugin_page_1.py
--rw-r--r--   0 briford    (501) staff       (20)     2464 2024-04-16 15:58:18.000000 sageworks-0.6.8/examples/plugins/pages/plugin_page_2.py
--rw-r--r--   0 briford    (501) staff       (20)     5810 2024-05-27 22:25:50.000000 sageworks-0.6.8/examples/plugins/pages/plugin_page_3.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.043555 sageworks-0.6.8/examples/plugins/views/
--rw-r--r--   0 briford    (501) staff       (20)     1588 2024-04-06 16:51:44.000000 sageworks-0.6.8/examples/plugins/views/model_plugin_view.py
--rw-r--r--   0 briford    (501) staff       (20)     1264 2024-04-06 16:51:44.000000 sageworks-0.6.8/examples/plugins/views/my_view_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.044262 sageworks-0.6.8/examples/plugins/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     1733 2024-04-16 15:58:18.000000 sageworks-0.6.8/examples/plugins/web_components/custom_plugin.py
--rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-16 15:58:18.000000 sageworks-0.6.8/examples/plugins/web_components/endpoint_plugin.py
--rw-r--r--   0 briford    (501) staff       (20)     3660 2024-04-16 15:58:18.000000 sageworks-0.6.8/examples/plugins/web_components/endpoint_turbo.py
--rw-r--r--   0 briford    (501) staff       (20)     2596 2024-04-16 15:58:18.000000 sageworks-0.6.8/examples/plugins/web_components/model_markdown.py
--rw-r--r--   0 briford    (501) staff       (20)     2238 2024-04-16 15:58:18.000000 sageworks-0.6.8/examples/plugins/web_components/model_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.045321 sageworks-0.6.8/examples/storage/
--rw-r--r--   0 briford    (501) staff       (20)     1222 2024-03-27 20:40:53.000000 sageworks-0.6.8/examples/storage/data_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)      856 2024-03-27 20:40:53.000000 sageworks-0.6.8/examples/storage/data_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     1371 2024-05-28 20:18:51.000000 sageworks-0.6.8/examples/storage/endpoint_inference.py
--rw-r--r--   0 briford    (501) staff       (20)     1847 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/hello_world_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)     4380 2024-04-16 15:58:18.000000 sageworks-0.6.8/examples/storage/plugin_page_example.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.046086 sageworks-0.6.8/examples/storage/sagemaker_pipelines/
--rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/sagemaker_pipelines/all_steps.py
--rw-r--r--   0 briford    (501) staff       (20)       40 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/sagemaker_pipelines/hello.py
--rw-r--r--   0 briford    (501) staff       (20)     1487 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/sagemaker_pipelines/ml_pipeline.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.992444 sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.046816 sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/
--rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)      203 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)      160 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
--rw-r--r--   0 briford    (501) staff       (20)     1599 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)      367 2024-03-28 17:23:43.000000 sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
--rw-r--r--   0 briford    (501) staff       (20)     3285 2024-05-24 14:48:45.000000 sageworks-0.6.8/mkdocs.yml
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.047634 sageworks-0.6.8/notebooks/
--rw-r--r--   0 briford    (501) staff       (20)    17688 2024-05-29 15:28:13.000000 sageworks-0.6.8/notebooks/ML_Pipeline_with_SageWorks.ipynb
--rw-r--r--   0 briford    (501) staff       (20)    16418 2024-05-29 15:28:13.000000 sageworks-0.6.8/notebooks/ML_Pipeline_with_SageWorks_2.ipynb
--rw-r--r--   0 briford    (501) staff       (20)    12554 2024-05-30 16:49:52.000000 sageworks-0.6.8/notebooks/Outliers_in_SageWorks.ipynb
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.055729 sageworks-0.6.8/notebooks/images/
--rw-r--r--   0 briford    (501) staff       (20)   142099 2023-12-24 17:18:24.000000 sageworks-0.6.8/notebooks/images/athena_query_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   191022 2023-12-24 17:18:24.000000 sageworks-0.6.8/notebooks/images/aws_dashboard_aqsol.png
--rw-r--r--   0 briford    (501) staff       (20)   222686 2023-12-24 17:18:24.000000 sageworks-0.6.8/notebooks/images/dashboard_aqsol_features.png
--rw-r--r--   0 briford    (501) staff       (20)   171441 2023-12-24 17:18:24.000000 sageworks-0.6.8/notebooks/images/model_screenshot.png
--rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.8/notebooks/images/sageworks_concepts.png
--rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.8/notebooks/images/scp_labs.png
--rw-r--r--   0 briford    (501) staff       (20)      196 2024-05-30 17:04:13.000000 sageworks-0.6.8/pyproject.toml
--rw-r--r--   0 briford    (501) staff       (20)      444 2024-05-19 21:32:59.000000 sageworks-0.6.8/requirements.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.058315 sageworks-0.6.8/scripts/
--rw-r--r--   0 briford    (501) staff       (20)     1710 2024-04-16 15:58:18.000000 sageworks-0.6.8/scripts/ag_table_row_selection.py
--rw-r--r--   0 briford    (501) staff       (20)     2290 2024-03-28 17:23:43.000000 sageworks-0.6.8/scripts/athena_ddl_mixed_case.py
--rw-r--r--   0 briford    (501) staff       (20)     2178 2024-03-27 20:32:26.000000 sageworks-0.6.8/scripts/copy_data_catalog_db.py
--rw-r--r--   0 briford    (501) staff       (20)     1222 2024-04-16 15:58:18.000000 sageworks-0.6.8/scripts/create_glue_workflow_with_trigger.py
--rw-r--r--   0 briford    (501) staff       (20)      706 2024-01-10 18:45:51.000000 sageworks-0.6.8/scripts/delete_redis_keys.py
--rw-r--r--   0 briford    (501) staff       (20)     1761 2024-03-28 17:23:43.000000 sageworks-0.6.8/scripts/glue_mixed_case.py
--rw-r--r--   0 briford    (501) staff       (20)     5544 2024-03-28 17:23:43.000000 sageworks-0.6.8/scripts/model_endpoint_sanity_check.py
--rw-r--r--   0 briford    (501) staff       (20)      715 2024-03-28 17:23:43.000000 sageworks-0.6.8/scripts/onboard_endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      694 2024-03-28 17:23:43.000000 sageworks-0.6.8/scripts/onboard_models.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.058716 sageworks-0.6.8/scripts/storage/
--rw-r--r--   0 briford    (501) staff       (20)     1003 2024-03-27 20:32:27.000000 sageworks-0.6.8/scripts/storage/dns_data_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     1723 2024-04-06 16:51:44.000000 sageworks-0.6.8/scripts/storage/generate_jsonl_data.py
--rw-r--r--   0 briford    (501) staff       (20)      955 2024-03-28 17:23:43.000000 sageworks-0.6.8/scripts/test_feature_resolution.py
--rw-r--r--   0 briford    (501) staff       (20)      427 2024-05-30 17:23:31.104761 sageworks-0.6.8/setup.cfg
--rw-r--r--   0 briford    (501) staff       (20)     1657 2024-05-30 17:21:02.000000 sageworks-0.6.8/setup.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.993054 sageworks-0.6.8/src/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.059008 sageworks-0.6.8/src/sageworks/
--rw-r--r--   0 briford    (501) staff       (20)     1091 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.060012 sageworks-0.6.8/src/sageworks/algorithms/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.8/src/sageworks/algorithms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.061767 sageworks-0.6.8/src/sageworks/algorithms/dataframe/
--rw-r--r--   0 briford    (501) staff       (20)      378 2023-12-24 17:18:24.000000 sageworks-0.6.8/src/sageworks/algorithms/dataframe/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     2852 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/algorithms/dataframe/aggregation.py
--rw-r--r--   0 briford    (501) staff       (20)     1606 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/algorithms/dataframe/data_source_eda.py
--rw-r--r--   0 briford    (501) staff       (20)     5388 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/algorithms/dataframe/dimensionality_reduction.py
--rw-r--r--   0 briford    (501) staff       (20)     9406 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/algorithms/dataframe/feature_resolution.py
--rw-r--r--   0 briford    (501) staff       (20)    12309 2024-05-28 20:18:51.000000 sageworks-0.6.8/src/sageworks/algorithms/dataframe/feature_spider.py
--rw-r--r--   0 briford    (501) staff       (20)     4968 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/algorithms/dataframe/row_tagger.py
--rw-r--r--   0 briford    (501) staff       (20)     4628 2024-03-27 20:32:27.000000 sageworks-0.6.8/src/sageworks/algorithms/dataframe/target_gradients.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.993406 sageworks-0.6.8/src/sageworks/algorithms/graph/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.062042 sageworks-0.6.8/src/sageworks/algorithms/graph/heavy/
--rw-r--r--   0 briford    (501) staff       (20)       96 2023-12-24 17:18:24.000000 sageworks-0.6.8/src/sageworks/algorithms/graph/heavy/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.062316 sageworks-0.6.8/src/sageworks/algorithms/graph/light/
--rw-r--r--   0 briford    (501) staff       (20)      122 2023-12-24 17:18:24.000000 sageworks-0.6.8/src/sageworks/algorithms/graph/light/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.062526 sageworks-0.6.8/src/sageworks/algorithms/spark/
--rw-r--r--   0 briford    (501) staff       (20)      615 2023-12-24 17:18:24.000000 sageworks-0.6.8/src/sageworks/algorithms/spark/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.064055 sageworks-0.6.8/src/sageworks/algorithms/sql/
--rw-r--r--   0 briford    (501) staff       (20)      685 2023-12-24 17:18:24.000000 sageworks-0.6.8/src/sageworks/algorithms/sql/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)     6221 2024-05-30 15:14:43.000000 sageworks-0.6.8/src/sageworks/algorithms/sql/column_stats.py
--rw-r--r--   0 briford    (501) staff       (20)     3666 2024-05-30 14:49:00.000000 sageworks-0.6.8/src/sageworks/algorithms/sql/correlations.py
--rw-r--r--   0 briford    (501) staff       (20)     4045 2024-05-30 15:05:13.000000 sageworks-0.6.8/src/sageworks/algorithms/sql/descriptive_stats.py
--rw-r--r--   0 briford    (501) staff       (20)    10377 2024-05-30 16:34:27.000000 sageworks-0.6.8/src/sageworks/algorithms/sql/outliers.py
--rw-r--r--   0 briford    (501) staff       (20)     2352 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/algorithms/sql/sample_rows.py
--rw-r--r--   0 briford    (501) staff       (20)     3466 2024-05-30 14:49:00.000000 sageworks-0.6.8/src/sageworks/algorithms/sql/value_counts.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.066372 sageworks-0.6.8/src/sageworks/api/
--rw-r--r--   0 briford    (501) staff       (20)      708 2024-04-18 20:46:23.000000 sageworks-0.6.8/src/sageworks/api/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     7811 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/api/data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2634 2024-05-29 14:06:46.000000 sageworks-0.6.8/src/sageworks/api/endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     4224 2024-05-28 21:46:10.000000 sageworks-0.6.8/src/sageworks/api/feature_set.py
--rw-r--r--   0 briford    (501) staff       (20)    16482 2024-04-21 15:28:58.000000 sageworks-0.6.8/src/sageworks/api/meta.py
--rw-r--r--   0 briford    (501) staff       (20)     2595 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/api/model.py
--rw-r--r--   0 briford    (501) staff       (20)     5261 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/api/monitor.py
--rw-r--r--   0 briford    (501) staff       (20)     6953 2024-04-26 21:22:37.000000 sageworks-0.6.8/src/sageworks/api/pipeline.py
--rw-r--r--   0 briford    (501) staff       (20)     6659 2024-04-26 21:22:37.000000 sageworks-0.6.8/src/sageworks/api/pipeline_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.066969 sageworks-0.6.8/src/sageworks/aws_service_broker/
--rw-r--r--   0 briford    (501) staff       (20)     9393 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_account_clamp.py
--rw-r--r--   0 briford    (501) staff       (20)    11198 2024-05-09 14:32:45.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_broker.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.068603 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     1834 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
--rw-r--r--   0 briford    (501) staff       (20)     3258 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)     4055 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)     5238 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)     3712 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
--rw-r--r--   0 briford    (501) staff       (20)     3889 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     3736 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.068753 sageworks-0.6.8/src/sageworks/core/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.071386 sageworks-0.6.8/src/sageworks/core/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)      941 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/artifacts/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    17938 2024-04-15 22:06:08.000000 sageworks-0.6.8/src/sageworks/core/artifacts/artifact.py
--rw-r--r--   0 briford    (501) staff       (20)    22432 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/core/artifacts/athena_source.py
--rw-r--r--   0 briford    (501) staff       (20)    12683 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/artifacts/data_source_abstract.py
--rw-r--r--   0 briford    (501) staff       (20)     2447 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/artifacts/data_source_factory.py
--rw-r--r--   0 briford    (501) staff       (20)    37061 2024-05-29 13:52:08.000000 sageworks-0.6.8/src/sageworks/core/artifacts/endpoint_core.py
--rw-r--r--   0 briford    (501) staff       (20)    29698 2024-04-22 20:46:36.000000 sageworks-0.6.8/src/sageworks/core/artifacts/feature_set_core.py
--rw-r--r--   0 briford    (501) staff       (20)    36644 2024-05-29 18:45:32.000000 sageworks-0.6.8/src/sageworks/core/artifacts/model_core.py
--rw-r--r--   0 briford    (501) staff       (20)    21029 2024-05-28 20:40:35.000000 sageworks-0.6.8/src/sageworks/core/artifacts/monitor_core.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.071725 sageworks-0.6.8/src/sageworks/core/pipelines/
--rw-r--r--   0 briford    (501) staff       (20)     6919 2024-04-26 21:22:37.000000 sageworks-0.6.8/src/sageworks/core/pipelines/pipeline_executor.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.072407 sageworks-0.6.8/src/sageworks/core/transforms/
--rw-r--r--   0 briford    (501) staff       (20)     1432 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/Readme.md
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.072692 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.073165 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/heavy/
--rw-r--r--   0 briford    (501) staff       (20)      298 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/heavy/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     9866 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.074309 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/
--rw-r--r--   0 briford    (501) staff       (20)      543 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3011 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     2927 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py
--rw-r--r--   0 briford    (501) staff       (20)     4225 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.074638 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.074766 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.074890 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.075180 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.075743 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     2237 2024-03-27 20:40:53.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/light/clean_data.py
--rw-r--r--   0 briford    (501) staff       (20)     2687 2024-03-27 20:40:53.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.075988 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.076101 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.076317 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/chunk/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/chunk/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     4551 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.076666 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.076834 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.077000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/storage/
--rw-r--r--   0 briford    (501) staff       (20)     6702 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.077633 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/light/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/light/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3827 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
--rw-r--r--   0 briford    (501) staff       (20)     5674 2024-04-23 15:16:38.000000 sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.077965 sageworks-0.6.8/src/sageworks/core/transforms/features_to_features/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/features_to_features/__init__.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:30.995463 sageworks-0.6.8/src/sageworks/core/transforms/features_to_features/heavy/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.078074 sageworks-0.6.8/src/sageworks/core/transforms/features_to_features/heavy/emr/
--rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.078223 sageworks-0.6.8/src/sageworks/core/transforms/features_to_features/heavy/glue/
--rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.078473 sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    13050 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/features_to_model.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.079273 sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/light_model_harness/
--rw-r--r--   0 briford    (501) staff       (20)    13982 2024-05-28 20:18:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/light_model_harness/generated_xgb_model.py
--rw-r--r--   0 briford    (501) staff       (20)       19 2024-02-27 23:40:48.000000 sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
--rw-r--r--   0 briford    (501) staff       (20)    10806 2024-05-28 20:18:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.079678 sageworks-0.6.8/src/sageworks/core/transforms/model_to_endpoint/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/core/transforms/model_to_endpoint/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     8185 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.081035 sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/
--rw-r--r--   0 briford    (501) staff       (20)      894 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)     3615 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     3445 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
--rw-r--r--   0 briford    (501) staff       (20)     8604 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py
--rw-r--r--   0 briford    (501) staff       (20)    18139 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py
--rw-r--r--   0 briford    (501) staff       (20)     4440 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py
--rw-r--r--   0 briford    (501) staff       (20)     5391 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/core/transforms/transform.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.081243 sageworks-0.6.8/src/sageworks/experiments/
--rw-r--r--   0 briford    (501) staff       (20)    10658 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/experiments/view_manager.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.081636 sageworks-0.6.8/src/sageworks/repl/
--rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/repl/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    15486 2024-04-21 15:35:25.000000 sageworks-0.6.8/src/sageworks/repl/sageworks_shell.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.082149 sageworks-0.6.8/src/sageworks/resources/
--rw-r--r--   0 briford    (501) staff       (20)      361 2024-01-23 15:36:53.000000 sageworks-0.6.8/src/sageworks/resources/open_source_api.key
--rw-r--r--   0 briford    (501) staff       (20)      272 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/resources/signature_verify_pub.pem
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.089062 sageworks-0.6.8/src/sageworks/utils/
--rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.8/src/sageworks/utils/__init__.py
--rw-r--r--   0 briford    (501) staff       (20)    15587 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/utils/aws_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5447 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/utils/cache.py
--rw-r--r--   0 briford    (501) staff       (20)      722 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/chem_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    16543 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/utils/config_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     7392 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/dashboard_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)     4194 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/utils/datetime_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     5292 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/df_to_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     1681 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/docker_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2866 2024-03-27 20:43:31.000000 sageworks-0.6.8/src/sageworks/utils/ecs_info.py
--rw-r--r--   0 briford    (501) staff       (20)     7657 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/endpoint_metrics.py
--rw-r--r--   0 briford    (501) staff       (20)     3098 2024-05-28 20:18:49.000000 sageworks-0.6.8/src/sageworks/utils/endpoint_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     6979 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/extract_model_artifact.py
--rw-r--r--   0 briford    (501) staff       (20)     1131 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/glue_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     6404 2024-05-20 15:33:17.000000 sageworks-0.6.8/src/sageworks/utils/license_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     1439 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/utils/markdown_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    15517 2024-04-22 20:45:19.000000 sageworks-0.6.8/src/sageworks/utils/pandas_utils.py
--rw-r--r--   0 briford    (501) staff       (20)    12684 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/utils/plugin_manager.py
--rw-r--r--   0 briford    (501) staff       (20)     9533 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/utils/redis_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     4166 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/repl_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2089 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/s3_utils.py
--rw-r--r--   0 briford    (501) staff       (20)     2163 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/sageworks_cache.py
--rw-r--r--   0 briford    (501) staff       (20)     3474 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/sageworks_event_bridge.py
--rw-r--r--   0 briford    (501) staff       (20)     5359 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/sageworks_logging.py
--rw-r--r--   0 briford    (501) staff       (20)     2120 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/sageworks_sqs.py
--rw-r--r--   0 briford    (501) staff       (20)     1108 2024-01-10 18:45:51.000000 sageworks-0.6.8/src/sageworks/utils/symbols.py
--rw-r--r--   0 briford    (501) staff       (20)     6414 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/test_data_generator.py
--rw-r--r--   0 briford    (501) staff       (20)     2092 2024-03-27 20:43:31.000000 sageworks-0.6.8/src/sageworks/utils/trace_calls.py
--rw-r--r--   0 briford    (501) staff       (20)     1470 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/utils/type_abbrev.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.090585 sageworks-0.6.8/src/sageworks/views/
--rw-r--r--   0 briford    (501) staff       (20)     3517 2024-04-16 22:29:17.000000 sageworks-0.6.8/src/sageworks/views/artifacts_text_view.py
--rw-r--r--   0 briford    (501) staff       (20)     7780 2024-04-28 17:17:45.000000 sageworks-0.6.8/src/sageworks/views/artifacts_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3158 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/views/data_source_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     2150 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/views/endpoint_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     3206 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/views/feature_set_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/views/model_web_view.py
--rw-r--r--   0 briford    (501) staff       (20)     1092 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/views/view.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.093567 sageworks-0.6.8/src/sageworks/web_components/
--rw-r--r--   0 briford    (501) staff       (20)     5916 2024-04-25 23:06:38.000000 sageworks-0.6.8/src/sageworks/web_components/component_interface.py
--rw-r--r--   0 briford    (501) staff       (20)     3525 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/confusion_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     5854 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/correlation_matrix.py
--rw-r--r--   0 briford    (501) staff       (20)     9328 2024-04-06 16:51:44.000000 sageworks-0.6.8/src/sageworks/web_components/data_details_markdown.py
--rw-r--r--   0 briford    (501) staff       (20)     3068 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/endpoint_metric_plots.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.095682 sageworks-0.6.8/src/sageworks/web_components/experiments/
--rw-r--r--   0 briford    (501) staff       (20)      837 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/color_maps.py
--rw-r--r--   0 briford    (501) staff       (20)     1633 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/compound_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2974 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/dashboard_metric_plots.py
--rw-r--r--   0 briford    (501) staff       (20)     2240 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/data_table.py
--rw-r--r--   0 briford    (501) staff       (20)     2453 2024-04-02 16:53:34.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/graph_test.py
--rw-r--r--   0 briford    (501) staff       (20)     1765 2024-04-02 16:53:34.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/hello.py
--rw-r--r--   0 briford    (501) staff       (20)     1183 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/histogram.py
--rw-r--r--   0 briford    (501) staff       (20)      838 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/line_chart.py
--rw-r--r--   0 briford    (501) staff       (20)     3680 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/outlier_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     2373 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/plugin_callbacks.py
--rw-r--r--   0 briford    (501) staff       (20)     2279 2024-03-28 17:23:43.000000 sageworks-0.6.8/src/sageworks/web_components/experiments/scatter_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     2278 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/model_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     7681 2024-05-27 16:52:27.000000 sageworks-0.6.8/src/sageworks/web_components/plugin_interface.py
--rw-r--r--   0 briford    (501) staff       (20)     3627 2024-05-27 19:18:14.000000 sageworks-0.6.8/src/sageworks/web_components/plugin_unit_test.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.096865 sageworks-0.6.8/src/sageworks/web_components/plugins/
--rw-r--r--   0 briford    (501) staff       (20)     2786 2024-04-26 21:04:42.000000 sageworks-0.6.8/src/sageworks/web_components/plugins/ag_table.py
--rw-r--r--   0 briford    (501) staff       (20)     3749 2024-05-28 15:15:12.000000 sageworks-0.6.8/src/sageworks/web_components/plugins/endpoint_details.py
--rw-r--r--   0 briford    (501) staff       (20)     5498 2024-05-22 14:54:18.000000 sageworks-0.6.8/src/sageworks/web_components/plugins/license_details.py
--rw-r--r--   0 briford    (501) staff       (20)     7607 2024-05-29 18:44:03.000000 sageworks-0.6.8/src/sageworks/web_components/plugins/model_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2429 2024-04-26 21:22:37.000000 sageworks-0.6.8/src/sageworks/web_components/plugins/pipeline_details.py
--rw-r--r--   0 briford    (501) staff       (20)     2959 2024-05-29 15:29:46.000000 sageworks-0.6.8/src/sageworks/web_components/regression_plot.py
--rw-r--r--   0 briford    (501) staff       (20)     6838 2024-05-06 17:24:24.000000 sageworks-0.6.8/src/sageworks/web_components/table.py
--rw-r--r--   0 briford    (501) staff       (20)     5185 2024-04-16 15:58:18.000000 sageworks-0.6.8/src/sageworks/web_components/violin_plots.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.103860 sageworks-0.6.8/src/sageworks.egg-info/
--rw-r--r--   0 briford    (501) staff       (20)     4961 2024-05-30 17:23:30.000000 sageworks-0.6.8/src/sageworks.egg-info/PKG-INFO
--rw-r--r--   0 briford    (501) staff       (20)    19412 2024-05-30 17:23:30.000000 sageworks-0.6.8/src/sageworks.egg-info/SOURCES.txt
--rw-r--r--   0 briford    (501) staff       (20)        1 2024-05-30 17:23:30.000000 sageworks-0.6.8/src/sageworks.egg-info/dependency_links.txt
--rw-r--r--   0 briford    (501) staff       (20)       74 2024-05-30 17:23:30.000000 sageworks-0.6.8/src/sageworks.egg-info/entry_points.txt
--rw-r--r--   0 briford    (501) staff       (20)      421 2024-05-30 17:23:30.000000 sageworks-0.6.8/src/sageworks.egg-info/requires.txt
--rw-r--r--   0 briford    (501) staff       (20)       10 2024-05-30 17:23:30.000000 sageworks-0.6.8/src/sageworks.egg-info/top_level.txt
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.098055 sageworks-0.6.8/tests/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.098874 sageworks-0.6.8/tests/artifacts/
--rw-r--r--   0 briford    (501) staff       (20)     1548 2024-03-30 19:27:28.000000 sageworks-0.6.8/tests/artifacts/data_source_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     2442 2024-05-28 20:18:51.000000 sageworks-0.6.8/tests/artifacts/endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1160 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/artifacts/feature_set_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      805 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/artifacts/model_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.099285 sageworks-0.6.8/tests/aws_account/
--rw-r--r--   0 briford    (501) staff       (20)      962 2023-12-24 17:18:24.000000 sageworks-0.6.8/tests/aws_account/aws_account_clamp_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      642 2023-12-24 17:18:24.000000 sageworks-0.6.8/tests/aws_account/aws_service_broker_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.100337 sageworks-0.6.8/tests/connectors/
--rw-r--r--   0 briford    (501) staff       (20)      725 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/connectors/data_catalog.py
--rw-r--r--   0 briford    (501) staff       (20)      737 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/connectors/endpoints.py
--rw-r--r--   0 briford    (501) staff       (20)      702 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/connectors/feature_store.py
--rw-r--r--   0 briford    (501) staff       (20)      644 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/connectors/glue_jobs.py
--rw-r--r--   0 briford    (501) staff       (20)      799 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/connectors/model_registry.py
--rw-r--r--   0 briford    (501) staff       (20)     1008 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/connectors/s3_bucket.py
--rw-r--r--   0 briford    (501) staff       (20)     5618 2024-04-26 21:04:42.000000 sageworks-0.6.8/tests/create_aqsol_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     3217 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/create_basic_test_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)      870 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/create_realtime_endpoint.py
--rw-r--r--   0 briford    (501) staff       (20)     2378 2024-04-22 20:46:36.000000 sageworks-0.6.8/tests/create_training_adjusted_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     2096 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/create_wine_artifacts.py
--rw-r--r--   0 briford    (501) staff       (20)     4448 2024-04-16 15:58:18.000000 sageworks-0.6.8/tests/delete_test_artifacts.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.100483 sageworks-0.6.8/tests/plugin_tests/
--rw-r--r--   0 briford    (501) staff       (20)     1885 2024-04-16 15:58:18.000000 sageworks-0.6.8/tests/plugin_tests/crashing_plugin.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.100763 sageworks-0.6.8/tests/specific/
--rw-r--r--   0 briford    (501) staff       (20)      639 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/specific/capital_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1513 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/specific/deletion_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.101846 sageworks-0.6.8/tests/transforms/
--rw-r--r--   0 briford    (501) staff       (20)      592 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/transforms/data_to_data_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     1025 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/transforms/data_to_features_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      773 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/transforms/features_to_model_tests.py
--rw-r--r--   0 briford    (501) staff       (20)     5134 2024-05-29 18:44:03.000000 sageworks-0.6.8/tests/transforms/model_metrics_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      795 2024-03-28 17:23:43.000000 sageworks-0.6.8/tests/transforms/model_to_endpoint_tests.py
--rw-r--r--   0 briford    (501) staff       (20)      633 2024-03-27 20:40:53.000000 sageworks-0.6.8/tests/transforms/pandas_to_data_tests.py
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.102548 sageworks-0.6.8/tests/web_components/
--rw-r--r--   0 briford    (501) staff       (20)      681 2024-04-16 15:58:18.000000 sageworks-0.6.8/tests/web_components/confusion_matrix_test.py
--rw-r--r--   0 briford    (501) staff       (20)      677 2024-04-16 15:58:18.000000 sageworks-0.6.8/tests/web_components/correlation_matrix_test.py
--rw-r--r--   0 briford    (501) staff       (20)     5269 2024-04-16 15:58:18.000000 sageworks-0.6.8/tests/web_components/plugin_interface_test.py
--rw-r--r--   0 briford    (501) staff       (20)     1112 2024-05-29 18:21:35.000000 sageworks-0.6.8/tox.ini
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.103324 sageworks-0.6.8/ui_testing/
-drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-30 17:23:31.103548 sageworks-0.6.8/ui_testing/assets/
--rw-r--r--   0 briford    (501) staff       (20)      597 2024-05-13 15:14:49.000000 sageworks-0.6.8/ui_testing/assets/custom.css
--rw-r--r--   0 briford    (501) staff       (20)     5770 2024-05-19 19:25:10.000000 sageworks-0.6.8/ui_testing/table_comparison.py
--rw-r--r--   0 briford    (501) staff       (20)     2025 2024-05-19 19:25:10.000000 sageworks-0.6.8/ui_testing/theme_switching.py
--rw-r--r--   0 briford    (501) staff       (20)     1819 2024-05-19 19:25:10.000000 sageworks-0.6.8/ui_testing/theme_switching_2.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.614052 sageworks-0.6.9/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.490881 sageworks-0.6.9/.github/
+-rw-r--r--   0 briford    (501) staff       (20)     1338 2024-03-28 17:23:43.000000 sageworks-0.6.9/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 briford    (501) staff       (20)      499 2023-12-24 17:18:24.000000 sageworks-0.6.9/.github/dependabot.yml
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.491322 sageworks-0.6.9/.github/workflows/
+-rw-r--r--   0 briford    (501) staff       (20)      598 2024-01-10 18:45:51.000000 sageworks-0.6.9/.github/workflows/deploy-docs.yml
+-rw-r--r--   0 briford    (501) staff       (20)      556 2024-01-23 15:36:53.000000 sageworks-0.6.9/.github/workflows/python-lint.yml
+-rw-r--r--   0 briford    (501) staff       (20)     2037 2024-05-15 21:28:12.000000 sageworks-0.6.9/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)      791 2024-04-16 15:58:18.000000 sageworks-0.6.9/CONTRIBUTING.md
+-rw-r--r--   0 briford    (501) staff       (20)      102 2024-03-28 17:23:43.000000 sageworks-0.6.9/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)     1080 2024-03-28 17:23:43.000000 sageworks-0.6.9/LICENSE
+-rw-r--r--   0 briford    (501) staff       (20)     1426 2023-12-24 17:18:24.000000 sageworks-0.6.9/Makefile
+-rw-r--r--   0 briford    (501) staff       (20)     4927 2024-05-31 23:16:54.613968 sageworks-0.6.9/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)     3510 2024-05-09 14:32:45.000000 sageworks-0.6.9/README.md
+-rw-r--r--   0 briford    (501) staff       (20)      463 2023-12-24 17:18:24.000000 sageworks-0.6.9/SECURITY.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.479530 sageworks-0.6.9/applications/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.493691 sageworks-0.6.9/applications/aws_dashboard/
+-rw-r--r--   0 briford    (501) staff       (20)     1071 2024-05-24 14:50:34.000000 sageworks-0.6.9/applications/aws_dashboard/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      331 2024-03-28 17:23:43.000000 sageworks-0.6.9/applications/aws_dashboard/Dockerfile_plugins
+-rw-r--r--   0 briford    (501) staff       (20)      841 2024-01-10 18:45:51.000000 sageworks-0.6.9/applications/aws_dashboard/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1526 2024-04-09 14:37:33.000000 sageworks-0.6.9/applications/aws_dashboard/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.495081 sageworks-0.6.9/applications/aws_dashboard/assets/
+-rw-r--r--   0 briford    (501) staff       (20)   232839 2024-04-06 16:51:44.000000 sageworks-0.6.9/applications/aws_dashboard/assets/bootstrap_darkly.min.css
+-rw-r--r--   0 briford    (501) staff       (20)    14995 2024-04-06 16:51:44.000000 sageworks-0.6.9/applications/aws_dashboard/assets/default.css
+-rw-r--r--   0 briford    (501) staff       (20)    10375 2024-04-16 15:58:18.000000 sageworks-0.6.9/applications/aws_dashboard/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)      732 2023-12-24 17:18:24.000000 sageworks-0.6.9/applications/aws_dashboard/assets/trash.png
+-rwxr-xr-x   0 briford    (501) staff       (20)      637 2024-04-26 21:03:22.000000 sageworks-0.6.9/applications/aws_dashboard/dashboard
+-rw-r--r--   0 briford    (501) staff       (20)      205 2023-12-24 17:18:24.000000 sageworks-0.6.9/applications/aws_dashboard/nginx.conf
+-rw-r--r--   0 briford    (501) staff       (20)      684 2024-03-28 17:23:43.000000 sageworks-0.6.9/applications/aws_dashboard/open_source_config.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.479458 sageworks-0.6.9/applications/aws_dashboard/pages/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.495794 sageworks-0.6.9/applications/aws_dashboard/pages/data_sources/
+-rw-r--r--   0 briford    (501) staff       (20)    11700 2024-04-16 15:58:18.000000 sageworks-0.6.9/applications/aws_dashboard/pages/data_sources/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2756 2024-03-28 17:23:43.000000 sageworks-0.6.9/applications/aws_dashboard/pages/data_sources/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2555 2024-03-28 17:23:43.000000 sageworks-0.6.9/applications/aws_dashboard/pages/data_sources/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.496505 sageworks-0.6.9/applications/aws_dashboard/pages/endpoints/
+-rw-r--r--   0 briford    (501) staff       (20)     4439 2024-05-28 15:10:23.000000 sageworks-0.6.9/applications/aws_dashboard/pages/endpoints/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2677 2024-04-16 15:58:18.000000 sageworks-0.6.9/applications/aws_dashboard/pages/endpoints/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2550 2024-05-28 15:10:23.000000 sageworks-0.6.9/applications/aws_dashboard/pages/endpoints/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.497194 sageworks-0.6.9/applications/aws_dashboard/pages/feature_sets/
+-rw-r--r--   0 briford    (501) staff       (20)    11614 2024-04-16 15:58:18.000000 sageworks-0.6.9/applications/aws_dashboard/pages/feature_sets/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2438 2024-03-28 17:23:43.000000 sageworks-0.6.9/applications/aws_dashboard/pages/feature_sets/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2505 2024-03-28 17:23:43.000000 sageworks-0.6.9/applications/aws_dashboard/pages/feature_sets/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.497476 sageworks-0.6.9/applications/aws_dashboard/pages/license/
+-rw-r--r--   0 briford    (501) staff       (20)     1531 2024-05-19 19:25:10.000000 sageworks-0.6.9/applications/aws_dashboard/pages/license/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.498390 sageworks-0.6.9/applications/aws_dashboard/pages/main/
+-rw-r--r--   0 briford    (501) staff       (20)     4899 2024-04-06 16:51:44.000000 sageworks-0.6.9/applications/aws_dashboard/pages/main/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     3307 2024-05-19 19:21:21.000000 sageworks-0.6.9/applications/aws_dashboard/pages/main/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1844 2024-03-28 17:23:43.000000 sageworks-0.6.9/applications/aws_dashboard/pages/main/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.499242 sageworks-0.6.9/applications/aws_dashboard/pages/models/
+-rw-r--r--   0 briford    (501) staff       (20)     4195 2024-05-28 15:10:23.000000 sageworks-0.6.9/applications/aws_dashboard/pages/models/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2234 2024-04-27 20:59:25.000000 sageworks-0.6.9/applications/aws_dashboard/pages/models/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     2227 2024-05-28 15:10:23.000000 sageworks-0.6.9/applications/aws_dashboard/pages/models/page.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.499947 sageworks-0.6.9/applications/aws_dashboard/pages/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     1791 2024-04-26 21:07:33.000000 sageworks-0.6.9/applications/aws_dashboard/pages/pipelines/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2664 2024-04-26 20:07:24.000000 sageworks-0.6.9/applications/aws_dashboard/pages/pipelines/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)     1927 2024-04-26 21:04:41.000000 sageworks-0.6.9/applications/aws_dashboard/pages/pipelines/page.py
+-rw-r--r--   0 briford    (501) staff       (20)      388 2024-05-30 17:40:49.000000 sageworks-0.6.9/applications/aws_dashboard/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)      457 2023-12-24 17:18:24.000000 sageworks-0.6.9/applications/aws_dashboard/supervisord.conf
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.479583 sageworks-0.6.9/applications/experiments/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.501474 sageworks-0.6.9/applications/experiments/compound_explorer/
+-rw-r--r--   0 briford    (501) staff       (20)      181 2023-12-24 17:18:24.000000 sageworks-0.6.9/applications/experiments/compound_explorer/Dockerfile
+-rw-r--r--   0 briford    (501) staff       (20)      360 2023-12-24 17:18:24.000000 sageworks-0.6.9/applications/experiments/compound_explorer/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     3082 2024-04-06 16:51:44.000000 sageworks-0.6.9/applications/experiments/compound_explorer/app.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.501972 sageworks-0.6.9/applications/experiments/compound_explorer/assets/
+-rw-r--r--   0 briford    (501) staff       (20)    12861 2023-12-24 17:18:24.000000 sageworks-0.6.9/applications/experiments/compound_explorer/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)      318 2023-12-24 17:18:24.000000 sageworks-0.6.9/applications/experiments/compound_explorer/assets/favicon.ico
+-rw-r--r--   0 briford    (501) staff       (20)     7678 2024-04-16 15:58:18.000000 sageworks-0.6.9/applications/experiments/compound_explorer/callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     4860 2024-03-28 17:23:43.000000 sageworks-0.6.9/applications/experiments/compound_explorer/layout.py
+-rw-r--r--   0 briford    (501) staff       (20)       94 2023-12-24 17:18:24.000000 sageworks-0.6.9/applications/experiments/compound_explorer/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.502494 sageworks-0.6.9/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     3582 2024-03-28 17:23:43.000000 sageworks-0.6.9/aws_setup/aws_account_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.9/aws_setup/aws_identity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)     2629 2024-03-28 17:23:43.000000 sageworks-0.6.9/aws_setup/build_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.502655 sageworks-0.6.9/aws_setup/event_bridge/
+-rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/event_bridge/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.503444 sageworks-0.6.9/aws_setup/event_bridge/dynamic_docker/
+-rw-r--r--   0 briford    (501) staff       (20)       60 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/event_bridge/dynamic_docker/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     1007 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/event_bridge/dynamic_docker/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/event_bridge/dynamic_docker/cdk.json
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.503781 sageworks-0.6.9/aws_setup/event_bridge/dynamic_docker/lambda/
+-rw-r--r--   0 briford    (501) staff       (20)     1812 2024-01-10 18:45:51.000000 sageworks-0.6.9/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py
+-rw-r--r--   0 briford    (501) staff       (20)     2599 2024-03-27 20:43:31.000000 sageworks-0.6.9/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.505033 sageworks-0.6.9/aws_setup/sageworks_core/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_core/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1028 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_core/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1403 2024-03-28 17:23:43.000000 sageworks-0.6.9/aws_setup/sageworks_core/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     1998 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_core/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_core/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       53 2024-01-10 18:45:51.000000 sageworks-0.6.9/aws_setup/sageworks_core/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.505415 sageworks-0.6.9/aws_setup/sageworks_core/sageworks_core/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.9/aws_setup/sageworks_core/sageworks_core/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    23575 2024-03-28 17:23:43.000000 sageworks-0.6.9/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_core/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.505780 sageworks-0.6.9/aws_setup/sageworks_core/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_core/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.505978 sageworks-0.6.9/aws_setup/sageworks_core/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_core/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      720 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.507456 sageworks-0.6.9/aws_setup/sageworks_dashboard_full/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_full/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_full/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1907 2024-03-28 17:23:43.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_full/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_full/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       14 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_full/requirements-dev.txt
+-rw-r--r--   0 briford    (501) staff       (20)       47 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_full/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.507715 sageworks-0.6.9/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7022 2024-04-24 21:53:47.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py
+-rw-r--r--   0 briford    (501) staff       (20)      437 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_full/source.bat
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.508082 sageworks-0.6.9/aws_setup/sageworks_dashboard_full/tests/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_full/tests/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.508286 sageworks-0.6.9/aws_setup/sageworks_dashboard_full/tests/unit/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_full/tests/unit/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)      565 2023-12-24 17:18:24.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.509050 sageworks-0.6.9/aws_setup/sageworks_dashboard_lite/
+-rw-r--r--   0 briford    (501) staff       (20)      119 2024-03-28 17:23:43.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_lite/.gitignore
+-rw-r--r--   0 briford    (501) staff       (20)     1778 2024-03-28 17:23:43.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_lite/README.md
+-rw-r--r--   0 briford    (501) staff       (20)     1928 2024-03-28 17:23:43.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_lite/app.py
+-rw-r--r--   0 briford    (501) staff       (20)     2567 2024-03-28 17:23:43.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_lite/cdk.json
+-rw-r--r--   0 briford    (501) staff       (20)       47 2024-03-28 17:23:43.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_lite/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.509323 sageworks-0.6.9/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-03-28 17:23:43.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     6849 2024-05-24 14:56:58.000000 sageworks-0.6.9/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.510735 sageworks-0.6.9/data/
+-rw-r--r--   0 briford    (501) staff       (20)   191978 2023-12-24 17:18:24.000000 sageworks-0.6.9/data/abalone.csv
+-rw-r--r--   0 briford    (501) staff       (20)     1515 2023-12-24 17:18:24.000000 sageworks-0.6.9/data/test_data.csv
+-rw-r--r--   0 briford    (501) staff       (20)     2270 2023-12-24 17:18:24.000000 sageworks-0.6.9/data/test_data.json
+-rw-r--r--   0 briford    (501) staff       (20)    12977 2024-01-10 18:45:51.000000 sageworks-0.6.9/data/wine_dataset.csv
+-rw-r--r--   0 briford    (501) staff       (20)       66 2024-05-30 17:51:10.000000 sageworks-0.6.9/dev-requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.510991 sageworks-0.6.9/docs/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.511510 sageworks-0.6.9/docs/admin/
+-rw-r--r--   0 briford    (501) staff       (20)     2176 2024-04-16 15:58:18.000000 sageworks-0.6.9/docs/admin/docker_push.md
+-rw-r--r--   0 briford    (501) staff       (20)     1594 2024-05-30 16:53:00.000000 sageworks-0.6.9/docs/admin/pypi_release.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.513538 sageworks-0.6.9/docs/api_classes/
+-rw-r--r--   0 briford    (501) staff       (20)     3595 2024-01-23 15:36:53.000000 sageworks-0.6.9/docs/api_classes/data_source.md
+-rw-r--r--   0 briford    (501) staff       (20)     5199 2024-05-28 20:18:51.000000 sageworks-0.6.9/docs/api_classes/endpoint.md
+-rw-r--r--   0 briford    (501) staff       (20)     6299 2024-03-28 17:23:43.000000 sageworks-0.6.9/docs/api_classes/feature_set.md
+-rw-r--r--   0 briford    (501) staff       (20)     5350 2024-04-06 16:51:44.000000 sageworks-0.6.9/docs/api_classes/meta.md
+-rw-r--r--   0 briford    (501) staff       (20)     4356 2024-05-28 20:18:51.000000 sageworks-0.6.9/docs/api_classes/model.md
+-rw-r--r--   0 briford    (501) staff       (20)     2218 2024-01-10 18:45:51.000000 sageworks-0.6.9/docs/api_classes/monitor.md
+-rw-r--r--   0 briford    (501) staff       (20)     3549 2024-05-28 20:18:51.000000 sageworks-0.6.9/docs/api_classes/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)     4894 2024-04-19 15:50:50.000000 sageworks-0.6.9/docs/api_classes/pipelines.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.515346 sageworks-0.6.9/docs/aws_setup/
+-rw-r--r--   0 briford    (501) staff       (20)     1121 2024-03-28 17:23:43.000000 sageworks-0.6.9/docs/aws_setup/aws_access_management.md
+-rw-r--r--   0 briford    (501) staff       (20)     5610 2024-05-06 14:50:56.000000 sageworks-0.6.9/docs/aws_setup/aws_tips_and_tricks.md
+-rw-r--r--   0 briford    (501) staff       (20)     4210 2024-05-09 14:32:45.000000 sageworks-0.6.9/docs/aws_setup/core_stack.md
+-rw-r--r--   0 briford    (501) staff       (20)     2075 2024-03-28 17:23:43.000000 sageworks-0.6.9/docs/aws_setup/dashboard_stack.md
+-rw-r--r--   0 briford    (501) staff       (20)     7313 2024-05-15 23:47:50.000000 sageworks-0.6.9/docs/aws_setup/domain_cert_setup.md
+-rw-r--r--   0 briford    (501) staff       (20)     2540 2024-01-23 15:36:53.000000 sageworks-0.6.9/docs/aws_setup/full_pipeline.md
+-rw-r--r--   0 briford    (501) staff       (20)     3438 2024-05-09 14:20:27.000000 sageworks-0.6.9/docs/aws_setup/sso_setup.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.516255 sageworks-0.6.9/docs/blogs_research/
+-rw-r--r--   0 briford    (501) staff       (20)      912 2024-03-28 17:23:43.000000 sageworks-0.6.9/docs/blogs_research/eda.md
+-rw-r--r--   0 briford    (501) staff       (20)     2017 2024-03-28 17:23:43.000000 sageworks-0.6.9/docs/blogs_research/htg.md
+-rw-r--r--   0 briford    (501) staff       (20)      802 2024-05-21 22:30:34.000000 sageworks-0.6.9/docs/blogs_research/index.md
+-rw-r--r--   0 briford    (501) staff       (20)     1245 2024-05-28 20:18:51.000000 sageworks-0.6.9/docs/blogs_research/residual_analysis.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.516567 sageworks-0.6.9/docs/concepts/
+-rw-r--r--   0 briford    (501) staff       (20)      907 2024-05-28 20:18:51.000000 sageworks-0.6.9/docs/concepts/model_monitoring.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.516793 sageworks-0.6.9/docs/core_classes/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.518353 sageworks-0.6.9/docs/core_classes/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      464 2024-01-23 15:36:53.000000 sageworks-0.6.9/docs/core_classes/artifacts/artifact.md
+-rw-r--r--   0 briford    (501) staff       (20)      290 2024-01-10 18:45:51.000000 sageworks-0.6.9/docs/core_classes/artifacts/athena_source.md
+-rw-r--r--   0 briford    (501) staff       (20)      479 2024-01-23 15:36:53.000000 sageworks-0.6.9/docs/core_classes/artifacts/data_source_abstract.md
+-rw-r--r--   0 briford    (501) staff       (20)      292 2024-01-10 18:45:51.000000 sageworks-0.6.9/docs/core_classes/artifacts/endpoint_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      294 2024-01-10 18:45:51.000000 sageworks-0.6.9/docs/core_classes/artifacts/feature_set_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      281 2024-01-10 18:45:51.000000 sageworks-0.6.9/docs/core_classes/artifacts/model_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      289 2024-01-10 18:45:51.000000 sageworks-0.6.9/docs/core_classes/artifacts/monitor_core.md
+-rw-r--r--   0 briford    (501) staff       (20)      861 2024-01-10 18:45:51.000000 sageworks-0.6.9/docs/core_classes/artifacts/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)     2119 2024-01-10 18:45:51.000000 sageworks-0.6.9/docs/core_classes/overview.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.519726 sageworks-0.6.9/docs/core_classes/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      352 2024-01-10 18:45:51.000000 sageworks-0.6.9/docs/core_classes/transforms/data_loaders_heavy.md
+-rw-r--r--   0 briford    (501) staff       (20)      396 2024-01-10 18:45:51.000000 sageworks-0.6.9/docs/core_classes/transforms/data_loaders_light.md
+-rw-r--r--   0 briford    (501) staff       (20)      349 2024-03-28 17:23:43.000000 sageworks-0.6.9/docs/core_classes/transforms/data_to_features.md
+-rw-r--r--   0 briford    (501) staff       (20)      265 2024-01-10 18:45:51.000000 sageworks-0.6.9/docs/core_classes/transforms/features_to_model.md
+-rw-r--r--   0 briford    (501) staff       (20)      264 2024-01-10 18:45:51.000000 sageworks-0.6.9/docs/core_classes/transforms/model_to_endpoint.md
+-rw-r--r--   0 briford    (501) staff       (20)     1177 2024-01-10 18:45:51.000000 sageworks-0.6.9/docs/core_classes/transforms/overview.md
+-rw-r--r--   0 briford    (501) staff       (20)      970 2024-01-23 15:36:53.000000 sageworks-0.6.9/docs/core_classes/transforms/pandas_transforms.md
+-rw-r--r--   0 briford    (501) staff       (20)      521 2024-01-23 15:36:53.000000 sageworks-0.6.9/docs/core_classes/transforms/transform.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.520487 sageworks-0.6.9/docs/enterprise/
+-rw-r--r--   0 briford    (501) staff       (20)     4075 2024-05-20 20:55:48.000000 sageworks-0.6.9/docs/enterprise/index.md
+-rw-r--r--   0 briford    (501) staff       (20)      786 2024-04-28 17:52:09.000000 sageworks-0.6.9/docs/enterprise/project_branding.md
+-rw-r--r--   0 briford    (501) staff       (20)      892 2024-04-28 18:00:11.000000 sageworks-0.6.9/docs/enterprise/themes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.520812 sageworks-0.6.9/docs/getting_started/
+-rw-r--r--   0 briford    (501) staff       (20)     1975 2024-05-09 14:38:45.000000 sageworks-0.6.9/docs/getting_started/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.521041 sageworks-0.6.9/docs/glue/
+-rw-r--r--   0 briford    (501) staff       (20)     4837 2024-03-28 17:23:43.000000 sageworks-0.6.9/docs/glue/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.529404 sageworks-0.6.9/docs/images/
+-rw-r--r--   0 briford    (501) staff       (20)   605827 2023-12-24 17:18:24.000000 sageworks-0.6.9/docs/images/big_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)    32320 2023-12-24 17:18:24.000000 sageworks-0.6.9/docs/images/graph_representation.png
+-rw-r--r--   0 briford    (501) staff       (20)    15549 2023-12-24 17:18:24.000000 sageworks-0.6.9/docs/images/powered_aws_dark_blue.png
+-rw-r--r--   0 briford    (501) staff       (20)    10003 2023-12-24 17:18:24.000000 sageworks-0.6.9/docs/images/powered_aws_transparent.png
+-rw-r--r--   0 briford    (501) staff       (20)     6435 2023-12-24 17:18:24.000000 sageworks-0.6.9/docs/images/powered_aws_white.png
+-rw-r--r--   0 briford    (501) staff       (20)    21174 2023-12-24 17:18:24.000000 sageworks-0.6.9/docs/images/powered_aws_with_tm_grey.png
+-rw-r--r--   0 briford    (501) staff       (20)    51137 2023-12-24 17:18:24.000000 sageworks-0.6.9/docs/images/sageworks.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.9/docs/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)    30017 2023-12-24 17:18:24.000000 sageworks-0.6.9/docs/images/scp.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.9/docs/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)   381209 2023-12-24 17:18:24.000000 sageworks-0.6.9/docs/images/small_spider.png
+-rw-r--r--   0 briford    (501) staff       (20)     3443 2024-05-09 14:20:27.000000 sageworks-0.6.9/docs/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.531115 sageworks-0.6.9/docs/misc/
+-rw-r--r--   0 briford    (501) staff       (20)     2791 2024-03-28 17:23:43.000000 sageworks-0.6.9/docs/misc/faq.md
+-rw-r--r--   0 briford    (501) staff       (20)     5069 2024-01-10 18:45:51.000000 sageworks-0.6.9/docs/misc/general_info.md
+-rw-r--r--   0 briford    (501) staff       (20)      667 2024-01-10 18:45:51.000000 sageworks-0.6.9/docs/misc/sageworks_classes_concepts.md
+-rw-r--r--   0 briford    (501) staff       (20)     1873 2024-01-10 18:45:51.000000 sageworks-0.6.9/docs/misc/scp_consulting.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.531634 sageworks-0.6.9/docs/plugins/
+-rw-r--r--   0 briford    (501) staff       (20)     3361 2024-04-16 15:58:18.000000 sageworks-0.6.9/docs/plugins/index.md
+-rw-r--r--   0 briford    (501) staff       (20)      750 2024-04-06 16:51:44.000000 sageworks-0.6.9/docs/plugins/plugin_api_changes.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.531871 sageworks-0.6.9/docs/repl/
+-rw-r--r--   0 briford    (501) staff       (20)     2080 2024-05-09 14:40:59.000000 sageworks-0.6.9/docs/repl/index.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.532117 sageworks-0.6.9/examples/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.532352 sageworks-0.6.9/examples/ag-grid/
+-rw-r--r--   0 briford    (501) staff       (20)      496 2024-04-06 16:51:44.000000 sageworks-0.6.9/examples/ag-grid/hello_world.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.533548 sageworks-0.6.9/examples/datasource/
+-rw-r--r--   0 briford    (501) staff       (20)      326 2024-01-10 18:45:51.000000 sageworks-0.6.9/examples/datasource/datasource_from_df.py
+-rw-r--r--   0 briford    (501) staff       (20)      332 2024-01-10 18:45:51.000000 sageworks-0.6.9/examples/datasource/datasource_from_s3.py
+-rw-r--r--   0 briford    (501) staff       (20)      536 2024-01-23 15:36:53.000000 sageworks-0.6.9/examples/datasource/datasource_query.py
+-rw-r--r--   0 briford    (501) staff       (20)      680 2024-01-23 15:36:53.000000 sageworks-0.6.9/examples/datasource/datasource_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)      223 2024-01-10 18:45:51.000000 sageworks-0.6.9/examples/datasource/datasource_to_featureset.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.534068 sageworks-0.6.9/examples/endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)      199 2024-01-10 18:45:51.000000 sageworks-0.6.9/examples/endpoint/endpoint_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      834 2024-05-28 20:18:51.000000 sageworks-0.6.9/examples/endpoint/endpoint_inference.py
+-rw-r--r--   0 briford    (501) staff       (20)      481 2024-01-10 18:45:51.000000 sageworks-0.6.9/examples/endpoint/endpoint_metrics.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.534590 sageworks-0.6.9/examples/featureset/
+-rw-r--r--   0 briford    (501) staff       (20)      744 2024-01-10 18:45:51.000000 sageworks-0.6.9/examples/featureset/featureset_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)      560 2024-03-28 17:23:43.000000 sageworks-0.6.9/examples/featureset/featureset_query.py
+-rw-r--r--   0 briford    (501) staff       (20)      421 2024-03-27 20:32:26.000000 sageworks-0.6.9/examples/featureset/featureset_to_model.py
+-rw-r--r--   0 briford    (501) staff       (20)     1534 2024-05-28 20:18:51.000000 sageworks-0.6.9/examples/full_ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.535320 sageworks-0.6.9/examples/glue/
+-rw-r--r--   0 briford    (501) staff       (20)      580 2024-01-23 15:36:53.000000 sageworks-0.6.9/examples/glue/glue_hello_world.py
+-rw-r--r--   0 briford    (501) staff       (20)      942 2024-01-23 15:36:53.000000 sageworks-0.6.9/examples/glue/glue_hello_world_with_log.py
+-rw-r--r--   0 briford    (501) staff       (20)      686 2024-01-23 15:36:53.000000 sageworks-0.6.9/examples/glue/glue_load_s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.535885 sageworks-0.6.9/examples/meta/
+-rw-r--r--   0 briford    (501) staff       (20)      363 2024-04-06 16:51:44.000000 sageworks-0.6.9/examples/meta/meta_list_endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      328 2024-04-06 16:51:44.000000 sageworks-0.6.9/examples/meta/meta_list_models.py
+-rw-r--r--   0 briford    (501) staff       (20)      659 2024-04-06 16:51:44.000000 sageworks-0.6.9/examples/meta/meta_model_metrics.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.536447 sageworks-0.6.9/examples/model/
+-rw-r--r--   0 briford    (501) staff       (20)      564 2024-05-29 18:44:03.000000 sageworks-0.6.9/examples/model/model_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)      312 2024-03-27 20:32:26.000000 sageworks-0.6.9/examples/model/model_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)      705 2024-05-08 21:58:54.000000 sageworks-0.6.9/examples/model/onboard_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.536820 sageworks-0.6.9/examples/monitor/
+-rw-r--r--   0 briford    (501) staff       (20)      400 2024-01-10 18:45:51.000000 sageworks-0.6.9/examples/monitor/monitor_setup.py
+-rw-r--r--   0 briford    (501) staff       (20)      765 2024-01-10 18:45:51.000000 sageworks-0.6.9/examples/monitor/monitor_usage.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.538295 sageworks-0.6.9/examples/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     1000 2024-04-19 14:53:32.000000 sageworks-0.6.9/examples/pipelines/abalone_pipeline_v1.json
+-rw-r--r--   0 briford    (501) staff       (20)     1073 2024-04-19 19:42:10.000000 sageworks-0.6.9/examples/pipelines/abalone_pipeline_v2.json
+-rw-r--r--   0 briford    (501) staff       (20)     4435 2024-04-20 17:35:29.000000 sageworks-0.6.9/examples/pipelines/aqsol_pipeline_v1.json
+-rw-r--r--   0 briford    (501) staff       (20)      142 2024-04-19 14:55:38.000000 sageworks-0.6.9/examples/pipelines/pipeline_details.py
+-rw-r--r--   0 briford    (501) staff       (20)      324 2024-04-19 14:55:38.000000 sageworks-0.6.9/examples/pipelines/pipeline_execute.py
+-rw-r--r--   0 briford    (501) staff       (20)      556 2024-04-19 14:51:51.000000 sageworks-0.6.9/examples/pipelines/pipeline_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.482943 sageworks-0.6.9/examples/plugins/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.539239 sageworks-0.6.9/examples/plugins/pages/
+-rw-r--r--   0 briford    (501) staff       (20)     2467 2024-04-09 15:13:19.000000 sageworks-0.6.9/examples/plugins/pages/my_plugin_page.py
+-rw-r--r--   0 briford    (501) staff       (20)     1635 2024-04-16 15:58:18.000000 sageworks-0.6.9/examples/plugins/pages/plugin_page_1.py
+-rw-r--r--   0 briford    (501) staff       (20)     2464 2024-04-16 15:58:18.000000 sageworks-0.6.9/examples/plugins/pages/plugin_page_2.py
+-rw-r--r--   0 briford    (501) staff       (20)     5810 2024-05-27 22:25:50.000000 sageworks-0.6.9/examples/plugins/pages/plugin_page_3.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.539597 sageworks-0.6.9/examples/plugins/views/
+-rw-r--r--   0 briford    (501) staff       (20)     1588 2024-04-06 16:51:44.000000 sageworks-0.6.9/examples/plugins/views/model_plugin_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1264 2024-04-06 16:51:44.000000 sageworks-0.6.9/examples/plugins/views/my_view_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.540295 sageworks-0.6.9/examples/plugins/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     1733 2024-04-16 15:58:18.000000 sageworks-0.6.9/examples/plugins/web_components/custom_plugin.py
+-rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-16 15:58:18.000000 sageworks-0.6.9/examples/plugins/web_components/endpoint_plugin.py
+-rw-r--r--   0 briford    (501) staff       (20)     3660 2024-04-16 15:58:18.000000 sageworks-0.6.9/examples/plugins/web_components/endpoint_turbo.py
+-rw-r--r--   0 briford    (501) staff       (20)     2596 2024-04-16 15:58:18.000000 sageworks-0.6.9/examples/plugins/web_components/model_markdown.py
+-rw-r--r--   0 briford    (501) staff       (20)     2238 2024-04-16 15:58:18.000000 sageworks-0.6.9/examples/plugins/web_components/model_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.541380 sageworks-0.6.9/examples/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     1222 2024-03-27 20:40:53.000000 sageworks-0.6.9/examples/storage/data_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)      856 2024-03-27 20:40:53.000000 sageworks-0.6.9/examples/storage/data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1371 2024-05-28 20:18:51.000000 sageworks-0.6.9/examples/storage/endpoint_inference.py
+-rw-r--r--   0 briford    (501) staff       (20)     1847 2024-03-28 17:23:43.000000 sageworks-0.6.9/examples/storage/hello_world_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)     4380 2024-04-16 15:58:18.000000 sageworks-0.6.9/examples/storage/plugin_page_example.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.542067 sageworks-0.6.9/examples/storage/sagemaker_pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.9/examples/storage/sagemaker_pipelines/all_steps.py
+-rw-r--r--   0 briford    (501) staff       (20)       40 2024-03-28 17:23:43.000000 sageworks-0.6.9/examples/storage/sagemaker_pipelines/hello.py
+-rw-r--r--   0 briford    (501) staff       (20)     1487 2024-03-28 17:23:43.000000 sageworks-0.6.9/examples/storage/sagemaker_pipelines/ml_pipeline.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.483202 sageworks-0.6.9/examples/storage/sagemaker_pipelines/storage/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.542797 sageworks-0.6.9/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/
+-rw-r--r--   0 briford    (501) staff       (20)      854 2024-03-28 17:23:43.000000 sageworks-0.6.9/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)      203 2024-03-28 17:23:43.000000 sageworks-0.6.9/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)      160 2024-03-28 17:23:43.000000 sageworks-0.6.9/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/feature_set.py
+-rw-r--r--   0 briford    (501) staff       (20)     1599 2024-03-28 17:23:43.000000 sageworks-0.6.9/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)      367 2024-03-28 17:23:43.000000 sageworks-0.6.9/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/model.py
+-rw-r--r--   0 briford    (501) staff       (20)     3285 2024-05-24 14:48:45.000000 sageworks-0.6.9/mkdocs.yml
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.543784 sageworks-0.6.9/notebooks/
+-rw-r--r--   0 briford    (501) staff       (20)    17688 2024-05-31 21:50:47.000000 sageworks-0.6.9/notebooks/ML_Pipeline_with_SageWorks.ipynb
+-rw-r--r--   0 briford    (501) staff       (20)    16418 2024-05-31 21:50:47.000000 sageworks-0.6.9/notebooks/ML_Pipeline_with_SageWorks_2.ipynb
+-rw-r--r--   0 briford    (501) staff       (20)    12554 2024-05-30 23:29:04.000000 sageworks-0.6.9/notebooks/Outliers_in_SageWorks.ipynb
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.547853 sageworks-0.6.9/notebooks/images/
+-rw-r--r--   0 briford    (501) staff       (20)   142099 2023-12-24 17:18:24.000000 sageworks-0.6.9/notebooks/images/athena_query_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   191022 2023-12-24 17:18:24.000000 sageworks-0.6.9/notebooks/images/aws_dashboard_aqsol.png
+-rw-r--r--   0 briford    (501) staff       (20)   222686 2023-12-24 17:18:24.000000 sageworks-0.6.9/notebooks/images/dashboard_aqsol_features.png
+-rw-r--r--   0 briford    (501) staff       (20)   171441 2023-12-24 17:18:24.000000 sageworks-0.6.9/notebooks/images/model_screenshot.png
+-rw-r--r--   0 briford    (501) staff       (20)   489672 2023-12-24 17:18:24.000000 sageworks-0.6.9/notebooks/images/sageworks_concepts.png
+-rw-r--r--   0 briford    (501) staff       (20)   139307 2023-12-24 17:18:24.000000 sageworks-0.6.9/notebooks/images/scp_labs.png
+-rw-r--r--   0 briford    (501) staff       (20)      196 2024-05-30 17:04:13.000000 sageworks-0.6.9/pyproject.toml
+-rw-r--r--   0 briford    (501) staff       (20)      425 2024-05-30 17:39:59.000000 sageworks-0.6.9/requirements.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.550449 sageworks-0.6.9/scripts/
+-rw-r--r--   0 briford    (501) staff       (20)     1710 2024-04-16 15:58:18.000000 sageworks-0.6.9/scripts/ag_table_row_selection.py
+-rw-r--r--   0 briford    (501) staff       (20)     2290 2024-03-28 17:23:43.000000 sageworks-0.6.9/scripts/athena_ddl_mixed_case.py
+-rw-r--r--   0 briford    (501) staff       (20)     2178 2024-03-27 20:32:26.000000 sageworks-0.6.9/scripts/copy_data_catalog_db.py
+-rw-r--r--   0 briford    (501) staff       (20)     1222 2024-04-16 15:58:18.000000 sageworks-0.6.9/scripts/create_glue_workflow_with_trigger.py
+-rw-r--r--   0 briford    (501) staff       (20)      706 2024-01-10 18:45:51.000000 sageworks-0.6.9/scripts/delete_redis_keys.py
+-rw-r--r--   0 briford    (501) staff       (20)     1761 2024-03-28 17:23:43.000000 sageworks-0.6.9/scripts/glue_mixed_case.py
+-rw-r--r--   0 briford    (501) staff       (20)     5544 2024-03-28 17:23:43.000000 sageworks-0.6.9/scripts/model_endpoint_sanity_check.py
+-rw-r--r--   0 briford    (501) staff       (20)      715 2024-03-28 17:23:43.000000 sageworks-0.6.9/scripts/onboard_endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      694 2024-03-28 17:23:43.000000 sageworks-0.6.9/scripts/onboard_models.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.550831 sageworks-0.6.9/scripts/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     1003 2024-03-27 20:32:27.000000 sageworks-0.6.9/scripts/storage/dns_data_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     1723 2024-04-06 16:51:44.000000 sageworks-0.6.9/scripts/storage/generate_jsonl_data.py
+-rw-r--r--   0 briford    (501) staff       (20)      955 2024-03-28 17:23:43.000000 sageworks-0.6.9/scripts/test_feature_resolution.py
+-rw-r--r--   0 briford    (501) staff       (20)      427 2024-05-31 23:16:54.614441 sageworks-0.6.9/setup.cfg
+-rw-r--r--   0 briford    (501) staff       (20)     1657 2024-05-30 17:21:02.000000 sageworks-0.6.9/setup.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.483656 sageworks-0.6.9/src/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.551058 sageworks-0.6.9/src/sageworks/
+-rw-r--r--   0 briford    (501) staff       (20)     1091 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.552003 sageworks-0.6.9/src/sageworks/algorithms/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.9/src/sageworks/algorithms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.554006 sageworks-0.6.9/src/sageworks/algorithms/dataframe/
+-rw-r--r--   0 briford    (501) staff       (20)      378 2023-12-24 17:18:24.000000 sageworks-0.6.9/src/sageworks/algorithms/dataframe/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     2852 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/algorithms/dataframe/aggregation.py
+-rw-r--r--   0 briford    (501) staff       (20)     1606 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/algorithms/dataframe/data_source_eda.py
+-rw-r--r--   0 briford    (501) staff       (20)     5388 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/algorithms/dataframe/dimensionality_reduction.py
+-rw-r--r--   0 briford    (501) staff       (20)     9406 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/algorithms/dataframe/feature_resolution.py
+-rw-r--r--   0 briford    (501) staff       (20)    12309 2024-05-28 20:18:51.000000 sageworks-0.6.9/src/sageworks/algorithms/dataframe/feature_spider.py
+-rw-r--r--   0 briford    (501) staff       (20)     4968 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/algorithms/dataframe/row_tagger.py
+-rw-r--r--   0 briford    (501) staff       (20)     4628 2024-03-27 20:32:27.000000 sageworks-0.6.9/src/sageworks/algorithms/dataframe/target_gradients.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.483979 sageworks-0.6.9/src/sageworks/algorithms/graph/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.554354 sageworks-0.6.9/src/sageworks/algorithms/graph/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)       96 2023-12-24 17:18:24.000000 sageworks-0.6.9/src/sageworks/algorithms/graph/heavy/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.554581 sageworks-0.6.9/src/sageworks/algorithms/graph/light/
+-rw-r--r--   0 briford    (501) staff       (20)      122 2023-12-24 17:18:24.000000 sageworks-0.6.9/src/sageworks/algorithms/graph/light/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.554778 sageworks-0.6.9/src/sageworks/algorithms/spark/
+-rw-r--r--   0 briford    (501) staff       (20)      615 2023-12-24 17:18:24.000000 sageworks-0.6.9/src/sageworks/algorithms/spark/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.556344 sageworks-0.6.9/src/sageworks/algorithms/sql/
+-rw-r--r--   0 briford    (501) staff       (20)      685 2023-12-24 17:18:24.000000 sageworks-0.6.9/src/sageworks/algorithms/sql/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)     6221 2024-05-30 15:14:43.000000 sageworks-0.6.9/src/sageworks/algorithms/sql/column_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)     3666 2024-05-30 14:49:00.000000 sageworks-0.6.9/src/sageworks/algorithms/sql/correlations.py
+-rw-r--r--   0 briford    (501) staff       (20)     4045 2024-05-30 15:05:13.000000 sageworks-0.6.9/src/sageworks/algorithms/sql/descriptive_stats.py
+-rw-r--r--   0 briford    (501) staff       (20)    10377 2024-05-30 16:34:27.000000 sageworks-0.6.9/src/sageworks/algorithms/sql/outliers.py
+-rw-r--r--   0 briford    (501) staff       (20)     2352 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/algorithms/sql/sample_rows.py
+-rw-r--r--   0 briford    (501) staff       (20)     3466 2024-05-30 14:49:00.000000 sageworks-0.6.9/src/sageworks/algorithms/sql/value_counts.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.558635 sageworks-0.6.9/src/sageworks/api/
+-rw-r--r--   0 briford    (501) staff       (20)      708 2024-04-18 20:46:23.000000 sageworks-0.6.9/src/sageworks/api/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     7811 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/api/data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2634 2024-05-29 14:06:46.000000 sageworks-0.6.9/src/sageworks/api/endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     4224 2024-05-28 21:46:10.000000 sageworks-0.6.9/src/sageworks/api/feature_set.py
+-rw-r--r--   0 briford    (501) staff       (20)    16482 2024-04-21 15:28:58.000000 sageworks-0.6.9/src/sageworks/api/meta.py
+-rw-r--r--   0 briford    (501) staff       (20)     2595 2024-04-16 15:58:18.000000 sageworks-0.6.9/src/sageworks/api/model.py
+-rw-r--r--   0 briford    (501) staff       (20)     5261 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/api/monitor.py
+-rw-r--r--   0 briford    (501) staff       (20)     6953 2024-04-26 21:22:37.000000 sageworks-0.6.9/src/sageworks/api/pipeline.py
+-rw-r--r--   0 briford    (501) staff       (20)     6659 2024-04-26 21:22:37.000000 sageworks-0.6.9/src/sageworks/api/pipeline_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.559384 sageworks-0.6.9/src/sageworks/aws_service_broker/
+-rw-r--r--   0 briford    (501) staff       (20)     9393 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/aws_service_broker/aws_account_clamp.py
+-rw-r--r--   0 briford    (501) staff       (20)    11198 2024-05-09 14:32:45.000000 sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_broker.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.560864 sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_connectors/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_connectors/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     1834 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_connectors/connector.py
+-rw-r--r--   0 briford    (501) staff       (20)     3258 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)     4055 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)     5238 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)     3712 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)     3889 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     3736 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.560997 sageworks-0.6.9/src/sageworks/core/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.563681 sageworks-0.6.9/src/sageworks/core/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)      941 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/artifacts/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    17938 2024-04-15 22:06:08.000000 sageworks-0.6.9/src/sageworks/core/artifacts/artifact.py
+-rw-r--r--   0 briford    (501) staff       (20)    22432 2024-04-06 16:51:44.000000 sageworks-0.6.9/src/sageworks/core/artifacts/athena_source.py
+-rw-r--r--   0 briford    (501) staff       (20)    12683 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/artifacts/data_source_abstract.py
+-rw-r--r--   0 briford    (501) staff       (20)     2447 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/artifacts/data_source_factory.py
+-rw-r--r--   0 briford    (501) staff       (20)    37061 2024-05-29 13:52:08.000000 sageworks-0.6.9/src/sageworks/core/artifacts/endpoint_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    29821 2024-05-31 19:52:45.000000 sageworks-0.6.9/src/sageworks/core/artifacts/feature_set_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    36884 2024-05-31 20:59:08.000000 sageworks-0.6.9/src/sageworks/core/artifacts/model_core.py
+-rw-r--r--   0 briford    (501) staff       (20)    21029 2024-05-28 20:40:35.000000 sageworks-0.6.9/src/sageworks/core/artifacts/monitor_core.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.564165 sageworks-0.6.9/src/sageworks/core/pipelines/
+-rw-r--r--   0 briford    (501) staff       (20)     6919 2024-04-26 21:22:37.000000 sageworks-0.6.9/src/sageworks/core/pipelines/pipeline_executor.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.564808 sageworks-0.6.9/src/sageworks/core/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)     1432 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/Readme.md
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.565197 sageworks-0.6.9/src/sageworks/core/transforms/data_loaders/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_loaders/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.565565 sageworks-0.6.9/src/sageworks/core/transforms/data_loaders/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)      298 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_loaders/heavy/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     9866 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.566462 sageworks-0.6.9/src/sageworks/core/transforms/data_loaders/light/
+-rw-r--r--   0 briford    (501) staff       (20)      543 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_loaders/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3011 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     2927 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py
+-rw-r--r--   0 briford    (501) staff       (20)     4225 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.566720 sageworks-0.6.9/src/sageworks/core/transforms/data_to_data/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_data/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.566819 sageworks-0.6.9/src/sageworks/core/transforms/data_to_data/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_data/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.566919 sageworks-0.6.9/src/sageworks/core/transforms/data_to_data/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_data/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.567187 sageworks-0.6.9/src/sageworks/core/transforms/data_to_data/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_data/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.567771 sageworks-0.6.9/src/sageworks/core/transforms/data_to_data/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_data/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     2237 2024-03-27 20:40:53.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_data/light/clean_data.py
+-rw-r--r--   0 briford    (501) staff       (20)     2687 2024-03-27 20:40:53.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.568010 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.568128 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/heavy/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/heavy/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.568340 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/heavy/chunk/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/heavy/chunk/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     4551 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.568644 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.568805 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.568974 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/heavy/storage/
+-rw-r--r--   0 briford    (501) staff       (20)     6702 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.569526 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/light/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/light/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3827 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py
+-rw-r--r--   0 briford    (501) staff       (20)     5674 2024-04-23 15:16:38.000000 sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.569807 sageworks-0.6.9/src/sageworks/core/transforms/features_to_features/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/features_to_features/__init__.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.485912 sageworks-0.6.9/src/sageworks/core/transforms/features_to_features/heavy/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.569913 sageworks-0.6.9/src/sageworks/core/transforms/features_to_features/heavy/emr/
+-rw-r--r--   0 briford    (501) staff       (20)       68 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/features_to_features/heavy/emr/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.570075 sageworks-0.6.9/src/sageworks/core/transforms/features_to_features/heavy/glue/
+-rw-r--r--   0 briford    (501) staff       (20)       48 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/features_to_features/heavy/glue/Readme.md
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.570331 sageworks-0.6.9/src/sageworks/core/transforms/features_to_model/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/features_to_model/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    13103 2024-05-31 21:53:43.000000 sageworks-0.6.9/src/sageworks/core/transforms/features_to_model/features_to_model.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.571537 sageworks-0.6.9/src/sageworks/core/transforms/features_to_model/light_model_harness/
+-rw-r--r--   0 briford    (501) staff       (20)    13982 2024-05-28 20:18:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/features_to_model/light_model_harness/generated_xgb_model.py
+-rw-r--r--   0 briford    (501) staff       (20)       19 2024-02-27 23:40:48.000000 sageworks-0.6.9/src/sageworks/core/transforms/features_to_model/light_model_harness/requirements.txt
+-rw-r--r--   0 briford    (501) staff       (20)    10806 2024-05-28 20:18:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.571936 sageworks-0.6.9/src/sageworks/core/transforms/model_to_endpoint/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/core/transforms/model_to_endpoint/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     8185 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.573159 sageworks-0.6.9/src/sageworks/core/transforms/pandas_transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      894 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/transforms/pandas_transforms/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)     3615 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     3445 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py
+-rw-r--r--   0 briford    (501) staff       (20)     8604 2024-04-06 16:51:44.000000 sageworks-0.6.9/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py
+-rw-r--r--   0 briford    (501) staff       (20)    18139 2024-04-06 16:51:44.000000 sageworks-0.6.9/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py
+-rw-r--r--   0 briford    (501) staff       (20)     4440 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py
+-rw-r--r--   0 briford    (501) staff       (20)     5391 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/core/transforms/transform.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.573322 sageworks-0.6.9/src/sageworks/experiments/
+-rw-r--r--   0 briford    (501) staff       (20)    10658 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/experiments/view_manager.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.573705 sageworks-0.6.9/src/sageworks/repl/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/repl/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    15486 2024-04-21 15:35:25.000000 sageworks-0.6.9/src/sageworks/repl/sageworks_shell.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.574191 sageworks-0.6.9/src/sageworks/resources/
+-rw-r--r--   0 briford    (501) staff       (20)      361 2024-01-23 15:36:53.000000 sageworks-0.6.9/src/sageworks/resources/open_source_api.key
+-rw-r--r--   0 briford    (501) staff       (20)      272 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/resources/signature_verify_pub.pem
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.581156 sageworks-0.6.9/src/sageworks/utils/
+-rw-r--r--   0 briford    (501) staff       (20)        0 2023-12-24 17:18:24.000000 sageworks-0.6.9/src/sageworks/utils/__init__.py
+-rw-r--r--   0 briford    (501) staff       (20)    15584 2024-05-30 22:36:42.000000 sageworks-0.6.9/src/sageworks/utils/aws_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5447 2024-04-16 15:58:18.000000 sageworks-0.6.9/src/sageworks/utils/cache.py
+-rw-r--r--   0 briford    (501) staff       (20)      722 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/utils/chem_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    16543 2024-04-16 15:58:18.000000 sageworks-0.6.9/src/sageworks/utils/config_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     7392 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/utils/dashboard_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)     4194 2024-04-06 16:51:44.000000 sageworks-0.6.9/src/sageworks/utils/datetime_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     5292 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/utils/df_to_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     1681 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/utils/docker_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2866 2024-03-27 20:43:31.000000 sageworks-0.6.9/src/sageworks/utils/ecs_info.py
+-rw-r--r--   0 briford    (501) staff       (20)     7657 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/utils/endpoint_metrics.py
+-rw-r--r--   0 briford    (501) staff       (20)     3098 2024-05-28 20:18:49.000000 sageworks-0.6.9/src/sageworks/utils/endpoint_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     6979 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/utils/extract_model_artifact.py
+-rw-r--r--   0 briford    (501) staff       (20)     1131 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/utils/glue_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     6404 2024-05-20 15:33:17.000000 sageworks-0.6.9/src/sageworks/utils/license_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     1439 2024-04-06 16:51:44.000000 sageworks-0.6.9/src/sageworks/utils/markdown_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    15517 2024-04-22 20:45:19.000000 sageworks-0.6.9/src/sageworks/utils/pandas_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)    12684 2024-04-16 15:58:18.000000 sageworks-0.6.9/src/sageworks/utils/plugin_manager.py
+-rw-r--r--   0 briford    (501) staff       (20)     9533 2024-04-06 16:51:44.000000 sageworks-0.6.9/src/sageworks/utils/redis_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     4166 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/utils/repl_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2089 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/utils/s3_utils.py
+-rw-r--r--   0 briford    (501) staff       (20)     2163 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/utils/sageworks_cache.py
+-rw-r--r--   0 briford    (501) staff       (20)     3474 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/utils/sageworks_event_bridge.py
+-rw-r--r--   0 briford    (501) staff       (20)     5359 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/utils/sageworks_logging.py
+-rw-r--r--   0 briford    (501) staff       (20)     2120 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/utils/sageworks_sqs.py
+-rw-r--r--   0 briford    (501) staff       (20)     1108 2024-01-10 18:45:51.000000 sageworks-0.6.9/src/sageworks/utils/symbols.py
+-rw-r--r--   0 briford    (501) staff       (20)     6414 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/utils/test_data_generator.py
+-rw-r--r--   0 briford    (501) staff       (20)     2092 2024-03-27 20:43:31.000000 sageworks-0.6.9/src/sageworks/utils/trace_calls.py
+-rw-r--r--   0 briford    (501) staff       (20)     1470 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/utils/type_abbrev.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.582554 sageworks-0.6.9/src/sageworks/views/
+-rw-r--r--   0 briford    (501) staff       (20)     3517 2024-04-16 22:29:17.000000 sageworks-0.6.9/src/sageworks/views/artifacts_text_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     7780 2024-04-28 17:17:45.000000 sageworks-0.6.9/src/sageworks/views/artifacts_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3158 2024-04-06 16:51:44.000000 sageworks-0.6.9/src/sageworks/views/data_source_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2150 2024-04-06 16:51:44.000000 sageworks-0.6.9/src/sageworks/views/endpoint_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     3206 2024-04-06 16:51:44.000000 sageworks-0.6.9/src/sageworks/views/feature_set_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     2029 2024-04-06 16:51:44.000000 sageworks-0.6.9/src/sageworks/views/model_web_view.py
+-rw-r--r--   0 briford    (501) staff       (20)     1092 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/views/view.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.585266 sageworks-0.6.9/src/sageworks/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)     5916 2024-04-25 23:06:38.000000 sageworks-0.6.9/src/sageworks/web_components/component_interface.py
+-rw-r--r--   0 briford    (501) staff       (20)     3525 2024-04-16 15:58:18.000000 sageworks-0.6.9/src/sageworks/web_components/confusion_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     5854 2024-04-16 15:58:18.000000 sageworks-0.6.9/src/sageworks/web_components/correlation_matrix.py
+-rw-r--r--   0 briford    (501) staff       (20)     9328 2024-04-06 16:51:44.000000 sageworks-0.6.9/src/sageworks/web_components/data_details_markdown.py
+-rw-r--r--   0 briford    (501) staff       (20)     3068 2024-04-16 15:58:18.000000 sageworks-0.6.9/src/sageworks/web_components/endpoint_metric_plots.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.587664 sageworks-0.6.9/src/sageworks/web_components/experiments/
+-rw-r--r--   0 briford    (501) staff       (20)      837 2024-04-16 15:58:18.000000 sageworks-0.6.9/src/sageworks/web_components/experiments/color_maps.py
+-rw-r--r--   0 briford    (501) staff       (20)     1633 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/web_components/experiments/compound_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2974 2024-04-16 15:58:18.000000 sageworks-0.6.9/src/sageworks/web_components/experiments/dashboard_metric_plots.py
+-rw-r--r--   0 briford    (501) staff       (20)     2240 2024-04-16 15:58:18.000000 sageworks-0.6.9/src/sageworks/web_components/experiments/data_table.py
+-rw-r--r--   0 briford    (501) staff       (20)     2453 2024-04-02 16:53:34.000000 sageworks-0.6.9/src/sageworks/web_components/experiments/graph_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     1765 2024-04-02 16:53:34.000000 sageworks-0.6.9/src/sageworks/web_components/experiments/hello.py
+-rw-r--r--   0 briford    (501) staff       (20)     1183 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/web_components/experiments/histogram.py
+-rw-r--r--   0 briford    (501) staff       (20)      838 2024-04-16 15:58:18.000000 sageworks-0.6.9/src/sageworks/web_components/experiments/line_chart.py
+-rw-r--r--   0 briford    (501) staff       (20)     3680 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/web_components/experiments/outlier_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     2373 2024-04-16 15:58:18.000000 sageworks-0.6.9/src/sageworks/web_components/experiments/plugin_callbacks.py
+-rw-r--r--   0 briford    (501) staff       (20)     2279 2024-03-28 17:23:43.000000 sageworks-0.6.9/src/sageworks/web_components/experiments/scatter_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     2278 2024-04-16 15:58:18.000000 sageworks-0.6.9/src/sageworks/web_components/model_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     7681 2024-05-27 16:52:27.000000 sageworks-0.6.9/src/sageworks/web_components/plugin_interface.py
+-rw-r--r--   0 briford    (501) staff       (20)     3627 2024-05-27 19:18:14.000000 sageworks-0.6.9/src/sageworks/web_components/plugin_unit_test.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.588870 sageworks-0.6.9/src/sageworks/web_components/plugins/
+-rw-r--r--   0 briford    (501) staff       (20)     2786 2024-04-26 21:04:42.000000 sageworks-0.6.9/src/sageworks/web_components/plugins/ag_table.py
+-rw-r--r--   0 briford    (501) staff       (20)     3749 2024-05-28 15:15:12.000000 sageworks-0.6.9/src/sageworks/web_components/plugins/endpoint_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     5498 2024-05-22 14:54:18.000000 sageworks-0.6.9/src/sageworks/web_components/plugins/license_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     7607 2024-05-29 18:44:03.000000 sageworks-0.6.9/src/sageworks/web_components/plugins/model_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2429 2024-04-26 21:22:37.000000 sageworks-0.6.9/src/sageworks/web_components/plugins/pipeline_details.py
+-rw-r--r--   0 briford    (501) staff       (20)     2959 2024-05-29 15:29:46.000000 sageworks-0.6.9/src/sageworks/web_components/regression_plot.py
+-rw-r--r--   0 briford    (501) staff       (20)     6838 2024-05-06 17:24:24.000000 sageworks-0.6.9/src/sageworks/web_components/table.py
+-rw-r--r--   0 briford    (501) staff       (20)     5185 2024-04-16 15:58:18.000000 sageworks-0.6.9/src/sageworks/web_components/violin_plots.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.613501 sageworks-0.6.9/src/sageworks.egg-info/
+-rw-r--r--   0 briford    (501) staff       (20)     4927 2024-05-31 23:16:54.000000 sageworks-0.6.9/src/sageworks.egg-info/PKG-INFO
+-rw-r--r--   0 briford    (501) staff       (20)    19433 2024-05-31 23:16:54.000000 sageworks-0.6.9/src/sageworks.egg-info/SOURCES.txt
+-rw-r--r--   0 briford    (501) staff       (20)        1 2024-05-31 23:16:54.000000 sageworks-0.6.9/src/sageworks.egg-info/dependency_links.txt
+-rw-r--r--   0 briford    (501) staff       (20)       74 2024-05-31 23:16:54.000000 sageworks-0.6.9/src/sageworks.egg-info/entry_points.txt
+-rw-r--r--   0 briford    (501) staff       (20)      402 2024-05-31 23:16:54.000000 sageworks-0.6.9/src/sageworks.egg-info/requires.txt
+-rw-r--r--   0 briford    (501) staff       (20)       10 2024-05-31 23:16:54.000000 sageworks-0.6.9/src/sageworks.egg-info/top_level.txt
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.590189 sageworks-0.6.9/tests/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.591073 sageworks-0.6.9/tests/artifacts/
+-rw-r--r--   0 briford    (501) staff       (20)     1548 2024-03-30 19:27:28.000000 sageworks-0.6.9/tests/artifacts/data_source_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     2442 2024-05-28 20:18:51.000000 sageworks-0.6.9/tests/artifacts/endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1160 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/artifacts/feature_set_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      805 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/artifacts/model_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.591465 sageworks-0.6.9/tests/aws_account/
+-rw-r--r--   0 briford    (501) staff       (20)      962 2023-12-24 17:18:24.000000 sageworks-0.6.9/tests/aws_account/aws_account_clamp_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      642 2023-12-24 17:18:24.000000 sageworks-0.6.9/tests/aws_account/aws_service_broker_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.605266 sageworks-0.6.9/tests/connectors/
+-rw-r--r--   0 briford    (501) staff       (20)      725 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/connectors/data_catalog.py
+-rw-r--r--   0 briford    (501) staff       (20)      737 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/connectors/endpoints.py
+-rw-r--r--   0 briford    (501) staff       (20)      702 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/connectors/feature_store.py
+-rw-r--r--   0 briford    (501) staff       (20)      644 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/connectors/glue_jobs.py
+-rw-r--r--   0 briford    (501) staff       (20)      799 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/connectors/model_registry.py
+-rw-r--r--   0 briford    (501) staff       (20)     1008 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/connectors/s3_bucket.py
+-rw-r--r--   0 briford    (501) staff       (20)     5618 2024-04-26 21:04:42.000000 sageworks-0.6.9/tests/create_aqsol_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     3217 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/create_basic_test_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)      870 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/create_realtime_endpoint.py
+-rw-r--r--   0 briford    (501) staff       (20)     2378 2024-04-22 20:46:36.000000 sageworks-0.6.9/tests/create_training_adjusted_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     2096 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/create_wine_artifacts.py
+-rw-r--r--   0 briford    (501) staff       (20)     4448 2024-04-16 15:58:18.000000 sageworks-0.6.9/tests/delete_test_artifacts.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.605451 sageworks-0.6.9/tests/plugin_tests/
+-rw-r--r--   0 briford    (501) staff       (20)     1885 2024-04-16 15:58:18.000000 sageworks-0.6.9/tests/plugin_tests/crashing_plugin.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.610171 sageworks-0.6.9/tests/specific/
+-rw-r--r--   0 briford    (501) staff       (20)      639 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/specific/capital_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1513 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/specific/deletion_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.611511 sageworks-0.6.9/tests/transforms/
+-rw-r--r--   0 briford    (501) staff       (20)      592 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/transforms/data_to_data_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     1025 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/transforms/data_to_features_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      773 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/transforms/features_to_model_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)     5134 2024-05-29 18:44:03.000000 sageworks-0.6.9/tests/transforms/model_metrics_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      795 2024-03-28 17:23:43.000000 sageworks-0.6.9/tests/transforms/model_to_endpoint_tests.py
+-rw-r--r--   0 briford    (501) staff       (20)      633 2024-03-27 20:40:53.000000 sageworks-0.6.9/tests/transforms/pandas_to_data_tests.py
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.612063 sageworks-0.6.9/tests/web_components/
+-rw-r--r--   0 briford    (501) staff       (20)      681 2024-04-16 15:58:18.000000 sageworks-0.6.9/tests/web_components/confusion_matrix_test.py
+-rw-r--r--   0 briford    (501) staff       (20)      677 2024-04-16 15:58:18.000000 sageworks-0.6.9/tests/web_components/correlation_matrix_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     5269 2024-04-16 15:58:18.000000 sageworks-0.6.9/tests/web_components/plugin_interface_test.py
+-rw-r--r--   0 briford    (501) staff       (20)     1112 2024-05-29 18:21:35.000000 sageworks-0.6.9/tox.ini
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.612915 sageworks-0.6.9/ui_testing/
+drwxr-xr-x   0 briford    (501) staff       (20)        0 2024-05-31 23:16:54.613130 sageworks-0.6.9/ui_testing/assets/
+-rw-r--r--   0 briford    (501) staff       (20)      597 2024-05-13 15:14:49.000000 sageworks-0.6.9/ui_testing/assets/custom.css
+-rw-r--r--   0 briford    (501) staff       (20)     5770 2024-05-19 19:25:10.000000 sageworks-0.6.9/ui_testing/table_comparison.py
+-rw-r--r--   0 briford    (501) staff       (20)     2025 2024-05-19 19:25:10.000000 sageworks-0.6.9/ui_testing/theme_switching.py
+-rw-r--r--   0 briford    (501) staff       (20)     1819 2024-05-19 19:25:10.000000 sageworks-0.6.9/ui_testing/theme_switching_2.py
```

### Comparing `sageworks-0.6.8/.github/PULL_REQUEST_TEMPLATE.md` & `sageworks-0.6.9/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/.github/workflows/deploy-docs.yml` & `sageworks-0.6.9/.github/workflows/deploy-docs.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/.github/workflows/python-lint.yml` & `sageworks-0.6.9/.github/workflows/python-lint.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/.gitignore` & `sageworks-0.6.9/.gitignore`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/CONTRIBUTING.md` & `sageworks-0.6.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/LICENSE` & `sageworks-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/Makefile` & `sageworks-0.6.9/Makefile`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/PKG-INFO` & `sageworks-0.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.6.8
+Version: 0.6.9
 Summary: SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 4 - Beta
@@ -32,15 +32,14 @@
 Requires-Dist: shap>=0.43.0
 Requires-Dist: xgboost>=2.0.2
 Requires-Dist: joblib>=1.3.2
 Requires-Dist: cryptography>=42.0.5
 Requires-Dist: rdkit>=2023.9.1
 Requires-Dist: mordred>=1.2.0
 Requires-Dist: ipython>=8.17.2
-Requires-Dist: setuptools>=69.0.2
 Requires-Dist: pyreadline3; sys_platform == "win32"
 
 
 # Welcome to SageWorks
 The SageWorks framework makes AWS® both easier to use and more powerful. SageWorks handles all the details around updating and managing a complex set of AWS Services. With a simple-to-use Python API and a beautiful set of web interfaces, SageWorks makes creating AWS ML pipelines a snap. It also dramatically improves both the usability and visibility across the entire spectrum of services: Glue Job, Athena, Feature Store, Models, and Endpoints, SageWorks makes it easy to build production ready, AWS powered, machine learning pipelines.
 
 <img align="right" width="480" alt="sageworks_new_light" src="https://github.com/SuperCowPowers/sageworks/assets/4806709/ed2ed1bd-e2d8-49a1-b350-b2e19e2b7832">
```

### Comparing `sageworks-0.6.8/README.md` & `sageworks-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/Dockerfile` & `sageworks-0.6.9/applications/aws_dashboard/Dockerfile`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/README.md` & `sageworks-0.6.9/applications/aws_dashboard/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/app.py` & `sageworks-0.6.9/applications/aws_dashboard/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/assets/bootstrap_darkly.min.css` & `sageworks-0.6.9/applications/aws_dashboard/assets/bootstrap_darkly.min.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/assets/default.css` & `sageworks-0.6.9/applications/aws_dashboard/assets/default.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/assets/favicon.ico` & `sageworks-0.6.9/applications/aws_dashboard/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/assets/trash.png` & `sageworks-0.6.9/applications/aws_dashboard/assets/trash.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/dashboard` & `sageworks-0.6.9/applications/aws_dashboard/dashboard`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/open_source_config.json` & `sageworks-0.6.9/applications/aws_dashboard/open_source_config.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/data_sources/callbacks.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/data_sources/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/data_sources/layout.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/data_sources/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/data_sources/page.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/data_sources/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/endpoints/callbacks.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/endpoints/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/endpoints/layout.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/endpoints/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/endpoints/page.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/endpoints/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/feature_sets/callbacks.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/feature_sets/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/feature_sets/layout.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/feature_sets/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/feature_sets/page.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/feature_sets/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/license/page.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/license/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/main/callbacks.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/main/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/main/layout.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/main/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/main/page.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/main/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/models/callbacks.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/models/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/models/layout.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/models/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/models/page.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/models/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/pipelines/callbacks.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/pipelines/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/pipelines/layout.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/pipelines/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/aws_dashboard/pages/pipelines/page.py` & `sageworks-0.6.9/applications/aws_dashboard/pages/pipelines/page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/experiments/compound_explorer/app.py` & `sageworks-0.6.9/applications/experiments/compound_explorer/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/experiments/compound_explorer/assets/custom.css` & `sageworks-0.6.9/applications/experiments/compound_explorer/assets/custom.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/experiments/compound_explorer/callbacks.py` & `sageworks-0.6.9/applications/experiments/compound_explorer/callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/applications/experiments/compound_explorer/layout.py` & `sageworks-0.6.9/applications/experiments/compound_explorer/layout.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/aws_account_check.py` & `sageworks-0.6.9/aws_setup/aws_account_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/aws_identity_check.py` & `sageworks-0.6.9/aws_setup/aws_identity_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/build_ml_pipeline.py` & `sageworks-0.6.9/aws_setup/build_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/app.py` & `sageworks-0.6.9/aws_setup/event_bridge/dynamic_docker/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/cdk.json` & `sageworks-0.6.9/aws_setup/event_bridge/dynamic_docker/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py` & `sageworks-0.6.9/aws_setup/event_bridge/dynamic_docker/lambda/lambda_replace_task.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py` & `sageworks-0.6.9/aws_setup/event_bridge/dynamic_docker/sageworks_image_update_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/sageworks_core/README.md` & `sageworks-0.6.9/aws_setup/sageworks_core/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/sageworks_core/app.py` & `sageworks-0.6.9/aws_setup/sageworks_core/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/sageworks_core/cdk.json` & `sageworks-0.6.9/aws_setup/sageworks_core/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py` & `sageworks-0.6.9/aws_setup/sageworks_core/sageworks_core/sageworks_core_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py` & `sageworks-0.6.9/aws_setup/sageworks_core/tests/unit/test_sageworks_sandbox_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/sageworks_dashboard_full/README.md` & `sageworks-0.6.9/aws_setup/sageworks_dashboard_full/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/sageworks_dashboard_full/app.py` & `sageworks-0.6.9/aws_setup/sageworks_dashboard_full/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/sageworks_dashboard_full/cdk.json` & `sageworks-0.6.9/aws_setup/sageworks_dashboard_full/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py` & `sageworks-0.6.9/aws_setup/sageworks_dashboard_full/sageworks_dashboard_full/sageworks_dashboard_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py` & `sageworks-0.6.9/aws_setup/sageworks_dashboard_full/tests/unit/test_sageworks_dashboard_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/README.md` & `sageworks-0.6.9/aws_setup/sageworks_dashboard_lite/README.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/app.py` & `sageworks-0.6.9/aws_setup/sageworks_dashboard_lite/app.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/cdk.json` & `sageworks-0.6.9/aws_setup/sageworks_dashboard_lite/cdk.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py` & `sageworks-0.6.9/aws_setup/sageworks_dashboard_lite/sageworks_dashboard_lite/sageworks_dashboard_stack.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/data/abalone.csv` & `sageworks-0.6.9/data/abalone.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/data/test_data.csv` & `sageworks-0.6.9/data/test_data.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/data/test_data.json` & `sageworks-0.6.9/data/test_data.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/data/wine_dataset.csv` & `sageworks-0.6.9/data/wine_dataset.csv`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/admin/docker_push.md` & `sageworks-0.6.9/docs/admin/docker_push.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/admin/pypi_release.md` & `sageworks-0.6.9/docs/admin/pypi_release.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/api_classes/data_source.md` & `sageworks-0.6.9/docs/api_classes/data_source.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/api_classes/endpoint.md` & `sageworks-0.6.9/docs/api_classes/endpoint.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/api_classes/feature_set.md` & `sageworks-0.6.9/docs/api_classes/feature_set.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/api_classes/meta.md` & `sageworks-0.6.9/docs/api_classes/meta.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/api_classes/model.md` & `sageworks-0.6.9/docs/api_classes/model.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/api_classes/monitor.md` & `sageworks-0.6.9/docs/api_classes/monitor.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/api_classes/overview.md` & `sageworks-0.6.9/docs/api_classes/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/api_classes/pipelines.md` & `sageworks-0.6.9/docs/api_classes/pipelines.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/aws_setup/aws_access_management.md` & `sageworks-0.6.9/docs/aws_setup/aws_access_management.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/aws_setup/aws_tips_and_tricks.md` & `sageworks-0.6.9/docs/aws_setup/aws_tips_and_tricks.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/aws_setup/core_stack.md` & `sageworks-0.6.9/docs/aws_setup/core_stack.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/aws_setup/dashboard_stack.md` & `sageworks-0.6.9/docs/aws_setup/dashboard_stack.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/aws_setup/domain_cert_setup.md` & `sageworks-0.6.9/docs/aws_setup/domain_cert_setup.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/aws_setup/full_pipeline.md` & `sageworks-0.6.9/docs/aws_setup/full_pipeline.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/aws_setup/sso_setup.md` & `sageworks-0.6.9/docs/aws_setup/sso_setup.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/blogs_research/eda.md` & `sageworks-0.6.9/docs/blogs_research/eda.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/blogs_research/htg.md` & `sageworks-0.6.9/docs/blogs_research/htg.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/blogs_research/index.md` & `sageworks-0.6.9/docs/blogs_research/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/blogs_research/residual_analysis.md` & `sageworks-0.6.9/docs/blogs_research/residual_analysis.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/concepts/model_monitoring.md` & `sageworks-0.6.9/docs/concepts/model_monitoring.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/core_classes/artifacts/overview.md` & `sageworks-0.6.9/docs/core_classes/artifacts/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/core_classes/overview.md` & `sageworks-0.6.9/docs/core_classes/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/core_classes/transforms/overview.md` & `sageworks-0.6.9/docs/core_classes/transforms/overview.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/core_classes/transforms/pandas_transforms.md` & `sageworks-0.6.9/docs/core_classes/transforms/pandas_transforms.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/core_classes/transforms/transform.md` & `sageworks-0.6.9/docs/core_classes/transforms/transform.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/enterprise/index.md` & `sageworks-0.6.9/docs/enterprise/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/enterprise/project_branding.md` & `sageworks-0.6.9/docs/enterprise/project_branding.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/enterprise/themes.md` & `sageworks-0.6.9/docs/enterprise/themes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/getting_started/index.md` & `sageworks-0.6.9/docs/getting_started/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/glue/index.md` & `sageworks-0.6.9/docs/glue/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/images/big_spider.png` & `sageworks-0.6.9/docs/images/big_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/images/graph_representation.png` & `sageworks-0.6.9/docs/images/graph_representation.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/images/powered_aws_dark_blue.png` & `sageworks-0.6.9/docs/images/powered_aws_dark_blue.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/images/powered_aws_transparent.png` & `sageworks-0.6.9/docs/images/powered_aws_transparent.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/images/powered_aws_white.png` & `sageworks-0.6.9/docs/images/powered_aws_white.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/images/powered_aws_with_tm_grey.png` & `sageworks-0.6.9/docs/images/powered_aws_with_tm_grey.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/images/sageworks.png` & `sageworks-0.6.9/docs/images/sageworks.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/images/sageworks_concepts.png` & `sageworks-0.6.9/docs/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/images/scp.png` & `sageworks-0.6.9/docs/images/scp.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/images/scp_labs.png` & `sageworks-0.6.9/docs/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/images/small_spider.png` & `sageworks-0.6.9/docs/images/small_spider.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/index.md` & `sageworks-0.6.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/misc/faq.md` & `sageworks-0.6.9/docs/misc/faq.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/misc/general_info.md` & `sageworks-0.6.9/docs/misc/general_info.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/misc/sageworks_classes_concepts.md` & `sageworks-0.6.9/docs/misc/sageworks_classes_concepts.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/misc/scp_consulting.md` & `sageworks-0.6.9/docs/misc/scp_consulting.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/plugins/index.md` & `sageworks-0.6.9/docs/plugins/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/plugins/plugin_api_changes.md` & `sageworks-0.6.9/docs/plugins/plugin_api_changes.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/docs/repl/index.md` & `sageworks-0.6.9/docs/repl/index.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/datasource/datasource_query.py` & `sageworks-0.6.9/examples/datasource/datasource_query.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/datasource/datasource_stats.py` & `sageworks-0.6.9/examples/datasource/datasource_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/endpoint/endpoint_inference.py` & `sageworks-0.6.9/examples/endpoint/endpoint_inference.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/featureset/featureset_eda.py` & `sageworks-0.6.9/examples/featureset/featureset_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/featureset/featureset_query.py` & `sageworks-0.6.9/examples/featureset/featureset_query.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/full_ml_pipeline.py` & `sageworks-0.6.9/examples/full_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/glue/glue_hello_world.py` & `sageworks-0.6.9/examples/glue/glue_hello_world.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/glue/glue_hello_world_with_log.py` & `sageworks-0.6.9/examples/glue/glue_hello_world_with_log.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/glue/glue_load_s3_bucket.py` & `sageworks-0.6.9/examples/glue/glue_load_s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/meta/meta_model_metrics.py` & `sageworks-0.6.9/examples/meta/meta_model_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/model/model_metrics.py` & `sageworks-0.6.9/examples/model/model_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/model/onboard_model.py` & `sageworks-0.6.9/examples/model/onboard_model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/monitor/monitor_usage.py` & `sageworks-0.6.9/examples/monitor/monitor_usage.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/pipelines/abalone_pipeline_v1.json` & `sageworks-0.6.9/examples/pipelines/abalone_pipeline_v1.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/pipelines/abalone_pipeline_v2.json` & `sageworks-0.6.9/examples/pipelines/abalone_pipeline_v2.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/pipelines/aqsol_pipeline_v1.json` & `sageworks-0.6.9/examples/pipelines/aqsol_pipeline_v1.json`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/pipelines/pipeline_manager.py` & `sageworks-0.6.9/examples/pipelines/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/plugins/pages/my_plugin_page.py` & `sageworks-0.6.9/examples/plugins/pages/my_plugin_page.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/plugins/pages/plugin_page_1.py` & `sageworks-0.6.9/examples/plugins/pages/plugin_page_1.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/plugins/pages/plugin_page_2.py` & `sageworks-0.6.9/examples/plugins/pages/plugin_page_2.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/plugins/pages/plugin_page_3.py` & `sageworks-0.6.9/examples/plugins/pages/plugin_page_3.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/plugins/views/model_plugin_view.py` & `sageworks-0.6.9/examples/plugins/views/model_plugin_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/plugins/views/my_view_plugin.py` & `sageworks-0.6.9/examples/plugins/views/my_view_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/plugins/web_components/custom_plugin.py` & `sageworks-0.6.9/examples/plugins/web_components/custom_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/plugins/web_components/endpoint_plugin.py` & `sageworks-0.6.9/examples/plugins/web_components/endpoint_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/plugins/web_components/endpoint_turbo.py` & `sageworks-0.6.9/examples/plugins/web_components/endpoint_turbo.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/plugins/web_components/model_markdown.py` & `sageworks-0.6.9/examples/plugins/web_components/model_markdown.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/plugins/web_components/model_plugin.py` & `sageworks-0.6.9/examples/plugins/web_components/model_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/storage/data_to_data.py` & `sageworks-0.6.9/examples/storage/data_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/storage/data_to_features.py` & `sageworks-0.6.9/examples/storage/data_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/storage/endpoint_inference.py` & `sageworks-0.6.9/examples/storage/endpoint_inference.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/storage/hello_world_pipeline.py` & `sageworks-0.6.9/examples/storage/hello_world_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/storage/plugin_page_example.py` & `sageworks-0.6.9/examples/storage/plugin_page_example.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/storage/sagemaker_pipelines/all_steps.py` & `sageworks-0.6.9/examples/storage/sagemaker_pipelines/all_steps.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/storage/sagemaker_pipelines/ml_pipeline.py` & `sageworks-0.6.9/examples/storage/sagemaker_pipelines/ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py` & `sageworks-0.6.9/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py` & `sageworks-0.6.9/examples/storage/sagemaker_pipelines/storage/full_pipeline_experiment/ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/mkdocs.yml` & `sageworks-0.6.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/notebooks/ML_Pipeline_with_SageWorks.ipynb` & `sageworks-0.6.9/notebooks/ML_Pipeline_with_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/notebooks/ML_Pipeline_with_SageWorks_2.ipynb` & `sageworks-0.6.9/notebooks/ML_Pipeline_with_SageWorks_2.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/notebooks/Outliers_in_SageWorks.ipynb` & `sageworks-0.6.9/notebooks/Outliers_in_SageWorks.ipynb`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/notebooks/images/athena_query_aqsol.png` & `sageworks-0.6.9/notebooks/images/athena_query_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/notebooks/images/aws_dashboard_aqsol.png` & `sageworks-0.6.9/notebooks/images/aws_dashboard_aqsol.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/notebooks/images/dashboard_aqsol_features.png` & `sageworks-0.6.9/notebooks/images/dashboard_aqsol_features.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/notebooks/images/model_screenshot.png` & `sageworks-0.6.9/notebooks/images/model_screenshot.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/notebooks/images/sageworks_concepts.png` & `sageworks-0.6.9/notebooks/images/sageworks_concepts.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/notebooks/images/scp_labs.png` & `sageworks-0.6.9/notebooks/images/scp_labs.png`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/scripts/ag_table_row_selection.py` & `sageworks-0.6.9/scripts/ag_table_row_selection.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/scripts/athena_ddl_mixed_case.py` & `sageworks-0.6.9/scripts/athena_ddl_mixed_case.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/scripts/copy_data_catalog_db.py` & `sageworks-0.6.9/scripts/copy_data_catalog_db.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/scripts/create_glue_workflow_with_trigger.py` & `sageworks-0.6.9/scripts/create_glue_workflow_with_trigger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/scripts/delete_redis_keys.py` & `sageworks-0.6.9/scripts/delete_redis_keys.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/scripts/glue_mixed_case.py` & `sageworks-0.6.9/scripts/glue_mixed_case.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/scripts/model_endpoint_sanity_check.py` & `sageworks-0.6.9/scripts/model_endpoint_sanity_check.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/scripts/onboard_endpoints.py` & `sageworks-0.6.9/scripts/onboard_endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/scripts/onboard_models.py` & `sageworks-0.6.9/scripts/onboard_models.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/scripts/storage/dns_data_to_features.py` & `sageworks-0.6.9/scripts/storage/dns_data_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/scripts/storage/generate_jsonl_data.py` & `sageworks-0.6.9/scripts/storage/generate_jsonl_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/scripts/test_feature_resolution.py` & `sageworks-0.6.9/scripts/test_feature_resolution.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/setup.py` & `sageworks-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/__init__.py` & `sageworks-0.6.9/src/sageworks/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/algorithms/dataframe/aggregation.py` & `sageworks-0.6.9/src/sageworks/algorithms/dataframe/aggregation.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/algorithms/dataframe/data_source_eda.py` & `sageworks-0.6.9/src/sageworks/algorithms/dataframe/data_source_eda.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/algorithms/dataframe/dimensionality_reduction.py` & `sageworks-0.6.9/src/sageworks/algorithms/dataframe/dimensionality_reduction.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/algorithms/dataframe/feature_resolution.py` & `sageworks-0.6.9/src/sageworks/algorithms/dataframe/feature_resolution.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/algorithms/dataframe/feature_spider.py` & `sageworks-0.6.9/src/sageworks/algorithms/dataframe/feature_spider.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/algorithms/dataframe/row_tagger.py` & `sageworks-0.6.9/src/sageworks/algorithms/dataframe/row_tagger.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/algorithms/dataframe/target_gradients.py` & `sageworks-0.6.9/src/sageworks/algorithms/dataframe/target_gradients.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/algorithms/spark/Readme.md` & `sageworks-0.6.9/src/sageworks/algorithms/spark/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/algorithms/sql/Readme.md` & `sageworks-0.6.9/src/sageworks/algorithms/sql/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/algorithms/sql/column_stats.py` & `sageworks-0.6.9/src/sageworks/algorithms/sql/column_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/algorithms/sql/correlations.py` & `sageworks-0.6.9/src/sageworks/algorithms/sql/correlations.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/algorithms/sql/descriptive_stats.py` & `sageworks-0.6.9/src/sageworks/algorithms/sql/descriptive_stats.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/algorithms/sql/outliers.py` & `sageworks-0.6.9/src/sageworks/algorithms/sql/outliers.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/algorithms/sql/sample_rows.py` & `sageworks-0.6.9/src/sageworks/algorithms/sql/sample_rows.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/algorithms/sql/value_counts.py` & `sageworks-0.6.9/src/sageworks/algorithms/sql/value_counts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/api/__init__.py` & `sageworks-0.6.9/src/sageworks/api/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/api/data_source.py` & `sageworks-0.6.9/src/sageworks/api/data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/api/endpoint.py` & `sageworks-0.6.9/src/sageworks/api/endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/api/feature_set.py` & `sageworks-0.6.9/src/sageworks/api/feature_set.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/api/meta.py` & `sageworks-0.6.9/src/sageworks/api/meta.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/api/model.py` & `sageworks-0.6.9/src/sageworks/api/model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/api/monitor.py` & `sageworks-0.6.9/src/sageworks/api/monitor.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/api/pipeline.py` & `sageworks-0.6.9/src/sageworks/api/pipeline.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/api/pipeline_manager.py` & `sageworks-0.6.9/src/sageworks/api/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_account_clamp.py` & `sageworks-0.6.9/src/sageworks/aws_service_broker/aws_account_clamp.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_broker.py` & `sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_broker.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/connector.py` & `sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_connectors/connector.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py` & `sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py` & `sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py` & `sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py` & `sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_connectors/glue_jobs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py` & `sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py` & `sageworks-0.6.9/src/sageworks/aws_service_broker/aws_service_connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/artifacts/__init__.py` & `sageworks-0.6.9/src/sageworks/core/artifacts/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/artifacts/artifact.py` & `sageworks-0.6.9/src/sageworks/core/artifacts/artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/artifacts/athena_source.py` & `sageworks-0.6.9/src/sageworks/core/artifacts/athena_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/artifacts/data_source_abstract.py` & `sageworks-0.6.9/src/sageworks/core/artifacts/data_source_abstract.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/artifacts/data_source_factory.py` & `sageworks-0.6.9/src/sageworks/core/artifacts/data_source_factory.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/artifacts/endpoint_core.py` & `sageworks-0.6.9/src/sageworks/core/artifacts/endpoint_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/artifacts/feature_set_core.py` & `sageworks-0.6.9/src/sageworks/core/artifacts/feature_set_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,14 +325,17 @@
         if cached_details and not recompute:
             return cached_details
 
         self.log.info(f"Recomputing FeatureSet Details ({self.uuid})...")
         details = self.summary()
         details["aws_url"] = self.aws_url()
 
+        # Store the AWS URL in the SageWorks Metadata
+        self.upsert_sageworks_meta({"aws_url": details["aws_url"]})
+
         # Now get a summary of the underlying DataSource
         details["storage_summary"] = self.data_source.summary()
 
         # Number of Columns
         details["num_columns"] = self.num_columns()
 
         # Number of Rows
```

### Comparing `sageworks-0.6.8/src/sageworks/core/artifacts/model_core.py` & `sageworks-0.6.9/src/sageworks/core/artifacts/model_core.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,14 +469,20 @@
         # Set the status to onboarding
         self.set_status("onboarding")
 
         # Determine the Model Type
         while self.is_model_unknown():
             self._determine_model_type()
 
+        # Is our input data set?
+        if self.get_input() in ["", "unknown"] or ask_everything:
+            input_data = input("Input Data?: ")
+            if input_data not in ["None", "none", "", "unknown"]:
+                self.set_input(input_data)
+
         # Determine the Target Column (can be None)
         target_column = self.target()
         if target_column is None or ask_everything:
             target_column = input("Target Column? (for unsupervised/transformer just type None): ")
             if target_column in ["None", "none", ""]:
                 target_column = None
 
@@ -834,15 +840,15 @@
 
     # Call the various methods
 
     # Let's do a check/validation of the Model
     print(f"Model Check: {my_model.exists()}")
 
     # Make sure the model is 'ready'
-    my_model.onboard(interactive=False)
+    my_model.onboard()
 
     # Get the ARN of the Model Group
     print(f"Model Group ARN: {my_model.group_arn()}")
     print(f"Model Package ARN: {my_model.arn()}")
 
     # Get the tags associated with this Model
     print(f"Tags: {my_model.get_tags()}")
```

### Comparing `sageworks-0.6.8/src/sageworks/core/artifacts/monitor_core.py` & `sageworks-0.6.9/src/sageworks/core/artifacts/monitor_core.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/pipelines/pipeline_executor.py` & `sageworks-0.6.9/src/sageworks/core/pipelines/pipeline_executor.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/Readme.md` & `sageworks-0.6.9/src/sageworks/core/transforms/Readme.md`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py` & `sageworks-0.6.9/src/sageworks/core/transforms/data_loaders/heavy/s3_heavy_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/__init__.py` & `sageworks-0.6.9/src/sageworks/core/transforms/data_loaders/light/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py` & `sageworks-0.6.9/src/sageworks/core/transforms/data_loaders/light/csv_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py` & `sageworks-0.6.9/src/sageworks/core/transforms/data_loaders/light/json_to_data_source.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py` & `sageworks-0.6.9/src/sageworks/core/transforms/data_loaders/light/s3_to_data_source_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/light/clean_data.py` & `sageworks-0.6.9/src/sageworks/core/transforms/data_to_data/light/clean_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py` & `sageworks-0.6.9/src/sageworks/core/transforms/data_to_data/light/data_to_data_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py` & `sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/heavy/chunk/data_to_features_chunk.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py` & `sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/heavy/storage/data_to_features_heavy_old.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py` & `sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/light/data_to_features_light.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py` & `sageworks-0.6.9/src/sageworks/core/transforms/data_to_features/light/molecular_descriptors.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/features_to_model.py` & `sageworks-0.6.9/src/sageworks/core/transforms/features_to_model/features_to_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -240,15 +240,15 @@
         output_model.upsert_sageworks_meta({"sageworks_model_target": self.target_column})
 
         # Store the class labels (if they exist)
         if self.class_labels:
             output_model.set_class_labels(self.class_labels)
 
         # Call the Model onboard method
-        output_model.onboard(interactive=False)
+        output_model.onboard_with_args(self.model_type, self.target_column, self.model_feature_list)
 
     def create_and_register_model(self):
         """Create and Register the Model"""
 
         # Get the metadata/tags to push into AWS
         aws_tags = self.get_aws_tags()
```

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/light_model_harness/generated_xgb_model.py` & `sageworks-0.6.9/src/sageworks/core/transforms/features_to_model/light_model_harness/generated_xgb_model.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template` & `sageworks-0.6.9/src/sageworks/core/transforms/features_to_model/light_model_harness/xgb_model.template`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py` & `sageworks-0.6.9/src/sageworks/core/transforms/model_to_endpoint/model_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/__init__.py` & `sageworks-0.6.9/src/sageworks/core/transforms/pandas_transforms/__init__.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py` & `sageworks-0.6.9/src/sageworks/core/transforms/pandas_transforms/data_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py` & `sageworks-0.6.9/src/sageworks/core/transforms/pandas_transforms/features_to_pandas.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py` & `sageworks-0.6.9/src/sageworks/core/transforms/pandas_transforms/pandas_to_data.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py` & `sageworks-0.6.9/src/sageworks/core/transforms/pandas_transforms/pandas_to_features.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py` & `sageworks-0.6.9/src/sageworks/core/transforms/pandas_transforms/pandas_to_features_chunked.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/core/transforms/transform.py` & `sageworks-0.6.9/src/sageworks/core/transforms/transform.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/experiments/view_manager.py` & `sageworks-0.6.9/src/sageworks/experiments/view_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/repl/sageworks_shell.py` & `sageworks-0.6.9/src/sageworks/repl/sageworks_shell.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/aws_utils.py` & `sageworks-0.6.9/src/sageworks/utils/aws_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
             aws_tags = sm_session.list_tags(arn)
             meta = _aws_tags_to_dict(aws_tags)  # Convert the AWS Tags to a dictionary
             return meta
 
         except botocore.exceptions.ClientError as e:
             error_code = e.response["Error"]["Code"]
             if error_code == "ThrottlingException":
-                log.warning(f"ThrottlingException: list_tags on {arn}")
+                log.info(f"ThrottlingException: list_tags on {arn}")
                 time.sleep(sleep_time)
                 sleep_time *= 2
             else:
                 # Handle other ClientErrors that may occur
                 log.error(f"Unexpected ClientError: {error_code}")
                 raise e
```

### Comparing `sageworks-0.6.8/src/sageworks/utils/cache.py` & `sageworks-0.6.9/src/sageworks/utils/cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/chem_utils.py` & `sageworks-0.6.9/src/sageworks/utils/chem_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/config_manager.py` & `sageworks-0.6.9/src/sageworks/utils/config_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/dashboard_metrics.py` & `sageworks-0.6.9/src/sageworks/utils/dashboard_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/datetime_utils.py` & `sageworks-0.6.9/src/sageworks/utils/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/df_to_endpoint.py` & `sageworks-0.6.9/src/sageworks/utils/df_to_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/docker_utils.py` & `sageworks-0.6.9/src/sageworks/utils/docker_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/ecs_info.py` & `sageworks-0.6.9/src/sageworks/utils/ecs_info.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/endpoint_metrics.py` & `sageworks-0.6.9/src/sageworks/utils/endpoint_metrics.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/endpoint_utils.py` & `sageworks-0.6.9/src/sageworks/utils/endpoint_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/extract_model_artifact.py` & `sageworks-0.6.9/src/sageworks/utils/extract_model_artifact.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/glue_utils.py` & `sageworks-0.6.9/src/sageworks/utils/glue_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/license_manager.py` & `sageworks-0.6.9/src/sageworks/utils/license_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/markdown_utils.py` & `sageworks-0.6.9/src/sageworks/utils/markdown_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/pandas_utils.py` & `sageworks-0.6.9/src/sageworks/utils/pandas_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/plugin_manager.py` & `sageworks-0.6.9/src/sageworks/utils/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/redis_cache.py` & `sageworks-0.6.9/src/sageworks/utils/redis_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/repl_utils.py` & `sageworks-0.6.9/src/sageworks/utils/repl_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/s3_utils.py` & `sageworks-0.6.9/src/sageworks/utils/s3_utils.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/sageworks_cache.py` & `sageworks-0.6.9/src/sageworks/utils/sageworks_cache.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/sageworks_event_bridge.py` & `sageworks-0.6.9/src/sageworks/utils/sageworks_event_bridge.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/sageworks_logging.py` & `sageworks-0.6.9/src/sageworks/utils/sageworks_logging.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/sageworks_sqs.py` & `sageworks-0.6.9/src/sageworks/utils/sageworks_sqs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/symbols.py` & `sageworks-0.6.9/src/sageworks/utils/symbols.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/test_data_generator.py` & `sageworks-0.6.9/src/sageworks/utils/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/trace_calls.py` & `sageworks-0.6.9/src/sageworks/utils/trace_calls.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/utils/type_abbrev.py` & `sageworks-0.6.9/src/sageworks/utils/type_abbrev.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/views/artifacts_text_view.py` & `sageworks-0.6.9/src/sageworks/views/artifacts_text_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/views/artifacts_web_view.py` & `sageworks-0.6.9/src/sageworks/views/artifacts_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/views/data_source_web_view.py` & `sageworks-0.6.9/src/sageworks/views/data_source_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/views/endpoint_web_view.py` & `sageworks-0.6.9/src/sageworks/views/endpoint_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/views/feature_set_web_view.py` & `sageworks-0.6.9/src/sageworks/views/feature_set_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/views/model_web_view.py` & `sageworks-0.6.9/src/sageworks/views/model_web_view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/views/view.py` & `sageworks-0.6.9/src/sageworks/views/view.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/component_interface.py` & `sageworks-0.6.9/src/sageworks/web_components/component_interface.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/confusion_matrix.py` & `sageworks-0.6.9/src/sageworks/web_components/confusion_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/correlation_matrix.py` & `sageworks-0.6.9/src/sageworks/web_components/correlation_matrix.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/data_details_markdown.py` & `sageworks-0.6.9/src/sageworks/web_components/data_details_markdown.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/endpoint_metric_plots.py` & `sageworks-0.6.9/src/sageworks/web_components/endpoint_metric_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/experiments/color_maps.py` & `sageworks-0.6.9/src/sageworks/web_components/experiments/color_maps.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/experiments/compound_details.py` & `sageworks-0.6.9/src/sageworks/web_components/experiments/compound_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/experiments/dashboard_metric_plots.py` & `sageworks-0.6.9/src/sageworks/web_components/experiments/dashboard_metric_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/experiments/data_table.py` & `sageworks-0.6.9/src/sageworks/web_components/experiments/data_table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/experiments/graph_test.py` & `sageworks-0.6.9/src/sageworks/web_components/experiments/graph_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/experiments/hello.py` & `sageworks-0.6.9/src/sageworks/web_components/experiments/hello.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/experiments/histogram.py` & `sageworks-0.6.9/src/sageworks/web_components/experiments/histogram.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/experiments/line_chart.py` & `sageworks-0.6.9/src/sageworks/web_components/experiments/line_chart.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/experiments/outlier_plot.py` & `sageworks-0.6.9/src/sageworks/web_components/experiments/outlier_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/experiments/plugin_callbacks.py` & `sageworks-0.6.9/src/sageworks/web_components/experiments/plugin_callbacks.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/experiments/scatter_plot.py` & `sageworks-0.6.9/src/sageworks/web_components/experiments/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/model_plot.py` & `sageworks-0.6.9/src/sageworks/web_components/model_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/plugin_interface.py` & `sageworks-0.6.9/src/sageworks/web_components/plugin_interface.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/plugin_unit_test.py` & `sageworks-0.6.9/src/sageworks/web_components/plugin_unit_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/plugins/ag_table.py` & `sageworks-0.6.9/src/sageworks/web_components/plugins/ag_table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/plugins/endpoint_details.py` & `sageworks-0.6.9/src/sageworks/web_components/plugins/endpoint_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/plugins/license_details.py` & `sageworks-0.6.9/src/sageworks/web_components/plugins/license_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/plugins/model_details.py` & `sageworks-0.6.9/src/sageworks/web_components/plugins/model_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/plugins/pipeline_details.py` & `sageworks-0.6.9/src/sageworks/web_components/plugins/pipeline_details.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/regression_plot.py` & `sageworks-0.6.9/src/sageworks/web_components/regression_plot.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/table.py` & `sageworks-0.6.9/src/sageworks/web_components/table.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks/web_components/violin_plots.py` & `sageworks-0.6.9/src/sageworks/web_components/violin_plots.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/src/sageworks.egg-info/PKG-INFO` & `sageworks-0.6.9/src/sageworks.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sageworks
-Version: 0.6.8
+Version: 0.6.9
 Summary: SageWorks: A Python WorkBench for creating and deploying AWS SageMaker Models
 Home-page: https://github.com/SuperCowPowers/sageworks
 Author: SuperCowPowers LLC
 Author-email: support@supercowpowers.com
 License: MIT
 Keywords: SageMaker,Machine Learning,AWS,Python,Utilities
 Classifier: Development Status :: 4 - Beta
@@ -32,15 +32,14 @@
 Requires-Dist: shap>=0.43.0
 Requires-Dist: xgboost>=2.0.2
 Requires-Dist: joblib>=1.3.2
 Requires-Dist: cryptography>=42.0.5
 Requires-Dist: rdkit>=2023.9.1
 Requires-Dist: mordred>=1.2.0
 Requires-Dist: ipython>=8.17.2
-Requires-Dist: setuptools>=69.0.2
 Requires-Dist: pyreadline3; sys_platform == "win32"
 
 
 # Welcome to SageWorks
 The SageWorks framework makes AWS® both easier to use and more powerful. SageWorks handles all the details around updating and managing a complex set of AWS Services. With a simple-to-use Python API and a beautiful set of web interfaces, SageWorks makes creating AWS ML pipelines a snap. It also dramatically improves both the usability and visibility across the entire spectrum of services: Glue Job, Athena, Feature Store, Models, and Endpoints, SageWorks makes it easy to build production ready, AWS powered, machine learning pipelines.
 
 <img align="right" width="480" alt="sageworks_new_light" src="https://github.com/SuperCowPowers/sageworks/assets/4806709/ed2ed1bd-e2d8-49a1-b350-b2e19e2b7832">
```

### Comparing `sageworks-0.6.8/src/sageworks.egg-info/SOURCES.txt` & `sageworks-0.6.9/src/sageworks.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 .gitignore
 CONTRIBUTING.md
 Dockerfile
 LICENSE
 Makefile
 README.md
 SECURITY.md
+dev-requirements.txt
 mkdocs.yml
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 .github/PULL_REQUEST_TEMPLATE.md
```

### Comparing `sageworks-0.6.8/tests/artifacts/data_source_tests.py` & `sageworks-0.6.9/tests/artifacts/data_source_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/artifacts/endpoint_tests.py` & `sageworks-0.6.9/tests/artifacts/endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/artifacts/feature_set_tests.py` & `sageworks-0.6.9/tests/artifacts/feature_set_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/artifacts/model_tests.py` & `sageworks-0.6.9/tests/artifacts/model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/aws_account/aws_account_clamp_tests.py` & `sageworks-0.6.9/tests/aws_account/aws_account_clamp_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/aws_account/aws_service_broker_tests.py` & `sageworks-0.6.9/tests/aws_account/aws_service_broker_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/connectors/data_catalog.py` & `sageworks-0.6.9/tests/connectors/data_catalog.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/connectors/endpoints.py` & `sageworks-0.6.9/tests/connectors/endpoints.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/connectors/feature_store.py` & `sageworks-0.6.9/tests/connectors/feature_store.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/connectors/glue_jobs.py` & `sageworks-0.6.9/tests/connectors/glue_jobs.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/connectors/model_registry.py` & `sageworks-0.6.9/tests/connectors/model_registry.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/connectors/s3_bucket.py` & `sageworks-0.6.9/tests/connectors/s3_bucket.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/create_aqsol_artifacts.py` & `sageworks-0.6.9/tests/create_aqsol_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/create_basic_test_artifacts.py` & `sageworks-0.6.9/tests/create_basic_test_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/create_realtime_endpoint.py` & `sageworks-0.6.9/tests/create_realtime_endpoint.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/create_training_adjusted_artifacts.py` & `sageworks-0.6.9/tests/create_training_adjusted_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/create_wine_artifacts.py` & `sageworks-0.6.9/tests/create_wine_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/delete_test_artifacts.py` & `sageworks-0.6.9/tests/delete_test_artifacts.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/plugin_tests/crashing_plugin.py` & `sageworks-0.6.9/tests/plugin_tests/crashing_plugin.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/specific/capital_tests.py` & `sageworks-0.6.9/tests/specific/capital_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/specific/deletion_tests.py` & `sageworks-0.6.9/tests/specific/deletion_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/transforms/data_to_data_tests.py` & `sageworks-0.6.9/tests/transforms/data_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/transforms/data_to_features_tests.py` & `sageworks-0.6.9/tests/transforms/data_to_features_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/transforms/features_to_model_tests.py` & `sageworks-0.6.9/tests/transforms/features_to_model_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/transforms/model_metrics_tests.py` & `sageworks-0.6.9/tests/transforms/model_metrics_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/transforms/model_to_endpoint_tests.py` & `sageworks-0.6.9/tests/transforms/model_to_endpoint_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/transforms/pandas_to_data_tests.py` & `sageworks-0.6.9/tests/transforms/pandas_to_data_tests.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/web_components/confusion_matrix_test.py` & `sageworks-0.6.9/tests/web_components/confusion_matrix_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/web_components/correlation_matrix_test.py` & `sageworks-0.6.9/tests/web_components/correlation_matrix_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tests/web_components/plugin_interface_test.py` & `sageworks-0.6.9/tests/web_components/plugin_interface_test.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/tox.ini` & `sageworks-0.6.9/tox.ini`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/ui_testing/assets/custom.css` & `sageworks-0.6.9/ui_testing/assets/custom.css`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/ui_testing/table_comparison.py` & `sageworks-0.6.9/ui_testing/table_comparison.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/ui_testing/theme_switching.py` & `sageworks-0.6.9/ui_testing/theme_switching.py`

 * *Files identical despite different names*

### Comparing `sageworks-0.6.8/ui_testing/theme_switching_2.py` & `sageworks-0.6.9/ui_testing/theme_switching_2.py`

 * *Files identical despite different names*

