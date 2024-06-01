# Comparing `tmp/beforerr-2024.5.30.tar.gz` & `tmp/beforerr-2024.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beforerr-2024.5.30.tar", last modified: Thu May 30 22:44:44 2024, max compression
+gzip compressed data, was "beforerr-2024.6.1.tar", last modified: Sat Jun  1 07:03:20 2024, max compression
```

## Comparing `beforerr-2024.5.30.tar` & `beforerr-2024.6.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11337 2023-04-27 10:12:58.000000 beforerr-2024.5.30/LICENSE
--rw-r--r--   0        0        0      185 2024-05-30 20:42:04.877118 beforerr-2024.5.30/README.md
--rw-r--r--   0        0        0       25 2024-05-30 22:14:38.279086 beforerr-2024.5.30/beforerr/__init__.py
--rw-r--r--   0        0        0     2609 2024-05-30 21:25:24.448237 beforerr-2024.5.30/beforerr/_modidx.py
--rw-r--r--   0        0        0      338 2024-05-30 21:25:23.994230 beforerr-2024.5.30/beforerr/basics.py
--rw-r--r--   0        0        0      214 2024-05-30 21:25:23.993466 beforerr-2024.5.30/beforerr/core.py
--rw-r--r--   0        0        0      965 2024-05-30 21:25:23.996239 beforerr-2024.5.30/beforerr/matplotlib.py
--rw-r--r--   0        0        0     2394 2024-05-30 21:25:23.998261 beforerr-2024.5.30/beforerr/polars.py
--rw-r--r--   0        0        0     5200 2024-05-30 21:25:24.001286 beforerr-2024.5.30/beforerr/project.py
--rw-r--r--   0        0        0      811 2024-05-30 21:25:23.995358 beforerr-2024.5.30/beforerr/r.py
--rw-r--r--   0        0        0      956 2024-05-30 22:44:44.822745 beforerr-2024.5.30/pyproject.toml
--rw-r--r--   0        0        0      658 1970-01-01 00:00:00.000000 beforerr-2024.5.30/PKG-INFO
+-rw-r--r--   0        0        0    11337 2024-03-29 05:10:27.069558 beforerr-2024.6.1/LICENSE
+-rw-r--r--   0        0        0      185 2024-05-31 23:01:42.632680 beforerr-2024.6.1/README.md
+-rw-r--r--   0        0        0       24 2024-06-01 07:03:19.687102 beforerr-2024.6.1/beforerr/__init__.py
+-rw-r--r--   0        0        0     2609 2024-06-01 07:03:19.692046 beforerr-2024.6.1/beforerr/_modidx.py
+-rw-r--r--   0        0        0      338 2024-06-01 07:03:19.678235 beforerr-2024.6.1/beforerr/basics.py
+-rw-r--r--   0        0        0      214 2024-06-01 07:03:19.677426 beforerr-2024.6.1/beforerr/core.py
+-rw-r--r--   0        0        0      965 2024-06-01 07:03:19.680479 beforerr-2024.6.1/beforerr/matplotlib.py
+-rw-r--r--   0        0        0     3546 2024-06-01 07:03:19.683037 beforerr-2024.6.1/beforerr/polars.py
+-rw-r--r--   0        0        0     5504 2024-06-01 07:03:19.686381 beforerr-2024.6.1/beforerr/project.py
+-rw-r--r--   0        0        0      811 2024-06-01 07:03:19.679199 beforerr-2024.6.1/beforerr/r.py
+-rw-r--r--   0        0        0      955 2024-06-01 07:03:20.955535 beforerr-2024.6.1/pyproject.toml
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 beforerr-2024.6.1/PKG-INFO
```

### Comparing `beforerr-2024.5.30/LICENSE` & `beforerr-2024.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `beforerr-2024.5.30/beforerr/_modidx.py` & `beforerr-2024.6.1/beforerr/_modidx.py`

 * *Files identical despite different names*

### Comparing `beforerr-2024.5.30/beforerr/matplotlib.py` & `beforerr-2024.6.1/beforerr/matplotlib.py`

 * *Files identical despite different names*

### Comparing `beforerr-2024.5.30/beforerr/project.py` & `beforerr-2024.6.1/beforerr/project.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: ../nbs/11_projects.ipynb.
 
 # %% auto 0
-__all__ = ['projectdir', 'datadir', 'savename', 'setup_run_dir', 'increment_backup_num', 'safesave']
+__all__ = ['projectdir', 'datadir', 'savename', 'setup_run_dir', 'safesave']
 
 # %% ../nbs/11_projects.ipynb 1
 import os
 from pathlib import Path
 import warnings
 from typing import Any, Callable, Dict, List, Tuple, Union
 from loguru import logger
