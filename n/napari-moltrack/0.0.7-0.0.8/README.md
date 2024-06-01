# Comparing `tmp/napari_moltrack-0.0.7.tar.gz` & `tmp/napari_moltrack-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari_moltrack-0.0.7.tar", last modified: Sat Jun  1 07:19:53 2024, max compression
+gzip compressed data, was "napari_moltrack-0.0.8.tar", last modified: Sat Jun  1 07:31:16 2024, max compression
```

## Comparing `napari_moltrack-0.0.7.tar` & `napari_moltrack-0.0.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 07:19:53.751804 napari_moltrack-0.0.7/
--rw-rw-rw-   0        0        0     1515 2024-05-29 16:12:09.000000 napari_moltrack-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      101 2024-05-29 16:12:09.000000 napari_moltrack-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     6468 2024-06-01 07:19:53.750834 napari_moltrack-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2705 2024-05-29 16:12:09.000000 napari_moltrack-0.0.7/README.md
--rw-rw-rw-   0        0        0     3406 2024-05-30 17:30:23.000000 napari_moltrack-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-01 07:19:53.751804 napari_moltrack-0.0.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-01 07:19:53.683434 napari_moltrack-0.0.7/src/
-drwxrwxrwx   0        0        0        0 2024-06-01 07:19:53.695432 napari_moltrack-0.0.7/src/moltrack/
-drwxrwxrwx   0        0        0        0 2024-06-01 07:19:53.698396 napari_moltrack-0.0.7/src/moltrack/GUI/
--rw-rw-rw-   0        0        0        0 2024-05-29 16:42:16.000000 napari_moltrack-0.0.7/src/moltrack/GUI/__init__.py
--rw-rw-rw-   0        0        0    67574 2024-06-01 07:17:47.000000 napari_moltrack-0.0.7/src/moltrack/GUI/widget_ui.py
--rw-rw-rw-   0        0        0       98 2024-06-01 07:19:45.000000 napari_moltrack-0.0.7/src/moltrack/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 07:19:53.701389 napari_moltrack-0.0.7/src/moltrack/_tests/
--rw-rw-rw-   0        0        0        0 2024-05-29 16:12:09.000000 napari_moltrack-0.0.7/src/moltrack/_tests/__init__.py
--rw-rw-rw-   0        0        0     2172 2024-05-29 16:15:26.000000 napari_moltrack-0.0.7/src/moltrack/_tests/test_widget.py
--rw-rw-rw-   0        0        0     7816 2024-05-31 18:10:07.000000 napari_moltrack-0.0.7/src/moltrack/_widget.py
-drwxrwxrwx   0        0        0        0 2024-06-01 07:19:53.719270 napari_moltrack-0.0.7/src/moltrack/funcs/
--rw-rw-rw-   0        0        0        0 2024-05-30 07:19:51.000000 napari_moltrack-0.0.7/src/moltrack/funcs/__init__.py
--rw-rw-rw-   0        0        0     8053 2024-05-30 10:37:04.000000 napari_moltrack-0.0.7/src/moltrack/funcs/compute_utils.py
--rw-rw-rw-   0        0        0    15734 2024-05-31 17:45:32.000000 napari_moltrack-0.0.7/src/moltrack/funcs/events_utils.py
--rw-rw-rw-   0        0        0     9068 2024-05-31 18:43:16.000000 napari_moltrack-0.0.7/src/moltrack/funcs/export_utils.py
--rw-rw-rw-   0        0        0    12905 2024-05-31 09:24:15.000000 napari_moltrack-0.0.7/src/moltrack/funcs/import_utils.py
--rw-rw-rw-   0        0        0     5422 2024-05-30 10:39:02.000000 napari_moltrack-0.0.7/src/moltrack/funcs/loc_filter_utils.py
--rw-rw-rw-   0        0        0    33886 2024-05-31 17:45:56.000000 napari_moltrack-0.0.7/src/moltrack/funcs/picasso_detect_utils.py
--rw-rw-rw-   0        0        0     3282 2024-05-30 10:49:15.000000 napari_moltrack-0.0.7/src/moltrack/funcs/picasso_render_utils.py
--rw-rw-rw-   0        0        0    11810 2024-06-01 07:08:45.000000 napari_moltrack-0.0.7/src/moltrack/funcs/segmentation_events.py
--rw-rw-rw-   0        0        0    19377 2024-06-01 06:45:42.000000 napari_moltrack-0.0.7/src/moltrack/funcs/segmentation_utils.py
--rw-rw-rw-   0        0        0     4609 2024-05-31 18:48:23.000000 napari_moltrack-0.0.7/src/moltrack/funcs/tracking_utils.py
--rw-rw-rw-   0        0        0      495 2024-05-29 16:15:26.000000 napari_moltrack-0.0.7/src/moltrack/napari.yaml
-drwxrwxrwx   0        0        0        0 2024-06-01 07:19:53.748839 napari_moltrack-0.0.7/src/napari_moltrack.egg-info/
--rw-rw-rw-   0        0        0     6468 2024-06-01 07:19:53.000000 napari_moltrack-0.0.7/src/napari_moltrack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1017 2024-06-01 07:19:53.000000 napari_moltrack-0.0.7/src/napari_moltrack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 07:19:53.000000 napari_moltrack-0.0.7/src/napari_moltrack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-06-01 07:19:53.000000 napari_moltrack-0.0.7/src/napari_moltrack.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      234 2024-06-01 07:19:53.000000 napari_moltrack-0.0.7/src/napari_moltrack.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-06-01 07:19:53.000000 napari_moltrack-0.0.7/src/napari_moltrack.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-06-01 07:19:53.745849 napari_moltrack-0.0.7/src/pygpufit/
--rw-rw-rw-   0        0        0  1982976 2024-05-21 11:03:35.000000 napari_moltrack-0.0.7/src/pygpufit/Gpufit.dll
--rw-rw-rw-   0        0        0        0 2024-05-21 11:03:35.000000 napari_moltrack-0.0.7/src/pygpufit/__init__.py
--rw-rw-rw-   0        0        0    14512 2024-05-21 11:03:35.000000 napari_moltrack-0.0.7/src/pygpufit/gpufit.py
--rw-rw-rw-   0        0        0      140 2024-05-21 11:03:35.000000 napari_moltrack-0.0.7/src/pygpufit/version.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:31:16.001935 napari_moltrack-0.0.8/
+-rw-rw-rw-   0        0        0     1515 2024-05-29 16:12:09.000000 napari_moltrack-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      101 2024-05-29 16:12:09.000000 napari_moltrack-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     6468 2024-06-01 07:31:16.000965 napari_moltrack-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2705 2024-05-29 16:12:09.000000 napari_moltrack-0.0.8/README.md
+-rw-rw-rw-   0        0        0     3406 2024-05-30 17:30:23.000000 napari_moltrack-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-01 07:31:16.001935 napari_moltrack-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-01 07:31:15.929432 napari_moltrack-0.0.8/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 07:31:15.941005 napari_moltrack-0.0.8/src/moltrack/
+drwxrwxrwx   0        0        0        0 2024-06-01 07:31:15.943119 napari_moltrack-0.0.8/src/moltrack/GUI/
+-rw-rw-rw-   0        0        0        0 2024-05-29 16:42:16.000000 napari_moltrack-0.0.8/src/moltrack/GUI/__init__.py
+-rw-rw-rw-   0        0        0    67574 2024-06-01 07:17:47.000000 napari_moltrack-0.0.8/src/moltrack/GUI/widget_ui.py
+-rw-rw-rw-   0        0        0       98 2024-06-01 07:31:07.000000 napari_moltrack-0.0.8/src/moltrack/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:31:15.947116 napari_moltrack-0.0.8/src/moltrack/_tests/
+-rw-rw-rw-   0        0        0        0 2024-05-29 16:12:09.000000 napari_moltrack-0.0.8/src/moltrack/_tests/__init__.py
+-rw-rw-rw-   0        0        0     2172 2024-05-29 16:15:26.000000 napari_moltrack-0.0.8/src/moltrack/_tests/test_widget.py
+-rw-rw-rw-   0        0        0     7126 2024-06-01 07:30:15.000000 napari_moltrack-0.0.8/src/moltrack/_widget.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:31:15.966059 napari_moltrack-0.0.8/src/moltrack/funcs/
+-rw-rw-rw-   0        0        0        0 2024-05-30 07:19:51.000000 napari_moltrack-0.0.8/src/moltrack/funcs/__init__.py
+-rw-rw-rw-   0        0        0     8053 2024-05-30 10:37:04.000000 napari_moltrack-0.0.8/src/moltrack/funcs/compute_utils.py
+-rw-rw-rw-   0        0        0    15734 2024-05-31 17:45:32.000000 napari_moltrack-0.0.8/src/moltrack/funcs/events_utils.py
+-rw-rw-rw-   0        0        0     9068 2024-05-31 18:43:16.000000 napari_moltrack-0.0.8/src/moltrack/funcs/export_utils.py
+-rw-rw-rw-   0        0        0    12905 2024-05-31 09:24:15.000000 napari_moltrack-0.0.8/src/moltrack/funcs/import_utils.py
+-rw-rw-rw-   0        0        0     5422 2024-05-30 10:39:02.000000 napari_moltrack-0.0.8/src/moltrack/funcs/loc_filter_utils.py
+-rw-rw-rw-   0        0        0    33886 2024-05-31 17:45:56.000000 napari_moltrack-0.0.8/src/moltrack/funcs/picasso_detect_utils.py
+-rw-rw-rw-   0        0        0     3282 2024-05-30 10:49:15.000000 napari_moltrack-0.0.8/src/moltrack/funcs/picasso_render_utils.py
+-rw-rw-rw-   0        0        0    11810 2024-06-01 07:08:45.000000 napari_moltrack-0.0.8/src/moltrack/funcs/segmentation_events.py
+-rw-rw-rw-   0        0        0    19377 2024-06-01 06:45:42.000000 napari_moltrack-0.0.8/src/moltrack/funcs/segmentation_utils.py
+-rw-rw-rw-   0        0        0     4609 2024-05-31 18:48:23.000000 napari_moltrack-0.0.8/src/moltrack/funcs/tracking_utils.py
+-rw-rw-rw-   0        0        0      495 2024-05-29 16:15:26.000000 napari_moltrack-0.0.8/src/moltrack/napari.yaml
+drwxrwxrwx   0        0        0        0 2024-06-01 07:31:15.997973 napari_moltrack-0.0.8/src/napari_moltrack.egg-info/
+-rw-rw-rw-   0        0        0     6468 2024-06-01 07:31:15.000000 napari_moltrack-0.0.8/src/napari_moltrack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1017 2024-06-01 07:31:15.000000 napari_moltrack-0.0.8/src/napari_moltrack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 07:31:15.000000 napari_moltrack-0.0.8/src/napari_moltrack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-06-01 07:31:15.000000 napari_moltrack-0.0.8/src/napari_moltrack.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      234 2024-06-01 07:31:15.000000 napari_moltrack-0.0.8/src/napari_moltrack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-06-01 07:31:15.000000 napari_moltrack-0.0.8/src/napari_moltrack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 07:31:15.995979 napari_moltrack-0.0.8/src/pygpufit/
+-rw-rw-rw-   0        0        0  1982976 2024-05-21 11:03:35.000000 napari_moltrack-0.0.8/src/pygpufit/Gpufit.dll
+-rw-rw-rw-   0        0        0        0 2024-05-21 11:03:35.000000 napari_moltrack-0.0.8/src/pygpufit/__init__.py
+-rw-rw-rw-   0        0        0    14512 2024-05-21 11:03:35.000000 napari_moltrack-0.0.8/src/pygpufit/gpufit.py
+-rw-rw-rw-   0        0        0      140 2024-05-21 11:03:35.000000 napari_moltrack-0.0.8/src/pygpufit/version.py
```

### Comparing `napari_moltrack-0.0.7/LICENSE` & `napari_moltrack-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/PKG-INFO` & `napari_moltrack-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-moltrack
-Version: 0.0.7
+Version: 0.0.8
 Summary: Single molecule tracking package for Napari
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: 
         Copyright (c) 2024, Piers Turner
         All rights reserved.
