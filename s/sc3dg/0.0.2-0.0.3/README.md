# Comparing `tmp/sc3dg-0.0.2.tar.gz` & `tmp/sc3dg-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc3dg-0.0.2.tar", last modified: Sat Jun  1 09:27:14 2024, max compression
+gzip compressed data, was "sc3dg-0.0.3.tar", last modified: Sat Jun  1 10:02:38 2024, max compression
```

## Comparing `sc3dg-0.0.2.tar` & `sc3dg-0.0.3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 09:27:14.000000 sc3dg-0.0.2/
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 09:27:14.000000 sc3dg-0.0.2/PKG-INFO
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9859 2024-06-01 08:07:24.000000 sc3dg-0.0.2/README.md
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 09:27:14.000000 sc3dg-0.0.2/sc3dg/
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2023-12-22 13:39:36.000000 sc3dg-0.0.2/sc3dg/__init__.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5480 2024-06-01 07:37:20.000000 sc3dg-0.0.2/sc3dg/main.py
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 09:27:14.000000 sc3dg-0.0.2/sc3dg/utils/
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2951 2023-12-22 13:39:38.000000 sc3dg-0.0.2/sc3dg/utils/Generate_scNanoHIC_pairs.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1361 2023-12-22 13:39:37.000000 sc3dg-0.0.2/sc3dg/utils/ReformSAM.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2023-12-22 13:39:37.000000 sc3dg-0.0.2/sc3dg/utils/__init__.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      179 2023-12-22 13:39:37.000000 sc3dg-0.0.2/sc3dg/utils/_version.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10612 2023-12-22 13:39:37.000000 sc3dg-0.0.2/sc3dg/utils/analysis.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     8049 2023-12-22 13:39:38.000000 sc3dg-0.0.2/sc3dg/utils/assembly.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)       72 2023-12-22 13:39:37.000000 sc3dg-0.0.2/sc3dg/utils/correct.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3026 2023-12-22 13:39:37.000000 sc3dg-0.0.2/sc3dg/utils/download.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3706 2023-12-22 13:39:37.000000 sc3dg-0.0.2/sc3dg/utils/embedding.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10805 2023-12-22 13:39:38.000000 sc3dg-0.0.2/sc3dg/utils/general.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1282 2023-12-22 13:39:38.000000 sc3dg-0.0.2/sc3dg/utils/help.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    30787 2023-12-22 13:39:37.000000 sc3dg-0.0.2/sc3dg/utils/hicCorrectMatrix.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3231 2023-12-22 13:39:37.000000 sc3dg-0.0.2/sc3dg/utils/iterativeCorrection.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9663 2023-12-22 13:39:37.000000 sc3dg-0.0.2/sc3dg/utils/plot.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7430 2023-12-22 13:44:16.000000 sc3dg-0.0.2/sc3dg/utils/scNano.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1423 2023-12-22 13:39:37.000000 sc3dg-0.0.2/sc3dg/utils/scNano_barcode.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    14322 2024-01-11 01:46:15.000000 sc3dg-0.0.2/sc3dg/utils/scSPRITE.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    25129 2024-01-04 01:09:13.000000 sc3dg-0.0.2/sc3dg/utils/scaffold.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12463 2023-12-22 13:39:37.000000 sc3dg-0.0.2/sc3dg/utils/sciHic.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12331 2023-12-22 13:39:37.000000 sc3dg-0.0.2/sc3dg/utils/sn_m3c.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5268 2023-12-22 13:57:33.000000 sc3dg-0.0.2/sc3dg/utils/tools.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    22875 2023-12-22 13:39:38.000000 sc3dg-0.0.2/sc3dg/utils/utilities.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2722 2023-12-22 13:39:37.000000 sc3dg-0.0.2/sc3dg/utils/visualize.py
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 09:27:14.000000 sc3dg-0.0.2/sc3dg.egg-info/
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 09:27:13.000000 sc3dg-0.0.2/sc3dg.egg-info/PKG-INFO
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      804 2024-06-01 09:27:13.000000 sc3dg-0.0.2/sc3dg.egg-info/SOURCES.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)        1 2024-06-01 09:27:13.000000 sc3dg-0.0.2/sc3dg.egg-info/dependency_links.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)       42 2024-06-01 09:27:13.000000 sc3dg-0.0.2/sc3dg.egg-info/entry_points.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      605 2024-06-01 09:27:13.000000 sc3dg-0.0.2/sc3dg.egg-info/requires.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)        6 2024-06-01 09:27:13.000000 sc3dg-0.0.2/sc3dg.egg-info/top_level.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)       38 2024-06-01 09:27:14.000000 sc3dg-0.0.2/setup.cfg
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      435 2021-02-01 01:57:25.000000 sc3dg-0.0.2/setup.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:02:38.000000 sc3dg-0.0.3/
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 10:02:38.000000 sc3dg-0.0.3/PKG-INFO
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9859 2024-06-01 08:07:24.000000 sc3dg-0.0.3/README.md
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:02:38.000000 sc3dg-0.0.3/sc3dg/
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2023-12-22 13:39:36.000000 sc3dg-0.0.3/sc3dg/__init__.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5510 2024-06-01 10:01:05.000000 sc3dg-0.0.3/sc3dg/main.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:02:38.000000 sc3dg-0.0.3/sc3dg/utils/
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2951 2023-12-22 13:39:38.000000 sc3dg-0.0.3/sc3dg/utils/Generate_scNanoHIC_pairs.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1361 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/ReformSAM.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/__init__.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      179 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/_version.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10612 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/analysis.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     8049 2023-12-22 13:39:38.000000 sc3dg-0.0.3/sc3dg/utils/assembly.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)       72 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/correct.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3026 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/download.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3706 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/embedding.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10805 2023-12-22 13:39:38.000000 sc3dg-0.0.3/sc3dg/utils/general.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1282 2023-12-22 13:39:38.000000 sc3dg-0.0.3/sc3dg/utils/help.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    30787 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/hicCorrectMatrix.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3231 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/iterativeCorrection.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9663 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/plot.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7430 2023-12-22 13:44:16.000000 sc3dg-0.0.3/sc3dg/utils/scNano.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1423 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/scNano_barcode.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    14322 2024-01-11 01:46:15.000000 sc3dg-0.0.3/sc3dg/utils/scSPRITE.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    25129 2024-01-04 01:09:13.000000 sc3dg-0.0.3/sc3dg/utils/scaffold.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12463 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/sciHic.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12331 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/sn_m3c.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5268 2023-12-22 13:57:33.000000 sc3dg-0.0.3/sc3dg/utils/tools.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    22875 2023-12-22 13:39:38.000000 sc3dg-0.0.3/sc3dg/utils/utilities.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2722 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/visualize.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:02:38.000000 sc3dg-0.0.3/sc3dg.egg-info/
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 10:02:37.000000 sc3dg-0.0.3/sc3dg.egg-info/PKG-INFO
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      804 2024-06-01 10:02:38.000000 sc3dg-0.0.3/sc3dg.egg-info/SOURCES.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)        1 2024-06-01 10:02:37.000000 sc3dg-0.0.3/sc3dg.egg-info/dependency_links.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)       42 2024-06-01 10:02:37.000000 sc3dg-0.0.3/sc3dg.egg-info/entry_points.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      605 2024-06-01 10:02:37.000000 sc3dg-0.0.3/sc3dg.egg-info/requires.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)        6 2024-06-01 10:02:37.000000 sc3dg-0.0.3/sc3dg.egg-info/top_level.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)       38 2024-06-01 10:02:38.000000 sc3dg-0.0.3/setup.cfg
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      435 2021-02-01 02:27:24.000000 sc3dg-0.0.3/setup.py
```

### Comparing `sc3dg-0.0.2/README.md` & `sc3dg-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/main.py` & `sc3dg-0.0.3/sc3dg/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import argparse
 import os
