# Comparing `tmp/fabrics-0.9.4.tar.gz` & `tmp/fabrics-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabrics-0.9.4.tar", max compression
+gzip compressed data, was "fabrics-0.9.5.tar", max compression
```

## Comparing `fabrics-0.9.4.tar` & `fabrics-0.9.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0    35306 2024-05-07 15:03:43.357805 fabrics-0.9.4/LICENSE
--rw-r--r--   0        0        0     4831 2024-05-07 15:03:43.357805 fabrics-0.9.4/README.md
--rw-r--r--   0        0        0       40 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/.gitignore
--rw-r--r--   0        0        0       71 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/__init__.py
--rw-r--r--   0        0        0      249 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/energies/execution_energies.py
--rw-r--r--   0        0        0     2720 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/environment/__init__.py
--rw-r--r--   0        0        0     3048 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/leaves/attractor.py
--rw-r--r--   0        0        0     2453 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/leaves/dynamic_attractor.py
--rw-r--r--   0        0        0     4354 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/leaves/dynamic_geometry.py
--rw-r--r--   0        0        0     2915 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/leaves/dynamic_leaf.py
--rw-r--r--   0        0        0    16601 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/leaves/geometry.py
--rw-r--r--   0        0        0     2733 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/leaves/leaf.py
--rw-r--r--   0        0        0     2807 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/maps/parameterized_maps.py
--rw-r--r--   0        0        0     2372 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/components/robot_representation/__init__.py
--rw-r--r--   0        0        0     1319 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/defaults/default_energies.py
--rw-r--r--   0        0        0     1609 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/defaults/default_geometries.py
--rw-r--r--   0        0        0      918 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/defaults/default_leaves.py
--rw-r--r--   0        0        0     1852 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/defaults/default_maps.py
--rw-r--r--   0        0        0      260 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/diffGeometry/casadi_helpers.py
--rw-r--r--   0        0        0     3587 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/diffGeometry/diffMap.py
--rw-r--r--   0        0        0     4007 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/diffGeometry/energized_geometry.py
--rw-r--r--   0        0        0     7171 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/diffGeometry/energy.py
--rw-r--r--   0        0        0     3355 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/diffGeometry/geometry.py
--rw-r--r--   0        0        0     6925 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/diffGeometry/spec.py
--rw-r--r--   0        0        0     2818 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/diffGeometry/speedControl.py
--rw-r--r--   0        0        0     7267 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/helpers/casadiFunctionWrapper.py
--rw-r--r--   0        0        0       75 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/helpers/constants.py
--rw-r--r--   0        0        0     9331 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/helpers/distances.py
--rw-r--r--   0        0        0      273 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/helpers/exceptions.py
--rw-r--r--   0        0        0     2688 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/helpers/functions.py
--rw-r--r--   0        0        0     7697 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/helpers/geometric_primitives.py
--rw-r--r--   0        0        0     4857 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/helpers/variables.py
--rw-r--r--   0        0        0     4099 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/planner/configuration_classes.py
--rw-r--r--   0        0        0     6225 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/planner/non_holonomic_parameterized_planner.py
--rw-r--r--   0        0        0    34405 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/planner/parameterized_planner.py
--rw-r--r--   0        0        0     1548 2024-05-07 15:03:43.505804 fabrics-0.9.4/fabrics/planner/serialized_planner.py
--rw-r--r--   0        0        0     1183 2024-05-07 15:03:43.505804 fabrics-0.9.4/pyproject.toml
--rw-r--r--   0        0        0     5921 1970-01-01 00:00:00.000000 fabrics-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0    35306 2024-06-01 00:44:48.222245 fabrics-0.9.5/LICENSE
+-rw-r--r--   0        0        0     4831 2024-06-01 00:44:48.222245 fabrics-0.9.5/README.md
+-rw-r--r--   0        0        0       40 2024-06-01 00:44:48.370244 fabrics-0.9.5/fabrics/.gitignore
+-rw-r--r--   0        0        0       71 2024-06-01 00:44:48.370244 fabrics-0.9.5/fabrics/__init__.py
+-rw-r--r--   0        0        0      249 2024-06-01 00:44:48.370244 fabrics-0.9.5/fabrics/components/energies/execution_energies.py
+-rw-r--r--   0        0        0     2720 2024-06-01 00:44:48.370244 fabrics-0.9.5/fabrics/components/environment/__init__.py
+-rw-r--r--   0        0        0     3048 2024-06-01 00:44:48.370244 fabrics-0.9.5/fabrics/components/leaves/attractor.py
+-rw-r--r--   0        0        0     2453 2024-06-01 00:44:48.370244 fabrics-0.9.5/fabrics/components/leaves/dynamic_attractor.py
+-rw-r--r--   0        0        0     4354 2024-06-01 00:44:48.370244 fabrics-0.9.5/fabrics/components/leaves/dynamic_geometry.py
+-rw-r--r--   0        0        0     2915 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/components/leaves/dynamic_leaf.py
+-rw-r--r--   0        0        0    16601 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/components/leaves/geometry.py
+-rw-r--r--   0        0        0     2733 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/components/leaves/leaf.py
+-rw-r--r--   0        0        0     2807 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/components/maps/parameterized_maps.py
+-rw-r--r--   0        0        0     2372 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/components/robot_representation/__init__.py
+-rw-r--r--   0        0        0     1319 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/defaults/default_energies.py
+-rw-r--r--   0        0        0     1609 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/defaults/default_geometries.py
+-rw-r--r--   0        0        0      918 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/defaults/default_leaves.py
+-rw-r--r--   0        0        0     1852 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/defaults/default_maps.py
+-rw-r--r--   0        0        0      260 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/diffGeometry/casadi_helpers.py
+-rw-r--r--   0        0        0     3587 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/diffGeometry/diffMap.py
+-rw-r--r--   0        0        0     4007 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/diffGeometry/energized_geometry.py
+-rw-r--r--   0        0        0     7171 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/diffGeometry/energy.py
+-rw-r--r--   0        0        0     3355 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/diffGeometry/geometry.py
+-rw-r--r--   0        0        0     6921 2024-06-01 00:45:10.650123 fabrics-0.9.5/fabrics/diffGeometry/spec.py
+-rw-r--r--   0        0        0     2818 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/diffGeometry/speedControl.py
+-rw-r--r--   0        0        0     7267 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/helpers/casadiFunctionWrapper.py
+-rw-r--r--   0        0        0       75 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/helpers/constants.py
+-rw-r--r--   0        0        0     9331 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/helpers/distances.py
+-rw-r--r--   0        0        0      273 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/helpers/exceptions.py
+-rw-r--r--   0        0        0     2688 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/helpers/functions.py
+-rw-r--r--   0        0        0     7697 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/helpers/geometric_primitives.py
+-rw-r--r--   0        0        0     4857 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/helpers/variables.py
+-rw-r--r--   0        0        0     4099 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/planner/configuration_classes.py
+-rw-r--r--   0        0        0     6225 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/planner/non_holonomic_parameterized_planner.py
+-rw-r--r--   0        0        0    34405 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/planner/parameterized_planner.py
+-rw-r--r--   0        0        0     1548 2024-06-01 00:44:48.374244 fabrics-0.9.5/fabrics/planner/serialized_planner.py
+-rw-r--r--   0        0        0     1183 2024-06-01 00:45:10.650123 fabrics-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0     5921 1970-01-01 00:00:00.000000 fabrics-0.9.5/PKG-INFO
```

### Comparing `fabrics-0.9.4/LICENSE` & `fabrics-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/README.md` & `fabrics-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/components/environment/__init__.py` & `fabrics-0.9.5/fabrics/components/environment/__init__.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/components/leaves/attractor.py` & `fabrics-0.9.5/fabrics/components/leaves/attractor.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/components/leaves/dynamic_attractor.py` & `fabrics-0.9.5/fabrics/components/leaves/dynamic_attractor.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/components/leaves/dynamic_geometry.py` & `fabrics-0.9.5/fabrics/components/leaves/dynamic_geometry.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/components/leaves/dynamic_leaf.py` & `fabrics-0.9.5/fabrics/components/leaves/dynamic_leaf.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/components/leaves/geometry.py` & `fabrics-0.9.5/fabrics/components/leaves/geometry.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/components/leaves/leaf.py` & `fabrics-0.9.5/fabrics/components/leaves/leaf.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/components/maps/parameterized_maps.py` & `fabrics-0.9.5/fabrics/components/maps/parameterized_maps.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/components/robot_representation/__init__.py` & `fabrics-0.9.5/fabrics/components/robot_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/defaults/default_energies.py` & `fabrics-0.9.5/fabrics/defaults/default_energies.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/defaults/default_geometries.py` & `fabrics-0.9.5/fabrics/defaults/default_geometries.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/defaults/default_leaves.py` & `fabrics-0.9.5/fabrics/defaults/default_leaves.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/defaults/default_maps.py` & `fabrics-0.9.5/fabrics/defaults/default_maps.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/diffGeometry/diffMap.py` & `fabrics-0.9.5/fabrics/diffGeometry/diffMap.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/diffGeometry/energized_geometry.py` & `fabrics-0.9.5/fabrics/diffGeometry/energized_geometry.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/diffGeometry/energy.py` & `fabrics-0.9.5/fabrics/diffGeometry/energy.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/diffGeometry/geometry.py` & `fabrics-0.9.5/fabrics/diffGeometry/geometry.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/diffGeometry/spec.py` & `fabrics-0.9.5/fabrics/diffGeometry/spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         if 'refTrajs' in kwargs:
             self._refTrajs = kwargs.get('refTrajs')
         if self.is_dynamic():
             self._J_ref = np.identity(self.x_ref().size()[0])
             self._J_ref_inv = np.identity(self.x_ref().size()[0])
         if "J_ref" in kwargs:
             self._J_ref = kwargs.get("J_ref")