```

### Comparing `napari_moltrack-0.0.7/README.md` & `napari_moltrack-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/pyproject.toml` & `napari_moltrack-0.0.8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/src/moltrack/GUI/widget_ui.py` & `napari_moltrack-0.0.8/src/moltrack/GUI/widget_ui.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/src/moltrack/_tests/test_widget.py` & `napari_moltrack-0.0.8/src/moltrack/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/src/moltrack/_widget.py` & `napari_moltrack-0.0.8/src/moltrack/_widget.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,26 +17,15 @@
 from moltrack.funcs.picasso_detect_utils import _picasso_detect_utils
 from moltrack.funcs.picasso_render_utils import _picasso_render_utils
 from moltrack.funcs.segmentation_events import _segmentation_events
 from moltrack.funcs.segmentation_utils import _segmentation_utils
 from moltrack.funcs.tracking_utils import _tracking_utils
 from moltrack.GUI.widget_ui import Ui_Frame as gui
 
-subclasses = [
-    _import_utils,
-    _compute_utils,
-    _events_utils,
-    _segmentation_utils,
-    _picasso_detect_utils,
-    _loc_filter_utils,
-    _picasso_render_utils,
-    _tracking_utils,
-    _export_utils,
-    _segmentation_events,
-]
+subclasses = [_import_utils, _compute_utils, _events_utils, _segmentation_utils, _picasso_detect_utils, _loc_filter_utils, _picasso_render_utils, _tracking_utils, _export_utils, _segmentation_events, ]
 
 
 class CustomPyQTGraphWidget(pg.GraphicsLayoutWidget):
 
     def __init__(self, parent):
         super().__init__()
 
