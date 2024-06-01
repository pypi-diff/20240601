# Comparing `tmp/lvmguider-0.5.1.tar.gz` & `tmp/lvmguider-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lvmguider-0.5.1.tar", max compression
+gzip compressed data, was "lvmguider-0.5.2.tar", max compression
```

## Comparing `lvmguider-0.5.1.tar` & `lvmguider-0.5.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0     1504 2024-02-12 21:43:15.775279 lvmguider-0.5.1/LICENSE.md
--rw-r--r--   0        0        0      531 2024-02-12 21:43:15.775279 lvmguider-0.5.1/README.md
--rw-r--r--   0        0        0     2962 2024-02-12 21:43:15.783280 lvmguider-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      551 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/__init__.py
--rw-r--r--   0        0        0     2407 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/__main__.py
--rw-r--r--   0        0        0      658 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/actor/__init__.py
--rw-r--r--   0        0        0     2951 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/actor/actor.py
--rw-r--r--   0        0        0      220 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/actor/commands/__init__.py
--rw-r--r--   0        0        0     1017 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/actor/commands/corrections.py
--rw-r--r--   0        0        0     1783 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/actor/commands/expose.py
--rw-r--r--   0        0        0     5525 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/actor/commands/focus.py
--rw-r--r--   0        0        0     3887 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/actor/commands/guide.py
--rw-r--r--   0        0        0     1525 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/actor/commands/set_pixel.py
--rw-r--r--   0        0        0      740 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/actor/commands/status.py
--rw-r--r--   0        0        0     1453 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/actor/commands/stop.py
--rw-r--r--   0        0        0    16559 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/astrometrynet.py
--rw-r--r--   0        0        0    10855 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/cameras.py
--rw-r--r--   0        0        0    52837 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/coadd.py
--rw-r--r--   0        0        0    19943 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/dataclasses.py
--rw-r--r--   0        0        0     8812 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/etc/datamodel.yml
--rw-r--r--   0        0        0     1446 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/etc/lvmguider.yml
--rw-r--r--   0        0        0    15193 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/extraction.py
--rw-r--r--   0        0        0    15980 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/focus.py
--rw-r--r--   0        0        0    28319 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/guider.py
--rw-r--r--   0        0        0     1002 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/maskbits.py
--rw-r--r--   0        0        0    17847 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/plotting.py
--rw-r--r--   0        0        0    26693 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/tools.py
--rw-r--r--   0        0        0    17416 2024-02-12 21:43:15.783280 lvmguider-0.5.1/src/lvmguider/transformations.py
--rw-r--r--   0        0        0      526 2024-02-12 21:43:15.787279 lvmguider-0.5.1/src/lvmguider/types.py
--rw-r--r--   0        0        0     2457 1970-01-01 00:00:00.000000 lvmguider-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-06-01 15:36:25.340728 lvmguider-0.5.2/LICENSE.md
+-rw-r--r--   0        0        0      531 2024-06-01 15:36:25.340728 lvmguider-0.5.2/README.md
+-rw-r--r--   0        0        0     2995 2024-06-01 15:36:25.348728 lvmguider-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      551 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/__init__.py
+-rw-r--r--   0        0        0     2407 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/__main__.py
+-rw-r--r--   0        0        0      658 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/actor/__init__.py
+-rw-r--r--   0        0        0     2951 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/actor/actor.py
+-rw-r--r--   0        0        0      220 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/actor/commands/__init__.py
+-rw-r--r--   0        0        0     1017 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/actor/commands/corrections.py
+-rw-r--r--   0        0        0     1783 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/actor/commands/expose.py
+-rw-r--r--   0        0        0     5525 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/actor/commands/focus.py
+-rw-r--r--   0        0        0     3887 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/actor/commands/guide.py
+-rw-r--r--   0        0        0     1525 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/actor/commands/set_pixel.py
+-rw-r--r--   0        0        0      740 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/actor/commands/status.py
+-rw-r--r--   0        0        0     1453 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/actor/commands/stop.py
+-rw-r--r--   0        0        0    16559 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/astrometrynet.py
+-rw-r--r--   0        0        0    10855 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/cameras.py
+-rw-r--r--   0        0        0    52837 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/coadd.py
+-rw-r--r--   0        0        0    19943 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/dataclasses.py
+-rw-r--r--   0        0        0     8799 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/etc/datamodel.yml
+-rw-r--r--   0        0        0     1446 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/etc/lvmguider.yml
+-rw-r--r--   0        0        0    15193 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/extraction.py
+-rw-r--r--   0        0        0    15980 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/focus.py
+-rw-r--r--   0        0        0    28318 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/guider.py
+-rw-r--r--   0        0        0     1002 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/maskbits.py
+-rw-r--r--   0        0        0    17847 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/plotting.py
+-rw-r--r--   0        0        0    26693 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/tools.py
+-rw-r--r--   0        0        0    17417 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/transformations.py
+-rw-r--r--   0        0        0      526 2024-06-01 15:36:25.348728 lvmguider-0.5.2/src/lvmguider/types.py
+-rw-r--r--   0        0        0     2457 1970-01-01 00:00:00.000000 lvmguider-0.5.2/PKG-INFO
```

### Comparing `lvmguider-0.5.1/LICENSE.md` & `lvmguider-0.5.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/README.md` & `lvmguider-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/pyproject.toml` & `lvmguider-0.5.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lvmguider"
-version = "0.5.1"
+version = "0.5.2"
 description = "Temporary package for LVM guiding and focusing"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmguider"
 repository = "https://github.com/sdss/lvmguider"
 documentation = "https://lvmguider.readthedocs.org"
@@ -77,26 +77,28 @@
 line-length = 88
 target-version = ['py311']
 fast = true
 
 [tool.ruff]
 line-length = 88
 target-version = 'py312'
