# Comparing `tmp/urdfenvs-0.9.8.tar.gz` & `tmp/urdfenvs-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "urdfenvs-0.9.8.tar", max compression
+gzip compressed data, was "urdfenvs-0.9.9.tar", max compression
```

## Comparing `urdfenvs-0.9.8.tar` & `urdfenvs-0.9.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0    35147 2024-03-01 01:03:30.442794 urdfenvs-0.9.8/LICENSE
--rw-r--r--   0        0        0     3651 2024-03-01 01:03:49.259107 urdfenvs-0.9.8/README.md
--rw-r--r--   0        0        0     1409 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/pyproject.toml
--rw-r--r--   0        0        0       71 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/__init__.py
--rw-r--r--   0        0        0     1536 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/assets/panda/panda_scene_temp.xml
--rw-r--r--   0        0        0      203 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/generic_mujoco/__init__.py
--rw-r--r--   0        0        0    13236 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/generic_mujoco/generic_mujoco_env.py
--rw-r--r--   0        0        0      683 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/generic_mujoco/generic_mujoco_robot.py
--rw-r--r--   0        0        0       30 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/keyboard_input/.gitignore
--rw-r--r--   0        0        0     6404 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/keyboard_input/keyboard_input_responder.py
--rw-r--r--   0        0        0      169 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/robots/generic_urdf/__init__.py
--rw-r--r--   0        0        0     2243 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/robots/generic_urdf/generic_diff_drive_robot.py
--rw-r--r--   0        0        0     1025 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/robots/generic_urdf/generic_urdf_reacher.py
--rw-r--r--   0        0        0       48 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/robots/iris/__init__.py
--rw-r--r--   0        0        0     1325 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/robots/iris/iris.py
--rw-r--r--   0        0        0     1649 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/scene_examples/goal.py
--rw-r--r--   0        0        0   233442 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/scene_examples/obstacle_data/duck.obj
--rw-r--r--   0        0        0      675 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/scene_examples/obstacle_data/duck.urdf
--rw-r--r--   0        0        0    11622 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/scene_examples/obstacle_data/duck_vhacd.obj
--rw-r--r--   0        0        0      546 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/scene_examples/obstacle_data/sphere_goal.urdf
--rw-r--r--   0        0        0   111602 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/scene_examples/obstacle_data/sphere_smooth.obj
--rw-r--r--   0        0        0     4955 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/scene_examples/obstacles.py
--rw-r--r--   0        0        0       12 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/sensors/.gitignore
--rw-r--r--   0        0        0        0 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/sensors/__init__.py
--rw-r--r--   0        0        0     2113 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/sensors/free_space_decomposition.py
--rw-r--r--   0        0        0     1897 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/sensors/free_space_occupancy.py
--rw-r--r--   0        0        0     3870 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/sensors/fsd.py
--rw-r--r--   0        0        0     4206 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/sensors/fsd_sensor.py
--rw-r--r--   0        0        0     7059 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/sensors/full_sensor.py
--rw-r--r--   0        0        0     3008 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/sensors/grid_sensor.py
--rw-r--r--   0        0        0     6254 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/sensors/lidar.py
--rw-r--r--   0        0        0     6360 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/sensors/lidar_3d.py
--rw-r--r--   0        0        0     3980 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/sensors/obstacle_sensor.py
--rw-r--r--   0        0        0     4092 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/sensors/occupancy_sensor.py
--rw-r--r--   0        0        0     4655 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/sensors/physics_engine_interface.py
--rw-r--r--   0        0        0     1782 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/sensors/sdf_sensor.py
--rw-r--r--   0        0        0     1431 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/sensors/sensor.py
--rw-r--r--   0        0        0       13 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/urdf_common/.gitignore
--rw-r--r--   0        0        0      162 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/urdf_common/__init__.py
--rw-r--r--   0        0        0    11660 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/urdf_common/bicycle_model.py
--rw-r--r--   0        0        0    15227 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/urdf_common/differential_drive_robot.py
--rw-r--r--   0        0        0     9586 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/urdf_common/generic_robot.py
--rw-r--r--   0        0        0     7990 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/urdf_common/helpers.py
--rw-r--r--   0        0        0     4887 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/urdf_common/holonomic_robot.py
--rw-r--r--   0        0        0     6379 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/urdf_common/meshes/checker_blue.png
--rw-r--r--   0        0        0      255 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/urdf_common/meshes/plane.mtl
--rw-r--r--   0        0        0      349 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/urdf_common/meshes/plane.obj
--rw-r--r--   0        0        0      170 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/urdf_common/plane.py
--rw-r--r--   0        0        0      690 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/urdf_common/plane.urdf
--rw-r--r--   0        0        0    10344 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/urdf_common/quadrotor.py
--rw-r--r--   0        0        0      135 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/urdf_common/reward.py
--rw-r--r--   0        0        0    21509 2024-03-01 01:03:49.279107 urdfenvs-0.9.8/urdfenvs/urdf_common/urdf_env.py
--rw-r--r--   0        0        0      880 2024-03-01 01:03:30.506795 urdfenvs-0.9.8/urdfenvs/wrappers/sb3_float32_action_wrapper.py
--rw-r--r--   0        0        0     5036 1970-01-01 00:00:00.000000 urdfenvs-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-03-01 22:59:01.220282 urdfenvs-0.9.9/LICENSE
+-rw-r--r--   0        0        0     3651 2024-03-01 22:59:01.220282 urdfenvs-0.9.9/README.md
+-rw-r--r--   0        0        0     1427 2024-03-01 22:59:21.540244 urdfenvs-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0       71 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/__init__.py
+-rw-r--r--   0        0        0     1536 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/assets/panda/panda_scene_temp.xml
+-rw-r--r--   0        0        0      225 2024-03-01 22:59:21.540244 urdfenvs-0.9.9/urdfenvs/generic_mujoco/__init__.py
+-rw-r--r--   0        0        0    13236 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/generic_mujoco/generic_mujoco_env.py
+-rw-r--r--   0        0        0      683 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/generic_mujoco/generic_mujoco_robot.py
+-rw-r--r--   0        0        0       30 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/keyboard_input/.gitignore
+-rw-r--r--   0        0        0     6404 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/keyboard_input/keyboard_input_responder.py
+-rw-r--r--   0        0        0      169 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/robots/generic_urdf/__init__.py
+-rw-r--r--   0        0        0     2243 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/robots/generic_urdf/generic_diff_drive_robot.py
+-rw-r--r--   0        0        0     1025 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/robots/generic_urdf/generic_urdf_reacher.py
+-rw-r--r--   0        0        0       48 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/robots/iris/__init__.py
+-rw-r--r--   0        0        0     1325 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/robots/iris/iris.py
+-rw-r--r--   0        0        0     1649 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/scene_examples/goal.py
+-rw-r--r--   0        0        0   233442 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/scene_examples/obstacle_data/duck.obj
+-rw-r--r--   0        0        0      675 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/scene_examples/obstacle_data/duck.urdf
+-rw-r--r--   0        0        0    11622 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/scene_examples/obstacle_data/duck_vhacd.obj
+-rw-r--r--   0        0        0      546 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/scene_examples/obstacle_data/sphere_goal.urdf
+-rw-r--r--   0        0        0   111602 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/scene_examples/obstacle_data/sphere_smooth.obj
+-rw-r--r--   0        0        0     4955 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/scene_examples/obstacles.py
+-rw-r--r--   0        0        0       12 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/sensors/.gitignore
+-rw-r--r--   0        0        0        0 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/sensors/__init__.py
+-rw-r--r--   0        0        0     2113 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/sensors/free_space_decomposition.py
+-rw-r--r--   0        0        0     1897 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/sensors/free_space_occupancy.py
+-rw-r--r--   0        0        0     3870 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/sensors/fsd.py
+-rw-r--r--   0        0        0     4206 2024-03-01 22:59:01.280281 urdfenvs-0.9.9/urdfenvs/sensors/fsd_sensor.py
+-rw-r--r--   0        0        0     7051 2024-03-01 22:59:21.540244 urdfenvs-0.9.9/urdfenvs/sensors/full_sensor.py
+-rw-r--r--   0        0        0     3008 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/sensors/grid_sensor.py
+-rw-r--r--   0        0        0     6254 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/sensors/lidar.py
+-rw-r--r--   0        0        0     6360 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/sensors/lidar_3d.py
+-rw-r--r--   0        0        0     3980 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/sensors/obstacle_sensor.py
+-rw-r--r--   0        0        0     4092 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/sensors/occupancy_sensor.py
+-rw-r--r--   0        0        0     5593 2024-03-01 22:59:21.540244 urdfenvs-0.9.9/urdfenvs/sensors/physics_engine_interface.py
+-rw-r--r--   0        0        0     1782 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/sensors/sdf_sensor.py
+-rw-r--r--   0        0        0     1431 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/sensors/sensor.py
+-rw-r--r--   0        0        0       13 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/urdf_common/.gitignore
+-rw-r--r--   0        0        0      162 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/urdf_common/__init__.py
+-rw-r--r--   0        0        0    11660 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/urdf_common/bicycle_model.py
+-rw-r--r--   0        0        0    15227 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/urdf_common/differential_drive_robot.py
+-rw-r--r--   0        0        0     9586 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/urdf_common/generic_robot.py
+-rw-r--r--   0        0        0     7990 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/urdf_common/helpers.py
+-rw-r--r--   0        0        0     4887 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/urdf_common/holonomic_robot.py
+-rw-r--r--   0        0        0     6379 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/urdf_common/meshes/checker_blue.png
+-rw-r--r--   0        0        0      255 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/urdf_common/meshes/plane.mtl
+-rw-r--r--   0        0        0      349 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/urdf_common/meshes/plane.obj
+-rw-r--r--   0        0        0      170 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/urdf_common/plane.py
+-rw-r--r--   0        0        0      690 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/urdf_common/plane.urdf
+-rw-r--r--   0        0        0    10344 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/urdf_common/quadrotor.py
+-rw-r--r--   0        0        0      135 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/urdf_common/reward.py
+-rw-r--r--   0        0        0    21509 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/urdf_common/urdf_env.py
+-rw-r--r--   0        0        0      880 2024-03-01 22:59:01.284282 urdfenvs-0.9.9/urdfenvs/wrappers/sb3_float32_action_wrapper.py
+-rw-r--r--   0        0        0     5036 1970-01-01 00:00:00.000000 urdfenvs-0.9.9/PKG-INFO
```

### Comparing `urdfenvs-0.9.8/LICENSE` & `urdfenvs-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/README.md` & `urdfenvs-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/pyproject.toml` & `urdfenvs-0.9.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "urdfenvs"
-version = "0.9.8"
+version = "0.9.9"
 description = "Simple simulation environment for robots, based on the urdf files."
 authors = ["Max Spahn <m.spahn@tudelft.nl>"]
 maintainers = [
   "Max Spahn <m.spahn@tudelft.nl>",
   "Chadi Salmi <c.salmi@tudelft.nl"
 ]
 license = "GPL-3.0-or-later"
