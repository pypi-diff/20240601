# Comparing `tmp/pypalex-1.3.4.tar.gz` & `tmp/pypalex-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypalex-1.3.4.tar", last modified: Fri May 17 05:32:39 2024, max compression
+gzip compressed data, was "pypalex-1.3.5.tar", last modified: Fri May 31 23:07:21 2024, max compression
```

## Comparing `pypalex-1.3.4.tar` & `pypalex-1.3.5.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:32:39.049581 pypalex-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-17 05:32:28.000000 pypalex-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-17 05:32:28.000000 pypalex-1.3.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-05-17 05:32:39.049581 pypalex-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-05-17 05:32:28.000000 pypalex-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:32:39.045581 pypalex-1.3.4/pypalex/
--rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/Extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13934 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/arg_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)     2325 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/conversion_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    38484 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/extraction_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/print_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-17 05:32:28.000000 pypalex-1.3.4/pypalex/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:32:39.045581 pypalex-1.3.4/pypalex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-05-17 05:32:38.000000 pypalex-1.3.4/pypalex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-17 05:32:39.000000 pypalex-1.3.4/pypalex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 05:32:38.000000 pypalex-1.3.4/pypalex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-17 05:32:38.000000 pypalex-1.3.4/pypalex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 05:32:38.000000 pypalex-1.3.4/pypalex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-17 05:32:38.000000 pypalex-1.3.4/pypalex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-17 05:32:38.000000 pypalex-1.3.4/pypalex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 05:32:39.049581 pypalex-1.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-17 05:32:28.000000 pypalex-1.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:07:21.603649 pypalex-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-05-31 23:07:11.000000 pypalex-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-31 23:07:11.000000 pypalex-1.3.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-05-31 23:07:21.603649 pypalex-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12894 2024-05-31 23:07:11.000000 pypalex-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:07:21.599649 pypalex-1.3.5/pypalex/
+-rw-r--r--   0 runner    (1001) docker     (127)    15575 2024-05-31 23:07:11.000000 pypalex-1.3.5/pypalex/Extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-31 23:07:11.000000 pypalex-1.3.5/pypalex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13934 2024-05-31 23:07:11.000000 pypalex-1.3.5/pypalex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-31 23:07:11.000000 pypalex-1.3.5/pypalex/arg_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2660 2024-05-31 23:07:11.000000 pypalex-1.3.5/pypalex/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4342 2024-05-31 23:07:11.000000 pypalex-1.3.5/pypalex/conversion_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47932 2024-05-31 23:07:11.000000 pypalex-1.3.5/pypalex/extraction_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-31 23:07:11.000000 pypalex-1.3.5/pypalex/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-31 23:07:11.000000 pypalex-1.3.5/pypalex/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13513 2024-05-31 23:07:11.000000 pypalex-1.3.5/pypalex/print_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1498 2024-05-31 23:07:11.000000 pypalex-1.3.5/pypalex/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:07:21.599649 pypalex-1.3.5/pypalex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13919 2024-05-31 23:07:21.000000 pypalex-1.3.5/pypalex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-31 23:07:21.000000 pypalex-1.3.5/pypalex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 23:07:21.000000 pypalex-1.3.5/pypalex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 23:07:21.000000 pypalex-1.3.5/pypalex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 23:07:21.000000 pypalex-1.3.5/pypalex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 23:07:21.000000 pypalex-1.3.5/pypalex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 23:07:21.000000 pypalex-1.3.5/pypalex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 23:07:21.603649 pypalex-1.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2001 2024-05-31 23:07:11.000000 pypalex-1.3.5/setup.py
```

### Comparing `pypalex-1.3.4/LICENSE` & `pypalex-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.4/PKG-INFO` & `pypalex-1.3.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pypalex
-Version: 1.3.4
+Version: 1.3.5
 Summary: Python Palette Extractor: extracts color palettes from images into json files.
 Home-page: https://github.com/AlTimofeyev/pypalex
 Author: Al Timofeyev
 Author-email: al.timofeyev@outlook.com
 License: MIT
-Download-URL: https://github.com/AlTimofeyev/pypalex/archive/1.3.4.tar.gz
+Download-URL: https://github.com/AlTimofeyev/pypalex/archive/1.3.5.tar.gz
 Keywords: python,pypalex,palex,color-palette,colorscheme,extract-colorscheme,extract-palette,extractor
 Platform: UNKNOWN
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: pypalex Version: 1.3.4 Summary: Python Palette
+Metadata-Version: 2.1 Name: pypalex Version: 1.3.5 Summary: Python Palette
 Extractor: extracts color palettes from images into json files. Home-page:
 https://github.com/AlTimofeyev/pypalex Author: Al Timofeyev Author-email:
 al.timofeyev@outlook.com License: MIT Download-URL: https://github.com/
