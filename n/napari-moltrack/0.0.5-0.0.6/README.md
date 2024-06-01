# Comparing `tmp/napari_moltrack-0.0.5.tar.gz` & `tmp/napari_moltrack-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_moltrack-0.0.5.tar", last modified: Fri May 31 18:42:22 2024, max compression
+gzip compressed data, was "napari_moltrack-0.0.6.tar", last modified: Fri May 31 18:49:50 2024, max compression
```

## Comparing `napari_moltrack-0.0.5.tar` & `napari_moltrack-0.0.6.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 18:42:22.193609 napari_moltrack-0.0.5/
--rw-rw-rw-   0        0        0     1515 2024-05-29 16:12:09.000000 napari_moltrack-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      101 2024-05-29 16:12:09.000000 napari_moltrack-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6468 2024-05-31 18:42:22.193609 napari_moltrack-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     2705 2024-05-29 16:12:09.000000 napari_moltrack-0.0.5/README.md
--rw-rw-rw-   0        0        0     3406 2024-05-30 17:30:23.000000 napari_moltrack-0.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-31 18:42:22.193609 napari_moltrack-0.0.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-31 18:42:22.108997 napari_moltrack-0.0.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-31 18:42:22.124618 napari_moltrack-0.0.5/src/moltrack/
-drwxrwxrwx   0        0        0        0 2024-05-31 18:42:22.124618 napari_moltrack-0.0.5/src/moltrack/GUI/
--rw-rw-rw-   0        0        0        0 2024-05-29 16:42:16.000000 napari_moltrack-0.0.5/src/moltrack/GUI/__init__.py
--rw-rw-rw-   0        0        0    65658 2024-05-31 18:12:06.000000 napari_moltrack-0.0.5/src/moltrack/GUI/widget_ui.py
--rw-rw-rw-   0        0        0       98 2024-05-31 18:42:09.000000 napari_moltrack-0.0.5/src/moltrack/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 18:42:22.140240 napari_moltrack-0.0.5/src/moltrack/_tests/
--rw-rw-rw-   0        0        0        0 2024-05-29 16:12:09.000000 napari_moltrack-0.0.5/src/moltrack/_tests/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-05-29 16:15:26.000000 napari_moltrack-0.0.5/src/moltrack/_tests/test_widget.py
--rw-rw-rw-   0        0        0     7816 2024-05-31 18:10:07.000000 napari_moltrack-0.0.5/src/moltrack/_widget.py
-drwxrwxrwx   0        0        0        0 2024-05-31 18:42:22.155861 napari_moltrack-0.0.5/src/moltrack/funcs/
--rw-rw-rw-   0        0        0        0 2024-05-30 07:19:51.000000 napari_moltrack-0.0.5/src/moltrack/funcs/__init__.py
--rw-rw-rw-   0        0        0     8053 2024-05-30 10:37:04.000000 napari_moltrack-0.0.5/src/moltrack/funcs/compute_utils.py
--rw-rw-rw-   0        0        0    15734 2024-05-31 17:45:32.000000 napari_moltrack-0.0.5/src/moltrack/funcs/events_utils.py
--rw-rw-rw-   0        0        0     9155 2024-05-31 18:41:20.000000 napari_moltrack-0.0.5/src/moltrack/funcs/export_utils.py
--rw-rw-rw-   0        0        0    12905 2024-05-31 09:24:15.000000 napari_moltrack-0.0.5/src/moltrack/funcs/import_utils.py
--rw-rw-rw-   0        0        0     5422 2024-05-30 10:39:02.000000 napari_moltrack-0.0.5/src/moltrack/funcs/loc_filter_utils.py
--rw-rw-rw-   0        0        0    33886 2024-05-31 17:45:56.000000 napari_moltrack-0.0.5/src/moltrack/funcs/picasso_detect_utils.py
--rw-rw-rw-   0        0        0     3282 2024-05-30 10:49:15.000000 napari_moltrack-0.0.5/src/moltrack/funcs/picasso_render_utils.py
--rw-rw-rw-   0        0        0    10414 2024-05-31 17:30:34.000000 napari_moltrack-0.0.5/src/moltrack/funcs/segmentation_events.py
--rw-rw-rw-   0        0        0    19142 2024-05-31 17:31:51.000000 napari_moltrack-0.0.5/src/moltrack/funcs/segmentation_utils.py
--rw-rw-rw-   0        0        0     4477 2024-05-31 18:18:34.000000 napari_moltrack-0.0.5/src/moltrack/funcs/tracking_utils.py
--rw-rw-rw-   0        0        0      495 2024-05-29 16:15:26.000000 napari_moltrack-0.0.5/src/moltrack/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-05-31 18:42:22.187104 napari_moltrack-0.0.5/src/napari_moltrack.egg-info/
--rw-rw-rw-   0        0        0     6468 2024-05-31 18:42:22.000000 napari_moltrack-0.0.5/src/napari_moltrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2024-05-31 18:42:22.000000 napari_moltrack-0.0.5/src/napari_moltrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 18:42:22.000000 napari_moltrack-0.0.5/src/napari_moltrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-05-31 18:42:22.000000 napari_moltrack-0.0.5/src/napari_moltrack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2024-05-31 18:42:22.000000 napari_moltrack-0.0.5/src/napari_moltrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-05-31 18:42:22.000000 napari_moltrack-0.0.5/src/napari_moltrack.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-31 18:42:22.187104 napari_moltrack-0.0.5/src/pygpufit/
--rw-rw-rw-   0        0        0  1982976 2024-05-21 11:03:35.000000 napari_moltrack-0.0.5/src/pygpufit/Gpufit.dll
--rw-rw-rw-   0        0        0        0 2024-05-21 11:03:35.000000 napari_moltrack-0.0.5/src/pygpufit/__init__.py
--rw-rw-rw-   0        0        0    14512 2024-05-21 11:03:35.000000 napari_moltrack-0.0.5/src/pygpufit/gpufit.py
--rw-rw-rw-   0        0        0      140 2024-05-21 11:03:35.000000 napari_moltrack-0.0.5/src/pygpufit/version.py
+drwxrwxrwx   0        0        0        0 2024-05-31 18:49:50.052069 napari_moltrack-0.0.6/
+-rw-rw-rw-   0        0        0     1515 2024-05-29 16:12:09.000000 napari_moltrack-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-05-29 16:12:09.000000 napari_moltrack-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6468 2024-05-31 18:49:50.036447 napari_moltrack-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2705 2024-05-29 16:12:09.000000 napari_moltrack-0.0.6/README.md
+-rw-rw-rw-   0        0        0     3406 2024-05-30 17:30:23.000000 napari_moltrack-0.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-31 18:49:50.052069 napari_moltrack-0.0.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-31 18:49:49.967448 napari_moltrack-0.0.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-31 18:49:49.989580 napari_moltrack-0.0.6/src/moltrack/
+drwxrwxrwx   0        0        0        0 2024-05-31 18:49:49.989580 napari_moltrack-0.0.6/src/moltrack/GUI/
+-rw-rw-rw-   0        0        0        0 2024-05-29 16:42:16.000000 napari_moltrack-0.0.6/src/moltrack/GUI/__init__.py
+-rw-rw-rw-   0        0        0    65658 2024-05-31 18:12:06.000000 napari_moltrack-0.0.6/src/moltrack/GUI/widget_ui.py
+-rw-rw-rw-   0        0        0       98 2024-05-31 18:49:39.000000 napari_moltrack-0.0.6/src/moltrack/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-31 18:49:49.989580 napari_moltrack-0.0.6/src/moltrack/_tests/
+-rw-rw-rw-   0        0        0        0 2024-05-29 16:12:09.000000 napari_moltrack-0.0.6/src/moltrack/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-05-29 16:15:26.000000 napari_moltrack-0.0.6/src/moltrack/_tests/test_widget.py
+-rw-rw-rw-   0        0        0     7816 2024-05-31 18:10:07.000000 napari_moltrack-0.0.6/src/moltrack/_widget.py
+drwxrwxrwx   0        0        0        0 2024-05-31 18:49:50.005204 napari_moltrack-0.0.6/src/moltrack/funcs/
+-rw-rw-rw-   0        0        0        0 2024-05-30 07:19:51.000000 napari_moltrack-0.0.6/src/moltrack/funcs/__init__.py
+-rw-rw-rw-   0        0        0     8053 2024-05-30 10:37:04.000000 napari_moltrack-0.0.6/src/moltrack/funcs/compute_utils.py
+-rw-rw-rw-   0        0        0    15734 2024-05-31 17:45:32.000000 napari_moltrack-0.0.6/src/moltrack/funcs/events_utils.py
+-rw-rw-rw-   0        0        0     9068 2024-05-31 18:43:16.000000 napari_moltrack-0.0.6/src/moltrack/funcs/export_utils.py
+-rw-rw-rw-   0        0        0    12905 2024-05-31 09:24:15.000000 napari_moltrack-0.0.6/src/moltrack/funcs/import_utils.py
+-rw-rw-rw-   0        0        0     5422 2024-05-30 10:39:02.000000 napari_moltrack-0.0.6/src/moltrack/funcs/loc_filter_utils.py
+-rw-rw-rw-   0        0        0    33886 2024-05-31 17:45:56.000000 napari_moltrack-0.0.6/src/moltrack/funcs/picasso_detect_utils.py
+-rw-rw-rw-   0        0        0     3282 2024-05-30 10:49:15.000000 napari_moltrack-0.0.6/src/moltrack/funcs/picasso_render_utils.py
+-rw-rw-rw-   0        0        0    10414 2024-05-31 17:30:34.000000 napari_moltrack-0.0.6/src/moltrack/funcs/segmentation_events.py
+-rw-rw-rw-   0        0        0    19142 2024-05-31 17:31:51.000000 napari_moltrack-0.0.6/src/moltrack/funcs/segmentation_utils.py
+-rw-rw-rw-   0        0        0     4609 2024-05-31 18:48:23.000000 napari_moltrack-0.0.6/src/moltrack/funcs/tracking_utils.py
+-rw-rw-rw-   0        0        0      495 2024-05-29 16:15:26.000000 napari_moltrack-0.0.6/src/moltrack/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-05-31 18:49:50.036447 napari_moltrack-0.0.6/src/napari_moltrack.egg-info/
+-rw-rw-rw-   0        0        0     6468 2024-05-31 18:49:49.000000 napari_moltrack-0.0.6/src/napari_moltrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2024-05-31 18:49:49.000000 napari_moltrack-0.0.6/src/napari_moltrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 18:49:49.000000 napari_moltrack-0.0.6/src/napari_moltrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-05-31 18:49:49.000000 napari_moltrack-0.0.6/src/napari_moltrack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2024-05-31 18:49:49.000000 napari_moltrack-0.0.6/src/napari_moltrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-31 18:49:49.000000 napari_moltrack-0.0.6/src/napari_moltrack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-31 18:49:50.036447 napari_moltrack-0.0.6/src/pygpufit/
+-rw-rw-rw-   0        0        0  1982976 2024-05-21 11:03:35.000000 napari_moltrack-0.0.6/src/pygpufit/Gpufit.dll
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:03:35.000000 napari_moltrack-0.0.6/src/pygpufit/__init__.py
+-rw-rw-rw-   0        0        0    14512 2024-05-21 11:03:35.000000 napari_moltrack-0.0.6/src/pygpufit/gpufit.py
+-rw-rw-rw-   0        0        0      140 2024-05-21 11:03:35.000000 napari_moltrack-0.0.6/src/pygpufit/version.py
```

### Comparing `napari_moltrack-0.0.5/LICENSE` & `napari_moltrack-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.5/PKG-INFO` & `napari_moltrack-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-moltrack
-Version: 0.0.5
+Version: 0.0.6
 Summary: Single molecule tracking package for Napari
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: 
         Copyright (c) 2024, Piers Turner
         All rights reserved.
