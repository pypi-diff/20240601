# Comparing `tmp/bpy_helper-0.0.0.tar.gz` & `tmp/bpy_helper-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bpy_helper-0.0.0.tar", last modified: Thu Mar 21 21:42:16 2024, max compression
+gzip compressed data, was "bpy_helper-0.0.1.tar", last modified: Sat Jun  1 06:54:23 2024, max compression
```

## Comparing `bpy_helper-0.0.0.tar` & `bpy_helper-0.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:42:16.477840 bpy_helper-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-03-21 21:42:11.000000 bpy_helper-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-21 21:42:16.473840 bpy_helper-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-03-21 21:42:11.000000 bpy_helper-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:42:16.473840 bpy_helper-0.0.0/bpy_helper/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-21 21:42:11.000000 bpy_helper-0.0.0/bpy_helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-03-21 21:42:11.000000 bpy_helper-0.0.0/bpy_helper/camera.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-21 21:42:11.000000 bpy_helper-0.0.0/bpy_helper/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-03-21 21:42:11.000000 bpy_helper-0.0.0/bpy_helper/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-03-21 21:42:11.000000 bpy_helper-0.0.0/bpy_helper/light.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-03-21 21:42:11.000000 bpy_helper-0.0.0/bpy_helper/material.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-03-21 21:42:11.000000 bpy_helper-0.0.0/bpy_helper/random.py
--rw-r--r--   0 runner    (1001) docker     (127)     5764 2024-03-21 21:42:11.000000 bpy_helper-0.0.0/bpy_helper/scene.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-03-21 21:42:11.000000 bpy_helper-0.0.0/bpy_helper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-21 21:42:16.473840 bpy_helper-0.0.0/bpy_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2454 2024-03-21 21:42:16.000000 bpy_helper-0.0.0/bpy_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-21 21:42:16.000000 bpy_helper-0.0.0/bpy_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-21 21:42:16.000000 bpy_helper-0.0.0/bpy_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-21 21:42:16.000000 bpy_helper-0.0.0/bpy_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-03-21 21:42:16.000000 bpy_helper-0.0.0/bpy_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-03-21 21:42:11.000000 bpy_helper-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-21 21:42:16.477840 bpy_helper-0.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:23.726412 bpy_helper-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-06-01 06:54:19.000000 bpy_helper-0.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-06-01 06:54:23.726412 bpy_helper-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-06-01 06:54:19.000000 bpy_helper-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:23.726412 bpy_helper-0.0.1/bpy_helper/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:19.000000 bpy_helper-0.0.1/bpy_helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2024-06-01 06:54:19.000000 bpy_helper-0.0.1/bpy_helper/camera.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-06-01 06:54:19.000000 bpy_helper-0.0.1/bpy_helper/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5994 2024-06-01 06:54:19.000000 bpy_helper-0.0.1/bpy_helper/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5977 2024-06-01 06:54:19.000000 bpy_helper-0.0.1/bpy_helper/light.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-06-01 06:54:19.000000 bpy_helper-0.0.1/bpy_helper/material.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-06-01 06:54:19.000000 bpy_helper-0.0.1/bpy_helper/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5939 2024-06-01 06:54:19.000000 bpy_helper-0.0.1/bpy_helper/scene.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-06-01 06:54:19.000000 bpy_helper-0.0.1/bpy_helper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 06:54:23.726412 bpy_helper-0.0.1/bpy_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-06-01 06:54:23.000000 bpy_helper-0.0.1/bpy_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-06-01 06:54:23.000000 bpy_helper-0.0.1/bpy_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 06:54:23.000000 bpy_helper-0.0.1/bpy_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-06-01 06:54:23.000000 bpy_helper-0.0.1/bpy_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-06-01 06:54:23.000000 bpy_helper-0.0.1/bpy_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-06-01 06:54:19.000000 bpy_helper-0.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 06:54:23.726412 bpy_helper-0.0.1/setup.cfg
```

### Comparing `bpy_helper-0.0.0/LICENSE` & `bpy_helper-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bpy_helper-0.0.0/PKG-INFO` & `bpy_helper-0.0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpy_helper
-Version: 0.0.0
+Version: 0.0.1
 Summary: A lightweight alternative to BlenderProc
 Author-email: NCJ <me@ncj.wiki>
 License: MIT License
         
         Copyright (c) 2024 NCJ
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,20 +36,23 @@
 Requires-Dist: bpy>=3.4.0
 Requires-Dist: numpy
 
 # bpy-helper
 
 A lightweight alternative to BlenderProc
 