@@ -34,45 +34,61 @@
 def savename(
     c: Dict,
     prefix: str = "",
     suffix: str = "",
     allowedtypes: Tuple = (int, float, str, bool),
     accesses: List[str] = [],
     ignores: List[str] = [],
-    digits: Union[int, None] = None,
+    digits: int = None,
     connector: str = "_",
+    equals: str = "=",
     expand: List[str] = [],
     sigdigits: int = 3,
     val2string: Callable = None,
     sort: bool = True,
-    equals: str = "=",
 ) -> str:
     """
     Create a shorthand name based on the parameters in the dictionary `c`.
-    
-    Parameters:
-        c (Dict): The input dictionary containing the parameters.
-        prefix (str): The prefix to start the name with.
-        suffix (str): The suffix to end the name with.
-        allowedtypes (Tuple): Only values of these types are included.
-        accesses (List[str]): Specific keys to include in the name.
-        ignores (List[str]): Specific keys to ignore.
-        digits (Union[int, None]): Number of decimal digits for rounding floats.
-        connector (str): String used to connect key-value pairs.
-        expand (List[str]): Keys that will be expanded to their nested savename.
-        sigdigits (int): Number of significant digits for rounding floats.
-        val_to_string (Callable): Function to convert values to strings.
-        sort (bool): Whether to sort the keys alphabetically.
-        equals (str): Connector between key and value.
 
-    Returns:
-        str: The generated shorthand name.
+    Parameters
+    ----------
+    c : Dict
+        The input dictionary containing the parameters.
+    prefix : str, optional
+        The prefix to start the name with.
+    suffix : str, optional
+        The suffix to end the name with.
+    allowedtypes : Tuple, optional
+        Only values of these types are included. (default: (int, float, str, bool))
+    accesses : List[str], optional
+        Specific keys to include in the name.
+    ignores : List[str], optional
+        Specific keys to ignore.
+    digits : Union[int, None], optional
+        Number of decimal digits for rounding floats.
+    connector : str, optional
+        String used to connect key-value pairs.
+    equals : str, optional
+        Connector between key and value.
+    expand : List[str], optional
+        Keys that will be expanded to their nested savename.
+    sigdigits : int, optional
+        Number of significant digits for rounding floats.
+    val2string : Callable, optional
+        Function to convert values to strings.
+    sort : bool, optional
+        Whether to sort the keys alphabetically.
+
+
+    Returns
+    -------
+    str
+        The generated shorthand name.
     """
 
-
     if any(sep in prefix for sep in ["/", "\\"]):
         warnings.warn(
             "Path separators in `savename` prefixes may break reproducibility on other OS. "
             "The recommended way is using `os.path.join` with `savename` (e.g. `os.path.join(datadir, savename(prefix, data))`)."
         )
 
     sigdigits = None if digits is not None else sigdigits
@@ -116,46 +132,51 @@
 
     if suffix:
         s += f".{suffix}"
 
     return s
 
 # %% ../nbs/11_projects.ipynb 7
-def setup_run_dir(c: Dict, base_dir: Path = datadir(), change_dir: bool = True, **kwargs):
+def setup_run_dir(c: Dict, base_dir: Callable = datadir, change_dir: bool = True, **kwargs):
     """
     Create a run directory based on the parameters in the dictionary `c`.
 
-    Parameters:
-        c (Dict): The dictionary containing the parameters.
-        base_dir (Path): The base directory to create the run directory in.
-
-    Returns:
-        Path: The run directory.
+    Parameters
+    ----------
+    c
+        The dictionary containing the parameters.
+    base_dir
+        The base directory to create the run directory in.
+
+    Returns
+    -------
+    Path
+        The run directory.
     """
 
     sub_dir = savename(c, **kwargs)
+    base_dir = Path(base_dir()) if callable(base_dir) else Path(base_dir)
     directory = base_dir / sub_dir
     os.makedirs(directory, exist_ok=True)
     if change_dir:
         os.chdir(directory)
         logger.info(f"Changed directory to {directory}")
 
 # %% ../nbs/11_projects.ipynb 8
 import shutil
 
-
 def increment_backup_num(filepath: Path):
     if "_" in filepath.stem and filepath.stem.rsplit("_", 1)[-1].isdigit():
         base, num = filepath.stem.rsplit("_", 1)
         new_num = int(num) + 1
     else:
         base, new_num = filepath.stem, 1
     return filepath.with_name(f"{base}_{new_num}{filepath.suffix}")
 
-
+# %% ../nbs/11_projects.ipynb 9
 def safesave(filepath: Path, data, save_func: Callable):
     if filepath.exists():
         backup_path = increment_backup_num(filepath)
         while backup_path.exists():
             backup_path = increment_backup_num(backup_path)
         shutil.move(str(filepath), str(backup_path))
     return save_func(filepath, data)
```

### Comparing `beforerr-2024.5.30/beforerr/r.py` & `beforerr-2024.6.1/beforerr/r.py`

 * *Files identical despite different names*

### Comparing `beforerr-2024.5.30/pyproject.toml` & `beforerr-2024.6.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ]
 requires-python = ">= 3.10"
 dependencies = [
     "pipe",
     "loguru",
 ]
 readme = "README.md"
-version = "2024.5.30"
+version = "2024.6.1"
 
 [project.optional-dependencies]
 r = [
     "rpy2",
     "rpy2_arrow",
 ]
```

### Comparing `beforerr-2024.5.30/PKG-INFO` & `beforerr-2024.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: beforerr
-Version: 2024.5.30
+Version: 2024.6.1
 Summary: Personal Python utility library
 Author-Email: Beforerr <zzj956959688@gmail.com>
 Project-URL: Homepage, https://beforerr.github.io/beforerr_dev
 Project-URL: Repository, https://github.com/beforerr/beforerr_dev
 Requires-Python: >=3.10
 Requires-Dist: pipe
 Requires-Dist: loguru
```