```

### Comparing `napari_moltrack-0.0.5/README.md` & `napari_moltrack-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.5/pyproject.toml` & `napari_moltrack-0.0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.5/src/moltrack/GUI/widget_ui.py` & `napari_moltrack-0.0.6/src/moltrack/GUI/widget_ui.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.5/src/moltrack/_tests/test_widget.py` & `napari_moltrack-0.0.6/src/moltrack/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.5/src/moltrack/_widget.py` & `napari_moltrack-0.0.6/src/moltrack/_widget.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.5/src/moltrack/funcs/compute_utils.py` & `napari_moltrack-0.0.6/src/moltrack/funcs/compute_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.5/src/moltrack/funcs/events_utils.py` & `napari_moltrack-0.0.6/src/moltrack/funcs/events_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.5/src/moltrack/funcs/export_utils.py` & `napari_moltrack-0.0.6/src/moltrack/funcs/export_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -179,16 +179,14 @@
 
                 locs, fitted, box_size, min_net_gradient = self.get_export_locs(dataset_name)
 
                 n_locs = len(locs)
 
                 if n_locs > 0:
 
-                    print(fitted, box_size, min_net_gradient, n_locs, dataset_name)
-
                     import_path = self.dataset_dict[dataset_name]["path"]
                     image_shape = self.dataset_dict[dataset_name]["data"].shape
 
                     base, ext = os.path.splitext(import_path)
 
                     hdf5_path = base + f"_moltrack_localisations.hdf5"
                     info_path = base + f"_moltrack_localisations.yaml"