+[![Upload Python Package](https://github.com/iamNCJ/bpy-helper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/iamNCJ/bpy-helper/actions/workflows/python-publish.yml)
+
 ## Why bpy-helper instead of BlenderProc?
 
 BlenderProc needs a separate blender installation, and a lot of restrictions when using with other pypi packages. Debugging a BlenderProc script is also painful especially when you are using a headless environment. Hence I decide to build my own blender wrapper using `bpy`.
 
 ## Installation
 
 ```bash
-pip install git+https://github.com/iamNCJ/bpy-helper.git
+pip install bpy-helper
 ```
 
 ## Projects using bpy-helper
 
 - [NRHints: Relighting Neural Radiance Fields with Shadow and Highlight Hints](https://nrhints.github.io/): bpy-helper is derived from the data rendering scripts of NRHints.
+- [DiLightNet: Fine-grained Lighting Control for Diffusion-based Image Generation](https://dilightnet.github.io/): bpy-helper is used to render the training data and radiance hints for DiLightNet.
```

### Comparing `bpy_helper-0.0.0/bpy_helper/camera.py` & `bpy_helper-0.0.1/bpy_helper/camera.py`

 * *Files identical despite different names*

### Comparing `bpy_helper-0.0.0/bpy_helper/io.py` & `bpy_helper-0.0.1/bpy_helper/io.py`

 * *Files identical despite different names*

### Comparing `bpy_helper-0.0.0/bpy_helper/light.py` & `bpy_helper-0.0.1/bpy_helper/light.py`

 * *Files identical despite different names*

### Comparing `bpy_helper-0.0.0/bpy_helper/material.py` & `bpy_helper-0.0.1/bpy_helper/material.py`

 * *Files identical despite different names*

### Comparing `bpy_helper-0.0.0/bpy_helper/random.py` & `bpy_helper-0.0.1/bpy_helper/random.py`

 * *Files identical despite different names*

### Comparing `bpy_helper-0.0.0/bpy_helper/scene.py` & `bpy_helper-0.0.1/bpy_helper/scene.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,19 +34,21 @@
     """
     Loads a 3d model into the scene.
     """
 
     if object_path.endswith(".glb"):
         bpy.ops.import_scene.gltf(filepath=object_path, merge_vertices=True)
     elif object_path.endswith(".obj"):
-        bpy.ops.import_scene.obj(filepath=object_path)
+        bpy.ops.wm.obj_import(filepath=object_path)
     elif object_path.endswith(".fbx"):
         bpy.ops.import_scene.fbx(filepath=object_path)
     elif object_path.endswith(".blend"):
         bpy.ops.wm.open_mainfile(filepath=object_path)
+    elif object_path.endswith(".ply"):
+        bpy.ops.import_mesh.ply(filepath=object_path)
     else:
         raise ValueError(f"Unsupported file type: {object_path}")
 
 
 def scene_root_objects():
     """
     Yields all root objects in the scene.
@@ -123,31 +125,32 @@
         raise RuntimeError("no objects in scene to compute bounding sphere for")
     x, y, z = [[point_co[i] for point_co in points_co_global] for i in range(3)]
     b_sphere_center = mathutils.Vector([get_center(axis) for axis in [x, y, z]]) if (x and y and z) else None
     b_sphere_radius = max(((point - b_sphere_center) for point in points_co_global)) if b_sphere_center else None
     return b_sphere_center, b_sphere_radius.length
 
 
-def normalize_scene(scale=None, offset=None, use_bounding_sphere=False) -> tuple[float, mathutils.Vector]:
+def normalize_scene(scale=None, offset=None, use_bounding_sphere=False, target_scale=0.5) -> tuple[float, mathutils.Vector]:
     """
     Normalize the scene by scaling and translating all objects.
 
     :param scale: scale factor
     :param offset: translation offset
     :param use_bounding_sphere: if True, use the bounding sphere to compute the scale factor
+    :param target_scale: the target scale factor
     :return: scale factor and translation offset
     """
 
     if scale is None:
         if not use_bounding_sphere:
             bbox_min, bbox_max = scene_bbox()
-            scale = 0.5 / max(bbox_max - bbox_min)
+            scale = target_scale / max(bbox_max - bbox_min)
         else:
             center, radius = scene_sphere()
-            scale = 0.5 / radius
+            scale = target_scale / radius
     for obj in scene_root_objects():
         obj.scale = obj.scale * scale
 
     # Apply scale to matrix_world.
     bpy.context.view_layer.update()
     if offset is None:
         bbox_min, bbox_max = scene_bbox()
```

### Comparing `bpy_helper-0.0.0/bpy_helper/utils.py` & `bpy_helper-0.0.1/bpy_helper/utils.py`

 * *Files identical despite different names*

### Comparing `bpy_helper-0.0.0/bpy_helper.egg-info/PKG-INFO` & `bpy_helper-0.0.1/bpy_helper.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bpy_helper
-Version: 0.0.0
+Version: 0.0.1
 Summary: A lightweight alternative to BlenderProc
 Author-email: NCJ <me@ncj.wiki>
 License: MIT License
         
         Copyright (c) 2024 NCJ
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -36,20 +36,23 @@
 Requires-Dist: bpy>=3.4.0
 Requires-Dist: numpy
 
 # bpy-helper
 
 A lightweight alternative to BlenderProc
 
+[![Upload Python Package](https://github.com/iamNCJ/bpy-helper/actions/workflows/python-publish.yml/badge.svg)](https://github.com/iamNCJ/bpy-helper/actions/workflows/python-publish.yml)
+
 ## Why bpy-helper instead of BlenderProc?
 
 BlenderProc needs a separate blender installation, and a lot of restrictions when using with other pypi packages. Debugging a BlenderProc script is also painful especially when you are using a headless environment. Hence I decide to build my own blender wrapper using `bpy`.
 
 ## Installation
 
 ```bash
-pip install git+https://github.com/iamNCJ/bpy-helper.git
+pip install bpy-helper
 ```
 
 ## Projects using bpy-helper
 
 - [NRHints: Relighting Neural Radiance Fields with Shadow and Highlight Hints](https://nrhints.github.io/): bpy-helper is derived from the data rendering scripts of NRHints.
+- [DiLightNet: Fine-grained Lighting Control for Diffusion-based Image Generation](https://dilightnet.github.io/): bpy-helper is used to render the training data and radiance hints for DiLightNet.
```

### Comparing `bpy_helper-0.0.0/pyproject.toml` & `bpy_helper-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "bpy_helper"
-version = "0.0.0"
+version = "0.0.1"
 description = "A lightweight alternative to BlenderProc"
 readme = "README.md"
 authors = [
     { name = "NCJ", email = "me@ncj.wiki" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
```