@@ -36,14 +36,15 @@
 [tool.poetry.group.dev.dependencies]
 pylint = "^3.0"
 autopep8 = "^1.6.0"
 pytest = "^6.2.5"
 Sphinx = "4.2.0"
 sphinx-rtd-theme = "1.0.0"
 sphinxcontrib-napoleon = "0.7"
+black = "^24.2.0"
 
 [tool.poetry.group.keyboard]
 optional = true
 
 [tool.poetry.group.mujoco]
 optional = true
```

### Comparing `urdfenvs-0.9.8/urdfenvs/assets/panda/panda_scene_temp.xml` & `urdfenvs-0.9.9/urdfenvs/assets/panda/panda_scene_temp.xml`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/generic_mujoco/generic_mujoco_env.py` & `urdfenvs-0.9.9/urdfenvs/generic_mujoco/generic_mujoco_env.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/generic_mujoco/generic_mujoco_robot.py` & `urdfenvs-0.9.9/urdfenvs/generic_mujoco/generic_mujoco_robot.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/keyboard_input/keyboard_input_responder.py` & `urdfenvs-0.9.9/urdfenvs/keyboard_input/keyboard_input_responder.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/robots/generic_urdf/generic_diff_drive_robot.py` & `urdfenvs-0.9.9/urdfenvs/robots/generic_urdf/generic_diff_drive_robot.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/robots/generic_urdf/generic_urdf_reacher.py` & `urdfenvs-0.9.9/urdfenvs/robots/generic_urdf/generic_urdf_reacher.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/robots/iris/iris.py` & `urdfenvs-0.9.9/urdfenvs/robots/iris/iris.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/scene_examples/goal.py` & `urdfenvs-0.9.9/urdfenvs/scene_examples/goal.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/scene_examples/obstacle_data/duck.obj` & `urdfenvs-0.9.9/urdfenvs/scene_examples/obstacle_data/duck.obj`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/scene_examples/obstacle_data/duck.urdf` & `urdfenvs-0.9.9/urdfenvs/scene_examples/obstacle_data/duck.urdf`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/scene_examples/obstacle_data/duck_vhacd.obj` & `urdfenvs-0.9.9/urdfenvs/scene_examples/obstacle_data/duck_vhacd.obj`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/scene_examples/obstacle_data/sphere_goal.urdf` & `urdfenvs-0.9.9/urdfenvs/scene_examples/obstacle_data/sphere_goal.urdf`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/scene_examples/obstacle_data/sphere_smooth.obj` & `urdfenvs-0.9.9/urdfenvs/scene_examples/obstacle_data/sphere_smooth.obj`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/scene_examples/obstacles.py` & `urdfenvs-0.9.9/urdfenvs/scene_examples/obstacles.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/sensors/free_space_decomposition.py` & `urdfenvs-0.9.9/urdfenvs/sensors/free_space_decomposition.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/sensors/free_space_occupancy.py` & `urdfenvs-0.9.9/urdfenvs/sensors/free_space_occupancy.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/sensors/fsd.py` & `urdfenvs-0.9.9/urdfenvs/sensors/fsd.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/sensors/fsd_sensor.py` & `urdfenvs-0.9.9/urdfenvs/sensors/fsd_sensor.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/sensors/full_sensor.py` & `urdfenvs-0.9.9/urdfenvs/sensors/full_sensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -148,18 +148,18 @@
             sensor_observation["obstacles"] = observations
 
         observations = {}
         for goal_id, goal in goals.items():
             observation = {}
             for mask_item in self._goal_mask:
                 if mask_item == "position":
