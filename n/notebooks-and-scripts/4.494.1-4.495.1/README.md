# Comparing `tmp/notebooks_and_scripts-4.494.1.tar.gz` & `tmp/notebooks_and_scripts-4.495.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notebooks_and_scripts-4.494.1.tar", last modified: Sat Jun  1 02:42:12 2024, max compression
+gzip compressed data, was "notebooks_and_scripts-4.495.1.tar", last modified: Sat Jun  1 02:44:24 2024, max compression
```

## Comparing `notebooks_and_scripts-4.494.1.tar` & `notebooks_and_scripts-4.495.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:42:12.428469 notebooks_and_scripts-4.494.1/
--rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.494.1/LICENSE
--rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:51:23.000000 notebooks_and_scripts-4.494.1/MANIFEST.in
--rw-r--r--   0 kamangir   (502) staff       (20)     5775 2024-06-01 02:42:12.427550 notebooks_and_scripts-4.494.1/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     4141 2024-05-19 23:00:17.000000 notebooks_and_scripts-4.494.1/README.md
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:42:12.397888 notebooks_and_scripts-4.494.1/notebooks_and_scripts/
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:42:12.411431 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/
--rw-r--r--   0 kamangir   (502) staff       (20)      172 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/actions.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      181 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/aka.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      487 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/alias.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:42:12.413732 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/aws_batch/
--rw-r--r--   0 kamangir   (502) staff       (20)     1211 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/aws_batch/browse.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      670 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/aws_batch/eval.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1550 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/aws_batch/list.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      666 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/aws_batch/submit.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      537 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/aws_batch.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     4164 2024-05-26 20:57:03.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/docker.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:42:12.418441 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/jupyter-notebook/
--rw-r--r--   0 kamangir   (502) staff       (20)      759 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/jupyter-notebook/build.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      455 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/jupyter-notebook/code.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      852 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/jupyter-notebook/connect.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      716 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/jupyter-notebook/create.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      739 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/jupyter-notebook/host.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      417 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/jupyter-notebook/open.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)      703 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/jupyter-notebook.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:42:12.420523 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/localflow/
--rw-r--r--   0 kamangir   (502) staff       (20)      771 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/localflow/eval.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      533 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/localflow/list.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1600 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/localflow/run.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      576 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/localflow.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1533 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/meta_scripts.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      798 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/notebooks-and-scripts.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      922 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/sagemaker.sh
--rwxr-xr-x   0 kamangir   (502) staff       (20)     5761 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/scripts.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:42:12.421733 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/tests/
--rw-r--r--   0 kamangir   (502) staff       (20)      250 2024-05-28 01:45:49.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/tests/version.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      528 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/tests/workflow_runner.sh
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:42:12.425069 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/workflow/
--rw-r--r--   0 kamangir   (502) staff       (20)      766 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/workflow/config.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      808 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/workflow/create.sh
--rw-r--r--   0 kamangir   (502) staff       (20)     1130 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/workflow/monitor.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      989 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/workflow/submit.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      680 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/workflow.sh
--rw-r--r--   0 kamangir   (502) staff       (20)      190 2024-06-01 02:42:04.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      269 2024-05-28 01:45:49.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/__main__.py
--rw-r--r--   0 kamangir   (502) staff       (20)      279 2024-05-08 01:33:41.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/config.env
--rw-r--r--   0 kamangir   (502) staff       (20)      443 2024-05-08 01:33:52.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/env.py
--rw-r--r--   0 kamangir   (502) staff       (20)      102 2024-03-24 00:15:57.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/logger.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:42:12.425716 notebooks_and_scripts-4.494.1/notebooks_and_scripts/sagemaker/
--rw-r--r--   0 kamangir   (502) staff       (20)      365 2024-03-04 07:47:37.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/sagemaker/__init__.py
--rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts/urls.py
-drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:42:12.426474 notebooks_and_scripts-4.494.1/notebooks_and_scripts.egg-info/
--rw-r--r--   0 kamangir   (502) staff       (20)     5775 2024-06-01 02:42:12.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts.egg-info/PKG-INFO
--rw-r--r--   0 kamangir   (502) staff       (20)     1993 2024-06-01 02:42:12.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts.egg-info/SOURCES.txt
--rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-06-01 02:42:12.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts.egg-info/dependency_links.txt
--rw-r--r--   0 kamangir   (502) staff       (20)      164 2024-06-01 02:42:12.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts.egg-info/requires.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       22 2024-06-01 02:42:12.000000 notebooks_and_scripts-4.494.1/notebooks_and_scripts.egg-info/top_level.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 04:14:57.000000 notebooks_and_scripts-4.494.1/pyproject.toml
--rw-r--r--   0 kamangir   (502) staff       (20)      366 2024-05-20 22:39:52.000000 notebooks_and_scripts-4.494.1/requirements.txt
--rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-06-01 02:42:12.428628 notebooks_and_scripts-4.494.1/setup.cfg
--rw-r--r--   0 kamangir   (502) staff       (20)      433 2024-05-26 20:39:45.000000 notebooks_and_scripts-4.494.1/setup.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:44:24.235602 notebooks_and_scripts-4.495.1/
+-rw-r--r--   0 kamangir   (502) staff       (20)     7048 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.495.1/LICENSE
+-rw-r--r--   0 kamangir   (502) staff       (20)       24 2024-05-20 04:51:23.000000 notebooks_and_scripts-4.495.1/MANIFEST.in
+-rw-r--r--   0 kamangir   (502) staff       (20)     5775 2024-06-01 02:44:24.235014 notebooks_and_scripts-4.495.1/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     4141 2024-05-19 23:00:17.000000 notebooks_and_scripts-4.495.1/README.md
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:44:24.203697 notebooks_and_scripts-4.495.1/notebooks_and_scripts/
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:44:24.221140 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/
+-rw-r--r--   0 kamangir   (502) staff       (20)      172 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/actions.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      181 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/aka.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      487 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/alias.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:44:24.223864 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/aws_batch/
+-rw-r--r--   0 kamangir   (502) staff       (20)     1211 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/aws_batch/browse.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      670 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/aws_batch/eval.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1550 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/aws_batch/list.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      666 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/aws_batch/submit.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      537 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/aws_batch.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     4164 2024-05-26 20:57:03.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/docker.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:44:24.227146 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/jupyter-notebook/
+-rw-r--r--   0 kamangir   (502) staff       (20)      759 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/jupyter-notebook/build.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      455 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/jupyter-notebook/code.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      852 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/jupyter-notebook/connect.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      716 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/jupyter-notebook/create.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      739 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/jupyter-notebook/host.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      417 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/jupyter-notebook/open.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)      703 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/jupyter-notebook.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:44:24.229953 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/localflow/
+-rw-r--r--   0 kamangir   (502) staff       (20)      771 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/localflow/eval.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      533 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/localflow/list.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1600 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/localflow/run.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      576 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/localflow.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1533 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/meta_scripts.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      798 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/notebooks-and-scripts.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      922 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/sagemaker.sh
+-rwxr-xr-x   0 kamangir   (502) staff       (20)     5761 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/scripts.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:44:24.231752 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/tests/
+-rw-r--r--   0 kamangir   (502) staff       (20)      250 2024-05-28 01:45:49.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/tests/version.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      528 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/tests/workflow_runner.sh
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:44:24.233577 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/workflow/
+-rw-r--r--   0 kamangir   (502) staff       (20)      766 2024-06-01 02:15:44.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/workflow/config.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      808 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/workflow/create.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)     1130 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/workflow/monitor.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      989 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/workflow/submit.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      680 2024-05-26 18:24:35.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/workflow.sh
+-rw-r--r--   0 kamangir   (502) staff       (20)      190 2024-06-01 02:44:17.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      269 2024-05-28 01:45:49.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/__main__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      279 2024-05-08 01:33:41.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/config.env
+-rw-r--r--   0 kamangir   (502) staff       (20)      443 2024-05-08 01:33:52.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/env.py
+-rw-r--r--   0 kamangir   (502) staff       (20)      102 2024-03-24 00:15:57.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/logger.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:44:24.233979 notebooks_and_scripts-4.495.1/notebooks_and_scripts/sagemaker/
+-rw-r--r--   0 kamangir   (502) staff       (20)      365 2024-03-04 07:47:37.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/sagemaker/__init__.py
+-rw-r--r--   0 kamangir   (502) staff       (20)       17 2023-09-26 02:32:46.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts/urls.py
+drwxr-xr-x   0 kamangir   (502) staff       (20)        0 2024-06-01 02:44:24.234441 notebooks_and_scripts-4.495.1/notebooks_and_scripts.egg-info/
+-rw-r--r--   0 kamangir   (502) staff       (20)     5775 2024-06-01 02:44:24.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts.egg-info/PKG-INFO
+-rw-r--r--   0 kamangir   (502) staff       (20)     1993 2024-06-01 02:44:24.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts.egg-info/SOURCES.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)        1 2024-06-01 02:44:24.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts.egg-info/dependency_links.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)      164 2024-06-01 02:44:24.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts.egg-info/requires.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       22 2024-06-01 02:44:24.000000 notebooks_and_scripts-4.495.1/notebooks_and_scripts.egg-info/top_level.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       81 2024-05-21 04:14:57.000000 notebooks_and_scripts-4.495.1/pyproject.toml
+-rw-r--r--   0 kamangir   (502) staff       (20)      366 2024-05-20 22:39:52.000000 notebooks_and_scripts-4.495.1/requirements.txt
+-rw-r--r--   0 kamangir   (502) staff       (20)       38 2024-06-01 02:44:24.235790 notebooks_and_scripts-4.495.1/setup.cfg
+-rw-r--r--   0 kamangir   (502) staff       (20)      433 2024-05-26 20:39:45.000000 notebooks_and_scripts-4.495.1/setup.py
```

### Comparing `notebooks_and_scripts-4.494.1/LICENSE` & `notebooks_and_scripts-4.495.1/LICENSE`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/PKG-INFO` & `notebooks_and_scripts-4.495.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebooks_and_scripts
-Version: 4.494.1
+Version: 4.495.1
 Summary: 📜 notebooks and scripts for ai experiments and aws batch jobs.
 Home-page: https://github.com/kamangir/notebooks-and-scripts
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `notebooks_and_scripts-4.494.1/README.md` & `notebooks_and_scripts-4.495.1/README.md`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/aws_batch/browse.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/aws_batch/browse.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/aws_batch/eval.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/aws_batch/eval.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/aws_batch/list.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/aws_batch/list.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/aws_batch/submit.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/aws_batch/submit.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/aws_batch.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/aws_batch.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/docker.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/docker.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/jupyter-notebook/build.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/jupyter-notebook/build.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/jupyter-notebook/connect.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/jupyter-notebook/connect.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/jupyter-notebook/create.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/jupyter-notebook/create.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/jupyter-notebook/host.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/jupyter-notebook/host.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/jupyter-notebook.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/jupyter-notebook.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/localflow/eval.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/localflow/eval.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/localflow/list.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/localflow/list.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/localflow/run.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/localflow/run.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/localflow.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/localflow.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/meta_scripts.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/meta_scripts.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/notebooks-and-scripts.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/notebooks-and-scripts.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/sagemaker.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/sagemaker.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/scripts.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/scripts.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/tests/workflow_runner.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/tests/workflow_runner.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/workflow/config.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/workflow/config.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/workflow/create.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/workflow/create.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/workflow/monitor.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/workflow/monitor.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/workflow/submit.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/workflow/submit.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts/.abcli/workflow.sh` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts/.abcli/workflow.sh`

 * *Files identical despite different names*

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts.egg-info/PKG-INFO` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: notebooks_and_scripts
-Version: 4.494.1
+Version: 4.495.1
 Summary: 📜 notebooks and scripts for ai experiments and aws batch jobs.
 Home-page: https://github.com/kamangir/notebooks-and-scripts
 Author: Arash Abadpour (Kamangir)
 Author-email: arash@kamangir.net
 License: Public Domain
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Unix Shell
```

### Comparing `notebooks_and_scripts-4.494.1/notebooks_and_scripts.egg-info/SOURCES.txt` & `notebooks_and_scripts-4.495.1/notebooks_and_scripts.egg-info/SOURCES.txt`

 * *Files identical despite different names*