```

### Comparing `napari_moltrack-0.0.5/src/moltrack/funcs/import_utils.py` & `napari_moltrack-0.0.6/src/moltrack/funcs/import_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.5/src/moltrack/funcs/loc_filter_utils.py` & `napari_moltrack-0.0.6/src/moltrack/funcs/loc_filter_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.5/src/moltrack/funcs/picasso_detect_utils.py` & `napari_moltrack-0.0.6/src/moltrack/funcs/picasso_detect_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.5/src/moltrack/funcs/picasso_render_utils.py` & `napari_moltrack-0.0.6/src/moltrack/funcs/picasso_render_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.5/src/moltrack/funcs/segmentation_events.py` & `napari_moltrack-0.0.6/src/moltrack/funcs/segmentation_events.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.5/src/moltrack/funcs/segmentation_utils.py` & `napari_moltrack-0.0.6/src/moltrack/funcs/segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.5/src/moltrack/funcs/tracking_utils.py` & `napari_moltrack-0.0.6/src/moltrack/funcs/tracking_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,15 @@
             memory = int(self.gui.trackpy_memory.value())
             min_track_length = int(self.gui.min_track_length.value())
 
             columns = list(locs.dtype.names)
 
             locdf = pd.DataFrame(locs, columns=columns)
 
