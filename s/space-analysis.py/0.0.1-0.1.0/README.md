# Comparing `tmp/space_analysis_py-0.0.1.tar.gz` & `tmp/space_analysis_py-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "space_analysis_py-0.0.1.tar", last modified: Fri May 31 23:11:20 2024, max compression
+gzip compressed data, was "space_analysis_py-0.1.0.tar", last modified: Fri May 31 21:30:32 2024, max compression
```

## Comparing `space_analysis_py-0.0.1.tar` & `space_analysis_py-0.1.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0    11337 2024-03-29 05:13:42.655866 space_analysis_py-0.0.1/LICENSE
--rw-r--r--   0        0        0     1002 2024-05-31 23:11:20.287333 space_analysis_py-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-26 15:22:29.982177 space_analysis_py-0.0.1/space_analysis/__init__.py
--rw-r--r--   0        0        0    29319 2024-05-31 23:09:39.453159 space_analysis_py-0.0.1/space_analysis/_modidx.py
--rw-r--r--   0        0        0     1739 2024-05-26 15:22:29.943930 space_analysis_py-0.0.1/space_analysis/core.py
--rw-r--r--   0        0        0        0 2024-05-26 15:22:29.981595 space_analysis_py-0.0.1/space_analysis/ds/__init__.py
--rw-r--r--   0        0        0     1808 2024-05-31 23:09:39.453756 space_analysis_py-0.0.1/space_analysis/ds/config.py
--rw-r--r--   0        0        0      740 2024-05-26 15:22:29.947356 space_analysis_py-0.0.1/space_analysis/ds/meta.py
--rw-r--r--   0        0        0     8103 2024-05-31 23:09:39.454542 space_analysis_py-0.0.1/space_analysis/ds/tplot.py
--rw-r--r--   0        0        0        0 2024-05-26 15:22:29.981787 space_analysis_py-0.0.1/space_analysis/io/__init__.py
--rw-r--r--   0        0        0     2022 2024-05-26 15:22:29.968280 space_analysis_py-0.0.1/space_analysis/io/cdf.py
--rw-r--r--   0        0        0        0 2024-05-26 15:22:29.981750 space_analysis_py-0.0.1/space_analysis/missions/__init__.py
--rw-r--r--   0        0        0     1667 2024-05-26 15:22:29.981645 space_analysis_py-0.0.1/space_analysis/missions/dscovr/__init__.py
--rw-r--r--   0        0        0      681 2024-03-29 05:13:42.665741 space_analysis_py-0.0.1/space_analysis/missions/dscovr/mag.py
--rw-r--r--   0        0        0      188 2024-05-26 15:22:29.981731 space_analysis_py-0.0.1/space_analysis/missions/juno/__init__.py
--rw-r--r--   0        0        0     3574 2024-05-26 15:22:29.972132 space_analysis_py-0.0.1/space_analysis/missions/juno/fgm.py
--rw-r--r--   0        0        0     2228 2024-05-26 15:22:29.981674 space_analysis_py-0.0.1/space_analysis/missions/psp/__init__.py
--rw-r--r--   0        0        0        0 2024-05-26 15:22:29.981699 space_analysis_py-0.0.1/space_analysis/missions/wind/__init__.py
--rw-r--r--   0        0        0      673 2024-05-26 15:22:29.974315 space_analysis_py-0.0.1/space_analysis/missions/wind/mag.py
--rw-r--r--   0        0        0      986 2024-05-26 15:22:29.975413 space_analysis_py-0.0.1/space_analysis/missions/wind/plasma.py
--rw-r--r--   0        0        0        0 2024-05-26 15:22:29.981517 space_analysis_py-0.0.1/space_analysis/plasma/__init__.py
--rw-r--r--   0        0        0     2269 2024-05-26 15:22:29.946020 space_analysis_py-0.0.1/space_analysis/plasma/formulary.py
--rw-r--r--   0        0        0     1312 2024-05-31 17:14:59.870447 space_analysis_py-0.0.1/space_analysis/plasma/mhd_waves.py
--rw-r--r--   0        0        0        0 2024-05-26 15:22:29.981560 space_analysis_py-0.0.1/space_analysis/plot/__init__.py
--rw-r--r--   0        0        0      652 2024-05-26 15:22:29.951157 space_analysis_py-0.0.1/space_analysis/plot/basic.py
--rw-r--r--   0        0        0     1944 2024-05-26 15:22:29.952456 space_analysis_py-0.0.1/space_analysis/plot/config.py
--rw-r--r--   0        0        0        0 2024-05-26 15:22:29.981841 space_analysis_py-0.0.1/space_analysis/simulation/__init__.py
--rw-r--r--   0        0        0    13494 2024-05-26 15:22:29.981209 space_analysis_py-0.0.1/space_analysis/simulation/warpx.py
--rw-r--r--   0        0        0        0 2024-05-26 15:22:29.981904 space_analysis_py-0.0.1/space_analysis/utils/__init__.py
--rw-r--r--   0        0        0      805 2024-05-26 15:22:29.940923 space_analysis_py-0.0.1/space_analysis/utils/basic.py
--rw-r--r--   0        0        0     2053 2024-05-26 15:22:29.966683 space_analysis_py-0.0.1/space_analysis/utils/cdas.py
--rw-r--r--   0        0        0      820 2024-05-26 15:22:29.969160 space_analysis_py-0.0.1/space_analysis/utils/lbl.py
--rw-r--r--   0        0        0      303 2024-05-26 15:22:29.946583 space_analysis_py-0.0.1/space_analysis/utils/math.py
--rw-r--r--   0        0        0     1031 2024-05-26 15:22:29.964870 space_analysis_py-0.0.1/space_analysis/utils/pds.py
--rw-r--r--   0        0        0     4440 2024-05-26 15:22:29.960580 space_analysis_py-0.0.1/space_analysis/utils/speasy.py
--rw-r--r--   0        0        0      401 1970-01-01 00:00:00.000000 space_analysis_py-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0    11337 2023-04-27 10:12:58.000000 space_analysis_py-0.1.0/LICENSE
+-rw-r--r--   0        0        0      904 2024-05-31 21:30:32.593606 space_analysis_py-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-31 21:21:32.927240 space_analysis_py-0.1.0/space_analysis/__init__.py
+-rw-r--r--   0        0        0    29319 2024-05-31 21:21:33.196473 space_analysis_py-0.1.0/space_analysis/_modidx.py
+-rw-r--r--   0        0        0     1739 2024-05-31 21:21:32.890333 space_analysis_py-0.1.0/space_analysis/core.py
+-rw-r--r--   0        0        0        0 2024-05-31 21:21:32.925903 space_analysis_py-0.1.0/space_analysis/ds/__init__.py
+-rw-r--r--   0        0        0     1808 2024-05-31 21:21:32.889091 space_analysis_py-0.1.0/space_analysis/ds/config.py
+-rw-r--r--   0        0        0      740 2024-05-31 21:21:32.893764 space_analysis_py-0.1.0/space_analysis/ds/meta.py
+-rw-r--r--   0        0        0     8103 2024-05-31 21:21:32.903549 space_analysis_py-0.1.0/space_analysis/ds/tplot.py
+-rw-r--r--   0        0        0        0 2024-05-31 21:21:32.926530 space_analysis_py-0.1.0/space_analysis/io/__init__.py
+-rw-r--r--   0        0        0     2022 2024-05-31 21:21:32.913633 space_analysis_py-0.1.0/space_analysis/io/cdf.py
+-rw-r--r--   0        0        0        0 2024-05-31 21:21:32.926278 space_analysis_py-0.1.0/space_analysis/missions/__init__.py
+-rw-r--r--   0        0        0     1667 2024-05-31 21:21:32.925947 space_analysis_py-0.1.0/space_analysis/missions/dscovr/__init__.py
+-rw-r--r--   0        0        0      681 2024-02-02 18:40:13.132516 space_analysis_py-0.1.0/space_analysis/missions/dscovr/mag.py
+-rw-r--r--   0        0        0      188 2024-05-31 21:21:32.926260 space_analysis_py-0.1.0/space_analysis/missions/juno/__init__.py
+-rw-r--r--   0        0        0     3574 2024-05-31 21:21:32.917590 space_analysis_py-0.1.0/space_analysis/missions/juno/fgm.py
+-rw-r--r--   0        0        0     2228 2024-05-31 21:21:32.925977 space_analysis_py-0.1.0/space_analysis/missions/psp/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 21:21:32.926004 space_analysis_py-0.1.0/space_analysis/missions/wind/__init__.py
+-rw-r--r--   0        0        0      673 2024-05-31 21:21:32.919047 space_analysis_py-0.1.0/space_analysis/missions/wind/mag.py
+-rw-r--r--   0        0        0      986 2024-05-31 21:21:32.919828 space_analysis_py-0.1.0/space_analysis/missions/wind/plasma.py
+-rw-r--r--   0        0        0        0 2024-05-31 21:21:32.925476 space_analysis_py-0.1.0/space_analysis/plasma/__init__.py
+-rw-r--r--   0        0        0     2269 2024-05-31 21:21:32.892011 space_analysis_py-0.1.0/space_analysis/plasma/formulary.py
+-rw-r--r--   0        0        0     1312 2024-05-31 21:21:32.897938 space_analysis_py-0.1.0/space_analysis/plasma/mhd_waves.py
+-rw-r--r--   0        0        0        0 2024-05-31 21:21:32.925728 space_analysis_py-0.1.0/space_analysis/plot/__init__.py
+-rw-r--r--   0        0        0      652 2024-05-31 21:21:32.896900 space_analysis_py-0.1.0/space_analysis/plot/basic.py
+-rw-r--r--   0        0        0     1944 2024-05-31 21:21:32.899253 space_analysis_py-0.1.0/space_analysis/plot/config.py
+-rw-r--r--   0        0        0        0 2024-05-31 21:21:32.926586 space_analysis_py-0.1.0/space_analysis/simulation/__init__.py
+-rw-r--r--   0        0        0    13494 2024-05-31 21:21:32.924969 space_analysis_py-0.1.0/space_analysis/simulation/warpx.py
+-rw-r--r--   0        0        0        0 2024-05-31 21:21:32.926807 space_analysis_py-0.1.0/space_analysis/utils/__init__.py
+-rw-r--r--   0        0        0      805 2024-05-31 21:21:32.887518 space_analysis_py-0.1.0/space_analysis/utils/basic.py
+-rw-r--r--   0        0        0     2053 2024-05-31 21:21:32.912479 space_analysis_py-0.1.0/space_analysis/utils/cdas.py
+-rw-r--r--   0        0        0      820 2024-05-31 21:21:32.914958 space_analysis_py-0.1.0/space_analysis/utils/lbl.py
+-rw-r--r--   0        0        0      303 2024-05-31 21:21:32.892730 space_analysis_py-0.1.0/space_analysis/utils/math.py
+-rw-r--r--   0        0        0     1031 2024-05-31 21:21:32.910587 space_analysis_py-0.1.0/space_analysis/utils/pds.py
+-rw-r--r--   0        0        0     4440 2024-05-31 21:21:32.906599 space_analysis_py-0.1.0/space_analysis/utils/speasy.py
+-rw-r--r--   0        0        0      380 1970-01-01 00:00:00.000000 space_analysis_py-0.1.0/PKG-INFO
```

### Comparing `space_analysis_py-0.0.1/LICENSE` & `space_analysis_py-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/pyproject.toml` & `space_analysis_py-0.1.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 [project]
 name = "space-analysis.py"
