# Comparing `tmp/vectorvision-0.1.0.tar.gz` & `tmp/vectorvision-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectorvision-0.1.0.tar", max compression
+gzip compressed data, was "vectorvision-0.1.1.tar", max compression
```

## Comparing `vectorvision-0.1.0.tar` & `vectorvision-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1073 2024-04-08 07:51:44.418437 vectorvision-0.1.0/LICENSE
--rw-r--r--   0        0        0     2275 2024-04-12 15:07:49.652892 vectorvision-0.1.0/README.md
--rw-r--r--   0        0        0     1092 2024-05-31 08:13:48.211975 vectorvision-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3707 2024-05-31 08:39:39.360039 vectorvision-0.1.0/vectorvision/Converter.py
--rw-r--r--   0        0        0        0 2024-04-12 15:07:49.652892 vectorvision-0.1.0/vectorvision/__init__.py
--rw-r--r--   0        0        0     7938 2024-05-30 18:59:15.404879 vectorvision-0.1.0/vectorvision/path_decomposition.py
--rw-r--r--   0        0        0    11004 2024-05-15 15:53:33.323607 vectorvision-0.1.0/vectorvision/polygons.py
--rw-r--r--   0        0        0     1952 2024-05-31 08:39:39.388039 vectorvision-0.1.0/vectorvision/smoothing.py
--rw-r--r--   0        0        0      539 2024-05-30 18:59:15.404879 vectorvision-0.1.0/vectorvision/utils.py
--rw-r--r--   0        0        0     3909 2024-05-30 18:59:15.404879 vectorvision-0.1.0/vectorvision/vertex_adjustment.py
--rw-r--r--   0        0        0     4002 1970-01-01 00:00:00.000000 vectorvision-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-08 07:51:44.418437 vectorvision-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1887 2024-05-31 18:34:50.906863 vectorvision-0.1.1/README.md
+-rw-r--r--   0        0        0     1154 2024-06-01 15:12:51.039194 vectorvision-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3683 2024-06-01 15:05:23.371106 vectorvision-0.1.1/vectorvision/Converter.py
+-rw-r--r--   0        0        0        0 2024-05-31 18:34:50.910864 vectorvision-0.1.1/vectorvision/__init__.py
+-rw-r--r--   0        0        0    19529 2024-06-01 15:05:23.371106 vectorvision-0.1.1/vectorvision/curve_optimization.py
+-rwxr-xr-x   0        0        0     1072 2024-06-01 15:05:23.371106 vectorvision-0.1.1/vectorvision/main.py
+-rw-r--r--   0        0        0     7922 2024-06-01 14:07:08.304047 vectorvision-0.1.1/vectorvision/path_decomposition.py
+-rw-r--r--   0        0        0    15876 2024-06-01 14:11:08.449167 vectorvision-0.1.1/vectorvision/polygons.py
+-rw-r--r--   0        0        0     2432 2024-06-01 15:05:23.375106 vectorvision-0.1.1/vectorvision/smoothing.py
+-rw-r--r--   0        0        0      546 2024-06-01 14:07:08.304047 vectorvision-0.1.1/vectorvision/utils.py
+-rw-r--r--   0        0        0     5126 2024-05-31 19:08:42.630392 vectorvision-0.1.1/vectorvision/vertex_adjustment.py
+-rw-r--r--   0        0        0     3614 1970-01-01 00:00:00.000000 vectorvision-0.1.1/PKG-INFO
```

### Comparing `vectorvision-0.1.0/LICENSE` & `vectorvision-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vectorvision-0.1.0/pyproject.toml` & `vectorvision-0.1.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vectorvision"
-version = "0.1.0"
+version = "0.1.1"
 description = "CLI tool for vectorizing raster graphics, written on the basis of the potrace algorithm."
 authors = ["Wojciech Łapacz", "Karol Ziarek", "Kajetan Rożej"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -39,11 +39,13 @@
 shapely = "2.0.4"
 six = "1.16.0"
 snowballstemmer = "2.2.0"
 tomli = "2.0.1"
 typing_extensions = "4.11.0"
 urllib3 = "2.2.1"
 
-
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.poetry.scripts]
+vectorvision = "vectorvision.main:main"
```

### Comparing `vectorvision-0.1.0/vectorvision/Converter.py` & `vectorvision-0.1.1/vectorvision/Converter.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from PIL import ImageOps, Image
 import time
