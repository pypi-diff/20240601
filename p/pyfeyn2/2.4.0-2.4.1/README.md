# Comparing `tmp/pyfeyn2-2.4.0.tar.gz` & `tmp/pyfeyn2-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfeyn2-2.4.0.tar", max compression
+gzip compressed data, was "pyfeyn2-2.4.1.tar", max compression
```

## Comparing `pyfeyn2-2.4.0.tar` & `pyfeyn2-2.4.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0    35149 2023-12-02 10:16:30.610881 pyfeyn2-2.4.0/LICENSE
--rw-r--r--   0        0        0     3380 2023-12-02 10:16:30.610881 pyfeyn2-2.4.0/README.md
--rw-r--r--   0        0        0      154 2023-12-02 10:16:30.686881 pyfeyn2-2.4.0/pyfeyn2/__init__.py
--rw-r--r--   0        0        0        0 2023-12-02 10:16:30.686881 pyfeyn2-2.4.0/pyfeyn2/auto/__init__.py
--rw-r--r--   0        0        0     2838 2023-12-02 10:16:30.686881 pyfeyn2-2.4.0/pyfeyn2/auto/bend.py
--rw-r--r--   0        0        0      647 2023-12-02 10:16:30.686881 pyfeyn2-2.4.0/pyfeyn2/auto/diagram.py
--rw-r--r--   0        0        0     1603 2023-12-02 10:16:30.686881 pyfeyn2-2.4.0/pyfeyn2/auto/label.py
--rw-r--r--   0        0        0    17291 2023-12-02 10:16:30.686881 pyfeyn2-2.4.0/pyfeyn2/auto/position.py
--rw-r--r--   0        0        0     3279 2023-12-02 10:16:30.686881 pyfeyn2-2.4.0/pyfeyn2/feynmandiagram.py
--rw-r--r--   0        0        0     2734 2023-12-02 10:16:30.686881 pyfeyn2-2.4.0/pyfeyn2/interface/dot.py
--rw-r--r--   0        0        0      279 2023-12-02 10:16:30.686881 pyfeyn2-2.4.0/pyfeyn2/interface/hepmc.py
--rw-r--r--   0        0        0      238 2023-12-02 10:16:30.686881 pyfeyn2-2.4.0/pyfeyn2/interface/qgraf.py
--rw-r--r--   0        0        0     2256 2023-12-02 10:16:30.686881 pyfeyn2-2.4.0/pyfeyn2/mkfeyndiag.py
--rw-r--r--   0        0        0        0 2023-12-02 10:16:30.686881 pyfeyn2-2.4.0/pyfeyn2/render/__init__.py
--rw-r--r--   0        0        0     4538 2023-12-02 10:16:30.686881 pyfeyn2-2.4.0/pyfeyn2/render/all.py
--rw-r--r--   0        0        0        0 2023-12-02 10:16:30.686881 pyfeyn2-2.4.0/pyfeyn2/render/js/__init__.py
--rw-r--r--   0        0        0     2491 2023-12-02 10:16:30.686881 pyfeyn2-2.4.0/pyfeyn2/render/js/mermaid.py
--rw-r--r--   0        0        0        0 2023-12-02 10:16:30.686881 pyfeyn2-2.4.0/pyfeyn2/render/latex/__init__.py
--rw-r--r--   0        0        0     3596 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/latex/dot.py
--rw-r--r--   0        0        0     7046 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/latex/feynmp.py
--rw-r--r--   0        0        0     2179 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/latex/latex.py
--rw-r--r--   0        0        0     2688 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/latex/metapost.py
--rw-r--r--   0        0        0     8729 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/latex/tikzfeynman.py
--rw-r--r--   0        0        0     7659 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/mpl/feynmanrender.py
--rw-r--r--   0        0        0    15951 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/ps/madgraph.py
--rw-r--r--   0        0        0        0 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/pyx/__init__.py
--rw-r--r--   0        0        0     7132 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/pyx/blobs.py
--rw-r--r--   0        0        0     1319 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/pyx/config.py
--rw-r--r--   0        0        0    13245 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/pyx/deco.py
--rw-r--r--   0        0        0     2561 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/pyx/diagrams.py
--rw-r--r--   0        0        0    41394 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/pyx/lines.py
--rw-r--r--   0        0        0     3549 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/pyx/paint.py
--rw-r--r--   0        0        0    12740 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/pyx/points.py
--rw-r--r--   0        0        0     9146 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/pyx/pyxrender.py
--rw-r--r--   0        0        0     1501 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/pyx/utils.py
--rw-r--r--   0        0        0     2989 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/render.py
--rw-r--r--   0        0        0     9925 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/text/ascii.py
--rw-r--r--   0        0        0      863 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/text/asciipdf.py
--rw-r--r--   0        0        0     2364 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/text/label.py
--rw-r--r--   0        0        0     1701 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/text/line.py
--rw-r--r--   0        0        0     2114 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/text/plainpdf.py
--rw-r--r--   0        0        0      527 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/text/point.py
--rw-r--r--   0        0        0     3850 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/text/style.py
--rw-r--r--   0        0        0     1770 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/text/unicode.py
--rw-r--r--   0        0        0     1976 2023-12-02 10:16:30.690881 pyfeyn2-2.4.0/pyfeyn2/render/text/unicodepdf.py
--rw-r--r--   0        0        0     2649 2023-12-02 10:16:31.662880 pyfeyn2-2.4.0/pyproject.toml
--rw-r--r--   0        0        0     5114 1970-01-01 00:00:00.000000 pyfeyn2-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-12 10:08:34.783389 pyfeyn2-2.4.1/LICENSE
+-rw-r--r--   0        0        0     3493 2024-04-12 10:08:34.783389 pyfeyn2-2.4.1/README.md
+-rw-r--r--   0        0        0      154 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/auto/__init__.py
+-rw-r--r--   0        0        0     2838 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/auto/bend.py
+-rw-r--r--   0        0        0      647 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/auto/diagram.py
+-rw-r--r--   0        0        0     1603 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/auto/label.py
+-rw-r--r--   0        0        0    18229 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/auto/position.py
+-rw-r--r--   0        0        0     3279 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/feynmandiagram.py
+-rw-r--r--   0        0        0     2734 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/interface/dot.py
+-rw-r--r--   0        0        0      279 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/interface/hepmc.py
+-rw-r--r--   0        0        0      238 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/interface/qgraf.py
+-rw-r--r--   0        0        0     2256 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/mkfeyndiag.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/__init__.py
+-rw-r--r--   0        0        0     4538 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/all.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/js/__init__.py
+-rw-r--r--   0        0        0     2491 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/js/mermaid.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/latex/__init__.py
+-rw-r--r--   0        0        0     3596 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/latex/dot.py
+-rw-r--r--   0        0        0     7046 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/latex/feynmp.py
+-rw-r--r--   0        0        0     2179 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/latex/latex.py
+-rw-r--r--   0        0        0     2688 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/latex/metapost.py
+-rw-r--r--   0        0        0     8807 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/latex/tikzfeynman.py
+-rw-r--r--   0        0        0     7659 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/mpl/feynmanrender.py
+-rw-r--r--   0        0        0    15951 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/ps/madgraph.py
+-rw-r--r--   0        0        0        0 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/pyx/__init__.py
+-rw-r--r--   0        0        0     7132 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/pyx/blobs.py
+-rw-r--r--   0        0        0     1319 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/pyx/config.py
+-rw-r--r--   0        0        0    13245 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/pyx/deco.py
+-rw-r--r--   0        0        0     2561 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/pyx/diagrams.py
+-rw-r--r--   0        0        0    41394 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/pyx/lines.py
+-rw-r--r--   0        0        0     3549 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/pyx/paint.py
+-rw-r--r--   0        0        0    12740 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/pyx/points.py
+-rw-r--r--   0        0        0     9146 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/pyx/pyxrender.py
+-rw-r--r--   0        0        0     1501 2024-04-12 10:08:34.859390 pyfeyn2-2.4.1/pyfeyn2/render/pyx/utils.py
+-rw-r--r--   0        0        0     2989 2024-04-12 10:08:34.863390 pyfeyn2-2.4.1/pyfeyn2/render/render.py
+-rw-r--r--   0        0        0     9925 2024-04-12 10:08:34.863390 pyfeyn2-2.4.1/pyfeyn2/render/text/ascii.py
+-rw-r--r--   0        0        0      863 2024-04-12 10:08:34.863390 pyfeyn2-2.4.1/pyfeyn2/render/text/asciipdf.py
+-rw-r--r--   0        0        0     2364 2024-04-12 10:08:34.863390 pyfeyn2-2.4.1/pyfeyn2/render/text/label.py
+-rw-r--r--   0        0        0     1701 2024-04-12 10:08:34.863390 pyfeyn2-2.4.1/pyfeyn2/render/text/line.py
+-rw-r--r--   0        0        0     2114 2024-04-12 10:08:34.863390 pyfeyn2-2.4.1/pyfeyn2/render/text/plainpdf.py
+-rw-r--r--   0        0        0      527 2024-04-12 10:08:34.863390 pyfeyn2-2.4.1/pyfeyn2/render/text/point.py
+-rw-r--r--   0        0        0     3850 2024-04-12 10:08:34.863390 pyfeyn2-2.4.1/pyfeyn2/render/text/style.py
+-rw-r--r--   0        0        0     1770 2024-04-12 10:08:34.863390 pyfeyn2-2.4.1/pyfeyn2/render/text/unicode.py
+-rw-r--r--   0        0        0     1976 2024-04-12 10:08:34.863390 pyfeyn2-2.4.1/pyfeyn2/render/text/unicodepdf.py
+-rw-r--r--   0        0        0     2999 2024-04-12 10:08:36.187408 pyfeyn2-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5227 1970-01-01 00:00:00.000000 pyfeyn2-2.4.1/PKG-INFO
```

### Comparing `pyfeyn2-2.4.0/LICENSE` & `pyfeyn2-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/README.md` & `pyfeyn2-2.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -32,14 +32,16 @@
 
 *   <https://github.com/ndeutschmann/qgraf-xml-drawer>
 *   <https://github.com/GkAntonius/feynman>
 *   <https://github.com/JP-Ellis/tikz-feynman>
 *   <https://pyfeyn.hepforge.org/> 
 *   <https://feynml.hepforge.org/>
 *   <http://www.feyndiagram.com/>
