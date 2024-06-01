# Comparing `tmp/thoi-0.1.0.tar.gz` & `tmp/thoi-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoi-0.1.0.tar", last modified: Sat Jun  1 03:17:54 2024, max compression
+gzip compressed data, was "thoi-0.1.8.tar", last modified: Sat Jun  1 03:28:44 2024, max compression
```

## Comparing `thoi-0.1.0.tar` & `thoi-0.1.8.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:54.009657 thoi-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-06-01 03:17:46.000000 thoi-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-06-01 03:17:54.009657 thoi-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-06-01 03:17:46.000000 thoi-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 03:17:54.009657 thoi-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-06-01 03:17:46.000000 thoi-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:54.009657 thoi-0.1.0/thoi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:46.000000 thoi-0.1.0/thoi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-06-01 03:17:46.000000 thoi-0.1.0/thoi/collectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-06-01 03:17:46.000000 thoi-0.1.0/thoi/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-06-01 03:17:46.000000 thoi-0.1.0/thoi/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:54.009657 thoi-0.1.0/thoi/measures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:46.000000 thoi-0.1.0/thoi/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-06-01 03:17:46.000000 thoi-0.1.0/thoi/measures/gaussian_copula.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:54.009657 thoi-0.1.0/thoi/synthetic_systems/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-01 03:17:46.000000 thoi-0.1.0/thoi/synthetic_systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-06-01 03:17:46.000000 thoi-0.1.0/thoi/synthetic_systems/flat.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-06-01 03:17:46.000000 thoi-0.1.0/thoi/synthetic_systems/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-06-01 03:17:46.000000 thoi-0.1.0/thoi/synthetic_systems/xor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:54.009657 thoi-0.1.0/thoi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-06-01 03:17:54.000000 thoi-0.1.0/thoi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-06-01 03:17:54.000000 thoi-0.1.0/thoi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 03:17:54.000000 thoi-0.1.0/thoi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-01 03:17:54.000000 thoi-0.1.0/thoi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-01 03:17:54.000000 thoi-0.1.0/thoi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:44.085034 thoi-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:44.081034 thoi-0.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:44.081034 thoi-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-06-01 03:28:38.000000 thoi-0.1.8/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-06-01 03:28:38.000000 thoi-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-06-01 03:28:44.085034 thoi-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-06-01 03:28:38.000000 thoi-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 03:28:38.000000 thoi-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 03:28:44.085034 thoi-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-06-01 03:28:38.000000 thoi-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:44.081034 thoi-0.1.8/thoi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:44.081034 thoi-0.1.8/thoi/measures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/measures/gaussian_copula.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:44.085034 thoi-0.1.8/thoi/synthetic_systems/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/synthetic_systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/synthetic_systems/flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/synthetic_systems/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/synthetic_systems/xor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:44.085034 thoi-0.1.8/thoi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-06-01 03:28:44.000000 thoi-0.1.8/thoi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-01 03:28:44.000000 thoi-0.1.8/thoi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 03:28:44.000000 thoi-0.1.8/thoi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-01 03:28:44.000000 thoi-0.1.8/thoi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-01 03:28:44.000000 thoi-0.1.8/thoi.egg-info/top_level.txt
```

### Comparing `thoi-0.1.0/LICENSE` & `thoi-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `thoi-0.1.0/PKG-INFO` & `thoi-0.1.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 Metadata-Version: 2.1
 Name: thoi
-Version: 0.1.0
+Version: 0.1.8
 Summary: Torch - Higher Order Interactions
 Home-page: https://github.com/Laouen/THOI
 Author: Laouen Mayal Louan Belloli, Ruben Herzog
 Author-email: laouen.belloli@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: torch
 Requires-Dist: tqdm
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: networkx
 
-A Python package to compute O information in Higher Order Interactions uing batch processing
+# O-information
+
+Authors: 
+* [Ruben Herzog](https://www.linkedin.com/in/rherzoga/)
+* [Laouen Belloli](https://www.linkedin.com/in/laouen-belloli/)
+
+## Installation
+
+```bash
+pip install thoi
+```
+
+## Usage
```

### Comparing `thoi-0.1.0/setup.py` & `thoi-0.1.8/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 from setuptools import setup, find_packages
 
+# Read the contents of README.md
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
 setup(
     name='thoi',
-    version='v0.1.0',
+    use_scm_version=True,
+    setup_requires=['setuptools_scm'],
     description='Torch - Higher Order Interactions',
-    long_description='A Python package to compute O information in Higher Order Interactions uing batch processing',
-    long_description_content_type='text/x-rst',
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     author='Laouen Mayal Louan Belloli, Ruben Herzog',
     author_email='laouen.belloli@gmail.com',
     url='https://github.com/Laouen/THOI',
     packages=find_packages(),
     install_requires=[
         'numpy',
         'torch',
```

### Comparing `thoi-0.1.0/thoi/collectors.py` & `thoi-0.1.8/thoi/collectors.py`

 * *Files identical despite different names*

### Comparing `thoi-0.1.0/thoi/dataset.py` & `thoi-0.1.8/thoi/dataset.py`

 * *Files identical despite different names*

### Comparing `thoi-0.1.0/thoi/graph.py` & `thoi-0.1.8/thoi/graph.py`

 * *Files identical despite different names*

### Comparing `thoi-0.1.0/thoi/measures/gaussian_copula.py` & `thoi-0.1.8/thoi/measures/gaussian_copula.py`

 * *Files identical despite different names*

### Comparing `thoi-0.1.0/thoi/synthetic_systems/flat.py` & `thoi-0.1.8/thoi/synthetic_systems/flat.py`

 * *Files identical despite different names*

### Comparing `thoi-0.1.0/thoi/synthetic_systems/relu.py` & `thoi-0.1.8/thoi/synthetic_systems/relu.py`

 * *Files identical despite different names*

### Comparing `thoi-0.1.0/thoi.egg-info/PKG-INFO` & `thoi-0.1.8/thoi.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 Metadata-Version: 2.1
 Name: thoi
-Version: 0.1.0
+Version: 0.1.8
 Summary: Torch - Higher Order Interactions
 Home-page: https://github.com/Laouen/THOI
 Author: Laouen Mayal Louan Belloli, Ruben Herzog
 Author-email: laouen.belloli@gmail.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: torch
 Requires-Dist: tqdm
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: networkx
 
-A Python package to compute O information in Higher Order Interactions uing batch processing
+# O-information
+
+Authors: 
+* [Ruben Herzog](https://www.linkedin.com/in/rherzoga/)
+* [Laouen Belloli](https://www.linkedin.com/in/laouen-belloli/)
+
+## Installation
+
+```bash
+pip install thoi
+```
+
+## Usage
```

