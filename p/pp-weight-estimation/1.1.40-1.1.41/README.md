# Comparing `tmp/pp_weight_estimation-1.1.40.tar.gz` & `tmp/pp_weight_estimation-1.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pp_weight_estimation-1.1.40.tar", last modified: Thu May 30 17:36:03 2024, max compression
+gzip compressed data, was "pp_weight_estimation-1.1.41.tar", last modified: Sat Jun  1 03:39:40 2024, max compression
```

## Comparing `pp_weight_estimation-1.1.40.tar` & `pp_weight_estimation-1.1.41.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 17:36:03.347084 pp_weight_estimation-1.1.40/
--rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-05-30 17:36:03.347084 pp_weight_estimation-1.1.40/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-23 00:15:21.000000 pp_weight_estimation-1.1.40/README.md
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 17:36:03.343084 pp_weight_estimation-1.1.40/pp_weight_estimation/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.40/pp_weight_estimation/__init__.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 17:36:03.347084 pp_weight_estimation-1.1.40/pp_weight_estimation/core/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.40/pp_weight_estimation/core/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)    11113 2024-05-30 11:49:39.000000 pp_weight_estimation-1.1.40/pp_weight_estimation/core/function_test.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     6734 2024-05-30 11:49:39.000000 pp_weight_estimation-1.1.40/pp_weight_estimation/core/get_weight.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1578 2024-05-24 09:16:34.000000 pp_weight_estimation-1.1.40/pp_weight_estimation/core/gpt_support.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1664 2024-05-30 17:35:50.000000 pp_weight_estimation-1.1.40/pp_weight_estimation/core/s3_io.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 17:36:03.347084 pp_weight_estimation-1.1.40/pp_weight_estimation/utils/
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:39:01.000000 pp_weight_estimation-1.1.40/pp_weight_estimation/utils/__init__.py
--rw-rw-r--   0 malav     (1000) malav     (1000)     1000 2024-05-23 00:53:12.000000 pp_weight_estimation-1.1.40/pp_weight_estimation/utils/slack_connect.py
--rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.40/pp_weight_estimation/utils/visulizer.py
--rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-05-30 17:35:53.000000 pp_weight_estimation-1.1.40/pp_weight_estimation/version.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 17:36:03.347084 pp_weight_estimation-1.1.40/pp_weight_estimation.egg-info/
--rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-05-30 17:36:03.000000 pp_weight_estimation-1.1.40/pp_weight_estimation.egg-info/PKG-INFO
--rw-rw-r--   0 malav     (1000) malav     (1000)      690 2024-05-30 17:36:03.000000 pp_weight_estimation-1.1.40/pp_weight_estimation.egg-info/SOURCES.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-05-30 17:36:03.000000 pp_weight_estimation-1.1.40/pp_weight_estimation.egg-info/dependency_links.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-05-30 17:36:03.000000 pp_weight_estimation-1.1.40/pp_weight_estimation.egg-info/requires.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-05-30 17:36:03.000000 pp_weight_estimation-1.1.40/pp_weight_estimation.egg-info/top_level.txt
--rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.40/pyproject.toml
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 17:36:03.343084 pp_weight_estimation-1.1.40/scripts/
--rw-rw-r--   0 malav     (1000) malav     (1000)      390 2024-05-23 00:02:20.000000 pp_weight_estimation-1.1.40/scripts/weight_pred.py
--rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-05-30 17:36:03.347084 pp_weight_estimation-1.1.40/setup.cfg
--rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-28 14:05:37.000000 pp_weight_estimation-1.1.40/setup.py
-drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-05-30 17:36:03.347084 pp_weight_estimation-1.1.40/tests/
--rw-rw-r--   0 malav     (1000) malav     (1000)     1892 2024-05-28 11:33:49.000000 pp_weight_estimation-1.1.40/tests/test_function_test.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/
+-rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)       56 2024-05-23 00:15:21.000000 pp_weight_estimation-1.1.41/README.md
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/pp_weight_estimation/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/__init__.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/pp_weight_estimation/core/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:38:28.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/core/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)    11113 2024-05-30 11:49:39.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/core/function_test.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     6734 2024-05-30 11:49:39.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/core/get_weight.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1578 2024-05-24 09:16:34.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/core/gpt_support.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1923 2024-06-01 03:39:23.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/core/s3_io.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/pp_weight_estimation/utils/
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-28 13:39:01.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/utils/__init__.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1000 2024-05-23 00:53:12.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/utils/slack_connect.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)        0 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/utils/visulizer.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)      207 2024-06-01 03:39:32.000000 pp_weight_estimation-1.1.41/pp_weight_estimation/version.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/pp_weight_estimation.egg-info/
+-rw-r--r--   0 malav     (1000) malav     (1000)      246 2024-06-01 03:39:40.000000 pp_weight_estimation-1.1.41/pp_weight_estimation.egg-info/PKG-INFO
+-rw-rw-r--   0 malav     (1000) malav     (1000)      690 2024-06-01 03:39:40.000000 pp_weight_estimation-1.1.41/pp_weight_estimation.egg-info/SOURCES.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)        1 2024-06-01 03:39:40.000000 pp_weight_estimation-1.1.41/pp_weight_estimation.egg-info/dependency_links.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       27 2024-06-01 03:39:40.000000 pp_weight_estimation-1.1.41/pp_weight_estimation.egg-info/requires.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       21 2024-06-01 03:39:40.000000 pp_weight_estimation-1.1.41/pp_weight_estimation.egg-info/top_level.txt
+-rw-rw-r--   0 malav     (1000) malav     (1000)       81 2024-05-17 03:44:16.000000 pp_weight_estimation-1.1.41/pyproject.toml
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/scripts/
+-rw-rw-r--   0 malav     (1000) malav     (1000)      390 2024-05-23 00:02:20.000000 pp_weight_estimation-1.1.41/scripts/weight_pred.py
+-rw-rw-r--   0 malav     (1000) malav     (1000)       38 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/setup.cfg
+-rw-rw-r--   0 malav     (1000) malav     (1000)      884 2024-05-28 14:05:37.000000 pp_weight_estimation-1.1.41/setup.py
+drwxrwxr-x   0 malav     (1000) malav     (1000)        0 2024-06-01 03:39:40.510914 pp_weight_estimation-1.1.41/tests/
+-rw-rw-r--   0 malav     (1000) malav     (1000)     1892 2024-05-28 11:33:49.000000 pp_weight_estimation-1.1.41/tests/test_function_test.py
```

### Comparing `pp_weight_estimation-1.1.40/pp_weight_estimation/core/function_test.py` & `pp_weight_estimation-1.1.41/pp_weight_estimation/core/function_test.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.40/pp_weight_estimation/core/get_weight.py` & `pp_weight_estimation-1.1.41/pp_weight_estimation/core/get_weight.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.40/pp_weight_estimation/core/gpt_support.py` & `pp_weight_estimation-1.1.41/pp_weight_estimation/core/gpt_support.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.40/pp_weight_estimation/utils/slack_connect.py` & `pp_weight_estimation-1.1.41/pp_weight_estimation/utils/slack_connect.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.40/pp_weight_estimation.egg-info/SOURCES.txt` & `pp_weight_estimation-1.1.41/pp_weight_estimation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.40/setup.py` & `pp_weight_estimation-1.1.41/setup.py`

 * *Files identical despite different names*

### Comparing `pp_weight_estimation-1.1.40/tests/test_function_test.py` & `pp_weight_estimation-1.1.41/tests/test_function_test.py`

 * *Files identical despite different names*