+*   <https://web.physik.rwth-aachen.de/user/harlander/software/feyngame/>
+*   <https://jaxodraw.sourceforge.io/>
 
 Several of these are integrated into pyfeyn2.
 
 ## Troubleshooting
 
 *   [ImageMagick security policy 'PDF' blocking conversion]( https://stackoverflow.com/questions/52998331/imagemagick-security-policy-pdf-blocking-conversion )
 *   [Graphviz missing on mac](https://graphviz.org/download/#mac)
```

### Comparing `pyfeyn2-2.4.0/pyfeyn2/auto/bend.py` & `pyfeyn2-2.4.1/pyfeyn2/auto/bend.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/auto/diagram.py` & `pyfeyn2-2.4.1/pyfeyn2/auto/diagram.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/auto/label.py` & `pyfeyn2-2.4.1/pyfeyn2/auto/label.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/auto/position.py` & `pyfeyn2-2.4.1/pyfeyn2/auto/position.py`

 * *Files 3% similar despite different names*

```diff
@@ -257,21 +257,21 @@
     xvalues = np.linspace(min_x, max_x, n_x)
     yvalues = np.linspace(min_y, max_y, n_y)
     xx, yy = np.meshgrid(xvalues, yvalues)
     positions = [[x, y] for x, y in zip(xx.flatten(), yy.flatten())]
     return positions
 
 
-def auto_position(fd, layout="neato", clear_vertices=True):
+def auto_position(fd, layout="neato", size=5, clear_vertices=True):
     """Automatically position the vertices and legs."""
     # fd = scale_positions(fd, 10)
     fd = fd.with_style(f"layout : {layout}")
     fd = incoming_to_left(fd)
     fd = outgoing_to_right(fd)
-    fd = feynman_adjust_points(fd, size=5, clear_vertices=clear_vertices)
+    fd = feynman_adjust_points(fd, size=size, clear_vertices=clear_vertices)
     # fd = remove_unnecessary_vertices(fd)
     return fd
 
 
 def incoming_to_left(fd):
     """Set the incoming legs to the left."""
     n = 0
@@ -368,15 +368,83 @@
                 )
             continue
         vertices.append(v)
     fd.vertices = vertices
     return fd
 
 
-def auto_vdw(fd, points=None, LJ=1.0, y_symmetry=0.0, x_symmetry=0.0, intersection=0.0):
+def quad(points, cons, all_points, *args, dis=1.0):
+    for i, p in enumerate(points):
+        p.x = args[2 * i]
+        p.y = args[2 * i + 1]
+    r = dis
+    LenJ = 0
+    if dis != 0.0:
+        for i, p in enumerate(points):
+            for j in cons[i]:
+                if all_points[j].x is not None and all_points[j].y is not None:
+                    LenJ = LenJ + (
+                        (
+                            (
+                                (
+                                    (p.x - all_points[j].x) ** 2
+                                    + (p.y - all_points[j].y) ** 2
+                                )
+                                ** 0.5
+                                - r
+                            )
+                        )
+                        ** 2
+                    )
+    return LenJ
+
+
+def lennard_jones(points, cons, all_points, *args, LJ=1.0):
+    for i, p in enumerate(points):
+        p.x = args[2 * i]
+        p.y = args[2 * i + 1]
+    r = LJ
+    LenJ = 0
+    if LJ != 0.0:
+        for i, p in enumerate(points):
+            for j in cons[i]:
+                if all_points[j].x is not None and all_points[j].y is not None:
+                    LenJ = (
+                        LenJ
+                        - (
+                            (
+                                (
+                                    (
+                                        (p.x - all_points[j].x) ** 2
+                                        + (p.y - all_points[j].y) ** 2
+                                    )
+                                    ** 0.5
+                                )
+                                / r
+                            )
+                            ** 6
+                        )
+                        + (
+                            (
+                                (
+                                    (p.x - all_points[j].x) ** 2
+                                    + (p.y - all_points[j].y) ** 2
+                                )
+                                ** 0.5
+                            )
+                            / r
+                        )
+                        ** 12
+                    )
+    return LenJ
+
+
+def auto_vdw(
+    fd, points=None, LJ=0.0, dis=4.0, y_symmetry=0.0, x_symmetry=0.0, intersection=0.0
+):
     """
     Minimizes Lennard-Jones potential between vertices and legs (scaled by LJ).
     Further the function to be minimized gets punished by the number of intersections scaled by intersection.
     The function to be minimized gets punished by the asymmetry in x and y direction scaled by x_symmetry and y_symmetry.
 
     Parameters
     ----------
@@ -393,21 +461,17 @@
     intersection : float, optional
         The strength of the punishment for intersections, by default 0.0
 
     Returns
     -------
     FeynmanDiagram
         The Feynman diagram with the vertices and legs positioned.
-
-
-
     """
     if points is None:
         points = fd.vertices
-    r = LJ
     all_points = [*fd.vertices, *fd.legs]
     set_none_xy_to_zero(points)
     # get distance to connected points
     cons = []
     # dist = []
     for p in points:
         n = []
@@ -422,46 +486,16 @@
         cons.append(n)
         # dist.append(dd)
 
     def fun(*args):
         for i, p in enumerate(points):
             p.x = args[2 * i]
             p.y = args[2 * i + 1]
-        LenJ = 0
-        if LJ != 0.0:
-            for i, p in enumerate(points):
-                for j in cons[i]:
-                    if all_points[j].x is not None and all_points[j].y is not None:
-                        LenJ = (
-                            LenJ
-                            - (
-                                (
-                                    (
-                                        (
-                                            (p.x - all_points[j].x) ** 2
-                                            + (p.y - all_points[j].y) ** 2
-                                        )
-                                        ** 0.5
-                                    )
-                                    / r
-                                )
-                                ** 6
-                            )
-                            + (
-                                (
-                                    (
-                                        (p.x - all_points[j].x) ** 2
-                                        + (p.y - all_points[j].y) ** 2
-                                    )
-                                    ** 0.5
-                                )
-                                / r
-                            )
-                            ** 12
-                        )
+        LenJ = lennard_jones(points, cons, all_points, *args, LJ=LJ)
+        qdis = quad(points, cons, all_points, *args, dis=dis)
         inter = 0
         if intersection != 0.0:
             inter += intersection * _compute_number_of_intersects(fd)
         pun_x = 0
         if x_symmetry != 0.0:
             min_x, min_y, max_x, max_y = fd.get_bounding_box()
             # get averate x and y
@@ -495,17 +529,15 @@
                     if pp.id == p.id or pp.x is None or pp.y is None:
                         continue
                     dist = np.sqrt((p.x - pp.x) ** 2 + (ny - pp.y) ** 2)
                     if dist < min_dist:
                         min_dist = dist
                 pun += min_dist
             pun_y = pun
-        # TODO add punishment for intersections
-        # TODO add punishment for asymmetry
-        return LenJ + inter + pun_x * x_symmetry + pun_y * y_symmetry
+        return qdis + LenJ + inter + pun_x * x_symmetry + pun_y * y_symmetry
 
     m = iminuit.Minuit(fun, *[0 for _ in range(len(points) * 2)])
     v = m.migrad()
     args = list(v.values.to_dict().values())
     for i, p in enumerate(points):
         p.x = args[2 * i]
         p.y = args[2 * i + 1]
```

### Comparing `pyfeyn2-2.4.0/pyfeyn2/feynmandiagram.py` & `pyfeyn2-2.4.1/pyfeyn2/feynmandiagram.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/interface/dot.py` & `pyfeyn2-2.4.1/pyfeyn2/interface/dot.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/mkfeyndiag.py` & `pyfeyn2-2.4.1/pyfeyn2/mkfeyndiag.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/all.py` & `pyfeyn2-2.4.1/pyfeyn2/render/all.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/js/mermaid.py` & `pyfeyn2-2.4.1/pyfeyn2/render/js/mermaid.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/latex/dot.py` & `pyfeyn2-2.4.1/pyfeyn2/render/latex/dot.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/latex/feynmp.py` & `pyfeyn2-2.4.1/pyfeyn2/render/latex/feynmp.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/latex/latex.py` & `pyfeyn2-2.4.1/pyfeyn2/render/latex/latex.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/latex/metapost.py` & `pyfeyn2-2.4.1/pyfeyn2/render/latex/metapost.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/latex/tikzfeynman.py` & `pyfeyn2-2.4.1/pyfeyn2/render/latex/tikzfeynman.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     "gluino": ["plain,gluon"],
     "higgs": ["scalar"],
     "vector": ["boson"],
     # UTIL
     "phantom": ["draw=none"],
     "line": ["plain"],
     "plain": ["plain"],
+    "remnant": ["plain", "double=none, double distance=%(double_distance)s"],
     "baryon": ["fermion", "double=none, double distance=%(double_distance)s"],
     "anti baryon": ["anti fermion", "double=none, double distance=%(double_distance)s"],
     "meson": ["double=none,double distance =%(double_distance)s"],
 }
 
 shape_map = {
     "dot": "dot",
```

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/mpl/feynmanrender.py` & `pyfeyn2-2.4.1/pyfeyn2/render/mpl/feynmanrender.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/ps/madgraph.py` & `pyfeyn2-2.4.1/pyfeyn2/render/ps/madgraph.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/pyx/blobs.py` & `pyfeyn2-2.4.1/pyfeyn2/render/pyx/blobs.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/pyx/config.py` & `pyfeyn2-2.4.1/pyfeyn2/render/pyx/config.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/pyx/deco.py` & `pyfeyn2-2.4.1/pyfeyn2/render/pyx/deco.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/pyx/diagrams.py` & `pyfeyn2-2.4.1/pyfeyn2/render/pyx/diagrams.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/pyx/lines.py` & `pyfeyn2-2.4.1/pyfeyn2/render/pyx/lines.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/pyx/paint.py` & `pyfeyn2-2.4.1/pyfeyn2/render/pyx/paint.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/pyx/points.py` & `pyfeyn2-2.4.1/pyfeyn2/render/pyx/points.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/pyx/pyxrender.py` & `pyfeyn2-2.4.1/pyfeyn2/render/pyx/pyxrender.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/pyx/utils.py` & `pyfeyn2-2.4.1/pyfeyn2/render/pyx/utils.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/render.py` & `pyfeyn2-2.4.1/pyfeyn2/render/render.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/text/ascii.py` & `pyfeyn2-2.4.1/pyfeyn2/render/text/ascii.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/text/asciipdf.py` & `pyfeyn2-2.4.1/pyfeyn2/render/text/asciipdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/text/label.py` & `pyfeyn2-2.4.1/pyfeyn2/render/text/label.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/text/line.py` & `pyfeyn2-2.4.1/pyfeyn2/render/text/line.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/text/plainpdf.py` & `pyfeyn2-2.4.1/pyfeyn2/render/text/plainpdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/text/point.py` & `pyfeyn2-2.4.1/pyfeyn2/render/text/point.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/text/style.py` & `pyfeyn2-2.4.1/pyfeyn2/render/text/style.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/text/unicode.py` & `pyfeyn2-2.4.1/pyfeyn2/render/text/unicode.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyfeyn2/render/text/unicodepdf.py` & `pyfeyn2-2.4.1/pyfeyn2/render/text/unicodepdf.py`

 * *Files identical despite different names*

### Comparing `pyfeyn2-2.4.0/pyproject.toml` & `pyfeyn2-2.4.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfeyn2"
-version = "2.4.0"
+version = "2.4.1"
 description = "PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around"
 authors = ["Alexander Puck Neuwirth <alexander@neuwirth-informatik.de>"]
 readme = "README.md"
 repository = "https://github.com/APN-Pucky/pyfeyn2"
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -38,15 +38,15 @@
 [tool.poetry.scripts]
 mkfeyndiag = "pyfeyn2.mkfeyndiag:main"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-sphinx = "<7.0.0"
+sphinx = "<8.0.0"
 sphinx-rtd-theme = "*"
 sphinxcontrib-napoleon = "*"
 nbsphinx = "*"
 jupyter-sphinx = "*"
 sphinx_autobuild = "*"
 sphinx_math_dollar = "*"
 myst-parser  = "*"
@@ -65,22 +65,31 @@
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = ">=2.20,<4.0"
 ipython =  "*"
 jupyterlab =  "*"
 jupyter = "*"
-poetry-dynamic-versioning = {extras = ["plugin"], version = ">=0.21.1,<1.2.0"}
+poetry-dynamic-versioning = {extras = ["plugin"], version = ">=0.21.1,<1.3.0"}
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "pep440"
 dirty = true
 # modified dunami default pattern without v
 pattern = '(?x)(?# ignore whitespace)^((?P<epoch>\d+)!)?(?P<base>\d+(\.\d+)*)(?# v1.2.3 or v1!2000.1.2)([-._]?((?P<stage>[a-zA-Z]+)[-._]?(?P<revision>\d+)?))?(?# b0)(\+(?P<tagged_metadata>.+))?$(?# +linux)'
 strict = true
 format-jinja = "{% if distance == 0 %}{{ base }}{% else %}{{ base }}.{{ distance }}{% endif %}"
+
+[tool.pytest.ini_options]
+minversion = "6.0"
+testpaths = ["tests"]
+addopts = [ "-Werror","-v","--cov=pyfeyn2","--cov-config=.coveragerc","--cov-append","--cov-report=term","--cov-report=xml","--doctest-modules","--ignore=docs/source/conf.py" ]
+filterwarnings = [
+    'error',
+    'ignore: pkg_resources is deprecated as an API:DeprecationWarning'
+]
```

### Comparing `pyfeyn2-2.4.0/PKG-INFO` & `pyfeyn2-2.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfeyn2
-Version: 2.4.0
+Version: 2.4.1
 Summary: PyFeyn is a package which makes drawing Feynman diagrams simple and programmatic.  Feynman diagrams are important constructs in perturbative field theory, so being able to draw them in a programmatic fashion is important if attempting to enumerate a large number of diagram configurations is important. The output quality of PyFeyn diagrams (into PDF or EPS formats) is very high, and special effects can be obtained by using constructs from PyX, which PyFeyn is based around
 Home-page: https://github.com/APN-Pucky/pyfeyn2
 Author: Alexander Puck Neuwirth
 Author-email: alexander@neuwirth-informatik.de
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -73,14 +73,16 @@
 
 *   <https://github.com/ndeutschmann/qgraf-xml-drawer>
 *   <https://github.com/GkAntonius/feynman>
 *   <https://github.com/JP-Ellis/tikz-feynman>
 *   <https://pyfeyn.hepforge.org/> 
 *   <https://feynml.hepforge.org/>
 *   <http://www.feyndiagram.com/>
+*   <https://web.physik.rwth-aachen.de/user/harlander/software/feyngame/>
+*   <https://jaxodraw.sourceforge.io/>
 
 Several of these are integrated into pyfeyn2.
 
 ## Troubleshooting
 
 *   [ImageMagick security policy 'PDF' blocking conversion]( https://stackoverflow.com/questions/52998331/imagemagick-security-policy-pdf-blocking-conversion )
 *   [Graphviz missing on mac](https://graphviz.org/download/#mac)
```