-AlTimofeyev/pypalex/archive/1.3.4.tar.gz Keywords: python,pypalex,palex,color-
+AlTimofeyev/pypalex/archive/1.3.5.tar.gz Keywords: python,pypalex,palex,color-
 palette,colorscheme,extract-colorscheme,extract-palette,extractor Platform:
 UNKNOWN Classifier: Environment :: X11 Applications Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: MacOS Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: Microsoft ::
 Windows Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `pypalex-1.3.4/README.md` & `pypalex-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.4/pypalex/Extractor.py` & `pypalex-1.3.5/pypalex/Extractor.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.4/pypalex/__init__.py` & `pypalex-1.3.5/pypalex/__init__.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.4/pypalex/__main__.py` & `pypalex-1.3.5/pypalex/__main__.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.4/pypalex/arg_messages.py` & `pypalex-1.3.5/pypalex/arg_messages.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.4/pypalex/constants.py` & `pypalex-1.3.5/pypalex/constants.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 ##  @file   constants.py
 #   @brief  A collection of constants for PyPalEx.
 #
 #   @section authors Author(s)
 #   - Created by Al Timofeyev on February 2, 2022.
 #   - Modified by Al Timofeyev on April 21, 2022.
 #   - Modified by Al Timofeyev on March 6, 2023.
+#   - Modified by Al Timofeyev on May 31, 2024.
 
 
 # RGB values for base colors.
 BLACK_RGB = [0, 0, 0]
 WHITE_RGB = [255, 255, 255]
 RED_RGB = [255, 0, 0]
 # YELLOW_RGB = [255, 255, 0]  # Original hex for yellow.
@@ -48,21 +49,23 @@
 GREEN_HUE_RANGE = [64, 170]
 CYAN_HUE_RANGE = [170, 210]
 BLUE_HUE_RANGE = [210, 260]
 MAGENTA_HUE_RANGE = [260, 330]
 # -----------------------------------------------
 
 # Brightness Value range [min, max] for grayscale/achromatic colors.
-BLACK_BRIGHTNESS_RANGE = [0.0, 50.0]    # Range of brightness for where a color can be considered dark.
-GRAY_BRIGHTNESS_RANGE = [50.0, 75.0]    # Range of brightness for where a color can be considered normal.
-WHITE_BRIGHTNESS_RANGE = [75.0, 100.0]  # Range of brightness for where a color can be considered light.
+BLACK_BRIGHTNESS_RANGE = [0.0, 35.0]    # Range of brightness for where a color can be considered black or indistinguishable.
+DARK_BRIGHTNESS_RANGE = [35.0, 55.0]    # Range of brightness for where a color can be considered dark.
+NORM_BRIGHTNESS_RANGE = [55.0, 80.0]    # Range of brightness for where a color can be considered normal.
+LIGHT_BRIGHTNESS_RANGE = [80.0, 100.0]  # Range of brightness for where a color can be considered light.
 # -----------------------------------------------
 
-# Saturation and Brightness Value ranges [min, max] that are tolerable for extracted colors
-SATURATION_RANGE = [5.0, 100.0]
-BRIGHTNESS_RANGE = [25.0, 100.0]
+# The tolerance range [min, max] for grayscale/achromatic colors.
+# If a color is less saturated than the min value in this range then it's considered grayscale/achromatic.
+# If a grayscale/achromatic color is borrowed from, then it's first normalized to be within this range
+SATURATION_TOLERANCE_RANGE = [10.0, 15.0]
 # -----------------------------------------------
 
 # Pastel Saturation and Brightness Value ranges [min, max]
 PASTEL_SATURATION_RANGE = [15.0, 75.0]
 PASTEL_BRIGHTNESS_RANGE = [50.0, 100.0]
 # -----------------------------------------------
```

### Comparing `pypalex-1.3.4/pypalex/conversion_utils.py` & `pypalex-1.3.5/pypalex/conversion_utils.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.4/pypalex/extraction_utils.py` & `pypalex-1.3.5/pypalex/extraction_utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #
 #   @section authors Author(s)
 #   - Created by Al Timofeyev on February 10, 2022.
 #   - Modified by Al Timofeyev on April 21, 2022.
 #   - Modified by Al Timofeyev on March 6, 2023.
 #   - Modified by Al Timofeyev on March 22, 2023.
 #   - Modified by Al Timofeyev on April 6, 2023.
+#   - Modified by Al Timofeyev on May 31, 2024.
 
 
 # ---- IMPORTS ----
 import multiprocessing
 import numpy
 import random
 import math