-                    value, _ = self._physics_engine.get_obstacle_pose(goal_id)
+                    value, _ = self._physics_engine.get_goal_pose(goal_id)
 
                 elif mask_item == "velocity":
-                    value, _ = self._physics_engine.get_obstacle_velocity(goal_id)
+                    value, _ = self._physics_engine.get_goal_velocity(goal_id)
                 else:
                     try:
                         value = getattr(goal, mask_item)(t=t)
                     except TypeError:
                         value = getattr(goal, mask_item)()
                 if isinstance(value, float):
                     value = [value]
```

### Comparing `urdfenvs-0.9.8/urdfenvs/sensors/grid_sensor.py` & `urdfenvs-0.9.9/urdfenvs/sensors/grid_sensor.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/sensors/lidar.py` & `urdfenvs-0.9.9/urdfenvs/sensors/lidar.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/sensors/lidar_3d.py` & `urdfenvs-0.9.9/urdfenvs/sensors/lidar_3d.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/sensors/obstacle_sensor.py` & `urdfenvs-0.9.9/urdfenvs/sensors/obstacle_sensor.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/sensors/occupancy_sensor.py` & `urdfenvs-0.9.9/urdfenvs/sensors/occupancy_sensor.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/sensors/physics_engine_interface.py` & `urdfenvs-0.9.9/urdfenvs/sensors/physics_engine_interface.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,22 @@
         pass
 
     @abstractmethod
     def get_obstacle_velocity(self, *args) -> Tuple[List[float], List[float]]:
         pass
 
     @abstractmethod