@@ -69,168 +58,107 @@
 
         # create threadpool and stop event
         self.threadpool = QThreadPool()
         manager = Manager()
         self.stop_event = manager.Event()
 
     def initialise_variables(self):
-
         # initialise graph PyQtGraph canvases
         self.gui.filter_graph_container.setLayout(QVBoxLayout())
         self.filter_graph_canvas = CustomPyQTGraphWidget(self)
-        self.gui.filter_graph_container.layout().addWidget(
-            self.filter_graph_canvas
-        )
+        self.gui.filter_graph_container.layout().addWidget(self.filter_graph_canvas)
 
         self.dataset_dict = {}
         self.localisation_dict = {}
         self.tracking_dict = {}
         self.contrast_dict = {}
 
         self.active_dataset = None
 
         self.verbose = False
 
         self.segmentation_mode = "panzoom"
         self.interface_mode = "segment"
 
     def initialise_events(self):
-
         self.gui.import_images.clicked.connect(self.init_import_data)
-        self.gui.moltrack_dataset_selector.currentIndexChanged.connect(
-            self.update_active_image
-        )
-
-        self.gui.segment_active.clicked.connect(
-            partial(self.initialise_cellpose, mode="active")
-        )
-        self.gui.segment_all.clicked.connect(
-            partial(self.initialise_cellpose, mode="all")
-        )
+        self.gui.moltrack_dataset_selector.currentIndexChanged.connect(self.update_active_image)
+
+        self.gui.segment_active.clicked.connect(partial(self.initialise_cellpose, mode="active"))
+        self.gui.segment_all.clicked.connect(partial(self.initialise_cellpose, mode="all"))
         self.gui.cellpose_load_model.clicked.connect(self.load_cellpose_model)