-            logging.warning("Casadi pseudo inverse is used in Lagrangian")
+            logging.debug("Casadi pseudo inverse is used in Lagrangian")
             self._J_ref_inv = ca.mtimes(ca.transpose(self._J_ref), ca.inv(ca.mtimes(self._J_ref, ca.transpose(self._J_ref)) + np.identity(self.x_ref().size()[0]) * eps))
         self._xdot_d = np.zeros(self.x().size()[0])
         self._vars.verify()
         assert isinstance(M, ca.SX)
         self._M = M
 
     def x_ref(self):
@@ -69,15 +69,15 @@
         else:
             return ca.mtimes(self.M(), self._h)
 
     def M(self):
         return self._M
 
     def Minv(self):
-        logging.warning("Casadi pseudo inverse is used in spec")
+        logging.debug("Casadi pseudo inverse is used in spec")
         return ca.pinv(self._M + np.identity(self.x().size()[0]) * eps)
 
     def x(self):
         return self._vars.position_variable()
 
     def xdot(self):
         return self._vars.velocity_variable()
```

### Comparing `fabrics-0.9.4/fabrics/diffGeometry/speedControl.py` & `fabrics-0.9.5/fabrics/diffGeometry/speedControl.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/helpers/casadiFunctionWrapper.py` & `fabrics-0.9.5/fabrics/helpers/casadiFunctionWrapper.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/helpers/distances.py` & `fabrics-0.9.5/fabrics/helpers/distances.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/helpers/functions.py` & `fabrics-0.9.5/fabrics/helpers/functions.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/helpers/geometric_primitives.py` & `fabrics-0.9.5/fabrics/helpers/geometric_primitives.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/helpers/variables.py` & `fabrics-0.9.5/fabrics/helpers/variables.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/planner/configuration_classes.py` & `fabrics-0.9.5/fabrics/planner/configuration_classes.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/planner/non_holonomic_parameterized_planner.py` & `fabrics-0.9.5/fabrics/planner/non_holonomic_parameterized_planner.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/planner/parameterized_planner.py` & `fabrics-0.9.5/fabrics/planner/parameterized_planner.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/fabrics/planner/serialized_planner.py` & `fabrics-0.9.5/fabrics/planner/serialized_planner.py`

 * *Files identical despite different names*

### Comparing `fabrics-0.9.4/pyproject.toml` & `fabrics-0.9.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fabrics"
-version = "0.9.4"
+version = "0.9.5"
 description = "Optimization fabrics in python."
 authors = ["Max Spahn <m.spahn@tudelft.nl>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://tud-amr/fabrics"
 keywords = ["robotics", "motion-planning", "geometry"]
```

### Comparing `fabrics-0.9.4/PKG-INFO` & `fabrics-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fabrics
-Version: 0.9.4
+Version: 0.9.5
 Summary: Optimization fabrics in python.
 Home-page: https://tud-amr/fabrics
 License: GPL-3.0-or-later
 Keywords: robotics,motion-planning,geometry
 Author: Max Spahn
 Author-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fabrics Version: 0.9.4 Summary: Optimization
+Metadata-Version: 2.1 Name: fabrics Version: 0.9.5 Summary: Optimization
 fabrics in python. Home-page: https://tud-amr/fabrics License: GPL-3.0-or-later
 Keywords: robotics,motion-planning,geometry Author: Max Spahn Author-email:
 m.spahn@tudelft.nl Requires-Python: >=3.8,<3.10 Classifier: License :: OSI
 Approved :: GNU General Public License v3 or later (GPLv3+) Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Requires-Dist: casadi
 (>=3.5.5) Requires-Dist: deprecation (>=2.1.0,<3.0.0) Requires-Dist:
```

