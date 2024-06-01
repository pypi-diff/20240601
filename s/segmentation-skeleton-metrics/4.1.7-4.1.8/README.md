# Comparing `tmp/segmentation_skeleton_metrics-4.1.7.tar.gz` & `tmp/segmentation_skeleton_metrics-4.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segmentation_skeleton_metrics-4.1.7.tar", last modified: Fri May 31 18:44:26 2024, max compression
+gzip compressed data, was "segmentation_skeleton_metrics-4.1.8.tar", last modified: Sat Jun  1 00:11:12 2024, max compression
```

## Comparing `segmentation_skeleton_metrics-4.1.7.tar` & `segmentation_skeleton_metrics-4.1.8.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.749428 segmentation_skeleton_metrics-4.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.713427 segmentation_skeleton_metrics-4.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.717427 segmentation_skeleton_metrics-4.1.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/.github/ISSUE_TEMPLATE/user-story.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.717427 segmentation_skeleton_metrics-4.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/.github/workflows/lint_and_test.yml
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/.github/workflows/tag_and_publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-31 18:44:26.749428 segmentation_skeleton_metrics-4.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.717427 segmentation_skeleton_metrics-4.1.7/doc_template/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/doc_template/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/doc_template/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.717427 segmentation_skeleton_metrics-4.1.7/doc_template/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.717427 segmentation_skeleton_metrics-4.1.7/doc_template/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/doc_template/source/_static/dark-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/doc_template/source/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/doc_template/source/_static/light-logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/doc_template/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/doc_template/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.729427 segmentation_skeleton_metrics-4.1.7/resources/
--rw-r--r--   0 runner    (1001) docker     (127)  9596734 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/resources/pred_labels.tif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.741428 segmentation_skeleton_metrics-4.1.7/resources/target_graphs/
--rw-r--r--   0 runner    (1001) docker     (127)    72420 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/resources/target_graphs/0.swc
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/resources/target_graphs/1.swc
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/resources/target_graphs/2.swc
--rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/resources/target_graphs/3.swc
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/resources/target_graphs/4.swc
--rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/resources/target_graphs/5.swc
--rw-r--r--   0 runner    (1001) docker     (127)  9602600 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/resources/target_labels.tif
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 18:44:26.749428 segmentation_skeleton_metrics-4.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.713427 segmentation_skeleton_metrics-4.1.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.745427 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-31 18:44:16.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/graph_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/merge_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    29165 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/skeleton_metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/split_detection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11025 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/swc_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.745427 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-05-31 18:44:26.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-31 18:44:26.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 18:44:26.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-31 18:44:26.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-31 18:44:26.000000 segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 18:44:26.745427 segmentation_skeleton_metrics-4.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 18:44:15.000000 segmentation_skeleton_metrics-4.1.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:11:12.832512 segmentation_skeleton_metrics-4.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:11:12.800512 segmentation_skeleton_metrics-4.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:11:12.800512 segmentation_skeleton_metrics-4.1.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/.github/ISSUE_TEMPLATE/user-story.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:11:12.800512 segmentation_skeleton_metrics-4.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/.github/workflows/lint_and_test.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/.github/workflows/tag_and_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2199 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-06-01 00:11:12.832512 segmentation_skeleton_metrics-4.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3073 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:11:12.800512 segmentation_skeleton_metrics-4.1.8/doc_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/doc_template/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/doc_template/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:11:12.804512 segmentation_skeleton_metrics-4.1.8/doc_template/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:11:12.804512 segmentation_skeleton_metrics-4.1.8/doc_template/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)     8733 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/doc_template/source/_static/dark-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   259838 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/doc_template/source/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     8712 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/doc_template/source/_static/light-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/doc_template/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/doc_template/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:11:12.816512 segmentation_skeleton_metrics-4.1.8/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)  9596734 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/resources/pred_labels.tif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:11:12.828512 segmentation_skeleton_metrics-4.1.8/resources/target_graphs/
+-rw-r--r--   0 runner    (1001) docker     (127)    72420 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/resources/target_graphs/0.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/resources/target_graphs/1.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/resources/target_graphs/2.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/resources/target_graphs/3.swc
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/resources/target_graphs/4.swc
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/resources/target_graphs/5.swc
+-rw-r--r--   0 runner    (1001) docker     (127)  9602600 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/resources/target_labels.tif
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 00:11:12.832512 segmentation_skeleton_metrics-4.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:11:12.800512 segmentation_skeleton_metrics-4.1.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:11:12.828512 segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-06-01 00:10:58.000000 segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5159 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics/graph_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4161 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics/merge_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29165 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics/skeleton_metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6577 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics/split_detection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics/swc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10636 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:11:12.828512 segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3943 2024-06-01 00:11:12.000000 segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-06-01 00:11:12.000000 segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:11:12.000000 segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-06-01 00:11:12.000000 segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-01 00:11:12.000000 segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:11:12.828512 segmentation_skeleton_metrics-4.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 00:10:57.000000 segmentation_skeleton_metrics-4.1.8/tests/__init__.py
```

### Comparing `segmentation_skeleton_metrics-4.1.7/.github/ISSUE_TEMPLATE/bug_report.md` & `segmentation_skeleton_metrics-4.1.8/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/.github/ISSUE_TEMPLATE/feature_request.md` & `segmentation_skeleton_metrics-4.1.8/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/.github/ISSUE_TEMPLATE/user-story.md` & `segmentation_skeleton_metrics-4.1.8/.github/ISSUE_TEMPLATE/user-story.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/.github/workflows/lint_and_test.yml` & `segmentation_skeleton_metrics-4.1.8/.github/workflows/lint_and_test.yml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/.github/workflows/tag_and_publish.yml` & `segmentation_skeleton_metrics-4.1.8/.github/workflows/tag_and_publish.yml`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/.gitignore` & `segmentation_skeleton_metrics-4.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/LICENSE` & `segmentation_skeleton_metrics-4.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/PKG-INFO` & `segmentation_skeleton_metrics-4.1.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: segmentation_skeleton_metrics
-Version: 4.1.7
+Version: 4.1.8
 Summary: Python package for evaluating neuron segmentations in terms of the number of splits and merges
 Author-email: Anna Grim <anna.grim@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: scikit-image
 Requires-Dist: tensorstore
 Requires-Dist: tifffile
+Requires-Dist: xlwt
 Requires-Dist: zarr
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `segmentation_skeleton_metrics-4.1.7/README.md` & `segmentation_skeleton_metrics-4.1.8/README.md`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/doc_template/Makefile` & `segmentation_skeleton_metrics-4.1.8/doc_template/Makefile`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/doc_template/make.bat` & `segmentation_skeleton_metrics-4.1.8/doc_template/make.bat`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/doc_template/source/_static/dark-logo.svg` & `segmentation_skeleton_metrics-4.1.8/doc_template/source/_static/dark-logo.svg`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/doc_template/source/_static/favicon.ico` & `segmentation_skeleton_metrics-4.1.8/doc_template/source/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/doc_template/source/_static/light-logo.svg` & `segmentation_skeleton_metrics-4.1.8/doc_template/source/_static/light-logo.svg`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/doc_template/source/conf.py` & `segmentation_skeleton_metrics-4.1.8/doc_template/source/conf.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/pyproject.toml` & `segmentation_skeleton_metrics-4.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 dependencies = [
     "networkx",
     "numpy",
     "scikit-image",
     "tensorstore",
     "tifffile",
+    "xlwt",
     "zarr",
 ]
 
 [project.optional-dependencies]
 dev = [
     'black',
     'coverage',
```