+
+[tool.ruff.lint]
 select = ["E", "F", "I"]
 unfixable = ["F841"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401", "F403", "E402"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["lvmguider"]
 lines-after-imports = 2
 section-order = ["future", "standard-library", "typing", "third-party", "sdss", "first-party", "local-folder"]
 
-[tool.ruff.isort.sections]
+[tool.ruff.lint.isort.sections]
 typing = ["typing"]
 sdss = ["sdsstools", "clu"]
 
 [tool.pytest.ini_options]
 addopts = "--cov lvmguider --cov-report xml --cov-report html --cov-report term -W ignore"
 asyncio_mode = "auto"
```

### Comparing `lvmguider-0.5.1/src/lvmguider/__init__.py` & `lvmguider-0.5.2/src/lvmguider/__init__.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/__main__.py` & `lvmguider-0.5.2/src/lvmguider/__main__.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/actor/__init__.py` & `lvmguider-0.5.2/src/lvmguider/actor/__init__.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/actor/actor.py` & `lvmguider-0.5.2/src/lvmguider/actor/actor.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/actor/commands/corrections.py` & `lvmguider-0.5.2/src/lvmguider/actor/commands/corrections.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/actor/commands/expose.py` & `lvmguider-0.5.2/src/lvmguider/actor/commands/expose.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/actor/commands/focus.py` & `lvmguider-0.5.2/src/lvmguider/actor/commands/focus.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/actor/commands/guide.py` & `lvmguider-0.5.2/src/lvmguider/actor/commands/guide.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/actor/commands/set_pixel.py` & `lvmguider-0.5.2/src/lvmguider/actor/commands/set_pixel.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/actor/commands/status.py` & `lvmguider-0.5.2/src/lvmguider/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/actor/commands/stop.py` & `lvmguider-0.5.2/src/lvmguider/actor/commands/stop.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/astrometrynet.py` & `lvmguider-0.5.2/src/lvmguider/astrometrynet.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/cameras.py` & `lvmguider-0.5.2/src/lvmguider/cameras.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/coadd.py` & `lvmguider-0.5.2/src/lvmguider/coadd.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/dataclasses.py` & `lvmguider-0.5.2/src/lvmguider/dataclasses.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/etc/datamodel.yml` & `lvmguider-0.5.2/src/lvmguider/etc/datamodel.yml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
   FWHM: [null, '[arcsec] FWHM from sources']
   RA: [null, '[deg] RA of central pixel from WCS']
   DEC: [null, '[deg] Dec of central pixel from WCS']
   PA: [null, '[deg] Position angle from WCS']
   ZEROPT: [null, '[mag] Zero point of the LVM magnitude']
   ORIGFILE: [null, 'Original file name']
   REPROC: [false, 'Has this file been reprocessed?']
-  REFFILE: [null, 'Reference file for astrometric solution']
+  REFFILE: [null, 'Astrom. solution ref. file']
   ISFSWEEP: [false, 'Is the exposure part of a focus sweep?']
   SOLVED: [false, 'Was an astrometric solution found?']
   WCSMODE: ['none', 'Method for fitting the astrometric solution']
 
 SOURCES:
   thresh: 'f8[pyarrow]'
   npix: 'int32[pyarrow]'
```

### Comparing `lvmguider-0.5.1/src/lvmguider/etc/lvmguider.yml` & `lvmguider-0.5.2/src/lvmguider/etc/lvmguider.yml`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/extraction.py` & `lvmguider-0.5.2/src/lvmguider/extraction.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/focus.py` & `lvmguider-0.5.2/src/lvmguider/focus.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/guider.py` & `lvmguider-0.5.2/src/lvmguider/guider.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     """Acquisition and guiding sequence.
 
     Parameters
     ----------
     command
         The actor command used to communicate with the actor system.
     field_centre
-        The field centre on which we want to guider (RA, Dec, PA).
+        The field centre on which we want to guide (RA, Dec, PA).
     pixel
         The ``(x,y)`` pixel of the full frame to use to determine the pointing.
         Default to the central pixel.
     apply_corrections
         Whether to apply the measured corrections. If `False`, outputs the
         measurements but does not command the telescope.
```

### Comparing `lvmguider-0.5.1/src/lvmguider/maskbits.py` & `lvmguider-0.5.2/src/lvmguider/maskbits.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/plotting.py` & `lvmguider-0.5.2/src/lvmguider/plotting.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/tools.py` & `lvmguider-0.5.2/src/lvmguider/tools.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/src/lvmguider/transformations.py` & `lvmguider-0.5.2/src/lvmguider/transformations.py`

 * *Files 0% similar despite different names*

```diff
@@ -215,15 +215,15 @@
                  [1] - angSlv         Rotation of field
                  [2] - pxScl          Arcsec / pixel of solve
 
     """
 
     lower_bound = 0.8  # Pixel scale hints (arcsec/pixel)
     upper_bound = 1.2
-    radius = 5  # Search radius in degrees
+    radius = 20  # Search radius in degrees
 
     if full_frame:
         midX, midZ = config["xz_full_frame"]  # Middle of full Frame
         index_paths_default = {
             5200: "/data/astrometrynet/5200",
             4100: "/data/astrometrynet/4100",
         }
```

### Comparing `lvmguider-0.5.1/src/lvmguider/types.py` & `lvmguider-0.5.2/src/lvmguider/types.py`

 * *Files identical despite different names*

### Comparing `lvmguider-0.5.1/PKG-INFO` & `lvmguider-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lvmguider
-Version: 0.5.1
+Version: 0.5.2
 Summary: Temporary package for LVM guiding and focusing
 Home-page: https://github.com/sdss/lvmguider
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<3.13
```

