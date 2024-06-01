# Comparing `tmp/napari_moltrack-0.0.8.tar.gz` & `tmp/napari_moltrack-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_moltrack-0.0.8.tar", last modified: Sat Jun  1 07:31:16 2024, max compression
+gzip compressed data, was "napari_moltrack-0.0.9.tar", last modified: Sat Jun  1 07:46:34 2024, max compression
```

## Comparing `napari_moltrack-0.0.8.tar` & `napari_moltrack-0.0.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 07:31:16.001935 napari_moltrack-0.0.8/
--rw-rw-rw-   0        0        0     1515 2024-05-29 16:12:09.000000 napari_moltrack-0.0.8/LICENSE
--rw-rw-rw-   0        0        0      101 2024-05-29 16:12:09.000000 napari_moltrack-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     6468 2024-06-01 07:31:16.000965 napari_moltrack-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     2705 2024-05-29 16:12:09.000000 napari_moltrack-0.0.8/README.md
--rw-rw-rw-   0        0        0     3406 2024-05-30 17:30:23.000000 napari_moltrack-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-01 07:31:16.001935 napari_moltrack-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-01 07:31:15.929432 napari_moltrack-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2024-06-01 07:31:15.941005 napari_moltrack-0.0.8/src/moltrack/
-drwxrwxrwx   0        0        0        0 2024-06-01 07:31:15.943119 napari_moltrack-0.0.8/src/moltrack/GUI/
--rw-rw-rw-   0        0        0        0 2024-05-29 16:42:16.000000 napari_moltrack-0.0.8/src/moltrack/GUI/__init__.py
--rw-rw-rw-   0        0        0    67574 2024-06-01 07:17:47.000000 napari_moltrack-0.0.8/src/moltrack/GUI/widget_ui.py
--rw-rw-rw-   0        0        0       98 2024-06-01 07:31:07.000000 napari_moltrack-0.0.8/src/moltrack/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 07:31:15.947116 napari_moltrack-0.0.8/src/moltrack/_tests/
--rw-rw-rw-   0        0        0        0 2024-05-29 16:12:09.000000 napari_moltrack-0.0.8/src/moltrack/_tests/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-05-29 16:15:26.000000 napari_moltrack-0.0.8/src/moltrack/_tests/test_widget.py
--rw-rw-rw-   0        0        0     7126 2024-06-01 07:30:15.000000 napari_moltrack-0.0.8/src/moltrack/_widget.py
-drwxrwxrwx   0        0        0        0 2024-06-01 07:31:15.966059 napari_moltrack-0.0.8/src/moltrack/funcs/
--rw-rw-rw-   0        0        0        0 2024-05-30 07:19:51.000000 napari_moltrack-0.0.8/src/moltrack/funcs/__init__.py
--rw-rw-rw-   0        0        0     8053 2024-05-30 10:37:04.000000 napari_moltrack-0.0.8/src/moltrack/funcs/compute_utils.py
--rw-rw-rw-   0        0        0    15734 2024-05-31 17:45:32.000000 napari_moltrack-0.0.8/src/moltrack/funcs/events_utils.py
--rw-rw-rw-   0        0        0     9068 2024-05-31 18:43:16.000000 napari_moltrack-0.0.8/src/moltrack/funcs/export_utils.py
--rw-rw-rw-   0        0        0    12905 2024-05-31 09:24:15.000000 napari_moltrack-0.0.8/src/moltrack/funcs/import_utils.py
--rw-rw-rw-   0        0        0     5422 2024-05-30 10:39:02.000000 napari_moltrack-0.0.8/src/moltrack/funcs/loc_filter_utils.py
--rw-rw-rw-   0        0        0    33886 2024-05-31 17:45:56.000000 napari_moltrack-0.0.8/src/moltrack/funcs/picasso_detect_utils.py
--rw-rw-rw-   0        0        0     3282 2024-05-30 10:49:15.000000 napari_moltrack-0.0.8/src/moltrack/funcs/picasso_render_utils.py
--rw-rw-rw-   0        0        0    11810 2024-06-01 07:08:45.000000 napari_moltrack-0.0.8/src/moltrack/funcs/segmentation_events.py
--rw-rw-rw-   0        0        0    19377 2024-06-01 06:45:42.000000 napari_moltrack-0.0.8/src/moltrack/funcs/segmentation_utils.py
--rw-rw-rw-   0        0        0     4609 2024-05-31 18:48:23.000000 napari_moltrack-0.0.8/src/moltrack/funcs/tracking_utils.py
--rw-rw-rw-   0        0        0      495 2024-05-29 16:15:26.000000 napari_moltrack-0.0.8/src/moltrack/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-06-01 07:31:15.997973 napari_moltrack-0.0.8/src/napari_moltrack.egg-info/
--rw-rw-rw-   0        0        0     6468 2024-06-01 07:31:15.000000 napari_moltrack-0.0.8/src/napari_moltrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2024-06-01 07:31:15.000000 napari_moltrack-0.0.8/src/napari_moltrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 07:31:15.000000 napari_moltrack-0.0.8/src/napari_moltrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-06-01 07:31:15.000000 napari_moltrack-0.0.8/src/napari_moltrack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2024-06-01 07:31:15.000000 napari_moltrack-0.0.8/src/napari_moltrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-06-01 07:31:15.000000 napari_moltrack-0.0.8/src/napari_moltrack.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-01 07:31:15.995979 napari_moltrack-0.0.8/src/pygpufit/
--rw-rw-rw-   0        0        0  1982976 2024-05-21 11:03:35.000000 napari_moltrack-0.0.8/src/pygpufit/Gpufit.dll
--rw-rw-rw-   0        0        0        0 2024-05-21 11:03:35.000000 napari_moltrack-0.0.8/src/pygpufit/__init__.py
--rw-rw-rw-   0        0        0    14512 2024-05-21 11:03:35.000000 napari_moltrack-0.0.8/src/pygpufit/gpufit.py
--rw-rw-rw-   0        0        0      140 2024-05-21 11:03:35.000000 napari_moltrack-0.0.8/src/pygpufit/version.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:46:34.992834 napari_moltrack-0.0.9/
+-rw-rw-rw-   0        0        0     1515 2024-05-29 16:12:09.000000 napari_moltrack-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-05-29 16:12:09.000000 napari_moltrack-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     7205 2024-06-01 07:46:34.991838 napari_moltrack-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3442 2024-06-01 07:46:05.000000 napari_moltrack-0.0.9/README.md
+-rw-rw-rw-   0        0        0     3406 2024-05-30 17:30:23.000000 napari_moltrack-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-01 07:46:34.992834 napari_moltrack-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-01 07:46:34.925690 napari_moltrack-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 07:46:34.937838 napari_moltrack-0.0.9/src/moltrack/
+drwxrwxrwx   0        0        0        0 2024-06-01 07:46:34.940931 napari_moltrack-0.0.9/src/moltrack/GUI/
+-rw-rw-rw-   0        0        0        0 2024-05-29 16:42:16.000000 napari_moltrack-0.0.9/src/moltrack/GUI/__init__.py
+-rw-rw-rw-   0        0        0    67574 2024-06-01 07:17:47.000000 napari_moltrack-0.0.9/src/moltrack/GUI/widget_ui.py
+-rw-rw-rw-   0        0        0       98 2024-06-01 07:46:27.000000 napari_moltrack-0.0.9/src/moltrack/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:46:34.943922 napari_moltrack-0.0.9/src/moltrack/_tests/
+-rw-rw-rw-   0        0        0        0 2024-05-29 16:12:09.000000 napari_moltrack-0.0.9/src/moltrack/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-05-29 16:15:26.000000 napari_moltrack-0.0.9/src/moltrack/_tests/test_widget.py
+-rw-rw-rw-   0        0        0     7126 2024-06-01 07:30:15.000000 napari_moltrack-0.0.9/src/moltrack/_widget.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:46:34.961709 napari_moltrack-0.0.9/src/moltrack/funcs/
+-rw-rw-rw-   0        0        0        0 2024-05-30 07:19:51.000000 napari_moltrack-0.0.9/src/moltrack/funcs/__init__.py
+-rw-rw-rw-   0        0        0     8053 2024-05-30 10:37:04.000000 napari_moltrack-0.0.9/src/moltrack/funcs/compute_utils.py
+-rw-rw-rw-   0        0        0    15734 2024-05-31 17:45:32.000000 napari_moltrack-0.0.9/src/moltrack/funcs/events_utils.py
+-rw-rw-rw-   0        0        0     9068 2024-05-31 18:43:16.000000 napari_moltrack-0.0.9/src/moltrack/funcs/export_utils.py
+-rw-rw-rw-   0        0        0    12905 2024-05-31 09:24:15.000000 napari_moltrack-0.0.9/src/moltrack/funcs/import_utils.py
+-rw-rw-rw-   0        0        0     5422 2024-05-30 10:39:02.000000 napari_moltrack-0.0.9/src/moltrack/funcs/loc_filter_utils.py
+-rw-rw-rw-   0        0        0    33886 2024-05-31 17:45:56.000000 napari_moltrack-0.0.9/src/moltrack/funcs/picasso_detect_utils.py
+-rw-rw-rw-   0        0        0     3282 2024-05-30 10:49:15.000000 napari_moltrack-0.0.9/src/moltrack/funcs/picasso_render_utils.py
+-rw-rw-rw-   0        0        0    11810 2024-06-01 07:08:45.000000 napari_moltrack-0.0.9/src/moltrack/funcs/segmentation_events.py
+-rw-rw-rw-   0        0        0    19377 2024-06-01 06:45:42.000000 napari_moltrack-0.0.9/src/moltrack/funcs/segmentation_utils.py
+-rw-rw-rw-   0        0        0     4609 2024-05-31 18:48:23.000000 napari_moltrack-0.0.9/src/moltrack/funcs/tracking_utils.py
+-rw-rw-rw-   0        0        0      495 2024-05-29 16:15:26.000000 napari_moltrack-0.0.9/src/moltrack/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-06-01 07:46:34.989843 napari_moltrack-0.0.9/src/napari_moltrack.egg-info/
+-rw-rw-rw-   0        0        0     7205 2024-06-01 07:46:34.000000 napari_moltrack-0.0.9/src/napari_moltrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2024-06-01 07:46:34.000000 napari_moltrack-0.0.9/src/napari_moltrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 07:46:34.000000 napari_moltrack-0.0.9/src/napari_moltrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-06-01 07:46:34.000000 napari_moltrack-0.0.9/src/napari_moltrack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2024-06-01 07:46:34.000000 napari_moltrack-0.0.9/src/napari_moltrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-06-01 07:46:34.000000 napari_moltrack-0.0.9/src/napari_moltrack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 07:46:34.986850 napari_moltrack-0.0.9/src/pygpufit/
+-rw-rw-rw-   0        0        0  1982976 2024-05-21 11:03:35.000000 napari_moltrack-0.0.9/src/pygpufit/Gpufit.dll
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:03:35.000000 napari_moltrack-0.0.9/src/pygpufit/__init__.py
+-rw-rw-rw-   0        0        0    14512 2024-05-21 11:03:35.000000 napari_moltrack-0.0.9/src/pygpufit/gpufit.py
+-rw-rw-rw-   0        0        0      140 2024-05-21 11:03:35.000000 napari_moltrack-0.0.9/src/pygpufit/version.py
```

### Comparing `napari_moltrack-0.0.8/LICENSE` & `napari_moltrack-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/PKG-INFO` & `napari_moltrack-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-moltrack
-Version: 0.0.8
+Version: 0.0.9
 Summary: Single molecule tracking package for Napari
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: 
         Copyright (c) 2024, Piers Turner
         All rights reserved.
         