-import os
 import numpy as np
 from vectorvision.path_decomposition import Bitmap
 from vectorvision.smoothing import smooth, POTRACE_CURVETO
 from vectorvision.polygons import get_best_polygon
 from vectorvision.vertex_adjustment import adjust_vertices, _Curve
+from vectorvision.curve_optimization import optimize_curve
 from contextlib import contextmanager
 from typing import TextIO
 
 
 @contextmanager
 def create_svg(name: str, width: int, height: int):
     file = open(f"{name}.svg", "+w")
@@ -51,52 +51,49 @@
                         np.isin(a, np.arange(0, color)),
                         0,
                         1,
                     )
                     self.convert_single_color(
                         color_table,
                         fh,
-                        color=color,
                         opacity=(1 - color / 255) * min(1, step / 60),
                     )
         e = time.process_time()
         print(f"Finished in {round(e - s, 2)} s\n")
 
-    def convert_single_color(self, color_table, fh, color=0, opacity=1):
+    def convert_single_color(self, color_table, fh, opacity=1):
         if not np.all(color_table):
             bm = Bitmap(color_table)
             paths_list = bm.generate_paths_list()
             polygons = [get_best_polygon(path) for path in paths_list]
             curves = list()
             for path, polygon in zip(paths_list, polygons):
                 curve = adjust_vertices(path, polygon)
-                smooth_curve = smooth(curve, 0.5)
-                curves.append(smooth_curve)
-            self._write_path_to_svg(fh, curves, color, opacity)
+                smooth_curve = smooth(curve, 1.0)
+                optimal_curve = optimize_curve(smooth_curve, 0.2)
+                curves.append(optimal_curve)
+            self._write_path_to_svg(fh, curves, opacity)
 
     def _write_path_to_svg(
-        self, fp: TextIO, curves: list[_Curve], color: int, opacity: float
+        self, fp: TextIO, curves: list[_Curve], opacity: float
     ) -> None:
         """Writes path of given color to the SVG file."""
 
         parts = list()
         for curve in curves:
             first_segment = curve.segments[-1].c[2]
             parts.append(f"M{first_segment[0]},{first_segment[1]}")
             for segment in curve.segments:
                 if segment.tag == POTRACE_CURVETO:
                     a = segment.c[0]
                     b = segment.c[1]
                     c = segment.c[2]
-                    parts.append(f"C{a[0]},{a[1]} {b[0]},{b[1]} {c[0]},{c[1]}")
+                    parts.append(f"C{a[0]} {a[1]}, {b[0]} {b[1]}, {c[0]} {c[1]}")
                 else:
                     a = segment.c[1]
                     b = segment.c[2]
-                    parts.append(f"Q{a[0]},{a[1]} {b[0]},{b[1]}")
+                    parts.append(f"L{a[0]} {a[1]} {b[0]},{b[1]}")
             parts.append("z")
 
-        rgb_color = (color, color, color)
-
-        print(opacity, rgb_color)
         fp.write(
             f'<path stroke="none" opacity="{opacity} " fill-rule="evenodd" d="{"".join(parts)}"/>'
         )
```

### Comparing `vectorvision-0.1.0/vectorvision/path_decomposition.py` & `vectorvision-0.1.1/vectorvision/path_decomposition.py`

 * *Files 21% similar despite different names*

```diff
@@ -119,44 +119,49 @@
         xa = points_in_path[0][0]
         for n in points_in_path:
             x, y = n[0], n[1]
             if y != y1:
                 self._xor_to_ref(x, min(y, y1), xa)
                 y1 = y
 
+
+    def _get_color_in_bounds(self, x_, y_):
+        """Get the color at a given point.
+
+        Args:
+            point: point in the bitmap
+
+        Returns:
+            Value of the color at the specified point. Returns 0 if point is out of range. -1 when white and 1 otherwise.
+        """
+        x_size, y_size = self.bitmap.shape
+        if y_ in range(x_size) and x_ in range(y_size):
+            return 1 if self.bitmap[y_][x_] else -1
+        return 0
+
+      
     def _get_majority_value(self, x: int, y: int) -> int:
         """Computes the "majority" value of bitmap bm at intersection (x,y). We
         assume that the bitmap is balanced at "radius" 1.
 
         Args:
             x: x-coord of a point
             y: y-coord of a point
 
         Returns:
             Majority color value.
         """
         for i in range(2, 5):
             ct = 0
             for a in range(-i + 1, i - 2):