@@ -281,23 +282,29 @@
 def extract_color_types(hsv_base_color_matrix_and_sat_prefs):
     hsv_base_color_matrix, sat_pref_list = hsv_base_color_matrix_and_sat_prefs
     sat_pref_light, sat_pref_normal, sat_pref_dark = sat_pref_list
 
     if len(hsv_base_color_matrix) == 0:
         return [numpy.array([]), numpy.array([]), numpy.array([])]
 
-    light_colors, norm_colors, dark_colors = sort_by_bright_value(hsv_base_color_matrix)
+    light_colors, norm_colors, dark_colors, black_colors, achromatic_light_colors, \
+    achromatic_norm_colors, achromatic_dark_colors, achromatic_black_colors = sort_by_sat_and_bright_value(hsv_base_color_matrix)
+
     light_color = extract_dominant_color(light_colors, sat_pref_light)
     norm_color = extract_dominant_color(norm_colors, sat_pref_normal)
     dark_color = extract_dominant_color(dark_colors, sat_pref_dark)
+    black_color = extract_dominant_color(black_colors, sat_pref_dark)
+
+    achromatic_light = extract_dominant_color(achromatic_light_colors, sat_pref_light)
+    achromatic_norm = extract_dominant_color(achromatic_norm_colors, sat_pref_normal)
+    achromatic_dark = extract_dominant_color(achromatic_dark_colors, sat_pref_dark)
+    achromatic_black = extract_dominant_color(achromatic_black_colors, sat_pref_dark)
 
-    check_missing_color_types(light_color, norm_color, dark_color)
-    check_sat_and_bright(light_color)
-    check_sat_and_bright(norm_color)
-    check_sat_and_bright(dark_color)
+    check_missing_color_types(light_color, norm_color, dark_color, black_color,
+                              achromatic_light, achromatic_norm, achromatic_dark, achromatic_black)
 
     return [light_color, norm_color, dark_color]
 
 
 # --------------------------------------------------------------------------
 # --------------------------------------------------------------------------
 
@@ -521,36 +528,52 @@
 
     return [[light_background_color, light_foreground_color], [dark_background_color, dark_foreground_color]]
 
 
 # **************************************************************************
 # **************************************************************************
 
-##  Sorts the colors by the brightness value.
-#   @details    A color type is either a light, normal, or
-#               dark version of a base color.
-#
-#   @param  hsv_base_color_matrix   A 2D numpy array of a base color in [h,s,v] format.
-#
-#   @return List of numpy array color types in [h,s,v] format.
-def sort_by_bright_value(hsv_base_color_matrix):
-    light_colors = []
-    norm_colors = []
-    dark_colors = []
+##  Sorts the colors by their saturation and brightness values.
+#   @details    A color type is either a light, normal, dark,
+#               black or achromatic version of a base color.
+#
+#   @param  hsv_base_color_matrix   A 2D numpy array of a base color, where
+#                                   each element is a list in [h,s,v] format.
+#
+#   @return A list of color types, where each element is a 2D numpy array
+#           of a color type whose elements are a list in [h,s,v] format.
+def sort_by_sat_and_bright_value(hsv_base_color_matrix):
+    light_colors, norm_colors, dark_colors, black_colors = [], [], [], []
+    achromatic_light, achromatic_norm, achromatic_dark, achromatic_black = [], [], [], []
 
     for pixel in hsv_base_color_matrix:
-        brightness = pixel[2]
-        if brightness > const.WHITE_BRIGHTNESS_RANGE[0]:    # -------- If light color.
-            light_colors.append(pixel)
-        elif brightness > const.GRAY_BRIGHTNESS_RANGE[0]:   # -------- If normal color.
-            norm_colors.append(pixel)
-        else:                                               # -------- If dark color.
-            dark_colors.append(pixel)
+        _, saturation, brightness = pixel
+        if brightness > const.LIGHT_BRIGHTNESS_RANGE[0]:    # -------- If light color.
+            if saturation < const.SATURATION_TOLERANCE_RANGE[0]:
+                achromatic_light.append(pixel)
+            else:
+                light_colors.append(pixel)
+        elif brightness > const.NORM_BRIGHTNESS_RANGE[0]:   # -------- If normal color.
+            if saturation < const.SATURATION_TOLERANCE_RANGE[0]:
+                achromatic_norm.append(pixel)
+            else:
+                norm_colors.append(pixel)
+        elif brightness > const.DARK_BRIGHTNESS_RANGE[0]:   # -------- If dark color.
+            if saturation < const.SATURATION_TOLERANCE_RANGE[0]:
+                achromatic_dark.append(pixel)
+            else:
+                dark_colors.append(pixel)
+        else:                                               # -------- If black color.
+            if saturation < const.SATURATION_TOLERANCE_RANGE[0]:
+                achromatic_black.append(pixel)
+            else:
+                black_colors.append(pixel)
 
