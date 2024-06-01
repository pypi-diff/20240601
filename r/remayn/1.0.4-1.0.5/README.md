# Comparing `tmp/remayn-1.0.4.tar.gz` & `tmp/remayn-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remayn-1.0.4.tar", last modified: Mon May 27 17:55:01 2024, max compression
+gzip compressed data, was "remayn-1.0.5.tar", last modified: Sat Jun  1 13:32:22 2024, max compression
```

## Comparing `remayn-1.0.4.tar` & `remayn-1.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-27 17:55:01.856765 remayn-1.0.4/
--rw-r--r--   0 victor   (10038) ayrna     (1001)     1492 2024-04-25 06:08:28.000000 remayn-1.0.4/LICENSE
--rw-r--r--   0 victor   (10038) ayrna     (1001)     5938 2024-05-27 17:55:01.842503 remayn-1.0.4/PKG-INFO
--rw-r--r--   0 victor   (10038) ayrna     (1001)     5002 2024-05-27 10:17:57.000000 remayn-1.0.4/README.md
--rw-r--r--   0 victor   (10038) ayrna     (1001)     1068 2024-05-27 17:49:31.000000 remayn-1.0.4/pyproject.toml
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-27 17:55:01.501487 remayn-1.0.4/remayn/
--rw-r--r--   0 victor   (10038) ayrna     (1001)       35 2024-05-27 17:49:39.000000 remayn-1.0.4/remayn/__init__.py
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-27 17:55:01.605460 remayn-1.0.4/remayn/report/
--rw-r--r--   0 victor   (10038) ayrna     (1001)      161 2024-05-19 11:27:24.000000 remayn-1.0.4/remayn/report/__init__.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)     5387 2024-05-21 08:03:44.000000 remayn-1.0.4/remayn/report/excel.py
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-27 17:55:01.652580 remayn-1.0.4/remayn/result/
--rw-r--r--   0 victor   (10038) ayrna     (1001)      142 2024-05-01 12:37:43.000000 remayn-1.0.4/remayn/result/__init__.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)    18991 2024-05-19 09:56:20.000000 remayn-1.0.4/remayn/result/result.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)     4145 2024-05-27 11:28:38.000000 remayn-1.0.4/remayn/result/result_data.py
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-27 17:55:01.725468 remayn-1.0.4/remayn/result_set/
--rw-r--r--   0 victor   (10038) ayrna     (1001)      100 2024-05-07 11:34:45.000000 remayn-1.0.4/remayn/result_set/__init__.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)    17304 2024-05-27 17:47:22.000000 remayn-1.0.4/remayn/result_set/result_set.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)     5258 2024-05-21 08:05:29.000000 remayn-1.0.4/remayn/result_set/utils.py
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-27 17:55:01.788552 remayn-1.0.4/remayn/utils/
--rw-r--r--   0 victor   (10038) ayrna     (1001)      296 2024-05-27 11:28:39.000000 remayn-1.0.4/remayn/utils/__init__.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)      849 2024-05-27 11:28:39.000000 remayn-1.0.4/remayn/utils/array.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)     1635 2024-05-12 12:47:43.000000 remayn-1.0.4/remayn/utils/dicts.py
--rw-r--r--   0 victor   (10038) ayrna     (1001)     2008 2024-05-09 10:08:48.000000 remayn-1.0.4/remayn/utils/json.py
-drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-05-27 17:55:01.807418 remayn-1.0.4/remayn.egg-info/
--rw-r--r--   0 victor   (10038) ayrna     (1001)     5938 2024-05-27 17:55:01.000000 remayn-1.0.4/remayn.egg-info/PKG-INFO
--rw-r--r--   0 victor   (10038) ayrna     (1001)      516 2024-05-27 17:55:01.000000 remayn-1.0.4/remayn.egg-info/SOURCES.txt
--rw-r--r--   0 victor   (10038) ayrna     (1001)        1 2024-05-27 17:55:01.000000 remayn-1.0.4/remayn.egg-info/dependency_links.txt
--rw-r--r--   0 victor   (10038) ayrna     (1001)      111 2024-05-27 17:55:01.000000 remayn-1.0.4/remayn.egg-info/requires.txt
--rw-r--r--   0 victor   (10038) ayrna     (1001)        7 2024-05-27 17:55:01.000000 remayn-1.0.4/remayn.egg-info/top_level.txt
--rw-r--r--   0 victor   (10038) ayrna     (1001)       38 2024-05-27 17:55:01.857066 remayn-1.0.4/setup.cfg
--rw-r--r--   0 victor   (10038) ayrna     (1001)       38 2024-04-27 10:55:10.000000 remayn-1.0.4/setup.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-06-01 13:32:22.141043 remayn-1.0.5/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     1492 2024-04-25 06:08:28.000000 remayn-1.0.5/LICENSE
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     5938 2024-06-01 13:32:22.136301 remayn-1.0.5/PKG-INFO
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     5002 2024-05-27 10:17:57.000000 remayn-1.0.5/README.md
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     1068 2024-06-01 13:06:23.000000 remayn-1.0.5/pyproject.toml
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-06-01 13:32:22.044182 remayn-1.0.5/remayn/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)       35 2024-06-01 13:06:17.000000 remayn-1.0.5/remayn/__init__.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-06-01 13:32:22.080888 remayn-1.0.5/remayn/report/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      161 2024-05-19 11:27:24.000000 remayn-1.0.5/remayn/report/__init__.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     5387 2024-05-21 08:03:44.000000 remayn-1.0.5/remayn/report/excel.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-06-01 13:32:22.094770 remayn-1.0.5/remayn/result/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      142 2024-05-01 12:37:43.000000 remayn-1.0.5/remayn/result/__init__.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)    19109 2024-06-01 13:30:57.000000 remayn-1.0.5/remayn/result/result.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     4360 2024-06-01 13:03:25.000000 remayn-1.0.5/remayn/result/result_data.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-06-01 13:32:22.107827 remayn-1.0.5/remayn/result_set/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      100 2024-05-07 11:34:45.000000 remayn-1.0.5/remayn/result_set/__init__.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)    17304 2024-05-27 17:47:22.000000 remayn-1.0.5/remayn/result_set/result_set.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     5356 2024-06-01 13:03:46.000000 remayn-1.0.5/remayn/result_set/utils.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-06-01 13:32:22.124946 remayn-1.0.5/remayn/utils/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      296 2024-05-27 11:28:39.000000 remayn-1.0.5/remayn/utils/__init__.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      849 2024-05-27 11:28:39.000000 remayn-1.0.5/remayn/utils/array.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     1635 2024-05-12 12:47:43.000000 remayn-1.0.5/remayn/utils/dicts.py
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     2008 2024-05-09 10:08:48.000000 remayn-1.0.5/remayn/utils/json.py
+drwxr-xr-x   0 victor   (10038) ayrna     (1001)        0 2024-06-01 13:32:22.130051 remayn-1.0.5/remayn.egg-info/
+-rw-r--r--   0 victor   (10038) ayrna     (1001)     5938 2024-06-01 13:32:21.000000 remayn-1.0.5/remayn.egg-info/PKG-INFO
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      516 2024-06-01 13:32:22.000000 remayn-1.0.5/remayn.egg-info/SOURCES.txt
+-rw-r--r--   0 victor   (10038) ayrna     (1001)        1 2024-06-01 13:32:21.000000 remayn-1.0.5/remayn.egg-info/dependency_links.txt
+-rw-r--r--   0 victor   (10038) ayrna     (1001)      111 2024-06-01 13:32:21.000000 remayn-1.0.5/remayn.egg-info/requires.txt
+-rw-r--r--   0 victor   (10038) ayrna     (1001)        7 2024-06-01 13:32:21.000000 remayn-1.0.5/remayn.egg-info/top_level.txt
+-rw-r--r--   0 victor   (10038) ayrna     (1001)       38 2024-06-01 13:32:22.141529 remayn-1.0.5/setup.cfg
+-rw-r--r--   0 victor   (10038) ayrna     (1001)       38 2024-04-27 10:55:10.000000 remayn-1.0.5/setup.py
```

### Comparing `remayn-1.0.4/LICENSE` & `remayn-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `remayn-1.0.4/PKG-INFO` & `remayn-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remayn
-Version: 1.0.4
+Version: 1.0.5
 Summary: REsults MAde easY in pythoN
 Author-email: Víctor Manuel Vargas <vvargas@uco.es>
 Project-URL: Source, https://github.com/ayrna/remayn
 Project-URL: Documentation, https://remayn.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `remayn-1.0.4/README.md` & `remayn-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `remayn-1.0.4/pyproject.toml` & `remayn-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel", "toml", "build"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "remayn"
-version = "1.0.4"
+version = "1.0.5"
 authors = [
     {name = "Víctor Manuel Vargas", email = "vvargas@uco.es"},
 ]
 description = "REsults MAde easY in pythoN"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `remayn-1.0.4/remayn/report/excel.py` & `remayn-1.0.5/remayn/report/excel.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.4/remayn/result/result.py` & `remayn-1.0.5/remayn/result/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         Base path where all the experiments are stored.
     id: str
         Unique identifier of the experiment.
     config: dict
         Dictionary containing the parameters used in the experiment. All the elements
         in the dictionary must be JSON serializable. Objects contained in this dict
         should implement a custom __str__ method.