### Comparing `segmentation_skeleton_metrics-4.1.7/resources/pred_labels.tif` & `segmentation_skeleton_metrics-4.1.8/resources/pred_labels.tif`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/resources/target_graphs/0.swc` & `segmentation_skeleton_metrics-4.1.8/resources/target_graphs/0.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/resources/target_graphs/1.swc` & `segmentation_skeleton_metrics-4.1.8/resources/target_graphs/1.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/resources/target_graphs/2.swc` & `segmentation_skeleton_metrics-4.1.8/resources/target_graphs/2.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/resources/target_graphs/3.swc` & `segmentation_skeleton_metrics-4.1.8/resources/target_graphs/3.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/resources/target_graphs/4.swc` & `segmentation_skeleton_metrics-4.1.8/resources/target_graphs/4.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/resources/target_graphs/5.swc` & `segmentation_skeleton_metrics-4.1.8/resources/target_graphs/5.swc`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/resources/target_labels.tif` & `segmentation_skeleton_metrics-4.1.8/resources/target_labels.tif`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/graph_utils.py` & `segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics/graph_utils.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/merge_detection.py` & `segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics/merge_detection.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/skeleton_metric.py` & `segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics/skeleton_metric.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/split_detection.py` & `segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics/split_detection.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/swc_utils.py` & `segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics/swc_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Created on Wed June 5 16:00:00 2023
 
 @author: Anna Grim
 @email: anna.grim@alleninstitute.org
 
 """
 
-from concurrent.futures import ThreadPoolExecutor, as_completed
+from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor, as_completed
 from io import BytesIO
 from zipfile import ZipFile
 
 import networkx as nx
 import numpy as np
 from google.cloud import storage
 
@@ -104,98 +104,104 @@
         Dictionary where each item is an swc_id and an array of the xyz
         coordinates read from cooresponding swc file.
 
     """
     # Initializations
     bucket = storage.Client().bucket(cloud_dict["bucket_name"])
     zip_paths = utils.list_gcs_filenames(bucket, cloud_dict["path"], ".zip")
-    chunk_size = int(len(zip_paths) * 0.02)
+    print("Downloading predicted swc files from cloud...")
+    print("# zip files:", len(zip_paths))
+    with ProcessPoolExecutor() as executor:
+        processes = []
+        for path in zip_paths:
+            zip_content = bucket.blob(path).download_as_bytes()
+            processes.append(
+                executor.submit(download, zip_content, anisotropy, min_size)
+            )
+    print("Processes Assigned!\n")
 
-    # Parse
+    # Store results
+    chunk_size = int(len(zip_paths) * 0.02)
     cnt = 1
     valid_labels = dict()