-    return [numpy.asarray(light_colors), numpy.asarray(norm_colors), numpy.asarray(dark_colors)]
+    return [numpy.asarray(light_colors), numpy.asarray(norm_colors), numpy.asarray(dark_colors), numpy.asarray(black_colors),
+            numpy.asarray(achromatic_light), numpy.asarray(achromatic_norm), numpy.asarray(achromatic_dark), numpy.asarray(achromatic_black)]
 
 
 # --------------------------------------------------------------------------
 # --------------------------------------------------------------------------
 
 ##  Extracts the dominant color from a color type.
 #   @details    A color type is either a light, normal, or
@@ -576,93 +599,193 @@
 
 # --------------------------------------------------------------------------
 # --------------------------------------------------------------------------
 
 ##  Checks to make sure all the color types have been properly set.
 #   @details    If a color type is missing, then it will
 #               be derived from the existing color types.
+#   @note   I'm using the normalization formula from https://stats.stackexchange.com/a/281164
 #
-#   @param  light_color A numpy array of a light color type in [h,s,v] format.
-#   @param  norm_color  A numpy array of a normal color type in [h,s,v] format.
-#   @param  dark_color  A numpy array of a dark color type in [h,s,v] format.
-def check_missing_color_types(light_color, norm_color, dark_color):
-    has_light = light_color[0] != -1
-    has_norm = norm_color[0] != -1
-    has_dark = dark_color[0] != -1
+#   @param  light_color         A numpy array of a light color type in [h,s,v] format.
+#   @param  norm_color          A numpy array of a normal color type in [h,s,v] format.
+#   @param  dark_color          A numpy array of a dark color type in [h,s,v] format.
+#   @param  black_color         A numpy array of a black color type in [h,s,v] format.
+#   @param  achromatic_light    A numpy array of an achromatic light color type in [h,s,v] format.
+#   @param  achromatic_norm     A numpy array of an achromatic normal color type in [h,s,v] format.
+#   @param  achromatic_dark     A numpy array of an achromatic dark color type in [h,s,v] format.
+#   @param  achromatic_black    A numpy array of an achromatic black color type in [h,s,v] format.
+def check_missing_color_types(light_color, norm_color, dark_color, black_color,
+                              achromatic_light, achromatic_norm, achromatic_dark, achromatic_black):
+    has_light = light_set = light_color[0] != -1
+    has_norm = norm_set = norm_color[0] != -1
+    has_dark = dark_set = dark_color[0] != -1
+    has_black = black_set = black_color[0] != -1
+
+    has_achro_light = achromatic_light[0] != -1
+    has_achro_norm = achromatic_norm[0] != -1
+    has_achro_dark = achromatic_dark[0] != -1
+    has_achro_black = achromatic_black[0] != -1
+
+    # Check and set black color using existing color types.
+    if not has_black:
+        if has_achro_black:
+            black_color[0], black_color[2] = achromatic_black[0], achromatic_black[2]
+            old_bounds = [0, const.SATURATION_TOLERANCE_RANGE[0]]
+            new_bounds = [const.SATURATION_TOLERANCE_RANGE[0], const.SATURATION_TOLERANCE_RANGE[1]]
+            black_color[1] = new_bounds[0] + (((achromatic_black[1] - old_bounds[0]) / (old_bounds[1] - old_bounds[0]))
+                                              * (new_bounds[1] - new_bounds[0]))
+            black_set = True
 
-    # Check and set dark color.
+    # Check and set dark color using existing color types.
     if not has_dark:
-        if has_light:
+        if has_black:
+            dark_color[0] = black_color[0]
+            dark_color[1] = black_color[1]
+            old_bounds = [const.BLACK_BRIGHTNESS_RANGE[0], const.BLACK_BRIGHTNESS_RANGE[1]]
+            new_bounds = [const.DARK_BRIGHTNESS_RANGE[0], const.DARK_BRIGHTNESS_RANGE[1]]
+            dark_color[2] = new_bounds[0] + (((black_color[2] - old_bounds[0]) / (old_bounds[1] - old_bounds[0]))
+                                             * (new_bounds[1] - new_bounds[0]))
+        elif has_light:
             dark_color[0] = light_color[0]
             dark_color[1] = light_color[1]