-dynamic = []
+version = "0.1.0"
 description = "Python library for data analysis in space physics"
 authors = [
     { name = "Beforerr", email = "zzj956959688@gmail.com" },
 ]
 requires-python = ">= 3.10, < 3.12"
 dependencies = [
     "pydantic",
     "polars",
     "plasmapy",
     "astropy",
-    "sunpy",
     "loguru",
     "rich",
     "humanize",
     "pycdfpp",
 ]
-version = "0.0.1"
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
-[tool.pdm.version]
-source = "file"
-path = "space_analysis/__init__.py"
-
 [tool.pixi.project]
 channels = [
     "conda-forge",
 ]
 platforms = [
     "osx-arm64",
 ]
```

### Comparing `space_analysis_py-0.0.1/space_analysis/_modidx.py` & `space_analysis_py-0.1.0/space_analysis/_modidx.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/core.py` & `space_analysis_py-0.1.0/space_analysis/core.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/ds/config.py` & `space_analysis_py-0.1.0/space_analysis/ds/config.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/ds/meta.py` & `space_analysis_py-0.1.0/space_analysis/ds/meta.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/ds/tplot.py` & `space_analysis_py-0.1.0/space_analysis/ds/tplot.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/io/cdf.py` & `space_analysis_py-0.1.0/space_analysis/io/cdf.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/missions/dscovr/__init__.py` & `space_analysis_py-0.1.0/space_analysis/missions/dscovr/__init__.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/missions/dscovr/mag.py` & `space_analysis_py-0.1.0/space_analysis/missions/dscovr/mag.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/missions/juno/fgm.py` & `space_analysis_py-0.1.0/space_analysis/missions/juno/fgm.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/missions/psp/__init__.py` & `space_analysis_py-0.1.0/space_analysis/missions/psp/__init__.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/missions/wind/mag.py` & `space_analysis_py-0.1.0/space_analysis/missions/wind/mag.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/missions/wind/plasma.py` & `space_analysis_py-0.1.0/space_analysis/missions/wind/plasma.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/plasma/formulary.py` & `space_analysis_py-0.1.0/space_analysis/plasma/formulary.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/plasma/mhd_waves.py` & `space_analysis_py-0.1.0/space_analysis/plasma/mhd_waves.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/plot/basic.py` & `space_analysis_py-0.1.0/space_analysis/plot/basic.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/plot/config.py` & `space_analysis_py-0.1.0/space_analysis/plot/config.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/simulation/warpx.py` & `space_analysis_py-0.1.0/space_analysis/simulation/warpx.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/utils/basic.py` & `space_analysis_py-0.1.0/space_analysis/utils/basic.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/utils/cdas.py` & `space_analysis_py-0.1.0/space_analysis/utils/cdas.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/utils/lbl.py` & `space_analysis_py-0.1.0/space_analysis/utils/lbl.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/utils/pds.py` & `space_analysis_py-0.1.0/space_analysis/utils/pds.py`

 * *Files identical despite different names*

### Comparing `space_analysis_py-0.0.1/space_analysis/utils/speasy.py` & `space_analysis_py-0.1.0/space_analysis/utils/speasy.py`

 * *Files identical despite different names*