-        self.gui.dilate_segmentations.clicked.connect(
-            self.dilate_segmentations
-        )
-
-        self.gui.smlm_detect_mode.currentIndexChanged.connect(
-            self.update_detect_options
-        )
-
-        self.gui.picasso_detect.clicked.connect(
-            partial(self.init_picasso, detect=True, fit=False)
-        )
-        self.gui.picasso_fit.clicked.connect(
-            partial(self.init_picasso, detect=False, fit=True)
-        )
-        self.gui.picasso_detectfit.clicked.connect(
-            partial(self.init_picasso, detect=True, fit=True)
-        )
-
-        self.gui.picasso_filter_dataset.currentIndexChanged.connect(
-            self.update_filter_criterion
-        )
-        self.gui.filter_criterion.currentIndexChanged.connect(
-            self.update_criterion_ranges
-        )
-        self.gui.filter_localisations.clicked.connect(
-            self.pixseq_filter_localisations
-        )
-        self.gui.picasso_filter_type.currentIndexChanged.connect(
-            self.update_filter_dataset
-        )
-
-        self.gui.picasso_vis_mode.currentIndexChanged.connect(
-            partial(self.draw_localisations, update_vis=True)
-        )
-        self.gui.picasso_vis_size.currentIndexChanged.connect(
-            partial(self.draw_localisations, update_vis=True)
-        )
-        self.gui.picasso_vis_opacity.currentIndexChanged.connect(
-            partial(self.draw_localisations, update_vis=True)
-        )
-        self.gui.picasso_vis_edge_width.currentIndexChanged.connect(
-            partial(self.draw_localisations, update_vis=True)
-        )
+        self.gui.dilate_segmentations.clicked.connect(self.dilate_segmentations)
+
+        self.gui.smlm_detect_mode.currentIndexChanged.connect(self.update_detect_options)
+
+        self.gui.picasso_detect.clicked.connect(partial(self.init_picasso, detect=True, fit=False))
+        self.gui.picasso_fit.clicked.connect(partial(self.init_picasso, detect=False, fit=True))
+        self.gui.picasso_detectfit.clicked.connect(partial(self.init_picasso, detect=True, fit=True))
+
+        self.gui.picasso_filter_dataset.currentIndexChanged.connect(self.update_filter_criterion)
+        self.gui.filter_criterion.currentIndexChanged.connect(self.update_criterion_ranges)
+        self.gui.filter_localisations.clicked.connect(self.pixseq_filter_localisations)
+        self.gui.picasso_filter_type.currentIndexChanged.connect(self.update_filter_dataset)
+
+        self.gui.picasso_vis_mode.currentIndexChanged.connect(partial(self.draw_localisations, update_vis=True))
+        self.gui.picasso_vis_size.currentIndexChanged.connect(partial(self.draw_localisations, update_vis=True))
+        self.gui.picasso_vis_opacity.currentIndexChanged.connect(partial(self.draw_localisations, update_vis=True))
+        self.gui.picasso_vis_edge_width.currentIndexChanged.connect(partial(self.draw_localisations, update_vis=True))
 
         self.gui.picasso_render.clicked.connect(self.initialise_picasso_render)
 
         self.gui.link_localisations.clicked.connect(self.initialise_tracking)
 
