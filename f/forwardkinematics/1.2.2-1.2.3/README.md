# Comparing `tmp/forwardkinematics-1.2.2.tar.gz` & `tmp/forwardkinematics-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forwardkinematics-1.2.2.tar", max compression
+gzip compressed data, was "forwardkinematics-1.2.3.tar", max compression
```

## Comparing `forwardkinematics-1.2.2.tar` & `forwardkinematics-1.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      582 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/README.md
--rw-r--r--   0        0        0      205 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/forwardkinematics/__init__.py
--rw-r--r--   0        0        0      940 2024-05-01 00:36:05.380183 forwardkinematics-1.2.2/forwardkinematics/fksCommon/fk.py
--rw-r--r--   0        0        0     2565 2024-05-01 00:36:05.380183 forwardkinematics-1.2.2/forwardkinematics/planarFks/planarArmFk.py
--rw-r--r--   0        0        0     1269 2024-05-01 00:36:05.380183 forwardkinematics-1.2.2/forwardkinematics/planarFks/planar_fk.py
--rw-r--r--   0        0        0     1617 2024-05-01 00:36:05.380183 forwardkinematics-1.2.2/forwardkinematics/planarFks/point_fk.py
--rw-r--r--   0        0        0        0 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/forwardkinematics/urdfFks/casadiConversion/__init__.py
--rw-r--r--   0        0        0        0 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/forwardkinematics/urdfFks/casadiConversion/geometry/__init__.py
--rw-r--r--   0        0        0     3442 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py
--rw-r--r--   0        0        0     6240 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/forwardkinematics/urdfFks/casadiConversion/urdfparser.py
--rw-r--r--   0        0        0      122 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/forwardkinematics/urdfFks/generic_urdf_fk.py
--rw-r--r--   0        0        0     4151 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/forwardkinematics/urdfFks/urdfFk.py
--rw-r--r--   0        0        0     7616 2024-05-01 00:35:45.524049 forwardkinematics-1.2.2/forwardkinematics/xmlFks/generic_xml_fk.py
--rw-r--r--   0        0        0      762 2024-05-01 00:36:05.380183 forwardkinematics-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 forwardkinematics-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      582 2024-06-01 00:37:22.628749 forwardkinematics-1.2.3/README.md
+-rw-r--r--   0        0        0      205 2024-06-01 00:37:22.628749 forwardkinematics-1.2.3/forwardkinematics/__init__.py
+-rw-r--r--   0        0        0      940 2024-06-01 00:37:22.628749 forwardkinematics-1.2.3/forwardkinematics/fksCommon/fk.py
+-rw-r--r--   0        0        0     2565 2024-06-01 00:37:22.628749 forwardkinematics-1.2.3/forwardkinematics/planarFks/planarArmFk.py
+-rw-r--r--   0        0        0     1269 2024-06-01 00:37:22.628749 forwardkinematics-1.2.3/forwardkinematics/planarFks/planar_fk.py
+-rw-r--r--   0        0        0     1617 2024-06-01 00:37:22.628749 forwardkinematics-1.2.3/forwardkinematics/planarFks/point_fk.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:37:22.628749 forwardkinematics-1.2.3/forwardkinematics/urdfFks/casadiConversion/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 00:37:22.628749 forwardkinematics-1.2.3/forwardkinematics/urdfFks/casadiConversion/geometry/__init__.py
+-rw-r--r--   0        0        0     3442 2024-06-01 00:37:22.628749 forwardkinematics-1.2.3/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py
+-rw-r--r--   0        0        0     6240 2024-06-01 00:37:22.628749 forwardkinematics-1.2.3/forwardkinematics/urdfFks/casadiConversion/urdfparser.py
+-rw-r--r--   0        0        0      122 2024-06-01 00:37:22.628749 forwardkinematics-1.2.3/forwardkinematics/urdfFks/generic_urdf_fk.py
+-rw-r--r--   0        0        0     4151 2024-06-01 00:37:22.628749 forwardkinematics-1.2.3/forwardkinematics/urdfFks/urdfFk.py
+-rw-r--r--   0        0        0     7888 2024-06-01 00:37:54.472550 forwardkinematics-1.2.3/forwardkinematics/xmlFks/generic_xml_fk.py
+-rw-r--r--   0        0        0      762 2024-06-01 00:37:54.476549 forwardkinematics-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1486 1970-01-01 00:00:00.000000 forwardkinematics-1.2.3/PKG-INFO
```

### Comparing `forwardkinematics-1.2.2/README.md` & `forwardkinematics-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.2/forwardkinematics/fksCommon/fk.py` & `forwardkinematics-1.2.3/forwardkinematics/fksCommon/fk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.2/forwardkinematics/planarFks/planarArmFk.py` & `forwardkinematics-1.2.3/forwardkinematics/planarFks/planarArmFk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.2/forwardkinematics/planarFks/planar_fk.py` & `forwardkinematics-1.2.3/forwardkinematics/planarFks/planar_fk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.2/forwardkinematics/planarFks/point_fk.py` & `forwardkinematics-1.2.3/forwardkinematics/planarFks/point_fk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.2/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py` & `forwardkinematics-1.2.3/forwardkinematics/urdfFks/casadiConversion/geometry/transformation_matrix.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.2/forwardkinematics/urdfFks/casadiConversion/urdfparser.py` & `forwardkinematics-1.2.3/forwardkinematics/urdfFks/casadiConversion/urdfparser.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.2/forwardkinematics/urdfFks/urdfFk.py` & `forwardkinematics-1.2.3/forwardkinematics/urdfFks/urdfFk.py`

 * *Files identical despite different names*

### Comparing `forwardkinematics-1.2.2/forwardkinematics/xmlFks/generic_xml_fk.py` & `forwardkinematics-1.2.3/forwardkinematics/xmlFks/generic_xml_fk.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from typing import Union, List, Optional
+import logging
 import xml.etree.ElementTree as ET
 import numpy as np
 import casadi as ca
 
 from forwardkinematics.fksCommon.fk import ForwardKinematics
 
 casadiOrNumpy = Union[ca.SX, np.ndarray]
