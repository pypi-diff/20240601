# Comparing `tmp/aggfly-0.1.2.tar.gz` & `tmp/aggfly-0.1.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aggfly-0.1.2.tar", max compression
+gzip compressed data, was "aggfly-0.1.2a0.tar", max compression
```

## Comparing `aggfly-0.1.2.tar` & `aggfly-0.1.2a0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11357 2024-05-31 18:56:17.825322 aggfly-0.1.2/LICENSE
--rw-r--r--   0        0        0     9754 2024-05-31 20:54:25.182789 aggfly-0.1.2/README.md
--rw-r--r--   0        0        0      727 2024-04-09 17:31:06.640231 aggfly-0.1.2/aggfly/__init__.py
--rw-r--r--   0        0        0      186 2023-11-15 02:07:57.896539 aggfly-0.1.2/aggfly/aggregate/__init__.py
--rw-r--r--   0        0        0     8480 2024-04-10 15:16:16.955244 aggfly-0.1.2/aggfly/aggregate/aggregate.py
--rw-r--r--   0        0        0     2296 2023-11-15 15:23:54.796559 aggfly-0.1.2/aggfly/aggregate/aggregate_utils.py
--rw-r--r--   0        0        0     5522 2024-04-09 18:58:18.372921 aggfly-0.1.2/aggfly/aggregate/spatial.py
--rw-r--r--   0        0        0     6382 2024-05-31 18:56:17.825322 aggfly-0.1.2/aggfly/aggregate/temporal.py
--rw-r--r--   0        0        0     3204 2023-11-05 21:38:29.962831 aggfly-0.1.2/aggfly/aggregate/z_old/spatial-Copy1.py
--rw-r--r--   0        0        0    16696 2023-11-05 21:38:29.962831 aggfly-0.1.2/aggfly/aggregate/z_old/temporal-Copy1.py
--rw-r--r--   0        0        0       72 2023-11-05 21:38:29.962831 aggfly-0.1.2/aggfly/cache/__init__.py
--rw-r--r--   0        0        0     4687 2024-05-31 18:56:17.825322 aggfly-0.1.2/aggfly/cache/project_cache.py
--rw-r--r--   0        0        0      108 2023-11-13 15:02:11.925887 aggfly-0.1.2/aggfly/dataset/__init__.py
--rw-r--r--   0        0        0    17959 2024-05-31 18:56:17.825322 aggfly-0.1.2/aggfly/dataset/dataset.py
--rw-r--r--   0        0        0     6964 2024-05-31 18:56:17.825322 aggfly-0.1.2/aggfly/dataset/grid.py
--rw-r--r--   0        0        0     5009 2023-11-16 02:11:10.922106 aggfly-0.1.2/aggfly/dataset/grid_utils.py
--rw-r--r--   0        0        0       79 2023-11-13 15:23:27.224464 aggfly-0.1.2/aggfly/regions/__init__.py
--rw-r--r--   0        0        0     7010 2024-06-01 13:23:08.680566 aggfly-0.1.2/aggfly/regions/georegions.py
--rw-r--r--   0        0        0     1411 2023-11-05 21:38:29.966832 aggfly-0.1.2/aggfly/regions/shp_utils.py
--rw-r--r--   0        0        0       29 2024-04-09 17:28:02.820266 aggfly-0.1.2/aggfly/tests/__init__.py
--rw-r--r--   0        0        0     4807 2024-05-31 18:03:36.223590 aggfly-0.1.2/aggfly/tests/test_aggregate.py
--rw-r--r--   0        0        0     1488 2024-05-31 18:56:17.825322 aggfly-0.1.2/aggfly/utils.py
--rw-r--r--   0        0        0      282 2024-02-18 18:50:06.939106 aggfly-0.1.2/aggfly/weights/__init__.py
--rw-r--r--   0        0        0     3105 2024-05-31 18:56:17.825322 aggfly-0.1.2/aggfly/weights/crop_weights.py
--rw-r--r--   0        0        0        0 2023-02-01 23:23:40.970310 aggfly-0.1.2/aggfly/weights/crop_weights_utils.py
--rw-r--r--   0        0        0    15387 2024-06-01 14:27:58.794839 aggfly-0.1.2/aggfly/weights/grid_weights.py
--rw-r--r--   0        0        0     2001 2024-05-31 18:56:17.825322 aggfly-0.1.2/aggfly/weights/pop_weights.py
--rw-r--r--   0        0        0     3656 2024-04-12 21:02:34.341449 aggfly-0.1.2/aggfly/weights/secondary_weights.py
--rw-r--r--   0        0        0     1068 2024-06-01 14:49:30.190914 aggfly-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    10770 1970-01-01 00:00:00.000000 aggfly-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-31 18:56:17.825322 aggfly-0.1.2a0/LICENSE
+-rw-r--r--   0        0        0     9754 2024-05-31 20:54:25.182789 aggfly-0.1.2a0/README.md
+-rw-r--r--   0        0        0      727 2024-04-09 17:31:06.640231 aggfly-0.1.2a0/aggfly/__init__.py
+-rw-r--r--   0        0        0      186 2023-11-15 02:07:57.896539 aggfly-0.1.2a0/aggfly/aggregate/__init__.py
+-rw-r--r--   0        0        0     8480 2024-04-10 15:16:16.955244 aggfly-0.1.2a0/aggfly/aggregate/aggregate.py
+-rw-r--r--   0        0        0     2296 2023-11-15 15:23:54.796559 aggfly-0.1.2a0/aggfly/aggregate/aggregate_utils.py
+-rw-r--r--   0        0        0     5522 2024-04-09 18:58:18.372921 aggfly-0.1.2a0/aggfly/aggregate/spatial.py
+-rw-r--r--   0        0        0     6382 2024-05-31 18:56:17.825322 aggfly-0.1.2a0/aggfly/aggregate/temporal.py
+-rw-r--r--   0        0        0     3204 2023-11-05 21:38:29.962831 aggfly-0.1.2a0/aggfly/aggregate/z_old/spatial-Copy1.py
+-rw-r--r--   0        0        0    16696 2023-11-05 21:38:29.962831 aggfly-0.1.2a0/aggfly/aggregate/z_old/temporal-Copy1.py
+-rw-r--r--   0        0        0       72 2023-11-05 21:38:29.962831 aggfly-0.1.2a0/aggfly/cache/__init__.py
+-rw-r--r--   0        0        0     4687 2024-05-31 18:56:17.825322 aggfly-0.1.2a0/aggfly/cache/project_cache.py
+-rw-r--r--   0        0        0      108 2023-11-13 15:02:11.925887 aggfly-0.1.2a0/aggfly/dataset/__init__.py
+-rw-r--r--   0        0        0    17959 2024-05-31 18:56:17.825322 aggfly-0.1.2a0/aggfly/dataset/dataset.py
+-rw-r--r--   0        0        0     6964 2024-05-31 18:56:17.825322 aggfly-0.1.2a0/aggfly/dataset/grid.py
+-rw-r--r--   0        0        0     5009 2023-11-16 02:11:10.922106 aggfly-0.1.2a0/aggfly/dataset/grid_utils.py
+-rw-r--r--   0        0        0       79 2023-11-13 15:23:27.224464 aggfly-0.1.2a0/aggfly/regions/__init__.py
+-rw-r--r--   0        0        0     7006 2024-06-01 14:52:09.550317 aggfly-0.1.2a0/aggfly/regions/georegions.py
+-rw-r--r--   0        0        0     1411 2023-11-05 21:38:29.966832 aggfly-0.1.2a0/aggfly/regions/shp_utils.py
+-rw-r--r--   0        0        0       29 2024-04-09 17:28:02.820266 aggfly-0.1.2a0/aggfly/tests/__init__.py
+-rw-r--r--   0        0        0     4807 2024-05-31 18:03:36.223590 aggfly-0.1.2a0/aggfly/tests/test_aggregate.py
+-rw-r--r--   0        0        0     1488 2024-05-31 18:56:17.825322 aggfly-0.1.2a0/aggfly/utils.py
+-rw-r--r--   0        0        0      282 2024-02-18 18:50:06.939106 aggfly-0.1.2a0/aggfly/weights/__init__.py
+-rw-r--r--   0        0        0     3105 2024-05-31 18:56:17.825322 aggfly-0.1.2a0/aggfly/weights/crop_weights.py
+-rw-r--r--   0        0        0        0 2023-02-01 23:23:40.970310 aggfly-0.1.2a0/aggfly/weights/crop_weights_utils.py
+-rw-r--r--   0        0        0    15332 2024-06-01 14:50:54.880723 aggfly-0.1.2a0/aggfly/weights/grid_weights.py
+-rw-r--r--   0        0        0     2001 2024-05-31 18:56:17.825322 aggfly-0.1.2a0/aggfly/weights/pop_weights.py
+-rw-r--r--   0        0        0     3656 2024-04-12 21:02:34.341449 aggfly-0.1.2a0/aggfly/weights/secondary_weights.py
+-rw-r--r--   0        0        0     1069 2024-06-01 14:52:19.942539 aggfly-0.1.2a0/pyproject.toml
+-rw-r--r--   0        0        0    10772 1970-01-01 00:00:00.000000 aggfly-0.1.2a0/PKG-INFO
```

### Comparing `aggfly-0.1.2/LICENSE` & `aggfly-0.1.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/README.md` & `aggfly-0.1.2a0/README.md`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/__init__.py` & `aggfly-0.1.2a0/aggfly/__init__.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/aggregate/aggregate.py` & `aggfly-0.1.2a0/aggfly/aggregate/aggregate.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/aggregate/aggregate_utils.py` & `aggfly-0.1.2a0/aggfly/aggregate/aggregate_utils.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/aggregate/spatial.py` & `aggfly-0.1.2a0/aggfly/aggregate/spatial.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/aggregate/temporal.py` & `aggfly-0.1.2a0/aggfly/aggregate/temporal.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/aggregate/z_old/spatial-Copy1.py` & `aggfly-0.1.2a0/aggfly/aggregate/z_old/spatial-Copy1.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/aggregate/z_old/temporal-Copy1.py` & `aggfly-0.1.2a0/aggfly/aggregate/z_old/temporal-Copy1.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/cache/project_cache.py` & `aggfly-0.1.2a0/aggfly/cache/project_cache.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/dataset/dataset.py` & `aggfly-0.1.2a0/aggfly/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/dataset/grid.py` & `aggfly-0.1.2a0/aggfly/dataset/grid.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/dataset/grid_utils.py` & `aggfly-0.1.2a0/aggfly/dataset/grid_utils.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/regions/georegions.py` & `aggfly-0.1.2a0/aggfly/regions/georegions.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,16 @@
 import warnings
 
 from .shp_utils import *
 
 # Weird bug in pyproj or geopandas that results in inf values the first time
 # a shapefile is loaded.. only for certain installations of PROJ
 # https://github.com/arup-group/genet/issues/213
-# import pyproj
-# pyproj.network.set_network_enabled(False)
+import pyproj
+pyproj.network.set_network_enabled(False)
 
 
 class GeoRegions:
     """
     A class used to represent geographical regions.
 
     Attributes
```