+    def get_goal_pose(self, goal_id: int) -> Tuple[List[float]]:
+        pass
+
+    @abstractmethod
+    def get_goal_velocity(self, goal_id: int) -> Tuple[List[float]]:
+        pass
+
+    @abstractmethod
     def get_link_position(self, *args) -> np.ndarray:
         pass
 
     @abstractmethod
     def get_link_orientation(self, *args) -> np.ndarray:
         pass
 
@@ -79,14 +87,22 @@
         position, orientation = pybullet.getBasePositionAndOrientation(obst_id)
         return position, orientation
 
     def get_obstacle_velocity(self, obst_id: int) -> Tuple[List[float], List[float]]:
         linear, angular = pybullet.getBaseVelocity(obst_id)
         return linear, angular
 
+    def get_goal_pose(self, goal_id: int) -> Tuple[List[float]]:
+        position, orientation = pybullet.getBasePositionAndOrientation(goal_id)
+        return position, orientation
+
+    def get_goal_velocity(self, goal_id: int) -> Tuple[List[float]]:
+        linear, angular = pybullet.getBaseVelocity(goal_id)
+        return linear, angular
+
     def get_link_position(self, robot, link_id) -> np.ndarray:
         link_position = np.array(pybullet.getLinkState(robot, link_id)[0])
         return link_position
 
     def get_link_orientation(self, robot, link_id) -> np.ndarray:
         link_orientation = np.array(pybullet.getLinkState(robot, link_id)[1])
         return link_orientation