+            tp.quiet()
             tracks_df = tp.link(
                 locdf, search_range=search_range, memory=memory
             )
 
             # Count the frames per track
             track_lengths = tracks_df.groupby("particle").size()
 
@@ -56,14 +57,17 @@
 
         try:
             dataset = self.gui.tracking_dataset.currentText()
 
             if dataset not in self.tracking_dict.keys():
                 self.tracking_dict[dataset] = tracks
 
+            n_tracks = np.unique(tracks["particle"])
+            print(f"Found {len(n_tracks)} tracks")
+
             remove_unlinked = self.gui.remove_unlinked.isChecked()
             n_frames = self.dataset_dict[dataset]["data"].shape[0]
 
             layers_names = [layer.name for layer in self.viewer.layers]
 
             render_tracks = pd.DataFrame(tracks)
             render_tracks = render_tracks[["particle", "frame", "y", "x"]]
```

### Comparing `napari_moltrack-0.0.5/src/napari_moltrack.egg-info/PKG-INFO` & `napari_moltrack-0.0.6/src/napari_moltrack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-moltrack
-Version: 0.0.5
+Version: 0.0.6
 Summary: Single molecule tracking package for Napari
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: 
         Copyright (c) 2024, Piers Turner
         All rights reserved.
```

### Comparing `napari_moltrack-0.0.5/src/napari_moltrack.egg-info/SOURCES.txt` & `napari_moltrack-0.0.6/src/napari_moltrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.5/src/pygpufit/Gpufit.dll` & `napari_moltrack-0.0.6/src/pygpufit/Gpufit.dll`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.5/src/pygpufit/gpufit.py` & `napari_moltrack-0.0.6/src/pygpufit/gpufit.py`

 * *Files identical despite different names*

