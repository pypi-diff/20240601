# Comparing `tmp/wwpdb_utils_dp-0.51.1.dev1.tar.gz` & `tmp/wwpdb_utils_dp-0.51.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb_utils_dp-0.51.1.dev1.tar", last modified: Thu May 23 12:01:37 2024, max compression
+gzip compressed data, was "wwpdb_utils_dp-0.51.2.tar", last modified: Sat Jun  1 10:00:08 2024, max compression
```

## Comparing `wwpdb_utils_dp-0.51.1.dev1.tar` & `wwpdb_utils_dp-0.51.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 12:01:37.805035 wwpdb_utils_dp-0.51.1.dev1/
--rw-r--r--   0 vsts      (1001) docker     (127)       96 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      104 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)      966 2024-05-23 12:01:37.805035 wwpdb_utils_dp-0.51.1.dev1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      180 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/README.md
--rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-05-23 12:01:37.805035 wwpdb_utils_dp-0.51.1.dev1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2215 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 12:01:37.801035 wwpdb_utils_dp-0.51.1.dev1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 12:01:37.801035 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 12:01:37.805035 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/
--rw-r--r--   0 vsts      (1001) docker     (127)     5395 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/CentreOfMass.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11569 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/DataFileAdapter.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2358 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/DensityWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/DepositorSyncUtil.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1918 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxChemShiftReport.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2694 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxMergeCategory.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5366 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxModelComplexity.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5231 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxSFMapCoefficients.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2368 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxStripCategory.py
--rw-r--r--   0 vsts      (1001) docker     (127)   212836 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/RcsbDpUtility.py
--rw-r--r--   0 vsts      (1001) docker     (127)    17219 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/RunRemote.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4429 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/ValidationWrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)      161 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 12:01:37.805035 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/electron_density/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/electron_density/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3930 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/electron_density/common_functions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3801 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/electron_density/em_density_map.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10363 2024-05-23 12:00:40.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/electron_density/x_ray_density_map.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-23 12:01:37.805035 wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      966 2024-05-23 12:01:37.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      972 2024-05-23 12:01:37.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-23 12:01:37.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-23 12:01:24.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)       96 2024-05-23 12:01:37.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-23 12:01:37.000000 wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 10:00:08.040489 wwpdb_utils_dp-0.51.2/
+-rw-r--r--   0 vsts      (1001) docker     (127)       96 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      104 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)      961 2024-06-01 10:00:08.040489 wwpdb_utils_dp-0.51.2/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      180 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/README.md
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-06-01 10:00:08.040489 wwpdb_utils_dp-0.51.2/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2215 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 10:00:08.032489 wwpdb_utils_dp-0.51.2/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 10:00:08.032489 wwpdb_utils_dp-0.51.2/wwpdb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 10:00:08.036489 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5395 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/CentreOfMass.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11569 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/DataFileAdapter.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2358 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/DensityWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1782 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/DepositorSyncUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1918 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/PdbxChemShiftReport.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2694 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/PdbxMergeCategory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5366 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/PdbxModelComplexity.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5231 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/PdbxSFMapCoefficients.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2368 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/PdbxStripCategory.py
+-rw-r--r--   0 vsts      (1001) docker     (127)   212836 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/RcsbDpUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    17219 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/RunRemote.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4429 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/ValidationWrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      156 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 10:00:08.036489 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/electron_density/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/electron_density/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3930 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/electron_density/common_functions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3801 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/electron_density/em_density_map.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10363 2024-06-01 09:59:15.000000 wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/electron_density/x_ray_density_map.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-06-01 10:00:08.036489 wwpdb_utils_dp-0.51.2/wwpdb.utils.dp.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      961 2024-06-01 10:00:07.000000 wwpdb_utils_dp-0.51.2/wwpdb.utils.dp.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      972 2024-06-01 10:00:07.000000 wwpdb_utils_dp-0.51.2/wwpdb.utils.dp.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-06-01 10:00:07.000000 wwpdb_utils_dp-0.51.2/wwpdb.utils.dp.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-06-01 09:59:53.000000 wwpdb_utils_dp-0.51.2/wwpdb.utils.dp.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)       96 2024-06-01 10:00:07.000000 wwpdb_utils_dp-0.51.2/wwpdb.utils.dp.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-06-01 10:00:07.000000 wwpdb_utils_dp-0.51.2/wwpdb.utils.dp.egg-info/top_level.txt
```

### Comparing `wwpdb_utils_dp-0.51.1.dev1/LICENSE` & `wwpdb_utils_dp-0.51.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/PKG-INFO` & `wwpdb_utils_dp-0.51.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.dp
-Version: 0.51.1.dev1
+Version: 0.51.2
 Summary: API for Common Data Processing Operations
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_dp
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb_utils_dp-0.51.1.dev1/setup.py` & `wwpdb_utils_dp-0.51.2/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/CentreOfMass.py` & `wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/CentreOfMass.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/DataFileAdapter.py` & `wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/DataFileAdapter.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/DensityWrapper.py` & `wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/DensityWrapper.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/DepositorSyncUtil.py` & `wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/DepositorSyncUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxChemShiftReport.py` & `wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/PdbxChemShiftReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxMergeCategory.py` & `wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/PdbxMergeCategory.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxModelComplexity.py` & `wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/PdbxModelComplexity.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxSFMapCoefficients.py` & `wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/PdbxSFMapCoefficients.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/PdbxStripCategory.py` & `wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/PdbxStripCategory.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/RcsbDpUtility.py` & `wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/RcsbDpUtility.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/RunRemote.py` & `wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/RunRemote.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/ValidationWrapper.py` & `wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/ValidationWrapper.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/electron_density/common_functions.py` & `wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/electron_density/common_functions.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/electron_density/em_density_map.py` & `wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/electron_density/em_density_map.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb/utils/dp/electron_density/x_ray_density_map.py` & `wwpdb_utils_dp-0.51.2/wwpdb/utils/dp/electron_density/x_ray_density_map.py`

 * *Files identical despite different names*

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/PKG-INFO` & `wwpdb_utils_dp-0.51.2/wwpdb.utils.dp.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.utils.dp
-Version: 0.51.1.dev1
+Version: 0.51.2
 Summary: API for Common Data Processing Operations
 Home-page: https://github.com/wwpdb/py-wwpdb_utils_dp
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb_utils_dp-0.51.1.dev1/wwpdb.utils.dp.egg-info/SOURCES.txt` & `wwpdb_utils_dp-0.51.2/wwpdb.utils.dp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

