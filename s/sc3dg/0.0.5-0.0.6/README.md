# Comparing `tmp/sc3dg-0.0.5.tar.gz` & `tmp/sc3dg-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc3dg-0.0.5.tar", last modified: Sat Jun  1 10:19:47 2024, max compression
+gzip compressed data, was "sc3dg-0.0.6.tar", last modified: Sat Jun  1 10:21:24 2024, max compression
```

## Comparing `sc3dg-0.0.5.tar` & `sc3dg-0.0.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:19:47.000000 sc3dg-0.0.5/
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 10:19:47.000000 sc3dg-0.0.5/PKG-INFO
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9859 2024-06-01 08:07:24.000000 sc3dg-0.0.5/README.md
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:19:47.000000 sc3dg-0.0.5/sc3dg/
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2023-12-22 13:39:36.000000 sc3dg-0.0.5/sc3dg/__init__.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5510 2024-06-01 10:01:05.000000 sc3dg-0.0.5/sc3dg/main.py
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:19:47.000000 sc3dg-0.0.5/sc3dg/utils/
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2951 2024-06-01 10:18:22.000000 sc3dg-0.0.5/sc3dg/utils/Generate_scNanoHIC_pairs.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1361 2024-06-01 10:18:22.000000 sc3dg-0.0.5/sc3dg/utils/ReformSAM.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      133 2024-06-01 10:19:40.000000 sc3dg-0.0.5/sc3dg/utils/__init__.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10612 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/analysis.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7503 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/assembly.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2555 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/download.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3706 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/embedding.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10805 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/general.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1282 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/help.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9663 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/plot.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    15197 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/scMethyl.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7287 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/scNano.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1423 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/scNano_barcode.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    13736 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/scSPRITE.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    25080 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/scaffold.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12463 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/sciHic.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12315 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/sn_m3c.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5223 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/tools.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2722 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/visualize.py
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:19:47.000000 sc3dg-0.0.5/sc3dg.egg-info/
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 10:19:46.000000 sc3dg-0.0.5/sc3dg.egg-info/PKG-INFO
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      689 2024-06-01 10:19:46.000000 sc3dg-0.0.5/sc3dg.egg-info/SOURCES.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)        1 2024-06-01 10:19:46.000000 sc3dg-0.0.5/sc3dg.egg-info/dependency_links.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)       42 2024-06-01 10:19:46.000000 sc3dg-0.0.5/sc3dg.egg-info/entry_points.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      605 2024-06-01 10:19:46.000000 sc3dg-0.0.5/sc3dg.egg-info/requires.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)        6 2024-06-01 10:19:46.000000 sc3dg-0.0.5/sc3dg.egg-info/top_level.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)       38 2024-06-01 10:19:47.000000 sc3dg-0.0.5/setup.cfg
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      435 2021-02-01 02:48:55.000000 sc3dg-0.0.5/setup.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:21:24.000000 sc3dg-0.0.6/
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 10:21:24.000000 sc3dg-0.0.6/PKG-INFO
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9859 2024-06-01 08:07:24.000000 sc3dg-0.0.6/README.md
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:21:24.000000 sc3dg-0.0.6/sc3dg/
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2023-12-22 13:39:36.000000 sc3dg-0.0.6/sc3dg/__init__.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5510 2024-06-01 10:01:05.000000 sc3dg-0.0.6/sc3dg/main.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:21:24.000000 sc3dg-0.0.6/sc3dg/utils/
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2951 2024-06-01 10:18:22.000000 sc3dg-0.0.6/sc3dg/utils/Generate_scNanoHIC_pairs.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1361 2024-06-01 10:18:22.000000 sc3dg-0.0.6/sc3dg/utils/ReformSAM.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      131 2024-06-01 10:21:06.000000 sc3dg-0.0.6/sc3dg/utils/__init__.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10612 2024-06-01 10:18:23.000000 sc3dg-0.0.6/sc3dg/utils/analysis.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7503 2024-06-01 10:18:23.000000 sc3dg-0.0.6/sc3dg/utils/assembly.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2555 2024-06-01 10:18:23.000000 sc3dg-0.0.6/sc3dg/utils/download.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3706 2024-06-01 10:18:23.000000 sc3dg-0.0.6/sc3dg/utils/embedding.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10805 2024-06-01 10:18:23.000000 sc3dg-0.0.6/sc3dg/utils/general.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1282 2024-06-01 10:18:23.000000 sc3dg-0.0.6/sc3dg/utils/help.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9663 2024-06-01 10:18:23.000000 sc3dg-0.0.6/sc3dg/utils/plot.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    15197 2024-06-01 10:18:23.000000 sc3dg-0.0.6/sc3dg/utils/scMethyl.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7287 2024-06-01 10:18:23.000000 sc3dg-0.0.6/sc3dg/utils/scNano.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1423 2024-06-01 10:18:23.000000 sc3dg-0.0.6/sc3dg/utils/scNano_barcode.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    13736 2024-06-01 10:18:23.000000 sc3dg-0.0.6/sc3dg/utils/scSPRITE.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    25080 2024-06-01 10:18:23.000000 sc3dg-0.0.6/sc3dg/utils/scaffold.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12463 2024-06-01 10:18:23.000000 sc3dg-0.0.6/sc3dg/utils/sciHic.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12315 2024-06-01 10:18:23.000000 sc3dg-0.0.6/sc3dg/utils/sn_m3c.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5223 2024-06-01 10:18:23.000000 sc3dg-0.0.6/sc3dg/utils/tools.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2722 2024-06-01 10:18:23.000000 sc3dg-0.0.6/sc3dg/utils/visualize.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:21:24.000000 sc3dg-0.0.6/sc3dg.egg-info/
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 10:21:23.000000 sc3dg-0.0.6/sc3dg.egg-info/PKG-INFO
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      689 2024-06-01 10:21:24.000000 sc3dg-0.0.6/sc3dg.egg-info/SOURCES.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)        1 2024-06-01 10:21:23.000000 sc3dg-0.0.6/sc3dg.egg-info/dependency_links.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)       42 2024-06-01 10:21:23.000000 sc3dg-0.0.6/sc3dg.egg-info/entry_points.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      605 2024-06-01 10:21:23.000000 sc3dg-0.0.6/sc3dg.egg-info/requires.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)        6 2024-06-01 10:21:23.000000 sc3dg-0.0.6/sc3dg.egg-info/top_level.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)       38 2024-06-01 10:21:24.000000 sc3dg-0.0.6/setup.cfg
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      435 2021-02-01 02:51:35.000000 sc3dg-0.0.6/setup.py
```

### Comparing `sc3dg-0.0.5/README.md` & `sc3dg-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/main.py` & `sc3dg-0.0.6/sc3dg/main.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/Generate_scNanoHIC_pairs.py` & `sc3dg-0.0.6/sc3dg/utils/Generate_scNanoHIC_pairs.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/ReformSAM.py` & `sc3dg-0.0.6/sc3dg/utils/ReformSAM.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/analysis.py` & `sc3dg-0.0.6/sc3dg/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/assembly.py` & `sc3dg-0.0.6/sc3dg/utils/assembly.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/download.py` & `sc3dg-0.0.6/sc3dg/utils/download.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/embedding.py` & `sc3dg-0.0.6/sc3dg/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/general.py` & `sc3dg-0.0.6/sc3dg/utils/general.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/help.py` & `sc3dg-0.0.6/sc3dg/utils/help.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/plot.py` & `sc3dg-0.0.6/sc3dg/utils/plot.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/scMethyl.py` & `sc3dg-0.0.6/sc3dg/utils/scMethyl.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/scNano.py` & `sc3dg-0.0.6/sc3dg/utils/scNano.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/scNano_barcode.py` & `sc3dg-0.0.6/sc3dg/utils/scNano_barcode.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/scSPRITE.py` & `sc3dg-0.0.6/sc3dg/utils/scSPRITE.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/scaffold.py` & `sc3dg-0.0.6/sc3dg/utils/scaffold.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/sciHic.py` & `sc3dg-0.0.6/sc3dg/utils/sciHic.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/sn_m3c.py` & `sc3dg-0.0.6/sc3dg/utils/sn_m3c.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/tools.py` & `sc3dg-0.0.6/sc3dg/utils/tools.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg/utils/visualize.py` & `sc3dg-0.0.6/sc3dg/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg.egg-info/SOURCES.txt` & `sc3dg-0.0.6/sc3dg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.5/sc3dg.egg-info/requires.txt` & `sc3dg-0.0.6/sc3dg.egg-info/requires.txt`

 * *Files identical despite different names*