-    data_: Optional[ResultData]
+    data\\_: Optional[ResultData]
         Contains the `ResultData` when loaded or None if it was not loaded yet.
         This attribute should not be accessed directly. Use get_result() instead to
         make sure that the ResultData is properly loaded before accessing it.
     data_md5sum_: Optional[str]
         md5sum of the ResultData file. It is None if the file was not loaded yet or if
         creating a new Result that was not saved yet.
     created_at_: Optional[float]
@@ -175,31 +175,31 @@
             return sanitize_json(self.config) == sanitize_json(other)
         else:
             raise TypeError(
                 f"Expected a Result or a dict, but got {type(other)} instead."
             )
 
     def load_data(self, force=False):
-        """Load the ResultData from the disk.
-        This method reads the ResultData from the disk and stores it in the data_
+        """Load the `ResultData` from the disk.
+        This method reads the `ResultData` from the disk and stores it in the `data\\_`
         attribute. It also checks the integrity of the pickle file using the md5sum.
-        This method is called automatically by get_result() when the ResultData is
+        This method is called automatically by get_result() when the `ResultData` is
         needed. However, you can call it manually to force the loading of the file.
         If the file was already loaded, this method does nothing, unless force=True is
         passed as an argument.
 
         Parameters
         ----------
         force: bool, optional, default=False
             If True, the file will be loaded even if it was already loaded.
 
         Raises
         ------
         FileNotFoundError