@@ -129,14 +145,23 @@
         return Rotation.from_matrix(link_orientation_matrix).as_quat()
 
     def get_obstacle_pose(self, obst_id: int) -> Tuple[List[float], List[float]]:
         pos = self._data.mocap_pos[obst_id]
         ori = self._data.mocap_quat[obst_id]
         return pos.tolist(), ori.tolist()
 
+    def get_goal_pose(self, goal_id: int) -> Tuple[List[float]]:
+        pos = self._data.site(goal_id).xpos
+        goal_rotation = np.reshape(self._data.site(goal_id).xmat, (3, 3))
+        ori = Rotation.from_matrix(goal_rotation).as_quat()
+        return pos.tolist(), ori.tolist()
+
+    def get_goal_velocity(self, goal_id: int) -> Tuple[List[float]]:
+        return [0, 0, 0], [0, 0, 0]
+
     def ray_cast(
         self,
         ray_start: np.ndarray,
         ray_end: np.ndarray,
         ray_index: int,
         ray_length: float
     ) -> np.ndarray:
```

### Comparing `urdfenvs-0.9.8/urdfenvs/sensors/sdf_sensor.py` & `urdfenvs-0.9.9/urdfenvs/sensors/sdf_sensor.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/sensors/sensor.py` & `urdfenvs-0.9.9/urdfenvs/sensors/sensor.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/urdf_common/bicycle_model.py` & `urdfenvs-0.9.9/urdfenvs/urdf_common/bicycle_model.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/urdf_common/differential_drive_robot.py` & `urdfenvs-0.9.9/urdfenvs/urdf_common/differential_drive_robot.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/urdf_common/generic_robot.py` & `urdfenvs-0.9.9/urdfenvs/urdf_common/generic_robot.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/urdf_common/helpers.py` & `urdfenvs-0.9.9/urdfenvs/urdf_common/helpers.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/urdf_common/holonomic_robot.py` & `urdfenvs-0.9.9/urdfenvs/urdf_common/holonomic_robot.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/urdf_common/meshes/checker_blue.png` & `urdfenvs-0.9.9/urdfenvs/urdf_common/meshes/checker_blue.png`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/urdf_common/plane.urdf` & `urdfenvs-0.9.9/urdfenvs/urdf_common/plane.urdf`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/urdf_common/quadrotor.py` & `urdfenvs-0.9.9/urdfenvs/urdf_common/quadrotor.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/urdf_common/urdf_env.py` & `urdfenvs-0.9.9/urdfenvs/urdf_common/urdf_env.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/urdfenvs/wrappers/sb3_float32_action_wrapper.py` & `urdfenvs-0.9.9/urdfenvs/wrappers/sb3_float32_action_wrapper.py`

 * *Files identical despite different names*

### Comparing `urdfenvs-0.9.8/PKG-INFO` & `urdfenvs-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: urdfenvs
-Version: 0.9.8
+Version: 0.9.9
 Summary: Simple simulation environment for robots, based on the urdf files.
 Home-page: https://maxspahn.github.io/gym_envs_urdf/
 License: GPL-3.0-or-later
 Keywords: robotics,motion-planning,simulation
 Author: Max Spahn
 Author-email: m.spahn@tudelft.nl
 Maintainer: Max Spahn
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: urdfenvs Version: 0.9.8 Summary: Simple simulation
+Metadata-Version: 2.1 Name: urdfenvs Version: 0.9.9 Summary: Simple simulation
 environment for robots, based on the urdf files. Home-page: https://
 maxspahn.github.io/gym_envs_urdf/ License: GPL-3.0-or-later Keywords:
 robotics,motion-planning,simulation Author: Max Spahn Author-email:
 m.spahn@tudelft.nl Maintainer: Max Spahn Maintainer-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: GNU General
 Public License v3 or later (GPLv3+) Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

