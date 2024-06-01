# Comparing `tmp/thoi-0.1.8.tar.gz` & `tmp/thoi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thoi-0.1.8.tar", last modified: Sat Jun  1 03:28:44 2024, max compression
+gzip compressed data, was "thoi-0.1.9.tar", last modified: Sat Jun  1 04:10:36 2024, max compression
```

## Comparing `thoi-0.1.8.tar` & `thoi-0.1.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:44.085034 thoi-0.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:44.081034 thoi-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:44.081034 thoi-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-06-01 03:28:38.000000 thoi-0.1.8/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-06-01 03:28:38.000000 thoi-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-06-01 03:28:44.085034 thoi-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-06-01 03:28:38.000000 thoi-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 03:28:38.000000 thoi-0.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 03:28:44.085034 thoi-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-06-01 03:28:38.000000 thoi-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:44.081034 thoi-0.1.8/thoi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/collectors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/graph.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:44.081034 thoi-0.1.8/thoi/measures/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/measures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/measures/gaussian_copula.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:44.085034 thoi-0.1.8/thoi/synthetic_systems/
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/synthetic_systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/synthetic_systems/flat.py
--rw-r--r--   0 runner    (1001) docker     (127)      560 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/synthetic_systems/relu.py
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-06-01 03:28:38.000000 thoi-0.1.8/thoi/synthetic_systems/xor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:28:44.085034 thoi-0.1.8/thoi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-06-01 03:28:44.000000 thoi-0.1.8/thoi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-01 03:28:44.000000 thoi-0.1.8/thoi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 03:28:44.000000 thoi-0.1.8/thoi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-06-01 03:28:44.000000 thoi-0.1.8/thoi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-01 03:28:44.000000 thoi-0.1.8/thoi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:10:36.130428 thoi-0.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:10:36.126428 thoi-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:10:36.126428 thoi-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-06-01 04:10:20.000000 thoi-0.1.9/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-06-01 04:10:20.000000 thoi-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-06-01 04:10:36.130428 thoi-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-06-01 04:10:20.000000 thoi-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 04:10:20.000000 thoi-0.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 04:10:36.130428 thoi-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-06-01 04:10:20.000000 thoi-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:10:36.126428 thoi-0.1.9/thoi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:10:20.000000 thoi-0.1.9/thoi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2017 2024-06-01 04:10:20.000000 thoi-0.1.9/thoi/collectors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-06-01 04:10:20.000000 thoi-0.1.9/thoi/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2758 2024-06-01 04:10:20.000000 thoi-0.1.9/thoi/graph.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:10:36.130428 thoi-0.1.9/thoi/measures/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 04:10:20.000000 thoi-0.1.9/thoi/measures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7204 2024-06-01 04:10:20.000000 thoi-0.1.9/thoi/measures/gaussian_copula.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:10:36.130428 thoi-0.1.9/thoi/synthetic_systems/
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-06-01 04:10:20.000000 thoi-0.1.9/thoi/synthetic_systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-06-01 04:10:20.000000 thoi-0.1.9/thoi/synthetic_systems/flat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      560 2024-06-01 04:10:20.000000 thoi-0.1.9/thoi/synthetic_systems/relu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-06-01 04:10:20.000000 thoi-0.1.9/thoi/synthetic_systems/xor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:10:36.130428 thoi-0.1.9/thoi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-06-01 04:10:36.000000 thoi-0.1.9/thoi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-06-01 04:10:36.000000 thoi-0.1.9/thoi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 04:10:36.000000 thoi-0.1.9/thoi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-06-01 04:10:36.000000 thoi-0.1.9/thoi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-06-01 04:10:36.000000 thoi-0.1.9/thoi.egg-info/top_level.txt
```

### Comparing `thoi-0.1.8/.github/workflows/python-publish.yml` & `thoi-0.1.9/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `thoi-0.1.8/LICENSE` & `thoi-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `thoi-0.1.8/PKG-INFO` & `thoi-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: thoi
-Version: 0.1.8
+Version: 0.1.9
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
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: torch
 Requires-Dist: tqdm
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: networkx
+Provides-Extra: cpu
+Requires-Dist: torch==1.8.1+cpu; extra == "cpu"
 
 # O-information
 
 Authors: 
 * [Ruben Herzog](https://www.linkedin.com/in/rherzoga/)
 * [Laouen Belloli](https://www.linkedin.com/in/laouen-belloli/)
```

### Comparing `thoi-0.1.8/setup.py` & `thoi-0.1.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,20 +13,22 @@
     long_description_content_type='text/markdown',
     author='Laouen Mayal Louan Belloli, Ruben Herzog',
     author_email='laouen.belloli@gmail.com',
     url='https://github.com/Laouen/THOI',
     packages=find_packages(),
     install_requires=[
         'numpy',
-        'torch',
         'tqdm',
         'scipy',
         'pandas',
         'networkx'
     ],
+    extras_require={
+        'cpu': ['torch==1.8.1+cpu'],
+    },
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Intended Audience :: Developers',
         'Intended Audience :: Education',
         'Programming Language :: Python :: 3'
     ],
```

### Comparing `thoi-0.1.8/thoi/collectors.py` & `thoi-0.1.9/thoi/collectors.py`

 * *Files identical despite different names*

### Comparing `thoi-0.1.8/thoi/dataset.py` & `thoi-0.1.9/thoi/dataset.py`

 * *Files identical despite different names*

### Comparing `thoi-0.1.8/thoi/graph.py` & `thoi-0.1.9/thoi/graph.py`

 * *Files identical despite different names*

### Comparing `thoi-0.1.8/thoi/measures/gaussian_copula.py` & `thoi-0.1.9/thoi/measures/gaussian_copula.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,15 +142,15 @@
         pd.DataFrame: DataFrame containing computed metrics.
     """
 
     if batch_aggregation is None:
         batch_aggregation = lambda X: [x for x in X if x is not None]
 
     if batch_data_collector is None:
-        batch_data_collector = lambda x: x
+        batch_data_collector = lambda *args: args
 
     T, N = X.shape
     max_order = N if max_order is None else max_order
 
     assert max_order <= N, f"max_order must be lower or equal than N. {max_order} > {N})"
     assert min_order <= max_order, f"min_order must be lower or equal than max_order. {min_order} > {max_order}"
```

### Comparing `thoi-0.1.8/thoi/synthetic_systems/flat.py` & `thoi-0.1.9/thoi/synthetic_systems/flat.py`

 * *Files identical despite different names*

### Comparing `thoi-0.1.8/thoi/synthetic_systems/relu.py` & `thoi-0.1.9/thoi/synthetic_systems/relu.py`

 * *Files identical despite different names*

### Comparing `thoi-0.1.8/thoi.egg-info/PKG-INFO` & `thoi-0.1.9/thoi.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: thoi
-Version: 0.1.8
+Version: 0.1.9
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
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
-Requires-Dist: torch
 Requires-Dist: tqdm
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: networkx
+Provides-Extra: cpu
+Requires-Dist: torch==1.8.1+cpu; extra == "cpu"
 
 # O-information
 
 Authors: 
 * [Ruben Herzog](https://www.linkedin.com/in/rherzoga/)
 * [Laouen Belloli](https://www.linkedin.com/in/laouen-belloli/)
```