-        self.gui.export_localisations.clicked.connect(
-            self.initialise_export_locs
-        )
+        self.gui.export_localisations.clicked.connect(self.initialise_export_locs)
 
         self.viewer.dims.events.current_step.connect(self.slider_event)
 
     def initialise_keybindings(self):
-
         self.viewer.bind_key("d", self.devfunc)
 
-        self.viewer.bind_key(
-            key="Control-Right",
-            func=lambda event: self.moltract_translation(direction="right"),
-            overwrite=True,
-        )
-        self.viewer.bind_key(
-            key="Control-Left",
-            func=lambda event: self.moltract_translation(direction="left"),
-            overwrite=True,
-        )
-        self.viewer.bind_key(
-            key="Control-Up",
-            func=lambda event: self.moltract_translation(direction="up"),
-            overwrite=True,
-        )
-        self.viewer.bind_key(
-            key="Control-Down",
-            func=lambda event: self.moltract_translation(direction="down"),
-            overwrite=True,
-        )
+        self.viewer.bind_key(key="Control-Right", func=lambda event: self.moltract_translation(direction="right"), overwrite=True, )
+        self.viewer.bind_key(key="Control-Left", func=lambda event: self.moltract_translation(direction="left"), overwrite=True, )
+        self.viewer.bind_key(key="Control-Up", func=lambda event: self.moltract_translation(direction="up"), overwrite=True, )
+        self.viewer.bind_key(key="Control-Down", func=lambda event: self.moltract_translation(direction="down"), overwrite=True, )
 
         self.register_segmentation_keybinds(self.viewer)
 
     def devfunc(self, viewer=None):
