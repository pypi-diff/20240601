# Comparing `tmp/trame-3.6.1.tar.gz` & `tmp/trame-3.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trame-3.6.1.tar", last modified: Mon May 27 22:50:21 2024, max compression
+gzip compressed data, was "trame-3.6.2.tar", last modified: Sat Jun  1 00:19:59 2024, max compression
```

## Comparing `trame-3.6.1.tar` & `trame-3.6.2.tar`

### file list

```diff
@@ -1,56 +1,57 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.933843 trame-3.6.1/
--rw-r--r--   0 root         (0) root         (0)      552 2024-05-27 22:50:18.000000 trame-3.6.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-27 22:50:18.000000 trame-3.6.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     7169 2024-05-27 22:50:21.933843 trame-3.6.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6431 2024-05-27 22:50:18.000000 trame-3.6.1/README.rst
--rw-r--r--   0 root         (0) root         (0)      918 2024-05-27 22:50:21.933843 trame-3.6.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 22:50:19.000000 trame-3.6.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.925844 trame-3.6.1/trame/
--rw-r--r--   0 root         (0) root         (0)      552 2024-05-27 22:50:18.000000 trame-3.6.1/trame/LICENSE
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-27 22:50:19.000000 trame-3.6.1/trame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.929844 trame-3.6.1/trame/app/
--rw-r--r--   0 root         (0) root         (0)     3132 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/__init__.py
--rw-r--r--   0 root         (0) root         (0)      271 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/asynchronous.py
--rw-r--r--   0 root         (0) root         (0)     2089 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/demo.py
--rw-r--r--   0 root         (0) root         (0)     1490 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/dev.py
--rw-r--r--   0 root         (0) root         (0)     1731 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/file_upload.py
--rw-r--r--   0 root         (0) root         (0)     2320 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/jupyter.py
--rw-r--r--   0 root         (0) root         (0)     1309 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/mimetypes.py
--rw-r--r--   0 root         (0) root         (0)      577 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/singleton.py
--rw-r--r--   0 root         (0) root         (0)     1677 2024-05-27 22:50:19.000000 trame-3.6.1/trame/app/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.929844 trame-3.6.1/trame/assets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-27 22:50:19.000000 trame-3.6.1/trame/assets/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4337 2024-05-27 22:50:19.000000 trame-3.6.1/trame/assets/local.py
--rw-r--r--   0 root         (0) root         (0)     4362 2024-05-27 22:50:19.000000 trame-3.6.1/trame/assets/remote.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.929844 trame-3.6.1/trame/decorators/
--rw-r--r--   0 root         (0) root         (0)      184 2024-05-27 22:50:19.000000 trame-3.6.1/trame/decorators/__init__.py
--rw-r--r--   0 root         (0) root         (0)       86 2024-05-27 22:50:19.000000 trame-3.6.1/trame/decorators/dev.py
--rw-r--r--   0 root         (0) root         (0)     5665 2024-05-27 22:50:19.000000 trame-3.6.1/trame/decorators/klass.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.929844 trame-3.6.1/trame/env/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 22:50:19.000000 trame-3.6.1/trame/env/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1863 2024-05-27 22:50:19.000000 trame-3.6.1/trame/env/paraview.py
--rw-r--r--   0 root         (0) root         (0)     3930 2024-05-27 22:50:19.000000 trame-3.6.1/trame/env/utils.py
--rw-r--r--   0 root         (0) root         (0)     1311 2024-05-27 22:50:19.000000 trame-3.6.1/trame/env/venv.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.929844 trame-3.6.1/trame/modules/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-27 22:50:19.000000 trame-3.6.1/trame/modules/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.929844 trame-3.6.1/trame/tools/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-27 22:50:19.000000 trame-3.6.1/trame/tools/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1418 2024-05-27 22:50:19.000000 trame-3.6.1/trame/tools/app.py
--rw-r--r--   0 root         (0) root         (0)     4461 2024-05-27 22:50:19.000000 trame-3.6.1/trame/tools/serve.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.933843 trame-3.6.1/trame/tools/widgets/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-27 22:50:19.000000 trame-3.6.1/trame/tools/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      597 2024-05-27 22:50:19.000000 trame-3.6.1/trame/tools/widgets/__main__.py
--rw-r--r--   0 root         (0) root         (0)    13964 2024-05-27 22:50:19.000000 trame-3.6.1/trame/tools/widgets/generator.py
--rw-r--r--   0 root         (0) root         (0)      603 2024-05-27 22:50:19.000000 trame-3.6.1/trame/tools/widgets/utils.py
--rw-r--r--   0 root         (0) root         (0)     3142 2024-05-27 22:50:19.000000 trame-3.6.1/trame/tools/www.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.933843 trame-3.6.1/trame/ui/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-27 22:50:19.000000 trame-3.6.1/trame/ui/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.933843 trame-3.6.1/trame/widgets/
--rw-r--r--   0 root         (0) root         (0)       65 2024-05-27 22:50:19.000000 trame-3.6.1/trame/widgets/__init__.py
--rw-r--r--   0 root         (0) root         (0)      934 2024-05-27 22:50:19.000000 trame-3.6.1/trame/widgets/helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-27 22:50:21.925844 trame-3.6.1/trame.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7169 2024-05-27 22:50:21.000000 trame-3.6.1/trame.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      957 2024-05-27 22:50:21.000000 trame-3.6.1/trame.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-27 22:50:21.000000 trame-3.6.1/trame.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-27 22:50:21.000000 trame-3.6.1/trame.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2024-05-27 22:50:21.000000 trame-3.6.1/trame.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 00:19:59.786940 trame-3.6.2/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-06-01 00:19:55.000000 trame-3.6.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       22 2024-06-01 00:19:55.000000 trame-3.6.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     7169 2024-06-01 00:19:59.786940 trame-3.6.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6431 2024-06-01 00:19:55.000000 trame-3.6.2/README.rst
+-rw-r--r--   0 root         (0) root         (0)      918 2024-06-01 00:19:59.786940 trame-3.6.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 00:19:56.000000 trame-3.6.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 00:19:59.782940 trame-3.6.2/trame/
+-rw-r--r--   0 root         (0) root         (0)      552 2024-06-01 00:19:55.000000 trame-3.6.2/trame/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       65 2024-06-01 00:19:56.000000 trame-3.6.2/trame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 00:19:59.782940 trame-3.6.2/trame/app/
+-rw-r--r--   0 root         (0) root         (0)     3132 2024-06-01 00:19:56.000000 trame-3.6.2/trame/app/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      271 2024-06-01 00:19:56.000000 trame-3.6.2/trame/app/asynchronous.py
+-rw-r--r--   0 root         (0) root         (0)     2042 2024-06-01 00:19:56.000000 trame-3.6.2/trame/app/demo.py
+-rw-r--r--   0 root         (0) root         (0)     1490 2024-06-01 00:19:56.000000 trame-3.6.2/trame/app/dev.py
+-rw-r--r--   0 root         (0) root         (0)     1731 2024-06-01 00:19:56.000000 trame-3.6.2/trame/app/file_upload.py
+-rw-r--r--   0 root         (0) root         (0)     2320 2024-06-01 00:19:56.000000 trame-3.6.2/trame/app/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)     1309 2024-06-01 00:19:56.000000 trame-3.6.2/trame/app/mimetypes.py
+-rw-r--r--   0 root         (0) root         (0)     2507 2024-06-01 00:19:56.000000 trame-3.6.2/trame/app/pv_demo.py
+-rw-r--r--   0 root         (0) root         (0)      577 2024-06-01 00:19:56.000000 trame-3.6.2/trame/app/singleton.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2024-06-01 00:19:56.000000 trame-3.6.2/trame/app/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 00:19:59.782940 trame-3.6.2/trame/assets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-06-01 00:19:56.000000 trame-3.6.2/trame/assets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4337 2024-06-01 00:19:56.000000 trame-3.6.2/trame/assets/local.py
+-rw-r--r--   0 root         (0) root         (0)     4362 2024-06-01 00:19:56.000000 trame-3.6.2/trame/assets/remote.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 00:19:59.786940 trame-3.6.2/trame/decorators/
+-rw-r--r--   0 root         (0) root         (0)      184 2024-06-01 00:19:56.000000 trame-3.6.2/trame/decorators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       86 2024-06-01 00:19:56.000000 trame-3.6.2/trame/decorators/dev.py
+-rw-r--r--   0 root         (0) root         (0)     5665 2024-06-01 00:19:56.000000 trame-3.6.2/trame/decorators/klass.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 00:19:59.786940 trame-3.6.2/trame/env/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-01 00:19:56.000000 trame-3.6.2/trame/env/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1863 2024-06-01 00:19:56.000000 trame-3.6.2/trame/env/paraview.py
+-rw-r--r--   0 root         (0) root         (0)     3930 2024-06-01 00:19:56.000000 trame-3.6.2/trame/env/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1311 2024-06-01 00:19:56.000000 trame-3.6.2/trame/env/venv.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 00:19:59.786940 trame-3.6.2/trame/modules/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-06-01 00:19:56.000000 trame-3.6.2/trame/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 00:19:59.786940 trame-3.6.2/trame/tools/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-06-01 00:19:56.000000 trame-3.6.2/trame/tools/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1418 2024-06-01 00:19:56.000000 trame-3.6.2/trame/tools/app.py
+-rw-r--r--   0 root         (0) root         (0)     4461 2024-06-01 00:19:56.000000 trame-3.6.2/trame/tools/serve.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 00:19:59.786940 trame-3.6.2/trame/tools/widgets/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-06-01 00:19:56.000000 trame-3.6.2/trame/tools/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      597 2024-06-01 00:19:56.000000 trame-3.6.2/trame/tools/widgets/__main__.py
+-rw-r--r--   0 root         (0) root         (0)    13964 2024-06-01 00:19:56.000000 trame-3.6.2/trame/tools/widgets/generator.py
+-rw-r--r--   0 root         (0) root         (0)      603 2024-06-01 00:19:56.000000 trame-3.6.2/trame/tools/widgets/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3142 2024-06-01 00:19:56.000000 trame-3.6.2/trame/tools/www.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 00:19:59.786940 trame-3.6.2/trame/ui/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-06-01 00:19:56.000000 trame-3.6.2/trame/ui/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 00:19:59.786940 trame-3.6.2/trame/widgets/
+-rw-r--r--   0 root         (0) root         (0)       65 2024-06-01 00:19:56.000000 trame-3.6.2/trame/widgets/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      934 2024-06-01 00:19:56.000000 trame-3.6.2/trame/widgets/helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 00:19:59.782940 trame-3.6.2/trame.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     7169 2024-06-01 00:19:59.000000 trame-3.6.2/trame.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      978 2024-06-01 00:19:59.000000 trame-3.6.2/trame.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 00:19:59.000000 trame-3.6.2/trame.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 00:19:59.000000 trame-3.6.2/trame.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2024-06-01 00:19:59.000000 trame-3.6.2/trame.egg-info/top_level.txt
```

### Comparing `trame-3.6.1/LICENSE` & `trame-3.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/PKG-INFO` & `trame-3.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame
-Version: 3.6.1
+Version: 3.6.2
 Summary: Trame, a framework to build applications in plain Python
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-3.6.1/README.rst` & `trame-3.6.2/README.rst`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/setup.cfg` & `trame-3.6.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = trame
-version = 3.6.1
+version = 3.6.2
 description = Trame, a framework to build applications in plain Python
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Kitware Inc.
 license = Apache License 2.0
 classifiers = 
 	Development Status :: 5 - Production/Stable
```