-            brightness_range = const.WHITE_BRIGHTNESS_RANGE[1] - const.WHITE_BRIGHTNESS_RANGE[0]
-            percent = (light_color[2] - const.WHITE_BRIGHTNESS_RANGE[0]) / brightness_range
-            brightness_offset = (const.BLACK_BRIGHTNESS_RANGE[1] - const.BLACK_BRIGHTNESS_RANGE[0]) * percent
-            dark_color[2] = const.BLACK_BRIGHTNESS_RANGE[1] - brightness_offset
+            old_bounds = [const.LIGHT_BRIGHTNESS_RANGE[0], const.LIGHT_BRIGHTNESS_RANGE[1]]
+            new_bounds = [const.DARK_BRIGHTNESS_RANGE[0], const.DARK_BRIGHTNESS_RANGE[1]]
+            dark_color[2] = new_bounds[1] - (((light_color[2] - old_bounds[0]) / (old_bounds[1] - old_bounds[0]))
+                                             * (new_bounds[1] - new_bounds[0]))
         elif has_norm:
             dark_color[0] = norm_color[0]
             sat_diff = math.sqrt(100 - norm_color[1]) if norm_color[1] < 50 else math.sqrt(norm_color[1])
             dark_color[1] = norm_color[1] + sat_diff if norm_color[1] < 50 else norm_color[1] - sat_diff
-            brightness_range = const.GRAY_BRIGHTNESS_RANGE[1] - const.GRAY_BRIGHTNESS_RANGE[0]
-            percent = (norm_color[2] - const.GRAY_BRIGHTNESS_RANGE[0]) / brightness_range
-            brightness_offset = (const.BLACK_BRIGHTNESS_RANGE[1] - const.BLACK_BRIGHTNESS_RANGE[0]) * percent
-            dark_color[2] = const.BLACK_BRIGHTNESS_RANGE[0] + brightness_offset
+            old_bounds = [const.NORM_BRIGHTNESS_RANGE[0], const.NORM_BRIGHTNESS_RANGE[1]]
+            new_bounds = [const.DARK_BRIGHTNESS_RANGE[0], const.DARK_BRIGHTNESS_RANGE[1]]
+            dark_color[2] = new_bounds[0] + (((norm_color[2] - old_bounds[0]) / (old_bounds[1] - old_bounds[0]))
+                                             * (new_bounds[1] - new_bounds[0]))
+        elif has_achro_dark:
+            dark_color[0], dark_color[2] = achromatic_dark[0], achromatic_dark[2]
+            old_bounds = [0, const.SATURATION_TOLERANCE_RANGE[0]]
+            new_bounds = [const.SATURATION_TOLERANCE_RANGE[0], const.SATURATION_TOLERANCE_RANGE[1]]
+            dark_color[1] = new_bounds[0] + (((achromatic_dark[1] - old_bounds[0]) / (old_bounds[1] - old_bounds[0]))
+                                             * (new_bounds[1] - new_bounds[0]))
+
+        if dark_color[0] != -1:     # If the dark color has been set by one of the options above.
+            dark_set = True
 
-    # Check and set light color.
+    # Check and set light color using existing color types.
     if not has_light:
         if has_dark:
             light_color[0] = dark_color[0]
             light_color[1] = dark_color[1]
-            brightness_range = const.BLACK_BRIGHTNESS_RANGE[1] - const.BLACK_BRIGHTNESS_RANGE[0]
-            percent = (dark_color[2] - const.BLACK_BRIGHTNESS_RANGE[0]) / brightness_range
-            brightness_offset = (const.WHITE_BRIGHTNESS_RANGE[1] - const.WHITE_BRIGHTNESS_RANGE[0]) * percent
-            light_color[2] = const.WHITE_BRIGHTNESS_RANGE[1] - brightness_offset
+            old_bounds = [const.DARK_BRIGHTNESS_RANGE[0], const.DARK_BRIGHTNESS_RANGE[1]]
+            new_bounds = [const.LIGHT_BRIGHTNESS_RANGE[0], const.LIGHT_BRIGHTNESS_RANGE[1]]
+            light_color[2] = new_bounds[1] - (((dark_color[2] - old_bounds[0]) / (old_bounds[1] - old_bounds[0]))
+                                              * (new_bounds[1] - new_bounds[0]))
         elif has_norm:
             light_color[0] = norm_color[0]
             sat_diff = math.sqrt(100 - norm_color[1]) if norm_color[1] < 50 else math.sqrt(norm_color[1])
             light_color[1] = norm_color[1] + sat_diff if norm_color[1] < 50 else norm_color[1] - sat_diff
