# Comparing `tmp/voxelworldapi-1.3.post20240601.tar.gz` & `tmp/voxelworldapi-1.6.320240531.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxelworldapi-1.3.post20240601.tar", last modified: Sat Jun  1 13:27:54 2024, max compression
+gzip compressed data, was "voxelworldapi-1.6.320240531.tar", last modified: Fri May 31 12:39:36 2024, max compression
```

## Comparing `voxelworldapi-1.3.post20240601.tar` & `voxelworldapi-1.6.320240531.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 seledka   (1000) seledka   (1000)        0 2024-06-01 13:27:54.682097 voxelworldapi-1.3.post20240601/
--rw-r--r--   0 seledka   (1000) seledka   (1000)     1074 2024-05-31 12:37:11.000000 voxelworldapi-1.3.post20240601/LICENSE
--rw-r--r--   0 seledka   (1000) seledka   (1000)     2528 2024-06-01 13:27:54.682097 voxelworldapi-1.3.post20240601/PKG-INFO
--rw-r--r--   0 seledka   (1000) seledka   (1000)       46 2024-06-01 13:27:54.683097 voxelworldapi-1.3.post20240601/setup.cfg
--rw-r--r--   0 seledka   (1000) seledka   (1000)      513 2024-06-01 13:27:43.000000 voxelworldapi-1.3.post20240601/setup.py
-drwxr-xr-x   0 seledka   (1000) seledka   (1000)        0 2024-06-01 13:27:54.681097 voxelworldapi-1.3.post20240601/voxelworldapi/
--rw-r--r--   0 seledka   (1000) seledka   (1000)       40 2024-05-31 10:28:52.000000 voxelworldapi-1.3.post20240601/voxelworldapi/__init__.py
--rw-r--r--   0 seledka   (1000) seledka   (1000)     1723 2024-05-31 11:20:18.000000 voxelworldapi-1.3.post20240601/voxelworldapi/voxelworldapi.py
-drwxr-xr-x   0 seledka   (1000) seledka   (1000)        0 2024-06-01 13:27:54.682097 voxelworldapi-1.3.post20240601/voxelworldapi.egg-info/
--rw-r--r--   0 seledka   (1000) seledka   (1000)     2528 2024-06-01 13:27:54.000000 voxelworldapi-1.3.post20240601/voxelworldapi.egg-info/PKG-INFO
--rw-r--r--   0 seledka   (1000) seledka   (1000)      267 2024-06-01 13:27:54.000000 voxelworldapi-1.3.post20240601/voxelworldapi.egg-info/SOURCES.txt
--rw-r--r--   0 seledka   (1000) seledka   (1000)        1 2024-06-01 13:27:54.000000 voxelworldapi-1.3.post20240601/voxelworldapi.egg-info/dependency_links.txt
--rw-r--r--   0 seledka   (1000) seledka   (1000)       12 2024-06-01 13:27:54.000000 voxelworldapi-1.3.post20240601/voxelworldapi.egg-info/requires.txt
--rw-r--r--   0 seledka   (1000) seledka   (1000)       14 2024-06-01 13:27:54.000000 voxelworldapi-1.3.post20240601/voxelworldapi.egg-info/top_level.txt
+drwxr-xr-x   0 seledka   (1000) seledka   (1000)        0 2024-05-31 12:39:36.031432 voxelworldapi-1.6.320240531/
+-rw-r--r--   0 seledka   (1000) seledka   (1000)     1074 2024-05-31 12:37:11.000000 voxelworldapi-1.6.320240531/LICENSE
+-rw-r--r--   0 seledka   (1000) seledka   (1000)     2525 2024-05-31 12:39:36.031432 voxelworldapi-1.6.320240531/PKG-INFO
+-rw-r--r--   0 seledka   (1000) seledka   (1000)       46 2024-05-31 12:39:36.031432 voxelworldapi-1.6.320240531/setup.cfg
+-rw-r--r--   0 seledka   (1000) seledka   (1000)      509 2024-05-31 12:36:38.000000 voxelworldapi-1.6.320240531/setup.py
+drwxr-xr-x   0 seledka   (1000) seledka   (1000)        0 2024-05-31 12:39:36.030431 voxelworldapi-1.6.320240531/voxelworldapi/
+-rw-r--r--   0 seledka   (1000) seledka   (1000)       40 2024-05-31 10:28:52.000000 voxelworldapi-1.6.320240531/voxelworldapi/__init__.py
+-rw-r--r--   0 seledka   (1000) seledka   (1000)     1723 2024-05-31 11:20:18.000000 voxelworldapi-1.6.320240531/voxelworldapi/voxelworldapi.py
+drwxr-xr-x   0 seledka   (1000) seledka   (1000)        0 2024-05-31 12:39:36.031432 voxelworldapi-1.6.320240531/voxelworldapi.egg-info/
+-rw-r--r--   0 seledka   (1000) seledka   (1000)     2525 2024-05-31 12:39:35.000000 voxelworldapi-1.6.320240531/voxelworldapi.egg-info/PKG-INFO
+-rw-r--r--   0 seledka   (1000) seledka   (1000)      267 2024-05-31 12:39:35.000000 voxelworldapi-1.6.320240531/voxelworldapi.egg-info/SOURCES.txt
+-rw-r--r--   0 seledka   (1000) seledka   (1000)        1 2024-05-31 12:39:35.000000 voxelworldapi-1.6.320240531/voxelworldapi.egg-info/dependency_links.txt
+-rw-r--r--   0 seledka   (1000) seledka   (1000)        9 2024-05-31 12:39:35.000000 voxelworldapi-1.6.320240531/voxelworldapi.egg-info/requires.txt
+-rw-r--r--   0 seledka   (1000) seledka   (1000)       14 2024-05-31 12:39:35.000000 voxelworldapi-1.6.320240531/voxelworldapi.egg-info/top_level.txt
```

### Comparing `voxelworldapi-1.3.post20240601/LICENSE` & `voxelworldapi-1.6.320240531/LICENSE`

 * *Files identical despite different names*

### Comparing `voxelworldapi-1.3.post20240601/PKG-INFO` & `voxelworldapi-1.6.320240531/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxelworldapi
-Version: 1.3.post20240601
+Version: 1.6.320240531
 Summary: A Python library for interacting with VoxelWorld API
 Home-page: https://github.com/callfishxt/voxelworldapi
 Author: CallFish
 Author-email: callfish@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `voxelworldapi-1.3.post20240601/voxelworldapi/voxelworldapi.py` & `voxelworldapi-1.6.320240531/voxelworldapi/voxelworldapi.py`

 * *Files identical despite different names*

### Comparing `voxelworldapi-1.3.post20240601/voxelworldapi.egg-info/PKG-INFO` & `voxelworldapi-1.6.320240531/voxelworldapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voxelworldapi
-Version: 1.3.post20240601
+Version: 1.6.320240531
 Summary: A Python library for interacting with VoxelWorld API
 Home-page: https://github.com/callfishxt/voxelworldapi
 Author: CallFish
 Author-email: callfish@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```
