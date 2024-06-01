# Comparing `tmp/sc3dg-0.0.3.tar.gz` & `tmp/sc3dg-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc3dg-0.0.3.tar", last modified: Sat Jun  1 10:02:38 2024, max compression
+gzip compressed data, was "sc3dg-0.0.4.tar", last modified: Sat Jun  1 10:13:05 2024, max compression
```

## Comparing `sc3dg-0.0.3.tar` & `sc3dg-0.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:02:38.000000 sc3dg-0.0.3/
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 10:02:38.000000 sc3dg-0.0.3/PKG-INFO
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9859 2024-06-01 08:07:24.000000 sc3dg-0.0.3/README.md
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:02:38.000000 sc3dg-0.0.3/sc3dg/
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2023-12-22 13:39:36.000000 sc3dg-0.0.3/sc3dg/__init__.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5510 2024-06-01 10:01:05.000000 sc3dg-0.0.3/sc3dg/main.py
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:02:38.000000 sc3dg-0.0.3/sc3dg/utils/
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2951 2023-12-22 13:39:38.000000 sc3dg-0.0.3/sc3dg/utils/Generate_scNanoHIC_pairs.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1361 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/ReformSAM.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/__init__.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      179 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/_version.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10612 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/analysis.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     8049 2023-12-22 13:39:38.000000 sc3dg-0.0.3/sc3dg/utils/assembly.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)       72 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/correct.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3026 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/download.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3706 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/embedding.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10805 2023-12-22 13:39:38.000000 sc3dg-0.0.3/sc3dg/utils/general.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1282 2023-12-22 13:39:38.000000 sc3dg-0.0.3/sc3dg/utils/help.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    30787 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/hicCorrectMatrix.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3231 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/iterativeCorrection.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9663 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/plot.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7430 2023-12-22 13:44:16.000000 sc3dg-0.0.3/sc3dg/utils/scNano.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1423 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/scNano_barcode.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    14322 2024-01-11 01:46:15.000000 sc3dg-0.0.3/sc3dg/utils/scSPRITE.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    25129 2024-01-04 01:09:13.000000 sc3dg-0.0.3/sc3dg/utils/scaffold.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12463 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/sciHic.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12331 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/sn_m3c.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5268 2023-12-22 13:57:33.000000 sc3dg-0.0.3/sc3dg/utils/tools.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    22875 2023-12-22 13:39:38.000000 sc3dg-0.0.3/sc3dg/utils/utilities.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2722 2023-12-22 13:39:37.000000 sc3dg-0.0.3/sc3dg/utils/visualize.py
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:02:38.000000 sc3dg-0.0.3/sc3dg.egg-info/
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 10:02:37.000000 sc3dg-0.0.3/sc3dg.egg-info/PKG-INFO
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      804 2024-06-01 10:02:38.000000 sc3dg-0.0.3/sc3dg.egg-info/SOURCES.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)        1 2024-06-01 10:02:37.000000 sc3dg-0.0.3/sc3dg.egg-info/dependency_links.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)       42 2024-06-01 10:02:37.000000 sc3dg-0.0.3/sc3dg.egg-info/entry_points.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      605 2024-06-01 10:02:37.000000 sc3dg-0.0.3/sc3dg.egg-info/requires.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)        6 2024-06-01 10:02:37.000000 sc3dg-0.0.3/sc3dg.egg-info/top_level.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)       38 2024-06-01 10:02:38.000000 sc3dg-0.0.3/setup.cfg
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      435 2021-02-01 02:27:24.000000 sc3dg-0.0.3/setup.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:13:05.000000 sc3dg-0.0.4/
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 10:13:05.000000 sc3dg-0.0.4/PKG-INFO
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9859 2024-06-01 08:07:24.000000 sc3dg-0.0.4/README.md
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:13:05.000000 sc3dg-0.0.4/sc3dg/
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2023-12-22 13:39:36.000000 sc3dg-0.0.4/sc3dg/__init__.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5510 2024-06-01 10:01:05.000000 sc3dg-0.0.4/sc3dg/main.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:13:05.000000 sc3dg-0.0.4/sc3dg/utils/
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2951 2023-12-22 13:39:38.000000 sc3dg-0.0.4/sc3dg/utils/Generate_scNanoHIC_pairs.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1361 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/ReformSAM.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      110 2024-06-01 10:12:53.000000 sc3dg-0.0.4/sc3dg/utils/__init__.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      179 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/_version.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10612 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/analysis.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     8049 2023-12-22 13:39:38.000000 sc3dg-0.0.4/sc3dg/utils/assembly.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)       72 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/correct.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3026 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/download.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3706 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/embedding.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10805 2023-12-22 13:39:38.000000 sc3dg-0.0.4/sc3dg/utils/general.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1282 2023-12-22 13:39:38.000000 sc3dg-0.0.4/sc3dg/utils/help.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    30787 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/hicCorrectMatrix.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3231 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/iterativeCorrection.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9663 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/plot.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7430 2023-12-22 13:44:16.000000 sc3dg-0.0.4/sc3dg/utils/scNano.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1423 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/scNano_barcode.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    14322 2024-01-11 01:46:15.000000 sc3dg-0.0.4/sc3dg/utils/scSPRITE.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    25129 2024-01-04 01:09:13.000000 sc3dg-0.0.4/sc3dg/utils/scaffold.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12463 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/sciHic.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12331 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/sn_m3c.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5268 2023-12-22 13:57:33.000000 sc3dg-0.0.4/sc3dg/utils/tools.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    22875 2023-12-22 13:39:38.000000 sc3dg-0.0.4/sc3dg/utils/utilities.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2722 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/visualize.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:13:05.000000 sc3dg-0.0.4/sc3dg.egg-info/
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 10:13:04.000000 sc3dg-0.0.4/sc3dg.egg-info/PKG-INFO
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      804 2024-06-01 10:13:05.000000 sc3dg-0.0.4/sc3dg.egg-info/SOURCES.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)        1 2024-06-01 10:13:04.000000 sc3dg-0.0.4/sc3dg.egg-info/dependency_links.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)       42 2024-06-01 10:13:04.000000 sc3dg-0.0.4/sc3dg.egg-info/entry_points.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      605 2024-06-01 10:13:04.000000 sc3dg-0.0.4/sc3dg.egg-info/requires.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)        6 2024-06-01 10:13:04.000000 sc3dg-0.0.4/sc3dg.egg-info/top_level.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)       38 2024-06-01 10:13:05.000000 sc3dg-0.0.4/setup.cfg
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      435 2021-02-01 02:43:23.000000 sc3dg-0.0.4/setup.py
```

### Comparing `sc3dg-0.0.3/README.md` & `sc3dg-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/main.py` & `sc3dg-0.0.4/sc3dg/main.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/Generate_scNanoHIC_pairs.py` & `sc3dg-0.0.4/sc3dg/utils/Generate_scNanoHIC_pairs.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/ReformSAM.py` & `sc3dg-0.0.4/sc3dg/utils/ReformSAM.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/analysis.py` & `sc3dg-0.0.4/sc3dg/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/assembly.py` & `sc3dg-0.0.4/sc3dg/utils/assembly.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/download.py` & `sc3dg-0.0.4/sc3dg/utils/download.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/embedding.py` & `sc3dg-0.0.4/sc3dg/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/general.py` & `sc3dg-0.0.4/sc3dg/utils/general.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/help.py` & `sc3dg-0.0.4/sc3dg/utils/help.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/hicCorrectMatrix.py` & `sc3dg-0.0.4/sc3dg/utils/hicCorrectMatrix.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/iterativeCorrection.py` & `sc3dg-0.0.4/sc3dg/utils/iterativeCorrection.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/plot.py` & `sc3dg-0.0.4/sc3dg/utils/plot.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/scNano.py` & `sc3dg-0.0.4/sc3dg/utils/scNano.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/scNano_barcode.py` & `sc3dg-0.0.4/sc3dg/utils/scNano_barcode.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/scSPRITE.py` & `sc3dg-0.0.4/sc3dg/utils/scSPRITE.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/scaffold.py` & `sc3dg-0.0.4/sc3dg/utils/scaffold.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/sciHic.py` & `sc3dg-0.0.4/sc3dg/utils/sciHic.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/sn_m3c.py` & `sc3dg-0.0.4/sc3dg/utils/sn_m3c.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/tools.py` & `sc3dg-0.0.4/sc3dg/utils/tools.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/utilities.py` & `sc3dg-0.0.4/sc3dg/utils/utilities.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg/utils/visualize.py` & `sc3dg-0.0.4/sc3dg/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg.egg-info/SOURCES.txt` & `sc3dg-0.0.4/sc3dg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.3/sc3dg.egg-info/requires.txt` & `sc3dg-0.0.4/sc3dg.egg-info/requires.txt`

 * *Files identical despite different names*