-    print("Downloading predicted swc files from cloud...")
-    print("# zip files:", len(zip_paths))
-    for i, path in enumerate(zip_paths):
-        valid_labels.update(download(bucket, path, min_size, anisotropy))
+    t0, t1 = utils.init_timers()
+    for i, process in enumerate(as_completed(processes)):
+        valid_labels.update(process.result())
         if i > cnt * chunk_size:
             utils.progress_bar(i + 1, len(zip_paths))
             cnt += 1
 
     # Report Results
     print("\n#Valid Labels:", len(valid_labels))
     print("")
     return valid_labels
 
 
-def download(bucket, zip_path, min_size, anisotropy):
+def download(zip_content, anisotropy, min_size):
     """
     Downloads the contents from each swc file contained in the zip file at
     "zip_path".
 
     Parameters
     ----------
-    bucket : str
-        Name of GCS bucket containing swc files to be read.
-    zip_path : str
-        Path to zip file contained in GCS bucket.
-    min_size : int
-        Threshold on the number of nodes contained in an swc file. Only swc
-        files with more than "min_size" nodes are stored in "valid_labels".
+    zip_content : ...
+        Contents of a zip file.
     anisotropy : list[float]
         Image to World scaling factors applied to xyz coordinates to account
         for anisotropy of the microscope.
+    min_size : int
+        Threshold on the number of nodes contained in an swc file. Only swc
+        files with more than "min_size" nodes are stored in "valid_labels".
 
     Returns
     -------
     valid_labels : dict
         Dictionary where each item is an swc_id and an array of the xyz
         coordinates read from cooresponding swc file.
 
     """
-    zip_content = bucket.blob(zip_path).download_as_bytes()
     with ZipFile(BytesIO(zip_content)) as zip_file:
         with ThreadPoolExecutor() as executor:
             # Assign threads
-            threads = []
-            for path in utils.list_files_in_gcs_zip(zip_content):
-                threads.append(
-                    executor.submit(
-                        parse_gcs_zip, zip_file, path, min_size, anisotropy
-                    )
+            paths = utils.list_files_in_gcs_zip(zip_content)
+            threads = [
+                executor.submit(
+                    parse_gcs_zip, zip_file, path, anisotropy, min_size
                 )
+                for path in paths
+            ]
 
-            # Process results
-            valid_labels = dict()
-            for thread in as_completed(threads):
-                valid_labels.update(thread.result())
+    # Process results
+    valid_labels = dict()
+    for thread in as_completed(threads):
+        valid_labels.update(thread.result())
     return valid_labels
 
 
-def parse_gcs_zip(zip_file, path, min_size, anisotropy):
+def parse_gcs_zip(zip_file, path, anisotropy, min_size):
     """
     Reads swc file stored at "path" which points to a file in a GCS bucket.
 
     Parameters
     ----------
     zip_file : ZipFile
         Zip file containing swc file to be read.
     path : str
         Path to swc file to be read.
-    min_size : int
-        Threshold on the number of nodes contained in an swc file. Only swc
-        files with more than "min_size" nodes are stored in "valid_labels".
     anisotropy : list[float]
         Image to World scaling factors applied to xyz coordinates to account
         for anisotropy of the microscope.
+    min_size : int
+        Threshold on the number of nodes contained in an swc file. Only swc
+        files with more than "min_size" nodes are stored in "valid_labels".
 
     Returns
     -------
     list
-        List such that each entry is a line from the swc file.
+        Entries of an swc file.
 
     """
     contents = read_from_cloud(zip_file, path)
     if len(contents) > min_size:
         swc_id = int(utils.get_id(path))
         return {swc_id: get_coords(contents, anisotropy)}
     else:
@@ -222,16 +228,16 @@
 
 
 def read_from_cloud(zip_file, path):
     """
     Reads the content of an swc file from a zip file in a GCS bucket.
 
     """
-    with zip_file.open(path) as text_file:
-        return text_file.read().decode("utf-8").splitlines()
+    with zip_file.open(path) as f:
+        return f.read().decode("utf-8").splitlines()
 
 
 def get_coords(contents, anisotropy):
     """
     Gets the xyz coords from the swc file at "path".
 
     Parameters
```

### Comparing `segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics/utils.py` & `segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics/utils.py`

 * *Files identical despite different names*

### Comparing `segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics.egg-info/PKG-INFO` & `segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: segmentation_skeleton_metrics
-Version: 4.1.7
+Version: 4.1.8
 Summary: Python package for evaluating neuron segmentations in terms of the number of splits and merges
 Author-email: Anna Grim <anna.grim@alleninstitute.org>
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: scikit-image
 Requires-Dist: tensorstore
 Requires-Dist: tifffile
+Requires-Dist: xlwt
 Requires-Dist: zarr
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: coverage; extra == "dev"
 Requires-Dist: flake8; extra == "dev"
 Requires-Dist: interrogate; extra == "dev"
 Requires-Dist: isort; extra == "dev"
```

### Comparing `segmentation_skeleton_metrics-4.1.7/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt` & `segmentation_skeleton_metrics-4.1.8/src/segmentation_skeleton_metrics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