-            brightness_range = const.GRAY_BRIGHTNESS_RANGE[1] - const.GRAY_BRIGHTNESS_RANGE[0]
-            percent = (norm_color[2] - const.GRAY_BRIGHTNESS_RANGE[0]) / brightness_range
-            brightness_offset = (const.WHITE_BRIGHTNESS_RANGE[1] - const.WHITE_BRIGHTNESS_RANGE[0]) * percent
-            light_color[2] = const.WHITE_BRIGHTNESS_RANGE[0] + brightness_offset
+            old_bounds = [const.NORM_BRIGHTNESS_RANGE[0], const.NORM_BRIGHTNESS_RANGE[1]]
+            new_bounds = [const.LIGHT_BRIGHTNESS_RANGE[0], const.LIGHT_BRIGHTNESS_RANGE[1]]
+            light_color[2] = new_bounds[0] + (((norm_color[2] - old_bounds[0]) / (old_bounds[1] - old_bounds[0]))
+                                              * (new_bounds[1] - new_bounds[0]))
+        elif has_achro_light:
+            light_color[0], light_color[2] = achromatic_light[0], achromatic_light[2]
+            old_bounds = [0, const.SATURATION_TOLERANCE_RANGE[0]]
+            new_bounds = [const.SATURATION_TOLERANCE_RANGE[0], const.SATURATION_TOLERANCE_RANGE[1]]
+            light_color[1] = new_bounds[0] + (((achromatic_light[1] - old_bounds[0]) / (old_bounds[1] - old_bounds[0]))
+                                              * (new_bounds[1] - new_bounds[0]))
 
-    # Check and set normal color, using averages.
+        if light_color[0] != -1:    # If the light color has been set by one of the options above.
+            light_set = True
+
+    # Check and set normal color using existing color types.
     if not has_norm:
+        if has_dark and has_light:
+            cos_light_hue, cos_dark_hue = math.cos(math.radians(light_color[0])), math.cos(math.radians(dark_color[0]))
+            sin_light_hue, sin_dark_hue = math.sin(math.radians(light_color[0])), math.sin(math.radians(dark_color[0]))
+            norm_color[0] = math.atan2(stats.mean([sin_light_hue, sin_dark_hue]), stats.mean([cos_light_hue, cos_dark_hue]))
+            norm_color[0] = round(math.degrees(norm_color[0])) % 360
+            norm_color[1] = (light_color[1] + dark_color[1]) / 2
+            light_percent = (light_color[2] - const.LIGHT_BRIGHTNESS_RANGE[0]) / (const.LIGHT_BRIGHTNESS_RANGE[1] - const.LIGHT_BRIGHTNESS_RANGE[0])
+            dark_percent = (dark_color[2] - const.DARK_BRIGHTNESS_RANGE[0]) / (const.DARK_BRIGHTNESS_RANGE[1] - const.DARK_BRIGHTNESS_RANGE[0])
+            avg_light_dark_brightness = (light_percent + dark_percent) / 2
+            norm_color[2] = const.NORM_BRIGHTNESS_RANGE[0] + (
+                    (const.NORM_BRIGHTNESS_RANGE[1] - const.NORM_BRIGHTNESS_RANGE[0]) * avg_light_dark_brightness)
+        elif has_achro_norm:
+            norm_color[0], norm_color[2] = achromatic_norm[0], achromatic_norm[2]
+            old_bounds = [0, const.SATURATION_TOLERANCE_RANGE[0]]
+            new_bounds = [const.SATURATION_TOLERANCE_RANGE[0], const.SATURATION_TOLERANCE_RANGE[1]]
+            norm_color[1] = new_bounds[0] + (((achromatic_norm[1] - old_bounds[0]) / (old_bounds[1] - old_bounds[0]))
+                                             * (new_bounds[1] - new_bounds[0]))
+
+        if norm_color[0] != -1:     # If the normal color has been set by one of the options above.
+            norm_set = True
+
+    # Double check for color types that haven't been set yet by using
+    # color types that have been set with the previous checks above.
+    # Check and set dark color using borrowed color types.
+    if not dark_set:
+        if black_set:
+            dark_color[0] = black_color[0]
+            dark_color[1] = black_color[1]
+            old_bounds = [const.BLACK_BRIGHTNESS_RANGE[0], const.BLACK_BRIGHTNESS_RANGE[1]]
+            new_bounds = [const.DARK_BRIGHTNESS_RANGE[0], const.DARK_BRIGHTNESS_RANGE[1]]
+            dark_color[2] = new_bounds[0] + (((black_color[2] - old_bounds[0]) / (old_bounds[1] - old_bounds[0]))
+                                             * (new_bounds[1] - new_bounds[0]))
+        elif light_set:
+            dark_color[0] = light_color[0]
+            dark_color[1] = light_color[1]
+            old_bounds = [const.LIGHT_BRIGHTNESS_RANGE[0], const.LIGHT_BRIGHTNESS_RANGE[1]]
+            new_bounds = [const.DARK_BRIGHTNESS_RANGE[0], const.DARK_BRIGHTNESS_RANGE[1]]
+            dark_color[2] = new_bounds[1] - (((light_color[2] - old_bounds[0]) / (old_bounds[1] - old_bounds[0]))
+                                             * (new_bounds[1] - new_bounds[0]))
+        elif norm_set:
+            dark_color[0] = norm_color[0]
+            sat_diff = math.sqrt(100 - norm_color[1]) if norm_color[1] < 50 else math.sqrt(norm_color[1])
+            dark_color[1] = norm_color[1] + sat_diff if norm_color[1] < 50 else norm_color[1] - sat_diff
+            old_bounds = [const.NORM_BRIGHTNESS_RANGE[0], const.NORM_BRIGHTNESS_RANGE[1]]
+            new_bounds = [const.DARK_BRIGHTNESS_RANGE[0], const.DARK_BRIGHTNESS_RANGE[1]]
+            dark_color[2] = new_bounds[0] + (((norm_color[2] - old_bounds[0]) / (old_bounds[1] - old_bounds[0]))
+                                             * (new_bounds[1] - new_bounds[0]))
+
+        if dark_color[0] != -1:     # If the dark color has been set by one of the options above.
+            dark_set = True
+
+    # Check and set light color using borrowed color types.
+    if not light_set:
+        if dark_set:
+            light_color[0] = dark_color[0]
+            light_color[1] = dark_color[1]
+            old_bounds = [const.DARK_BRIGHTNESS_RANGE[0], const.DARK_BRIGHTNESS_RANGE[1]]
+            new_bounds = [const.LIGHT_BRIGHTNESS_RANGE[0], const.LIGHT_BRIGHTNESS_RANGE[1]]
+            light_color[2] = new_bounds[1] - (((dark_color[2] - old_bounds[0]) / (old_bounds[1] - old_bounds[0]))
+                                              * (new_bounds[1] - new_bounds[0]))
+        elif norm_set:
+            light_color[0] = norm_color[0]
+            sat_diff = math.sqrt(100 - norm_color[1]) if norm_color[1] < 50 else math.sqrt(norm_color[1])
+            light_color[1] = norm_color[1] + sat_diff if norm_color[1] < 50 else norm_color[1] - sat_diff
+            old_bounds = [const.NORM_BRIGHTNESS_RANGE[0], const.NORM_BRIGHTNESS_RANGE[1]]
+            new_bounds = [const.LIGHT_BRIGHTNESS_RANGE[0], const.LIGHT_BRIGHTNESS_RANGE[1]]
+            light_color[2] = new_bounds[0] + (((norm_color[2] - old_bounds[0]) / (old_bounds[1] - old_bounds[0]))
+                                              * (new_bounds[1] - new_bounds[0]))
+
+        if light_color[0] != -1:    # If the light color has been set by one of the options above.
+            light_set = True
+
+    # Check and set normal color using borrowed color types.
+    if not norm_set:
         cos_light_hue, cos_dark_hue = math.cos(math.radians(light_color[0])), math.cos(math.radians(dark_color[0]))
         sin_light_hue, sin_dark_hue = math.sin(math.radians(light_color[0])), math.sin(math.radians(dark_color[0]))
         norm_color[0] = math.atan2(stats.mean([sin_light_hue, sin_dark_hue]), stats.mean([cos_light_hue, cos_dark_hue]))
         norm_color[0] = round(math.degrees(norm_color[0])) % 360
         norm_color[1] = (light_color[1] + dark_color[1]) / 2
