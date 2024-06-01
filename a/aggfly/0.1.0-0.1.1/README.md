# Comparing `tmp/aggfly-0.1.0.tar.gz` & `tmp/aggfly-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aggfly-0.1.0.tar", max compression
+gzip compressed data, was "aggfly-0.1.1.tar", max compression
```

## Comparing `aggfly-0.1.0.tar` & `aggfly-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11357 2024-05-31 17:29:33.970357 aggfly-0.1.0/LICENSE
--rw-r--r--   0        0        0     1111 2024-04-09 17:16:33.445901 aggfly-0.1.0/README.md
--rw-r--r--   0        0        0      727 2024-04-09 17:31:06.640231 aggfly-0.1.0/aggfly/__init__.py
--rw-r--r--   0        0        0      186 2023-11-15 02:07:57.896539 aggfly-0.1.0/aggfly/aggregate/__init__.py
--rw-r--r--   0        0        0     8480 2024-04-10 15:16:16.955244 aggfly-0.1.0/aggfly/aggregate/aggregate.py
--rw-r--r--   0        0        0     2296 2023-11-15 15:23:54.796559 aggfly-0.1.0/aggfly/aggregate/aggregate_utils.py
--rw-r--r--   0        0        0     5522 2024-04-09 18:58:18.372921 aggfly-0.1.0/aggfly/aggregate/spatial.py
--rw-r--r--   0        0        0     6380 2024-05-08 14:35:41.415864 aggfly-0.1.0/aggfly/aggregate/temporal.py
--rw-r--r--   0        0        0     3204 2023-11-05 21:38:29.962831 aggfly-0.1.0/aggfly/aggregate/z_old/spatial-Copy1.py
--rw-r--r--   0        0        0    16696 2023-11-05 21:38:29.962831 aggfly-0.1.0/aggfly/aggregate/z_old/temporal-Copy1.py
--rw-r--r--   0        0        0       72 2023-11-05 21:38:29.962831 aggfly-0.1.0/aggfly/cache/__init__.py
--rw-r--r--   0        0        0     4779 2023-11-05 21:38:29.962831 aggfly-0.1.0/aggfly/cache/project_cache.py
--rw-r--r--   0        0        0      108 2023-11-13 15:02:11.925887 aggfly-0.1.0/aggfly/dataset/__init__.py
--rw-r--r--   0        0        0    17788 2024-05-09 15:20:18.081105 aggfly-0.1.0/aggfly/dataset/dataset.py
--rw-r--r--   0        0        0     6957 2023-11-15 03:15:33.469303 aggfly-0.1.0/aggfly/dataset/grid.py
--rw-r--r--   0        0        0     5009 2023-11-16 02:11:10.922106 aggfly-0.1.0/aggfly/dataset/grid_utils.py
--rw-r--r--   0        0        0       79 2023-11-13 15:23:27.224464 aggfly-0.1.0/aggfly/regions/__init__.py
--rw-r--r--   0        0        0     6712 2024-04-12 20:54:47.807511 aggfly-0.1.0/aggfly/regions/georegions.py
--rw-r--r--   0        0        0     1411 2023-11-05 21:38:29.966832 aggfly-0.1.0/aggfly/regions/shp_utils.py
--rw-r--r--   0        0        0       29 2024-04-09 17:28:02.820266 aggfly-0.1.0/aggfly/tests/__init__.py
--rw-r--r--   0        0        0     4807 2024-04-12 21:05:10.796782 aggfly-0.1.0/aggfly/tests/test_aggregate.py
--rw-r--r--   0        0        0     1485 2023-11-05 21:38:29.966832 aggfly-0.1.0/aggfly/utils.py
--rw-r--r--   0        0        0      282 2024-02-18 18:50:06.939106 aggfly-0.1.0/aggfly/weights/__init__.py
--rw-r--r--   0        0        0     3182 2024-02-29 21:17:40.113926 aggfly-0.1.0/aggfly/weights/crop_weights.py
--rw-r--r--   0        0        0        0 2023-02-01 23:23:40.970310 aggfly-0.1.0/aggfly/weights/crop_weights_utils.py
--rw-r--r--   0        0        0    15332 2024-04-12 21:03:49.875059 aggfly-0.1.0/aggfly/weights/grid_weights.py
--rw-r--r--   0        0        0     2043 2024-02-29 21:17:58.286297 aggfly-0.1.0/aggfly/weights/pop_weights.py
--rw-r--r--   0        0        0     3656 2024-04-12 21:02:34.341449 aggfly-0.1.0/aggfly/weights/secondary_weights.py
--rw-r--r--   0        0        0      681 2024-05-31 17:15:34.761573 aggfly-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2116 1970-01-01 00:00:00.000000 aggfly-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-31 18:56:17.825322 aggfly-0.1.1/LICENSE
+-rw-r--r--   0        0        0     9754 2024-05-31 20:54:25.182789 aggfly-0.1.1/README.md
+-rw-r--r--   0        0        0      727 2024-04-09 17:31:06.640231 aggfly-0.1.1/aggfly/__init__.py
+-rw-r--r--   0        0        0      186 2023-11-15 02:07:57.896539 aggfly-0.1.1/aggfly/aggregate/__init__.py
+-rw-r--r--   0        0        0     8480 2024-04-10 15:16:16.955244 aggfly-0.1.1/aggfly/aggregate/aggregate.py
+-rw-r--r--   0        0        0     2296 2023-11-15 15:23:54.796559 aggfly-0.1.1/aggfly/aggregate/aggregate_utils.py
+-rw-r--r--   0        0        0     5522 2024-04-09 18:58:18.372921 aggfly-0.1.1/aggfly/aggregate/spatial.py
+-rw-r--r--   0        0        0     6382 2024-05-31 18:56:17.825322 aggfly-0.1.1/aggfly/aggregate/temporal.py
+-rw-r--r--   0        0        0     3204 2023-11-05 21:38:29.962831 aggfly-0.1.1/aggfly/aggregate/z_old/spatial-Copy1.py
+-rw-r--r--   0        0        0    16696 2023-11-05 21:38:29.962831 aggfly-0.1.1/aggfly/aggregate/z_old/temporal-Copy1.py
+-rw-r--r--   0        0        0       72 2023-11-05 21:38:29.962831 aggfly-0.1.1/aggfly/cache/__init__.py
+-rw-r--r--   0        0        0     4687 2024-05-31 18:56:17.825322 aggfly-0.1.1/aggfly/cache/project_cache.py
+-rw-r--r--   0        0        0      108 2023-11-13 15:02:11.925887 aggfly-0.1.1/aggfly/dataset/__init__.py
+-rw-r--r--   0        0        0    17959 2024-05-31 18:56:17.825322 aggfly-0.1.1/aggfly/dataset/dataset.py
+-rw-r--r--   0        0        0     6964 2024-05-31 18:56:17.825322 aggfly-0.1.1/aggfly/dataset/grid.py
+-rw-r--r--   0        0        0     5009 2023-11-16 02:11:10.922106 aggfly-0.1.1/aggfly/dataset/grid_utils.py
+-rw-r--r--   0        0        0       79 2023-11-13 15:23:27.224464 aggfly-0.1.1/aggfly/regions/__init__.py
+-rw-r--r--   0        0        0     7006 2024-05-31 18:56:17.825322 aggfly-0.1.1/aggfly/regions/georegions.py
+-rw-r--r--   0        0        0     1411 2023-11-05 21:38:29.966832 aggfly-0.1.1/aggfly/regions/shp_utils.py
+-rw-r--r--   0        0        0       29 2024-04-09 17:28:02.820266 aggfly-0.1.1/aggfly/tests/__init__.py
+-rw-r--r--   0        0        0     4807 2024-05-31 18:03:36.223590 aggfly-0.1.1/aggfly/tests/test_aggregate.py
+-rw-r--r--   0        0        0     1488 2024-05-31 18:56:17.825322 aggfly-0.1.1/aggfly/utils.py
+-rw-r--r--   0        0        0      282 2024-02-18 18:50:06.939106 aggfly-0.1.1/aggfly/weights/__init__.py
+-rw-r--r--   0        0        0     3105 2024-05-31 18:56:17.825322 aggfly-0.1.1/aggfly/weights/crop_weights.py
+-rw-r--r--   0        0        0        0 2023-02-01 23:23:40.970310 aggfly-0.1.1/aggfly/weights/crop_weights_utils.py
+-rw-r--r--   0        0        0    15332 2024-04-12 21:03:49.875059 aggfly-0.1.1/aggfly/weights/grid_weights.py
+-rw-r--r--   0        0        0     2001 2024-05-31 18:56:17.825322 aggfly-0.1.1/aggfly/weights/pop_weights.py
+-rw-r--r--   0        0        0     3656 2024-04-12 21:02:34.341449 aggfly-0.1.1/aggfly/weights/secondary_weights.py
+-rw-r--r--   0        0        0      689 2024-06-01 12:51:22.985566 aggfly-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0    10767 1970-01-01 00:00:00.000000 aggfly-0.1.1/PKG-INFO
```

### Comparing `aggfly-0.1.0/LICENSE` & `aggfly-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.0/aggfly/__init__.py` & `aggfly-0.1.1/aggfly/__init__.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.0/aggfly/aggregate/aggregate.py` & `aggfly-0.1.1/aggfly/aggregate/aggregate.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.0/aggfly/aggregate/aggregate_utils.py` & `aggfly-0.1.1/aggfly/aggregate/aggregate_utils.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.0/aggfly/aggregate/spatial.py` & `aggfly-0.1.1/aggfly/aggregate/spatial.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.0/aggfly/aggregate/temporal.py` & `aggfly-0.1.1/aggfly/aggregate/temporal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from copy import deepcopy
 import os