-            If the ResultData does not exist.
+            If the `ResultData` does not exist.
         ValueError
             If the md5sum of the file does not match the one stored in the experiment
             information.
         """
 
         if self.data_ is not None and not force:
             return
@@ -235,40 +235,40 @@
         str
             The md5sum of the ResultData file.
         """
 
         return self.data_md5sum_
 
     def get_data(self, force_reload=False):
-        """Gets the ResultData of the experiment. If it was not loaded yet, it loads it
+        """Gets the `ResultData` of the experiment. If it was not loaded yet, it loads it
         from the disk. If the file was already loaded, it returns the stored object.
-        This method should be used to access the ResultData instead of accessing the
-        data_ attribute directly.
+        This method should be used to access the `ResultData` instead of accessing the
+        `data\\_` attribute directly.
 
         Parameters
         ----------
         force_reload: bool, optional, default=False
-            If True, the ResultData will be reloaded even if it was already loaded.
-            If False, it will only load the ResultData when it has not been loaded yet.
+            If True, the `ResultData` will be reloaded even if it was already loaded.
+            If False, it will only load the `ResultData` when it has not been loaded yet.
 
         Returns
         -------
         ResultData
-            The ResultData object containing the results of the experiment. None if the
-            ResultData is empty.
+            The `ResultData` object containing the results of the experiment. None if the
+            `ResultData` is empty.
         """
 
         if self.data_ is None or force_reload:
             self.load_data(force=force_reload)
 
         return self.data_
 
     def set_data(self, data: ResultData):
         """Sets the ResultData of the experiment.
-        This method should be used to set the ResultData instead of setting the data_
+        This method should be used to set the ResultData instead of setting the `data\\_`
         attribute directly.
 
         Parameters
         ----------
         data: ResultData
             The ResultData object containing the results of the experiment.
         """
@@ -333,14 +333,17 @@
 
         # Save experiment info
         experiment_info = self.get_experiment_info()
         safe_info = None
         try:
             safe_info = sanitize_json(experiment_info, accept_default_str=False)
         except NonDefaultStrMethodError:
+            # Remove pickle file if an error occurs
+            data_path.unlink()
+
             raise ValueError(
                 "Experiment info contains some fields that are subject to change when"
                 " the experiment is loaded from disk. Please, make sure that all the"
                 " elements within the config are JSON serializable and show a"
                 f" deterministic representation.\n{safe_info=}"
             )
```

### Comparing `remayn-1.0.4/remayn/result/result_data.py` & `remayn-1.0.5/remayn/result/result_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,59 +1,59 @@
-from typing import Optional
+from typing import Optional, Union
 
 import numpy as np
 
 from ..utils import check_array
 
 
 class ResultData:
     """Stores the results of a experiment.
     ResultData objects only contain data and are usually stored as pickle files.
 
     Attributes
     ----------
-    targets: np.ndarray
+    targets: Union[np.ndarray, list]
         Numpy array of target values for the test set.