-        norm_color[2] = (light_color[2] + dark_color[2]) / 2
-
-
-# --------------------------------------------------------------------------
-# --------------------------------------------------------------------------
-
-##  Normalize saturation and brightness value.
-#   @details    The normalization process is to make sure
-#               that colors are visible, distinguishable and
-#               tolerable to look at. These ranges for saturation
-#               and brightness values are defined in constants.py.
-#               This step can be removed if it is not needed
-#               as it does not impact the extraction process.
-#
-#   @param  hsv_color   A numpy array of a color type in [h,s,v] format.
-def check_sat_and_bright(hsv_color):
-    # Edge case, don't do this for values of [-1, -1.0, -1.0 ]
-    if hsv_color[0] == -1:
-        return
-
-    # Check and normalize saturation.
-    if hsv_color[1] < const.SATURATION_RANGE[0]:
-        hsv_color[1] = random.uniform(const.SATURATION_RANGE[0], const.SATURATION_RANGE[0]+5)
-
-    # Check and normalize brightness value.
-    if hsv_color[2] < const.BRIGHTNESS_RANGE[0]:
-        hsv_color[2] = random.uniform(const.BRIGHTNESS_RANGE[0], const.BRIGHTNESS_RANGE[0]+5)
+        light_percent = (light_color[2] - const.LIGHT_BRIGHTNESS_RANGE[0]) / (const.LIGHT_BRIGHTNESS_RANGE[1] - const.LIGHT_BRIGHTNESS_RANGE[0])
+        dark_percent = (dark_color[2] - const.DARK_BRIGHTNESS_RANGE[0]) / (const.DARK_BRIGHTNESS_RANGE[1] - const.DARK_BRIGHTNESS_RANGE[0])
+        avg_light_dark_brightness = (light_percent + dark_percent) / 2
+        norm_color[2] = const.NORM_BRIGHTNESS_RANGE[0] + (
+                (const.NORM_BRIGHTNESS_RANGE[1] - const.NORM_BRIGHTNESS_RANGE[0]) * avg_light_dark_brightness)
 
 
 # **************************************************************************
 # **************************************************************************
 
 ##  Calculates the centroid for a color type.
 #   @details    The centroid is basically the average color of
```

### Comparing `pypalex-1.3.4/pypalex/file_utils.py` & `pypalex-1.3.5/pypalex/file_utils.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.4/pypalex/image_utils.py` & `pypalex-1.3.5/pypalex/image_utils.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.4/pypalex/print_utils.py` & `pypalex-1.3.5/pypalex/print_utils.py`

 * *Files identical despite different names*

### Comparing `pypalex-1.3.4/pypalex/settings.py` & `pypalex-1.3.5/pypalex/settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,20 +10,21 @@
 #   - Created by Al Timofeyev on March 2, 2022
 #   - Modified by Al Timofeyev on April 21, 2022.
 #   - Modified by Al Timofeyev on March 11, 2023.
 #   - Modified by Al Timofeyev on March 22, 2023.
 #   - Modified by Al Timofeyev on March 26, 2023.
 #   - Modified by Al Timofeyev on April 7, 2023.
 #   - Modified by Al Timofeyev on May 16, 2024.
+#   - Modified by Al Timofeyev on May 31, 2024.
 
 
 import os
 import platform
 
-__version__ = "1.3.4"
+__version__ = "1.3.5"
 __cache_version__ = "1.0.0"
 
 HOME = os.getenv("HOME", os.getenv("USERPROFILE"))
 XDG_CACHE_DIR = os.getenv("XDG_CACHE_HOME", os.path.join(HOME, ".cache"))
 XDG_CONF_DIR = os.getenv("XDG_CONFIG_HOME", os.path.join(HOME, ".config"))
 
 # NOTE: CONF_DIR will just be the place where PyPalEx saves color palettes
```

### Comparing `pypalex-1.3.4/pypalex.egg-info/PKG-INFO` & `pypalex-1.3.5/pypalex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pypalex
-Version: 1.3.4
+Version: 1.3.5
 Summary: Python Palette Extractor: extracts color palettes from images into json files.
 Home-page: https://github.com/AlTimofeyev/pypalex
 Author: Al Timofeyev
 Author-email: al.timofeyev@outlook.com
 License: MIT
-Download-URL: https://github.com/AlTimofeyev/pypalex/archive/1.3.4.tar.gz
+Download-URL: https://github.com/AlTimofeyev/pypalex/archive/1.3.5.tar.gz
 Keywords: python,pypalex,palex,color-palette,colorscheme,extract-colorscheme,extract-palette,extractor
 Platform: UNKNOWN
 Classifier: Environment :: X11 Applications
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: pypalex Version: 1.3.4 Summary: Python Palette
+Metadata-Version: 2.1 Name: pypalex Version: 1.3.5 Summary: Python Palette
 Extractor: extracts color palettes from images into json files. Home-page:
 https://github.com/AlTimofeyev/pypalex Author: Al Timofeyev Author-email:
 al.timofeyev@outlook.com License: MIT Download-URL: https://github.com/
-AlTimofeyev/pypalex/archive/1.3.4.tar.gz Keywords: python,pypalex,palex,color-
+AlTimofeyev/pypalex/archive/1.3.5.tar.gz Keywords: python,pypalex,palex,color-
 palette,colorscheme,extract-colorscheme,extract-palette,extractor Platform:
 UNKNOWN Classifier: Environment :: X11 Applications Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: MacOS Classifier:
 Operating System :: POSIX :: Linux Classifier: Operating System :: Microsoft ::
 Windows Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
```

### Comparing `pypalex-1.3.4/setup.py` & `pypalex-1.3.5/setup.py`

 * *Files identical despite different names*