-os.environ['USE_PYGEOS'] = '0'
+# os.environ['USE_PYGEOS'] = '0'
 
 import numpy as np
 import dask.array as da
 from .aggregate_utils import *
 from ..dataset import Dataset, array_lon_to_360
 from ..weights import GridWeights
```

### Comparing `aggfly-0.1.0/aggfly/aggregate/z_old/spatial-Copy1.py` & `aggfly-0.1.1/aggfly/aggregate/z_old/spatial-Copy1.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.0/aggfly/aggregate/z_old/temporal-Copy1.py` & `aggfly-0.1.1/aggfly/aggregate/z_old/temporal-Copy1.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.0/aggfly/cache/project_cache.py` & `aggfly-0.1.1/aggfly/cache/project_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,21 +10,15 @@
 from pprint import pformat, pprint
 
 import dill as pickle
 import numpy as np
 import pandas as pd
 import xarray as xr
 import geopandas as gpd
-import pygeos
-import dask
-import dask.array
-import rasterio
 from rasterio.enums import Resampling
-import rioxarray
-import pathlib
 import yaml
 
 
 class ProjectCache:
     def __init__(self, project_dir, module_type, module_dict, reset=False):
         self.project_dir = project_dir
         self.module_type = module_type
```

### Comparing `aggfly-0.1.0/aggfly/dataset/dataset.py` & `aggfly-0.1.1/aggfly/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,38 +68,39 @@
         georegions : GeoRegions, optional
             The geographical regions associated with the dataset (default is None).
         time_fix : bool, optional
             A flag indicating if the time needs to be fixed (default is False).
         name : str, optional
             The name of the dataset (default is None).
         """
+        
+        with dask.config.set(**{"array.slicing.split_large_chunks": False}):  
+            da = clean_dims(da, xycoords)
+            da = da.sortby("time")
+            if time_sel is not None:
+                da = da.sortby("time").sel(time=time_sel)
+                # time_fix=True
+            if preprocess is not None:
+                da = preprocess(da)
 
-        da = clean_dims(da, xycoords)
-        da = da.sortby("time")
-        if time_sel is not None:
-            da = da.sortby("time").sel(time=time_sel)
-            # time_fix=True
-        if preprocess is not None:
-            da = preprocess(da)
+            self.update(da, init=True)
+            self.name = name
+            self.lon_is_360 = lon_is_360
+            self.coords = self.da.coords
 
-        self.update(da, init=True)
-        self.name = name
-        self.lon_is_360 = lon_is_360
-        self.coords = self.da.coords
-
-        self.longitude = self.da.longitude
-        self.latitude = self.da.latitude
-        assert np.all([x in list(self.coords) for x in ["latitude", "longitude"]])
-        self.grid = Grid(self.longitude, self.latitude, self.name, self.lon_is_360)
-        self.history = []
-        self.georegions = georegions
-        if self.georegions is not None:
-            self.clip_data_to_georegions_extent(self.georegions)
-        if time_fix:
-            self.update(timefix(self.da), init=True)
+            self.longitude = self.da.longitude
+            self.latitude = self.da.latitude
+            assert np.all([x in list(self.coords) for x in ["latitude", "longitude"]])
+            self.grid = Grid(self.longitude, self.latitude, self.name, self.lon_is_360)
+            self.history = []
+            self.georegions = georegions
+            if self.georegions is not None:
+                self.clip_data_to_georegions_extent(self.georegions)
+            if time_fix:
+                self.update(timefix(self.da), init=True)
 
     def rechunk(self, chunks: str = "auto"):
         """
         Rechunks the data array.
 
         Parameters
         ----------