@@ -86,15 +86,25 @@
 [![License BSD-3](https://img.shields.io/pypi/l/napari-moltrack.svg?color=green)](https://github.com/piedrro/napari-moltrack/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-moltrack.svg?color=green)](https://pypi.org/project/napari-moltrack)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-moltrack.svg?color=green)](https://python.org)
 [![tests](https://github.com/piedrro/napari-moltrack/workflows/tests/badge.svg)](https://github.com/piedrro/napari-moltrack/actions)
 [![codecov](https://codecov.io/gh/piedrro/napari-moltrack/branch/main/graph/badge.svg)](https://codecov.io/gh/piedrro/napari-moltrack)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-moltrack)](https://napari-hub.org/plugins/napari-moltrack)
 
-Single molecule tracking package for Napari
+A plugin for single molecule localisation and tracking based on **Picasso**, **GPUfit** and **Trackpy**. Designed to work with single channel .tif and .fits files.
+
+All functions are parallelised/GPU accelerated where possible to increase performance. Multiple files can  be loaded and processed in parallel.
+
+Single molecule localisations can be filtered by their properties (e.g. photons, width, etc.) and can be rendered as a super resolution image.
+
+Segmentations can be used to exlude regions from single molecule localisaton and tracking. Segmentations can be added automatically using Cellpose or can be added manually.
+
+napari-moltrack was written by Piers Turner, Kapanidis Group, University of Oxford.
+
+https://www.physics.ox.ac.uk/research/group/gene-machines
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
```

### Comparing `napari_moltrack-0.0.8/README.md` & `napari_moltrack-0.0.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -3,15 +3,25 @@
 [![License BSD-3](https://img.shields.io/pypi/l/napari-moltrack.svg?color=green)](https://github.com/piedrro/napari-moltrack/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-moltrack.svg?color=green)](https://pypi.org/project/napari-moltrack)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-moltrack.svg?color=green)](https://python.org)
 [![tests](https://github.com/piedrro/napari-moltrack/workflows/tests/badge.svg)](https://github.com/piedrro/napari-moltrack/actions)
 [![codecov](https://codecov.io/gh/piedrro/napari-moltrack/branch/main/graph/badge.svg)](https://codecov.io/gh/piedrro/napari-moltrack)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-moltrack)](https://napari-hub.org/plugins/napari-moltrack)
 
-Single molecule tracking package for Napari
+A plugin for single molecule localisation and tracking based on **Picasso**, **GPUfit** and **Trackpy**. Designed to work with single channel .tif and .fits files.
+
+All functions are parallelised/GPU accelerated where possible to increase performance. Multiple files can  be loaded and processed in parallel.
+
+Single molecule localisations can be filtered by their properties (e.g. photons, width, etc.) and can be rendered as a super resolution image.
+
+Segmentations can be used to exlude regions from single molecule localisaton and tracking. Segmentations can be added automatically using Cellpose or can be added manually.
+
+napari-moltrack was written by Piers Turner, Kapanidis Group, University of Oxford.
+
+https://www.physics.ox.ac.uk/research/group/gene-machines
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
```

### Comparing `napari_moltrack-0.0.8/pyproject.toml` & `napari_moltrack-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/src/moltrack/GUI/widget_ui.py` & `napari_moltrack-0.0.9/src/moltrack/GUI/widget_ui.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/src/moltrack/_tests/test_widget.py` & `napari_moltrack-0.0.9/src/moltrack/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/src/moltrack/_widget.py` & `napari_moltrack-0.0.9/src/moltrack/_widget.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/src/moltrack/funcs/compute_utils.py` & `napari_moltrack-0.0.9/src/moltrack/funcs/compute_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/src/moltrack/funcs/events_utils.py` & `napari_moltrack-0.0.9/src/moltrack/funcs/events_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/src/moltrack/funcs/export_utils.py` & `napari_moltrack-0.0.9/src/moltrack/funcs/export_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/src/moltrack/funcs/import_utils.py` & `napari_moltrack-0.0.9/src/moltrack/funcs/import_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/src/moltrack/funcs/loc_filter_utils.py` & `napari_moltrack-0.0.9/src/moltrack/funcs/loc_filter_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/src/moltrack/funcs/picasso_detect_utils.py` & `napari_moltrack-0.0.9/src/moltrack/funcs/picasso_detect_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/src/moltrack/funcs/picasso_render_utils.py` & `napari_moltrack-0.0.9/src/moltrack/funcs/picasso_render_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/src/moltrack/funcs/segmentation_events.py` & `napari_moltrack-0.0.9/src/moltrack/funcs/segmentation_events.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/src/moltrack/funcs/segmentation_utils.py` & `napari_moltrack-0.0.9/src/moltrack/funcs/segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/src/moltrack/funcs/tracking_utils.py` & `napari_moltrack-0.0.9/src/moltrack/funcs/tracking_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/src/napari_moltrack.egg-info/PKG-INFO` & `napari_moltrack-0.0.9/src/napari_moltrack.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-moltrack
-Version: 0.0.8
+Version: 0.0.9
 Summary: Single molecule tracking package for Napari
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: 
         Copyright (c) 2024, Piers Turner
         All rights reserved.
         
@@ -86,15 +86,25 @@
 [![License BSD-3](https://img.shields.io/pypi/l/napari-moltrack.svg?color=green)](https://github.com/piedrro/napari-moltrack/raw/main/LICENSE)
 [![PyPI](https://img.shields.io/pypi/v/napari-moltrack.svg?color=green)](https://pypi.org/project/napari-moltrack)
 [![Python Version](https://img.shields.io/pypi/pyversions/napari-moltrack.svg?color=green)](https://python.org)
 [![tests](https://github.com/piedrro/napari-moltrack/workflows/tests/badge.svg)](https://github.com/piedrro/napari-moltrack/actions)
 [![codecov](https://codecov.io/gh/piedrro/napari-moltrack/branch/main/graph/badge.svg)](https://codecov.io/gh/piedrro/napari-moltrack)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-moltrack)](https://napari-hub.org/plugins/napari-moltrack)
 
-Single molecule tracking package for Napari
+A plugin for single molecule localisation and tracking based on **Picasso**, **GPUfit** and **Trackpy**. Designed to work with single channel .tif and .fits files.
+
+All functions are parallelised/GPU accelerated where possible to increase performance. Multiple files can  be loaded and processed in parallel.
+
+Single molecule localisations can be filtered by their properties (e.g. photons, width, etc.) and can be rendered as a super resolution image.
+
+Segmentations can be used to exlude regions from single molecule localisaton and tracking. Segmentations can be added automatically using Cellpose or can be added manually.
+
+napari-moltrack was written by Piers Turner, Kapanidis Group, University of Oxford.
+
+https://www.physics.ox.ac.uk/research/group/gene-machines
 
 ----------------------------------
 
 This [napari] plugin was generated with [Cookiecutter] using [@napari]'s [cookiecutter-napari-plugin] template.
 
 <!--
 Don't miss the full getting started guide to set up your new package:
```

### Comparing `napari_moltrack-0.0.8/src/napari_moltrack.egg-info/SOURCES.txt` & `napari_moltrack-0.0.9/src/napari_moltrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/src/pygpufit/Gpufit.dll` & `napari_moltrack-0.0.9/src/pygpufit/Gpufit.dll`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.8/src/pygpufit/gpufit.py` & `napari_moltrack-0.0.9/src/pygpufit/gpufit.py`

 * *Files identical despite different names*