-
         self.update_ui()
 
     def check_gpufit_availibility(self):
-
         self.gpufit_available = False
 
         try:
             from pygpufit import gpufit as gf
 
             package_installed = True
         except:
             package_installed = False
 
         if package_installed:
-
             if not gf.cuda_available():
                 print("Pygpufit not available due to missing CUDA")
             else:
                 runtime_version, driver_version = gf.get_cuda_version()
 
-                runtime_version = ".".join(
-                    [str(v) for v in list(runtime_version)]
-                )
-                driver_version = ".".join(
-                    [str(v) for v in list(driver_version)]
-                )
+                runtime_version = ".".join([str(v) for v in list(runtime_version)])
+                driver_version = ".".join([str(v) for v in list(driver_version)])
 
                 if runtime_version != driver_version:
-                    print(
-                        f"Pygpufit not available due to CUDA version mismatch. "
-                        f"Runtime: {runtime_version}, Driver: {driver_version}"
-                    )
+                    print(f"Pygpufit not available due to CUDA version mismatch. "
+                          f"Runtime: {runtime_version}, Driver: {driver_version}")
 
                 else:
                     self.gpufit_available = True
 
         else:
             print("Pygpufit not available due to missing package")
-            print("Install pygpufit package into napari-PixSeq root directory")
+
+            import moltrack
+            src_dir = moltrack.__file__.replace("\moltrack\__init__.py", "")
+            print(f"Add pygpufit package to moltrack src directory [{src_dir}] to enable GPUFit.")
 
         if self.gpufit_available:
             print("GPUFit available")
             self.gui.smlm_fit_mode.addItem("GPUFit")
             self.gui.smlm_fit_mode.setCurrentIndex(1)
```

### Comparing `napari_moltrack-0.0.7/src/moltrack/funcs/compute_utils.py` & `napari_moltrack-0.0.8/src/moltrack/funcs/compute_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/src/moltrack/funcs/events_utils.py` & `napari_moltrack-0.0.8/src/moltrack/funcs/events_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/src/moltrack/funcs/export_utils.py` & `napari_moltrack-0.0.8/src/moltrack/funcs/export_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/src/moltrack/funcs/import_utils.py` & `napari_moltrack-0.0.8/src/moltrack/funcs/import_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/src/moltrack/funcs/loc_filter_utils.py` & `napari_moltrack-0.0.8/src/moltrack/funcs/loc_filter_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/src/moltrack/funcs/picasso_detect_utils.py` & `napari_moltrack-0.0.8/src/moltrack/funcs/picasso_detect_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/src/moltrack/funcs/picasso_render_utils.py` & `napari_moltrack-0.0.8/src/moltrack/funcs/picasso_render_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/src/moltrack/funcs/segmentation_events.py` & `napari_moltrack-0.0.8/src/moltrack/funcs/segmentation_events.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/src/moltrack/funcs/segmentation_utils.py` & `napari_moltrack-0.0.8/src/moltrack/funcs/segmentation_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/src/moltrack/funcs/tracking_utils.py` & `napari_moltrack-0.0.8/src/moltrack/funcs/tracking_utils.py`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/src/napari_moltrack.egg-info/PKG-INFO` & `napari_moltrack-0.0.8/src/napari_moltrack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-moltrack
-Version: 0.0.7
+Version: 0.0.8
 Summary: Single molecule tracking package for Napari
 Author: Piers Turner
 Author-email: piers.turner@physics.ox.ac.uk
 License: 
         Copyright (c) 2024, Piers Turner
         All rights reserved.
```

### Comparing `napari_moltrack-0.0.7/src/napari_moltrack.egg-info/SOURCES.txt` & `napari_moltrack-0.0.8/src/napari_moltrack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/src/pygpufit/Gpufit.dll` & `napari_moltrack-0.0.8/src/pygpufit/Gpufit.dll`

 * *Files identical despite different names*

### Comparing `napari_moltrack-0.0.7/src/pygpufit/gpufit.py` & `napari_moltrack-0.0.8/src/pygpufit/gpufit.py`

 * *Files identical despite different names*