```

### Comparing `aggfly-0.1.0/aggfly/dataset/grid.py` & `aggfly-0.1.1/aggfly/dataset/grid.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import numpy as np
 import pandas as pd
 import xarray as xr
-import pygeos
+import shapely
 import geopandas as gpd
 import os
 import dask
 import dask.array
 import dask_geopandas
 from functools import lru_cache
 import warnings
@@ -30,16 +30,16 @@
         centroids = reformat_grid(self.lon_array, self.lat_array, datatype, chunks)
         return centroids
 
     def get_resolution(self):
         return abs(np.diff(self.latitude).mean())
 
     def get_cell_area(self):
-        cell = pygeos.box(0, 0, self.resolution, self.resolution)
-        return pygeos.area(cell)
+        cell = shapely.box(0, 0, self.resolution, self.resolution)
+        return shapely.area(cell)
     
     def get_index(self):
         if self.lon_is_360:
             longitude = lon_to_180(self.longitude)
         else:
             longitude = self.longitude
         
@@ -81,15 +81,15 @@
         )
 
     @lru_cache(maxsize=None)
     def mask(self, georegions, buffer=0, chunksize=100, compute=True):
         mask = (
             georegions.poly_array(buffer, "dask")
             .rechunk(chunksize)
-            .map_blocks(pygeos.contains, self.centroids(), dtype=float)
+            .map_blocks(shapely.contains, self.centroids(), dtype=float)
         )
         if compute:
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 # m = np.moveaxis(mask.compute().squeeze(), -1, 0)
                 m = mask.compute().squeeze()
                 da = xr.DataArray(
@@ -121,15 +121,15 @@
         poly_array = georegions.poly_array(buffer, chunks=self.chunks).squeeze()
 
         poly_shp = poly_array.shape
         poly_array = dask_geopandas.from_geopandas(
             gpd.GeoDataFrame(geometry=poly_array), npartitions=1
         )
 
-        # mask = fc.map_blocks(pygeos.within, poly_array, dtype=bool)
+        # mask = fc.map_blocks(shapely.within, poly_array, dtype=bool)
         mask = fc.sjoin(poly_array, predicate="within").compute()
 
         return mask
 
     def centroids_to_cell(
         self,
         georegions,
@@ -164,24 +164,24 @@
             for x in [-self.resolution / 2, self.resolution / 2]
         ]
         latpoints = [
             dask.array.from_array(mlat + x, chunks=(chunksize, -1, -1))
             for x in [-self.resolution / 2, self.resolution / 2]
         ]
         boxes = lonpoints[0].map_blocks(
-            pygeos.box, latpoints[0], lonpoints[1], latpoints[1], dtype=float
+            shapely.box, latpoints[0], lonpoints[1], latpoints[1], dtype=float
         )
 
         # Return full cells or intersection of cell and polygon (e.g. for area weights)
         if not intersect_cells:
             tr = boxes.compute()
             # tr = np.moveaxis(tr, 0, -1)
             return tr
 
-        result = pol.map_blocks(pygeos.intersection, boxes, dtype=float)
+        result = pol.map_blocks(shapely.intersection, boxes, dtype=float)
         if compute:
             with warnings.catch_warnings():
                 warnings.simplefilter("ignore")
                 tr = result.compute()
                 # tr = np.moveaxis(result.compute(), 0, -1)
             if datatype == "xarray":
                 return xr.DataArray(data=tr, dims=msk.dims, coords=msk.coords)
```

### Comparing `aggfly-0.1.0/aggfly/dataset/grid_utils.py` & `aggfly-0.1.1/aggfly/dataset/grid_utils.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.0/aggfly/regions/georegions.py` & `aggfly-0.1.1/aggfly/regions/georegions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,28 @@
+import os
 from typing import List, Optional, Union
 import numpy as np
 import matplotlib.pyplot as mpl
 
 import geopandas as gpd
+import geopandas as gpd
 import dask_geopandas
 import dask
 import dask.array
 from copy import deepcopy
 import warnings
 
 from .shp_utils import *
 
+# Weird bug in pyproj or geopandas that results in inf values the first time
+# a shapefile is loaded.. only for certain installations of PROJ
+# https://github.com/arup-group/genet/issues/213
+import pyproj
+pyproj.network.set_network_enabled(False)
+
 
 class GeoRegions:
     """
     A class used to represent geographical regions.
 
     Attributes
     ----------
@@ -54,15 +62,15 @@
             The name of the geographical regions (default is None).
         path : str, optional
             The path to the shapefile (default is None).
         """
         try: 
             shp.crs
             if crs != shp.crs:
-                f"Converting shapefile CRS to {crs}"
+                print(f"Converting shapefile CRS to {crs}")
                 shp = shp.to_crs(crs)   
         except:
             raise ValueError('Shapefile does not have a CRS assigned to it')
         self.shp = shp.reset_index(drop=True)
         self.regionid = regionid
         self.regions = self.shp[self.regionid]
         if region_list is not None:
@@ -190,14 +198,15 @@
         A list of regions to include (default is None, which means all regions are included).
 
     Returns
     -------
     GeoRegions
         The loaded GeoRegions object.
     """
+    
     shp = gpd.read_file(path)
     return GeoRegions(shp, regionid, region_list)
 
 
 def georegions_from_name(name="usa", region_list=None):
     """
     Returns a GeoRegions object based on the given name and region list.
```

### Comparing `aggfly-0.1.0/aggfly/regions/shp_utils.py` & `aggfly-0.1.1/aggfly/regions/shp_utils.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.0/aggfly/tests/test_aggregate.py` & `aggfly-0.1.1/aggfly/tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.0/aggfly/weights/crop_weights.py` & `aggfly-0.1.1/aggfly/weights/crop_weights.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,20 +5,15 @@
 import json
 from pprint import pformat, pprint
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 import geopandas as gpd
-import pygeos
-import dask
-import dask.array
-import rasterio
 from rasterio.enums import Resampling
-import rioxarray
 
 from .secondary_weights import RasterWeights
 from ..dataset import reformat_grid
 from ..cache import *
 
 
 class CropWeights(RasterWeights):
```

### Comparing `aggfly-0.1.0/aggfly/weights/grid_weights.py` & `aggfly-0.1.1/aggfly/weights/grid_weights.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.0/aggfly/weights/pop_weights.py` & `aggfly-0.1.1/aggfly/weights/pop_weights.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,15 @@
 import json
 from pprint import pformat, pprint
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 import geopandas as gpd
-import pygeos
-import dask
 import dask.array
-import rasterio
 from rasterio.enums import Resampling
 import rioxarray
 
 from .secondary_weights import RasterWeights
 from ..dataset import reformat_grid
 from ..cache import *
```

### Comparing `aggfly-0.1.0/aggfly/weights/secondary_weights.py` & `aggfly-0.1.1/aggfly/weights/secondary_weights.py`

 * *Files identical despite different names*

### Comparing `aggfly-0.1.0/pyproject.toml` & `aggfly-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "aggfly"
-version = "0.1.0"
+version = "0.1.1"
 description = "Efficient spatial and temporal aggregation of gridded climate data"
 authors = ["Dylan Hogan <dth2133@columbia.edu>"]
 readme = "README.md"
 packages = [{include = "aggfly"}]
 
 [tool.poetry.dependencies]
-python = ">=3.11.6"
+python = ">=3.11.6, <4.0"
 dask = "^2023.11.0"
 numpy = "^1.26.4"
 geopandas = "^0.14.4"
 dill = "^0.3.8"
 pyyaml = "^6.0.1"
 rasterio = "^1.3.10"
 pandas = "^2.2.2"
 xarray = "^2024.5.0"
 zarr = "^2.18.2"
 dask-geopandas = "^0.3.1"
 pytest = "^8.2.1"
 netcdf4 = "^1.6.5"
-pygeos = "^0.14"
 numba = "^0.59.1"
 matplotlib = "^3.9.0"
 rioxarray = "^0.15.5"
+shapely = "^2.0.4"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

