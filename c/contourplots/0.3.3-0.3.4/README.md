# Comparing `tmp/contourplots-0.3.3.tar.gz` & `tmp/contourplots-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\contourplots-0.3.3.tar", last modified: Fri May 31 05:08:06 2024, max compression
+gzip compressed data, was "dist\contourplots-0.3.4.tar", last modified: Sat Jun  1 19:10:03 2024, max compression
```

## Comparing `contourplots-0.3.3.tar` & `contourplots-0.3.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 05:08:06.000000 contourplots-0.3.3/
--rw-rw-rw-   0        0        0     1986 2022-11-13 16:15:08.000000 contourplots-0.3.3/LICENSE.txt
--rw-rw-rw-   0        0        0      608 2024-05-31 05:08:06.000000 contourplots-0.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      107 2022-11-13 16:29:55.000000 contourplots-0.3.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 05:08:06.000000 contourplots-0.3.3/contourplots/
--rw-rw-rw-   0        0        0      892 2024-05-31 05:07:58.000000 contourplots-0.3.3/contourplots/__init__.py
--rw-rw-rw-   0        0        0    66631 2024-05-31 04:31:15.000000 contourplots-0.3.3/contourplots/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 05:08:06.000000 contourplots-0.3.3/contourplots.egg-info/
--rw-rw-rw-   0        0        0      608 2024-05-31 05:08:06.000000 contourplots-0.3.3/contourplots.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      256 2024-05-31 05:08:06.000000 contourplots-0.3.3/contourplots.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 05:08:06.000000 contourplots-0.3.3/contourplots.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2024-05-31 05:08:06.000000 contourplots-0.3.3/contourplots.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 05:08:06.000000 contourplots-0.3.3/contourplots.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 05:08:06.000000 contourplots-0.3.3/setup.cfg
--rw-rw-rw-   0        0        0     1003 2024-05-31 05:08:02.000000 contourplots-0.3.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 19:10:03.000000 contourplots-0.3.4/
+-rw-rw-rw-   0        0        0     1986 2022-11-13 16:15:08.000000 contourplots-0.3.4/LICENSE.txt
+-rw-rw-rw-   0        0        0      608 2024-06-01 19:10:03.000000 contourplots-0.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      107 2022-11-13 16:29:55.000000 contourplots-0.3.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 19:10:03.000000 contourplots-0.3.4/contourplots/
+-rw-rw-rw-   0        0        0      892 2024-06-01 19:08:56.000000 contourplots-0.3.4/contourplots/__init__.py
+-rw-rw-rw-   0        0        0    66689 2024-06-01 19:07:46.000000 contourplots-0.3.4/contourplots/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 19:10:03.000000 contourplots-0.3.4/contourplots.egg-info/
+-rw-rw-rw-   0        0        0      608 2024-06-01 19:10:03.000000 contourplots-0.3.4/contourplots.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      256 2024-06-01 19:10:03.000000 contourplots-0.3.4/contourplots.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 19:10:03.000000 contourplots-0.3.4/contourplots.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2024-06-01 19:10:03.000000 contourplots-0.3.4/contourplots.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-01 19:10:03.000000 contourplots-0.3.4/contourplots.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 19:10:03.000000 contourplots-0.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     1003 2024-06-01 19:09:58.000000 contourplots-0.3.4/setup.py
```

### Comparing `contourplots-0.3.3/LICENSE.txt` & `contourplots-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `contourplots-0.3.3/PKG-INFO` & `contourplots-0.3.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contourplots
-Version: 0.3.3
+Version: 0.3.4
 Summary: A toolkit for generating multi-dimensional plots easily, usefully, and legibly.
 Home-page: https://github.com/sarangbhagwat/contourplots
 Author: Sarang S. Bhagwat
 Author-email: sarang.bhagwat.git@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `contourplots-0.3.3/contourplots/__init__.py` & `contourplots-0.3.4/contourplots/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # ContourPlots: A toolkit for generating multi-dimensional plots easily, usefully, and legibly.
 # Copyright (C) 2022-2023, Sarang Bhagwat <sarang.bhagwat.git@gmail.com>
 # 
 # This module is under the MIT open-source license. See 
 # https://github.com/sarangbhagwat/contourplots/blob/main/LICENSE
 # for license details.
 
-__version__ = '0.3.3'
+__version__ = '0.3.4'
 __author__ = 'Sarang S. Bhagwat'
 
 # %% Initialize ContourPlots 
 
 from . import utils
 
 animated_contourplot = utils.animated_contourplot
```

### Comparing `contourplots-0.3.3/contourplots/utils.py` & `contourplots-0.3.4/contourplots/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -455,14 +455,16 @@
         ax.set_xlabel(x_label + units_opening_brackets[0] + x_units + "]", 
                       fontsize=axis_title_fonts['size']['x'],
                       **fontname)
         
         ax.set_xticks(x_ticks)
         ax.set_yticks(y_ticks)
         
+        plt.rcParams["axes.axisbelow"] = False
+        
         if not contourplot_facecolor.all()==None:
             ax.set_facecolor(contourplot_facecolor)
         
         if text_boxes:
             text_boxes_keys = list(text_boxes.keys())
             for i in text_boxes_keys:
                 (xpos, ypos), textcolor = text_boxes[i]
```

### Comparing `contourplots-0.3.3/contourplots.egg-info/PKG-INFO` & `contourplots-0.3.4/contourplots.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contourplots
-Version: 0.3.3
+Version: 0.3.4
 Summary: A toolkit for generating multi-dimensional plots easily, usefully, and legibly.
 Home-page: https://github.com/sarangbhagwat/contourplots
 Author: Sarang S. Bhagwat
 Author-email: sarang.bhagwat.git@gmail.com
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `contourplots-0.3.3/setup.py` & `contourplots-0.3.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 
 from setuptools import setup
 
 setup(
     name='contourplots',
     packages=['contourplots'],
-    version='0.3.3',    
+    version='0.3.4',    
     description='A toolkit for generating multi-dimensional plots easily, usefully, and legibly.',
     url='https://github.com/sarangbhagwat/contourplots',
     author='Sarang S. Bhagwat',
     author_email='sarang.bhagwat.git@gmail.com',
     license='MIT',
     # packages=['contourplots'],
     install_requires=['matplotlib==3.5.2',
```