### Comparing `trame-3.6.1/trame/LICENSE` & `trame-3.6.2/trame/LICENSE`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/app/__init__.py` & `trame-3.6.2/trame/app/__init__.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/app/demo.py` & `trame-3.6.2/trame/app/demo.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from trame.app import get_server
-from trame.ui.vuetify import SinglePageLayout
-from trame.widgets import vuetify, vtk as vtk_widgets
+from trame.ui.vuetify3 import SinglePageLayout
+from trame.widgets import vuetify3 as v3, vtk as vtk_widgets
 
 
 class Cone:
     def __init__(self, server_or_name=None):
-        self.server = get_server(server_or_name, client_type="vue2")
+        self.server = get_server(server_or_name)
         self.ui = self._generate_ui()
 
     @property
     def ctrl(self):
         return self.server.controller
 
     @property
@@ -29,30 +29,30 @@
         self.resolution = 6
 
     def _generate_ui(self):
         with SinglePageLayout(self.server) as layout:
             layout.title.set_text("Trame demo")
             with layout.toolbar as toolbar:
                 toolbar.dense = True
-                vuetify.VSpacer()
-                vuetify.VSlider(
+                v3.VSpacer()
+                v3.VSlider(
                     v_model=("resolution", 6),
                     min=3,
                     max=60,
                     step=1,
                     hide_details=True,
                     style="max-width: 300px;",
                 )
-                with vuetify.VBtn(icon=True, click=self.reset_resolution):
-                    vuetify.VIcon("mdi-lock-reset")
-                with vuetify.VBtn(icon=True, click=self.ctrl.view_reset_camera):
-                    vuetify.VIcon("mdi-crop-free")
+                with v3.VBtn(icon=True, click=self.reset_resolution):
+                    v3.VIcon("mdi-lock-reset")
+                with v3.VBtn(icon=True, click=self.ctrl.view_reset_camera):
+                    v3.VIcon("mdi-crop-free")
 
             with layout.content:
-                with vuetify.VContainer(fluid=True, classes="pa-0 fill-height"):
+                with v3.VContainer(fluid=True, classes="pa-0 fill-height"):
                     with vtk_widgets.VtkView() as view:
                         self.ctrl.view_reset_camera = view.reset_camera
                         with vtk_widgets.VtkGeometryRepresentation():
                             vtk_widgets.VtkAlgorithm(
                                 vtk_class="vtkConeSource", state=("{ resolution }",)
                             )
```

### Comparing `trame-3.6.1/trame/app/dev.py` & `trame-3.6.2/trame/app/dev.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/app/file_upload.py` & `trame-3.6.2/trame/app/file_upload.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/app/jupyter.py` & `trame-3.6.2/trame/app/jupyter.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/app/mimetypes.py` & `trame-3.6.2/trame/app/mimetypes.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/app/singleton.py` & `trame-3.6.2/trame/app/singleton.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/app/testing.py` & `trame-3.6.2/trame/app/testing.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/assets/local.py` & `trame-3.6.2/trame/assets/local.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/assets/remote.py` & `trame-3.6.2/trame/assets/remote.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/decorators/klass.py` & `trame-3.6.2/trame/decorators/klass.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/env/paraview.py` & `trame-3.6.2/trame/env/paraview.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/env/utils.py` & `trame-3.6.2/trame/env/utils.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/env/venv.py` & `trame-3.6.2/trame/env/venv.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/tools/app.py` & `trame-3.6.2/trame/tools/app.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/tools/serve.py` & `trame-3.6.2/trame/tools/serve.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/tools/widgets/__main__.py` & `trame-3.6.2/trame/tools/widgets/__main__.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/tools/widgets/generator.py` & `trame-3.6.2/trame/tools/widgets/generator.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/tools/widgets/utils.py` & `trame-3.6.2/trame/tools/widgets/utils.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/tools/www.py` & `trame-3.6.2/trame/tools/www.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame/widgets/helper.py` & `trame-3.6.2/trame/widgets/helper.py`

 * *Files identical despite different names*

### Comparing `trame-3.6.1/trame.egg-info/PKG-INFO` & `trame-3.6.2/trame.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trame
-Version: 3.6.1
+Version: 3.6.2
 Summary: Trame, a framework to build applications in plain Python
 Author: Kitware Inc.
 License: Apache License 2.0
 Keywords: Python,Interactive,Web,Application,Framework
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `trame-3.6.1/trame.egg-info/SOURCES.txt` & `trame-3.6.2/trame.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 trame/app/__init__.py
 trame/app/asynchronous.py
 trame/app/demo.py
 trame/app/dev.py
 trame/app/file_upload.py
 trame/app/jupyter.py
 trame/app/mimetypes.py
+trame/app/pv_demo.py
 trame/app/singleton.py
 trame/app/testing.py
 trame/assets/__init__.py
 trame/assets/local.py
 trame/assets/remote.py
 trame/decorators/__init__.py
 trame/decorators/dev.py
```