-from utils import scSPRITE,sn_m3c,scNano,scMethyl
-from utils import help
-from utils import tools as tl
+from sc3dg.utils import scSPRITE,sn_m3c,scNano,scMethyl
+from sc3dg.utils import help
+from sc3dg.utils import tools as tl
 import time
 from multiprocessing import Process, Queue, Pool, Manager
-from utils.scaffold import *
-from utils.assembly import *
+from sc3dg.utils.scaffold import *
+from sc3dg.utils.assembly import *
 import logging
 Path = os.getcwd()
 print(Path)
 tech = {
         'scSPRITE':scSPRITE,
         
         'sn_m3c':sn_m3c,
```

### Comparing `sc3dg-0.0.2/sc3dg/utils/Generate_scNanoHIC_pairs.py` & `sc3dg-0.0.3/sc3dg/utils/Generate_scNanoHIC_pairs.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/ReformSAM.py` & `sc3dg-0.0.3/sc3dg/utils/ReformSAM.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/analysis.py` & `sc3dg-0.0.3/sc3dg/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/assembly.py` & `sc3dg-0.0.3/sc3dg/utils/assembly.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/download.py` & `sc3dg-0.0.3/sc3dg/utils/download.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/embedding.py` & `sc3dg-0.0.3/sc3dg/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/general.py` & `sc3dg-0.0.3/sc3dg/utils/general.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/help.py` & `sc3dg-0.0.3/sc3dg/utils/help.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/hicCorrectMatrix.py` & `sc3dg-0.0.3/sc3dg/utils/hicCorrectMatrix.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/iterativeCorrection.py` & `sc3dg-0.0.3/sc3dg/utils/iterativeCorrection.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/plot.py` & `sc3dg-0.0.3/sc3dg/utils/plot.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/scNano.py` & `sc3dg-0.0.3/sc3dg/utils/scNano.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/scNano_barcode.py` & `sc3dg-0.0.3/sc3dg/utils/scNano_barcode.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/scSPRITE.py` & `sc3dg-0.0.3/sc3dg/utils/scSPRITE.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/scaffold.py` & `sc3dg-0.0.3/sc3dg/utils/scaffold.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/sciHic.py` & `sc3dg-0.0.3/sc3dg/utils/sciHic.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/sn_m3c.py` & `sc3dg-0.0.3/sc3dg/utils/sn_m3c.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/tools.py` & `sc3dg-0.0.3/sc3dg/utils/tools.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/utilities.py` & `sc3dg-0.0.3/sc3dg/utils/utilities.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg/utils/visualize.py` & `sc3dg-0.0.3/sc3dg/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg.egg-info/SOURCES.txt` & `sc3dg-0.0.3/sc3dg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.2/sc3dg.egg-info/requires.txt` & `sc3dg-0.0.3/sc3dg.egg-info/requires.txt`

 * *Files identical despite different names*