### Comparing `aggfly-0.1.2/aggfly/regions/shp_utils.py` & `aggfly-0.1.2a0/aggfly/regions/shp_utils.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/tests/test_aggregate.py` & `aggfly-0.1.2a0/aggfly/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/utils.py` & `aggfly-0.1.2a0/aggfly/utils.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/weights/crop_weights.py` & `aggfly-0.1.2a0/aggfly/weights/crop_weights.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/weights/grid_weights.py` & `aggfly-0.1.2a0/aggfly/weights/grid_weights.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 from ..dataset import Dataset, Grid, array_lon_to_360
 from . import CropWeights, PopWeights
 from . import crop_weights, pop_weights
 from ..utils import *
 from ..cache import *
 from ..aggregate import is_distributed, shutdown_dask_client, start_dask_client
 
-# dask.config.set({"dataframe.query-planning": False})
 
 class GridWeights:
     def __init__(
         self,
         grid: Grid,
         georegions: GeoRegions,
         raster_weights: Optional[Union[CropWeights, PopWeights]] = None,
```

### Comparing `aggfly-0.1.2/aggfly/weights/pop_weights.py` & `aggfly-0.1.2a0/aggfly/weights/pop_weights.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/aggfly/weights/secondary_weights.py` & `aggfly-0.1.2a0/aggfly/weights/secondary_weights.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.2/pyproject.toml` & `aggfly-0.1.2a0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "aggfly"
-version = "0.1.2"
+version = "0.1.2a"
 description = "Efficient spatial and temporal aggregation of gridded climate data"
 authors = ["Dylan Hogan <dth2133@columbia.edu>"]
 readme = "README.md"
 packages = [{include = "aggfly"}]
 
 
 # 3.12.3 causing issues with dask and dask-geopandas
```

### Comparing `aggfly-0.1.2/PKG-INFO` & `aggfly-0.1.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aggfly
-Version: 0.1.2
+Version: 0.1.2a0
 Summary: Efficient spatial and temporal aggregation of gridded climate data
 Author: Dylan Hogan
 Author-email: dth2133@columbia.edu
 Requires-Python: >=3.11.6,<3.12.3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dask (>=2023.11.0,<2024.0.0)
```