@@ -161,23 +162,27 @@
         """
         root = self.root.find('.//worldbody')
         T = homogeneous_transformation()
         joint_counter = 0
         child_link_found = False
         for element in root.iter():
             if child_link_found:
-                return T
+                break
             T_element = np.eye(4)
             if element.tag == 'body':
                 T_element = get_T_element(element)
                 if element.get('name') == child_link:
                     child_link_found = True
             if element.tag == 'joint':
                 joint_type = 'hinge' if 'type' not in element.attrib else element.attrib['type']
-                joint_axis = [0, 0, 1] if 'axis' not in element.attrib else [int(x) for x in element.attrib['axis'].split()]
+                if 'axis' not in element.attrib:
+                    joint_axis = [0, 0, 1]
+                    logging.warning(f"Joint axis not found in XML. Assuming default axis {joint_axis}.")
+                else:
+                    joint_axis = [int(x) for x in element.attrib['axis'].split()]
                 if joint_type == 'hinge':
                     T_element = homogeneous_transformation(
                         rotation=axis2rotMat(
                             joint_axis,
                             q[joint_counter],
                         )
                     )
@@ -193,11 +198,14 @@
                 if element.get('mesh') == child_link:
                     T_element = get_T_element(element)
                     child_link_found = True
             T = matrix_multiply(T, T_element)
         if not child_link_found:
             raise ValueError(f"Child link {child_link} not found in XML.")
         else:
-            return T
+            if position_only:
+                return T[0:3,3]
+            else:
+                return T
```

### Comparing `forwardkinematics-1.2.2/pyproject.toml` & `forwardkinematics-1.2.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forwardkinematics"
-version = "1.2.2"
+version = "1.2.3"
 description = "\"Light-weight implementation of forward kinematics using casadi.\""
 authors = ["Max Spahn <m.spahn@tudelft.nl>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/maxspahn/forwardKinematics.git"
 repository = "https://github.com/maxspahn/forwardKinematics.git"
```

### Comparing `forwardkinematics-1.2.2/PKG-INFO` & `forwardkinematics-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forwardkinematics
-Version: 1.2.2
+Version: 1.2.3
 Summary: "Light-weight implementation of forward kinematics using casadi."
 Home-page: https://github.com/maxspahn/forwardKinematics.git
 License: MIT
 Author: Max Spahn
 Author-email: m.spahn@tudelft.nl
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