-                try:
-                    ct += 1 if self.bitmap[y + i - 1][x + a] else -1
-                except IndexError:
-                    pass
-                try:
-                    ct += 1 if self.bitmap[y + a - 1][x + i - 1] else -1
-                except IndexError:
-                    pass
-                try:
-                    ct += 1 if self.bitmap[y - i][x + a - 1] else -1
-                except IndexError:
-                    pass
-                try:
-                    ct += 1 if self.bitmap[y + a][x - i] else -1
-                except IndexError:
-                    pass
+                ct += self._get_color_in_bounds(x + a, y + i - 1)
+                ct += self._get_color_in_bounds(x + i - 1, y + a)
+                ct += self._get_color_in_bounds(x + a - 1, y - i)
+                ct += self._get_color_in_bounds(x - i, y + a)
+
             if ct > 0:
                 return 1
             elif ct < 0:
                 return 0
         return 0
 
     def _find_path(
@@ -197,32 +202,29 @@
 
             left, right = self._get_next_in_direction_points(x, y, step_x, step_y)
 
             left_color = self._get_color_at_point(left)
             right_color = self._get_color_at_point(right)
 
             if left_color and not right_color:
-                # if (
-                #     turnpolicy == Turnpolicy.RIGHT
-                #     or (
-                #         turnpolicy == Turnpolicy.MAJORITY
-                #         and self._get_majority_value(x, y)
-                #     )
-                #     or (
-                #         turnpolicy == Turnpolicy.MINORITY
-                #         and not self._get_majority_value(x, y)
-                #     )
-                # ):
-                #     step_x, step_y = step_y, -step_x  # right turn
-                #
-                # else:
-                # tmp = dirx  # /* left turn */
-                # dirx = -diry
-                # diry = tmp
-                step_x, step_y = -step_y, step_x  # left turn
+                if (
+                    turnpolicy == Turnpolicy.RIGHT
+                    or (
+                        turnpolicy == Turnpolicy.MAJORITY
+                        and self._get_majority_value(x, y)
+                    )
+                    or (
+                        turnpolicy == Turnpolicy.MINORITY
+                        and not self._get_majority_value(x, y)
+                    )
+                ):
+                    step_x, step_y = step_y, -step_x  # right turn
+
+                else:
+                    step_x, step_y = -step_y, step_x  # left turn
 
             elif left_color:  # left turn
                 step_x, step_y = step_y, -step_x
 
             elif not right_color:  # right turn
                 step_x, step_y = -step_y, step_x
```

### Comparing `vectorvision-0.1.0/vectorvision/smoothing.py` & `vectorvision-0.1.1/vectorvision/smoothing.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,89 @@
 from vectorvision.vertex_adjustment import _Curve
+from vectorvision.utils import interval
 import math
 import numpy as np
 
+
 # /* segment tags */
 POTRACE_CURVETO = 1
 POTRACE_CORNER = 2
 
 
-def interval(t: float, a, b):
-    return (a[0] + t * (b[0] - a[0]), a[1] + t * (b[1] - a[1]))
-
+def calculate_alpha(
+    point0: tuple[float, float],
+    point1: tuple[float, float],
+    point2: tuple[float, float],
+) -> float:
+    """Calculate the parameter alpha of Bezier curve necessary for corner detection and smoothing
+
+    Args:
+        point0: starting point
+        point1: vertex point
+        point2: end point
+
+    Returns:
+        value of alpha parameter
+    """
 
-def calculate_alpha(point0, point1, point2):
     point0_np = np.array(point0)
     point1_np = np.array(point1)
     point2_np = np.array(point2)
 
     l1_norm_p0_p2 = np.linalg.norm(point2_np - point0_np, ord=1)
     if l1_norm_p0_p2 != 0.0:
         cross_product_p1_p0_p2_p0 = np.cross(
             point1_np - point0_np, point2_np - point0_np
         )
         factor_of_proportionality = math.fabs(cross_product_p1_p0_p2_p0 / l1_norm_p0_p2)
         if factor_of_proportionality > 1:
             gamma = 1 - 1.0 / factor_of_proportionality
+
         else:
             gamma = 0
         alpha = gamma / 0.75
     else:
         alpha = 4 / 3.0
     return alpha
 
 
 def smooth(curve: _Curve, alphamax: float) -> None:
+    """
+    Calculate the point which is splitting section into two parts in given proportion
+
+    Args:
+        proportion: in which proportion segment should be splitted, ratio ax/ab
+        a: first point
+        b: second point
+
+    Returns:
+        point splitting segment ab in given proportion
+    """
+
     n_of_segments = curve.n
 
-    # /* examine each vertex and find its best fit */
     for i in range(n_of_segments):
         j = (i + 1) % n_of_segments
         k = (i + 2) % n_of_segments
 
         alpha = calculate_alpha(curve[i].vertex, curve[j].vertex, curve[k].vertex)
         p4 = interval(1 / 2.0, curve[j].vertex, curve[k].vertex)
 
-        if alpha >= alphamax:  # /* pointed corner */
+        if alpha >= alphamax:  # corner found
 
             curve[j].tag = POTRACE_CORNER
             curve[j].c[1] = curve[j].vertex
             curve[j].c[2] = p4
+
         else:
             if alpha < 0.55:
                 alpha = 0.55
             elif alpha > 1:
                 alpha = 1
-            p2 = interval(alpha, curve[i].vertex, curve[j].vertex)
-            p3 = interval(alpha, curve[k].vertex, curve[j].vertex)
+            p2 = interval(0.5 + 0.5 * alpha, curve[i].vertex, curve[j].vertex)
+            p3 = interval(0.5 + 0.5 * alpha, curve[k].vertex, curve[j].vertex)
             curve[j].tag = POTRACE_CURVETO
             curve[j].c[0] = p2
             curve[j].c[1] = p3
             curve[j].c[2] = p4
-        # curve[j].alpha = alpha  # /* store the "cropped" value of alpha */
 
     return curve
```

### Comparing `vectorvision-0.1.0/vectorvision/vertex_adjustment.py` & `vectorvision-0.1.1/vectorvision/vertex_adjustment.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from numpy.linalg import lstsq
 import numpy as np
 from shapely.geometry import Point, Polygon
 from shapely.ops import nearest_points
-from typing import Tuple
+from typing import Optional
 
 
 class _Curve:
     def __init__(self, m):
         self.segments = [_Segment() for _ in range(m)]
         self.alphacurve = False
 
@@ -28,87 +28,141 @@
         self.vertex = [0, 0]
         self.alpha = 0.0
         self.alpha0 = 0.0
         self.beta = 0.0
 
 
 def fit_least_squares(points: list[tuple[float, float]]) -> tuple[float, float]:
+    """Fit linear function to given points in 2D with least squares method
 
-    """Fit linear function to given points in 2D with least squares method"""
+    Args:
+        points: list of points to which straight should be fitted
+
+    Returns:
+        Tuple (a, b) with parameters of fitted straight in format y=ax+b
+    """
 
     x = np.array([point[0] for point in points])
     y = np.array([point[1] for point in points])
     A = np.vstack([x, np.ones(len(x))]).T
     return lstsq(A, y, rcond=None)[0]
 
 
-def calculate_intersection_point(first_parameters: tuple[float, float],
-                                 second_parameters: tuple[float, float]
-                                 ) -> tuple[float, float]:
+def calculate_intersection_point(
+    first_parameters: tuple[float, float], second_parameters: tuple[float, float]
+) -> Optional[tuple[float, float]]:
+    """Calculate point of intersection for two linear functions
+
+    Args:
+        first_parameters: Tuple (a, b), parameters of first straight in format ax+b
+        second_parameters: Tuple (c, d), parameters of second straight in format cx+d
 
-    """Calculate point of intersection for two linear functions"""
+    Returns:
+        Tuple (x, y) with point of intersection or None if straights are parallel
+    """
 
     a, b = first_parameters
     c, d = second_parameters
     if a == c:
-        return (0, 0)
-    x_intersection = (d-b)/(a-c)
+        return None
+    x_intersection = (d - b) / (a - c)
     y_intersection = x_intersection * a + b
     return (x_intersection, y_intersection)
 
 
-def find_closest_point_in_boundary(original_point: Tuple[float, float],
-                                   boundary_center: Tuple[float, float],
-                                   boundary_manhatan_range: float
-                                   ) -> Point:
+def find_closest_point_in_boundary(
+    original_point: tuple[float, float],
+    boundary_center: tuple[float, float],
+    boundary_manhatan_range: float,
+) -> Point:
+    """Find point closest to original point but lying inside the square boundary around another point
+
+    Args:
+        original_point: location of original point
+        boundary_center: center of boundary
+        boundary_manhatan_range: distance along all main directions designating boundary location
 
-    """Find point closest to original point but lying inside the square boundary around another point"""
+    Returns:
+        Point in boundary closest to original point
+    """
 
     boundary_center_x, boundary_center_y = boundary_center
-    poly = Polygon([(boundary_center_x+boundary_manhatan_range, boundary_center_y+boundary_manhatan_range),
-                    (boundary_center_x-boundary_manhatan_range, boundary_center_y+boundary_manhatan_range),
-                    (boundary_center_x-boundary_manhatan_range, boundary_center_y-boundary_manhatan_range),
-                    (boundary_center_x+boundary_manhatan_range, boundary_center_y-boundary_manhatan_range)])
+    poly = Polygon(
+        [
+            (
+                boundary_center_x + boundary_manhatan_range,
+                boundary_center_y + boundary_manhatan_range,
+            ),
+            (
+                boundary_center_x - boundary_manhatan_range,
+                boundary_center_y + boundary_manhatan_range,
+            ),
+            (
+                boundary_center_x - boundary_manhatan_range,
+                boundary_center_y - boundary_manhatan_range,
+            ),
+            (
+                boundary_center_x + boundary_manhatan_range,
+                boundary_center_y - boundary_manhatan_range,
+            ),
+        ]
+    )
     point = Point(original_point)
-    p1, p2 = nearest_points(poly, point)
+    p1, _ = nearest_points(poly, point)
     return p1
 
 
-def adjust_vertices(path: list[tuple[float, float]], polygon_points_idxs: list[int]) -> _Curve:
+def adjust_vertices(
+    path: list[tuple[float, float]], polygon_points_idxs: list[int]
+) -> _Curve:
     """
     Adjust vertices of optimal polygon: calculate the intersection of
      the two "optimal" line segments, then move it into the unit square
      if it lies outside.
+
+        Args:
+            path: list of points forming path
+            polygon_points_idxs: list of points indexes in path contained in optimal polygon
+
+        Returns:
+            Curve representation of path
     """
+
     curve = _Curve(len(polygon_points_idxs))
 
-    points = path[polygon_points_idxs[-2]:polygon_points_idxs[-1]+1]
+    points = path[polygon_points_idxs[-2] : polygon_points_idxs[-1] + 1]
     prev_coeff = fit_least_squares(points)
 
-    points = path[polygon_points_idxs[-1]:] + [path[polygon_points_idxs[0]]]
+    points = path[polygon_points_idxs[-1] :] + [path[polygon_points_idxs[0]]]
     coeffs = fit_least_squares(points)
 
     intersection_point = calculate_intersection_point(coeffs, prev_coeff)
+    if intersection_point is None:
+        intersection_point = (0, 0)
 
-    point_in_boundaries = find_closest_point_in_boundary(intersection_point, path[polygon_points_idxs[-1]], 0.5)
-
+    point_in_boundaries = find_closest_point_in_boundary(
+        intersection_point, path[polygon_points_idxs[-1]], 0.5
+    )
 
     curve[-1].vertex[0] = point_in_boundaries.x
     curve[-1].vertex[1] = point_in_boundaries.y
     prev_point_idx = polygon_points_idxs[0]
     prev_coeff = coeffs
 
-
     for i, polygon_point in enumerate(polygon_points_idxs[1:]):
 
-        points = path[prev_point_idx:polygon_point+1]
+        points = path[prev_point_idx : polygon_point + 1]
         coeffs = fit_least_squares(points)
 
         intersection_point = calculate_intersection_point(coeffs, prev_coeff)
-        point_in_boundaries = find_closest_point_in_boundary(intersection_point, path[prev_point_idx], 0.5)
+        if intersection_point is None:
+            intersection_point = (0, 0)
+        point_in_boundaries = find_closest_point_in_boundary(
+            intersection_point, path[prev_point_idx], 0.5
+        )
 
         curve[i].vertex[0] = point_in_boundaries.x
         curve[i].vertex[1] = point_in_boundaries.y
         prev_point_idx = polygon_point
         prev_coeff = coeffs
 
     return curve
```

### Comparing `vectorvision-0.1.0/PKG-INFO` & `vectorvision-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectorvision
-Version: 0.1.0
+Version: 0.1.1
 Summary: CLI tool for vectorizing raster graphics, written on the basis of the potrace algorithm.
 License: MIT
 Author: Wojciech Łapacz
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
@@ -47,50 +47,58 @@
 Description-Content-Type: text/markdown
 
 # Vectorvision
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 [![Documentation Status](https://readthedocs.org/projects/vectorvision/badge/?version=latest)](https://vectorvision.readthedocs.io/en/latest/?badge=latest)
 
 ## Overview
-Projekt polega na zaimplementowaniu narzędzia pozwalającego na konwersję obrazka z formatu rastrowego (np. .png lub .jpg) do wersji wektorowej (np. .svg).
-
-Aplikacja powinna wspierać przynajmniej formaty wejściowe PNG i JPG oraz format wyjściowy SVG. Utworzony plik SVG powinien zostać w miarę możliwości zoptymalizowany pod kątem rozmiaru. Aplikacja powinna działać z poziomu konsoli (CLI).
 
+Vectorvision is a tool for vectorizing raster graphics, written on the basis of the potrace (https://potrace.sourceforge.net/) program. A detailed description of the algorithm can be found in the publication about potrace (https://potrace.sourceforge.net/potrace.pdf).
+For now, available color formats are binary and grayscale, RGB images are firstly converted to grayscale and vectorized. You can convert images of any common format including: png, jpg, jpeg. The output format is SVG.
 
 ## Features
 
-Program powinien umożliwiać przetwarzanie obrazów z formatów rastrowych PNG i JPG do formatu wektorowego SVG. W pierwszej kolejności obsługiwana będzie konwersja prostych obrazów binarnych, docelowo również bardziej skomplikowanych obrazów monochromatycznych i kolorowych. Obsługa programu odbywać się będzie z poziomu linii komend. Użytkownik przed uruchomieniem będzie miał możliwość określenia parametrów konwersji związanych z używanym algorytmem oraz (potencjalnie) wyboru algorytmu konwersji za pomocą flag wywołania. Ostateczna decyzja dotycząca implementowanych wariantów algorytmów konwersji zostanie podjęta po dogłębniejszym zapoznaniu się z tematem w  najbliższych tygodniach.
-
-- Wsparcie dla formatów wejściowych: PNG, JPG.
-- Format wyjściowy: SVG.
-- Optymalizacja pliku wyjściowego SVG pod kątem rozmiaru.
-- Uruchomienie programu z poziomu konsoli komendą:
-	program <sciezka do pliku wejscia> <nazwa pliku wyjscia> <parametry konwersji>
+The program allows you to transfer images from raster formats, e.g. PNG, to the SVG vector format. The program is available from the command line.
+Features:
+- Support for utility formats: PNG, JPG, JPEG, BMP.
+- Output format: SVG.
+- Optimization of the SVG output file for functionality.
+- Starting the program from the command line.
 
 ## Tech Stack
-Projekt zrealizowany zostanie w języku Python. Na chwilę obecną zakładamy wykorzystanie następujących bibliotek:
+
+The language of this project is Python. These are main libraries that we use:
 - Sphinx
 - PIL
-- numpy 
-- argparse
-- OpenCV
+- numpy
+- shapely
 - pytest
 
 
-
 ## Docs
 See the documentation for detailed information:
 https://vectorvision.readthedocs.io/en/latest/?badge=latest
 
 ## Installation:
 
+To install this tool run:
+
+`pip install vectorvision`
+
 ## Usage:
 
+This is the command view that you can use to run the tool:
+
+`vectorvision -i <input_path>`
+
+The output image will have the same name as input and will be saved in the same directory.
 
 ## Authors
+
 - [@Karol Ziarek](https://github.com/ziarekk)
 - [@Wojciech Lapacz](https://github.com/WojciechL02)
 - [@Kajan Rożej](https://github.com/Kajotello)
 
 ## License
+
 Please check the MIT license that is listed in this repository.
```