-    predictions: np.ndarray
+    predictions: Union[np.ndarray, list]
         Numpy array of predicted values for the test set.
-    train_targets: Optional[np.ndarray], optional, default=None
+    train_targets: Optional[Union[np.ndarray, list]], optional, default=None
         Numpy array of target values for the training set.
-    train_predictions: Optional[np.ndarray], optional, default=None
+    train_predictions: Optional[Union[np.ndarray, list]], optional, default=None
         Numpy array of predicted values for the training set.
-    val_targets: Optional[np.ndarray], optional, default=None
+    val_targets: Optional[Union[np.ndarray, list]], optional, default=None
         Numpy array of target values for the validation set.
-    val_predictions: Optional[np.ndarray], optional, default=None
+    val_predictions: Optional[Union[np.ndarray, list]], optional, default=None
         Numpy array of predicted values for the validation set.
     time: float, optional, default=None
         Time taken to run the experiment.
-    train_history: Optional[np.ndarray], optional, default=None
+    train_history: Optional[Union[np.ndarray, list]], optional, default=None
         Training history of the model, represented as the value of the error on each
         iteration.
-    val_history: Optional[np.ndarray], optional, default=None
+    val_history: Optional[Union[np.ndarray, list]], optional, default=None
         Validation history of the model, represented as the value of the error on each
         iteration.
     best_params: Optional[dict], optional, default=None
         Dictionary of the best parameters found during the experiment.
         Can be used in case that the experiment employes a cross-validation process.
     best_model: Optional[object], optional, default=None
         Best model found during the experiment.
     """
 
     def __init__(
         self,
         *,
-        targets: np.ndarray,
-        predictions: np.ndarray,
-        train_targets: Optional[np.ndarray] = None,
-        train_predictions: Optional[np.ndarray] = None,
-        val_targets: Optional[np.ndarray] = None,
-        val_predictions: Optional[np.ndarray] = None,
+        targets: Union[np.ndarray, list],
+        predictions: Union[np.ndarray, list],
+        train_targets: Optional[Union[np.ndarray, list]] = None,
+        train_predictions: Optional[Union[np.ndarray, list]] = None,
+        val_targets: Optional[Union[np.ndarray, list]] = None,
+        val_predictions: Optional[Union[np.ndarray, list]] = None,
         time: Optional[float] = None,
-        train_history: Optional[np.ndarray] = None,
-        val_history: Optional[np.ndarray] = None,
+        train_history: Optional[Union[np.ndarray, list]] = None,
+        val_history: Optional[Union[np.ndarray, list]] = None,
         best_params: Optional[dict] = None,
         best_model: Optional[object] = None,
     ):
         targets = check_array(targets)
         predictions = check_array(predictions)
         train_targets = check_array(train_targets, allow_none=True)
         train_predictions = check_array(train_predictions, allow_none=True)
```

### Comparing `remayn-1.0.4/remayn/result_set/result_set.py` & `remayn-1.0.5/remayn/result_set/result_set.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.4/remayn/result_set/utils.py` & `remayn-1.0.5/remayn/result_set/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,16 +144,16 @@
             metrics_fn,
         )
         row = {**row, **val_metrics_row}
 
     row["time"] = time
 
     # Add best epoch and loss value if histories are available
-    if data.train_history is not None:
+    if isinstance(data.train_history, np.ndarray) and len(data.train_history.shape) > 0:
         row["best_train_epoch"] = data.train_history.argmin() + 1
         row["best_train_loss"] = data.train_history.min()
 
-    if data.val_history is not None:
+    if isinstance(data.val_history, np.ndarray) and len(data.val_history.shape) > 0:
         row["best_val_epoch"] = data.val_history.argmin() + 1
         row["best_val_loss"] = data.val_history.min()
 
     return row
```

### Comparing `remayn-1.0.4/remayn/utils/array.py` & `remayn-1.0.5/remayn/utils/array.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.4/remayn/utils/dicts.py` & `remayn-1.0.5/remayn/utils/dicts.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.4/remayn/utils/json.py` & `remayn-1.0.5/remayn/utils/json.py`

 * *Files identical despite different names*

### Comparing `remayn-1.0.4/remayn.egg-info/PKG-INFO` & `remayn-1.0.5/remayn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remayn
-Version: 1.0.4
+Version: 1.0.5
 Summary: REsults MAde easY in pythoN
 Author-email: Víctor Manuel Vargas <vvargas@uco.es>
 Project-URL: Source, https://github.com/ayrna/remayn
 Project-URL: Documentation, https://remayn.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
```

### Comparing `remayn-1.0.4/remayn.egg-info/SOURCES.txt` & `remayn-1.0.5/remayn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

