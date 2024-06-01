# Comparing `tmp/simple_space-0.9.0.tar.gz` & `tmp/simple_space-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_space-0.9.0.tar", last modified: Fri May 31 18:38:52 2024, max compression
+gzip compressed data, was "simple_space-1.0.0.tar", last modified: Sat Jun  1 08:49:36 2024, max compression
```

## Comparing `simple_space-0.9.0.tar` & `simple_space-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,25 @@
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-31 18:38:52.125286 simple_space-0.9.0/
--rw-rw-r--   0 user      (1000) user      (1000)     1062 2024-05-30 00:58:34.000000 simple_space-0.9.0/LICENSE
--rw-r--r--   0 user      (1000) user      (1000)    11079 2024-05-31 18:38:52.125286 simple_space-0.9.0/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)    10006 2024-05-30 19:17:31.000000 simple_space-0.9.0/README.md
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-31 18:38:52.121286 simple_space-0.9.0/SimpleS/
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-31 18:38:52.121286 simple_space-0.9.0/SimpleS/ImageRelated/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:36.000000 simple_space-0.9.0/SimpleS/ImageRelated/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     9535 2024-05-31 18:18:31.000000 simple_space-0.9.0/SimpleS/ImageRelated/basics.py
--rw-r--r--   0 user      (1000) user      (1000)     4425 2024-05-31 18:38:19.000000 simple_space-0.9.0/SimpleS/ImageRelated/enhancements.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-31 18:38:52.125286 simple_space-0.9.0/SimpleS/Points/
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:29.000000 simple_space-0.9.0/SimpleS/Points/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     4751 2024-05-31 18:21:41.000000 simple_space-0.9.0/SimpleS/Points/dim2.py
--rw-rw-r--   0 user      (1000) user      (1000)     8703 2024-05-31 18:21:04.000000 simple_space-0.9.0/SimpleS/Points/dim3.py
--rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 22:02:16.000000 simple_space-0.9.0/SimpleS/__init__.py
--rw-rw-r--   0 user      (1000) user      (1000)     1476 2024-05-31 18:22:46.000000 simple_space-0.9.0/SimpleS/utils.py
-drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-05-31 18:38:52.125286 simple_space-0.9.0/Simple_Space.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)    11079 2024-05-31 18:38:52.000000 simple_space-0.9.0/Simple_Space.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1000) user      (1000)      422 2024-05-31 18:38:52.000000 simple_space-0.9.0/Simple_Space.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1000) user      (1000)        1 2024-05-31 18:38:52.000000 simple_space-0.9.0/Simple_Space.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1000) user      (1000)       57 2024-05-31 18:38:52.000000 simple_space-0.9.0/Simple_Space.egg-info/requires.txt
--rw-rw-r--   0 user      (1000) user      (1000)        8 2024-05-31 18:38:52.000000 simple_space-0.9.0/Simple_Space.egg-info/top_level.txt
--rw-rw-r--   0 user      (1000) user      (1000)     1082 2024-05-31 18:38:45.000000 simple_space-0.9.0/pyproject.toml
--rw-rw-r--   0 user      (1000) user      (1000)       38 2024-05-31 18:38:52.125286 simple_space-0.9.0/setup.cfg
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-06-01 08:49:36.876934 simple_space-1.0.0/
+-rw-rw-r--   0 user      (1000) user      (1000)     1062 2024-05-30 00:58:34.000000 simple_space-1.0.0/LICENSE
+-rw-r--r--   0 user      (1000) user      (1000)    11235 2024-06-01 08:49:36.876934 simple_space-1.0.0/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)    10162 2024-06-01 07:21:16.000000 simple_space-1.0.0/README.md
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-06-01 08:49:36.876934 simple_space-1.0.0/SimpleS/
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-06-01 08:49:36.876934 simple_space-1.0.0/SimpleS/ImageRelated/
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:36.000000 simple_space-1.0.0/SimpleS/ImageRelated/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)    10405 2024-06-01 08:46:42.000000 simple_space-1.0.0/SimpleS/ImageRelated/basics.py
+-rw-r--r--   0 user      (1000) user      (1000)     4425 2024-05-31 18:38:19.000000 simple_space-1.0.0/SimpleS/ImageRelated/enhancements.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-06-01 08:49:36.876934 simple_space-1.0.0/SimpleS/Points/
+-rw-rw-r--   0 user      (1000) user      (1000)    10560 2024-06-01 08:43:06.000000 simple_space-1.0.0/SimpleS/Points/Circle.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4137 2024-06-01 08:43:22.000000 simple_space-1.0.0/SimpleS/Points/Line.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 07:48:29.000000 simple_space-1.0.0/SimpleS/Points/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     4751 2024-05-31 18:21:41.000000 simple_space-1.0.0/SimpleS/Points/dim2.py
+-rw-rw-r--   0 user      (1000) user      (1000)     7887 2024-06-01 08:46:46.000000 simple_space-1.0.0/SimpleS/Points/dim3.py
+-rw-rw-r--   0 user      (1000) user      (1000)        0 2024-05-30 22:02:16.000000 simple_space-1.0.0/SimpleS/__init__.py
+-rw-rw-r--   0 user      (1000) user      (1000)     1476 2024-05-31 18:22:46.000000 simple_space-1.0.0/SimpleS/utils.py
+drwxrwxr-x   0 user      (1000) user      (1000)        0 2024-06-01 08:49:36.876934 simple_space-1.0.0/Simple_Space.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)    11235 2024-06-01 08:49:36.000000 simple_space-1.0.0/Simple_Space.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1000) user      (1000)      470 2024-06-01 08:49:36.000000 simple_space-1.0.0/Simple_Space.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        1 2024-06-01 08:49:36.000000 simple_space-1.0.0/Simple_Space.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1000) user      (1000)       57 2024-06-01 08:49:36.000000 simple_space-1.0.0/Simple_Space.egg-info/requires.txt
+-rw-rw-r--   0 user      (1000) user      (1000)        8 2024-06-01 08:49:36.000000 simple_space-1.0.0/Simple_Space.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1000) user      (1000)     1082 2024-06-01 08:49:22.000000 simple_space-1.0.0/pyproject.toml
+-rw-rw-r--   0 user      (1000) user      (1000)       38 2024-06-01 08:49:36.876934 simple_space-1.0.0/setup.cfg
```

### Comparing `simple_space-0.9.0/LICENSE` & `simple_space-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_space-0.9.0/PKG-INFO` & `simple_space-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Space
-Version: 0.9.0
+Version: 1.0.0
 Summary: A Try at Better Understanding Space.
 Author-email: Hamed Hajipour <cloner174.org@gmail.com>
 Project-URL: Homepage, https://github.com/cloner174/Simple-Space
 Project-URL: Documentation, https://github.com/cloner174/Simple-Space#readme
 Project-URL: Repository, https://github.com/cloner174/Simple-Space.git
 Project-URL: Issues, https://github.com/cloner174/Simple-Space/issues
 Classifier: Programming Language :: Python :: 3.6
@@ -30,15 +30,16 @@
 
 ### Table of Contents
 
 - [Installation](#installation)
 - [Structure](#structure)
 - [Submodules](#submodules)
 + Points
-  - [dim3](#dim3)
+  - [dim3 Module](#dim3-module)
+  - dim2 Module
 + ImageRelated
   - [enhancements.py](#imagerelated-scripts--enhancementspy)
   - [basics.py](#imagerelated-scripts--basicspy)
 - [License](#license)
 - [Contact](#contact)
 
 ## Installation
@@ -55,76 +56,76 @@
 simple-space/
 │
 ├── SimpleS/
 │   ├── __init__.py
 │   ├── utils.py
 │   └── Points/
 │       ├── __init__.py
-│       ├── dimentions.py
+│       ├── dim3.py
+│       ├── dim2.py
 │   └── ImageRelated/
 │       ├── __init__.py
 │       ├── enhancements.py
 │       └── basics.py
 ├── README.md
 ├── LICENSE
 └── pyproject.toml
 ```
 ## Submodules
 1. Points
 
     - dim3.py:
-     Contains functions for 3D point data processing and visualization.
+     Contains basic functions for 3D point data processing and visualization.
     - dim2.py:
-     Contains some simple and basic functions for 2D point data processing and visualization.
+     Contains basic functions for 2D point data processing and visualization.
 2. ImageRelated
 
     - enhancements.py: Provides functions for image enhancement, including erosion and dilation.
     - basics.py: Contains basic image processing utilities like edge detection and color inversion.
 
-## dim3
+## dim3 Module
 
-The dim3 script offers tools for visualizing and processing 3D point data in Python, using libraries such as numpy, matplotlib, and scipy.
+The dim3 module offers tools for visualizing and processing 3D point data in Python, using libraries such as numpy, matplotlib, and scipy.
 
 ### Features
 
 - **Rotate 3D Points:** Rotate points around a specified axis by a given angle in degrees.
 - **Plot 3D Points/Mesh:** Visualize 3D points or a mesh, with customizable visual attributes.
 - **Create Grayscale Image from 3D Points:** Project 3D points onto a 2D plane using the z-coordinate for intensity.
 - **Fill Points in Binary Image:** Use morphological dilation to fill gaps in binary images.
 
 ### Usage
 
-#### Initializing the Class
+#### Importing
 
 ```python
 
 from SimpleS.Points import dim3
-
 ```
 ```python
 # But I recommend You Simply Use this one:
 
 from SimpleS.Points.dim3 import *
 
-# This one Lets you use all the functions inside dim3 script without any initialize word;
+# This one Lets you use all the functions inside dim3 module without any initialize word;
 # FOR EXAMPLE:
 
 dim3.rotate_points()
 
 # WOULD BE JUST:
 
-rotate_points()
+rotate_3d_points()
 ```
 **If you encounter any trouble determining the specifics of an import, such as which functions it includes, simply use the dir() function:**
 ```python
 from SimpleS.Points import dim3
 
-dir(dim3)
+dir(Dim3)
 ```
-This will show you the names of all functions inside the dim3 script.
+This will show you the names of all functions inside the dim3 module.
 
 After that, we will return to our simpler method:
 
 ```python
 from SimpleS.Points.dim3 import *
 ```
 
@@ -149,15 +150,15 @@
 
 
 #### Filling Points in a Binary Image
 
 ```python
 filled_image = fill_points(binary_image)
 ```
-For more detailed information on each method, please refer to the inline documentation within the class methods.
+For more detailed information on each method, please refer to the inline documentation within the module methods.
 
 
 ## ImageRelated Scripts : enhancements.py
 
 ### Introduction
 This Python script, titled "enhancements", is an enhanced version of the original image processing examples provided by OpenCV. It includes functionalities for applying erosion and dilatation transformations to images. This script can be used for educational purposes or integrated into larger image processing projects.
 
@@ -172,15 +173,15 @@
 
 ### Usage
 
 To use this script, you need to create an instance of the ErosAndDilat class with either a path to an image file or an image object. Here's a quick example on how to use the class:
 
 ```python
 
-from SimpleS.enhancements import ErosAndDilat
+from SimpleS.ImageRelated.enhancements import ErosAndDilat
 
 # Initialize with an image path
 image_processor = ErosAndDilat('path/to/your/image.jpg')
 
 # Perform erosion and dilatation, display results, and save them
 image_processor.main(eros=True, dilate=True, show=True, save=True)
 ```
@@ -214,23 +215,23 @@
     - save_path (optional): Directory to save the result.
     - file_name (optional): Name of the saved file.
 
 - Example:
 
 ```python
 
-from SimpleS import basics
+from SimpleS.ImageRelated import basics
 
 # Or :
 
-from SimpleS.basics import invert_image_color
+from SimpleS.ImageRelated.basics import invert_image_color
 
 #Or:
 
-from SimpleS.basics import * # Access to all
+from SimpleS.ImageRelated.basics import * # Access to all
 
 ```
 
 #### show_image
 
 - Displays an image using matplotlib.
 - Parameters:
@@ -242,15 +243,15 @@
     - save (optional): Whether to save the result.
     - save_path (optional): Directory to save the result.
     - file_name (optional): Name of the saved file.
 
 - Example:
 
 ```python
-from SimpleS.basics import *
+from SimpleS.ImageRelated.basics import *
 
 show_image('path_to_image.png', title="Example Image", save=True, save_path='./', file_name='example_image.png')
 ```
 
 #### fill_shape
 
 - Fills an area of a shape in an image based on the points defining the edges of the shape.
@@ -259,30 +260,30 @@
     - image: The image where the shape is to be filled.
     - points: A list of (x, y) tuples defining the vertices of the shape.
     - color: A tuple defining the color to fill the shape.
 
 - Example:
 
 ```python
-from SimpleS.basics import *
+from SimpleS.ImageRelated.basics import *
 
 filled_image = fill_shape(image, points, color=(255, 0, 0))
 ```
 
 #### force_image_to_GRAYSCALE
 
 + Converts a color image to grayscale.
 + Parameters:
 
     - image: The color image.
 
 + Example:
 
 ```python
-from SimpleS.basics import *
+from SimpleS.ImageRelated.basics import *
 
 grayscale_image = force_image_to_GRAYSCALE(color_image)
 ```
 
 #### read_image_in_grayscale
 
 + Reads an image in grayscale mode and optionally converts it to binary.
@@ -293,15 +294,15 @@
     + type (optional): Thresholding type.
     + also_make_it_binary (optional): Whether to convert to binary.
     + binary_image_color (optional): Color for binary conversion.
 
 + Example:
 
 ```python
-from SimpleS.basics import *
+from SimpleS.ImageRelated.basics import *
 
 binary_image = read_image_in_grayscale('path_to_image.png', thrhold=127, type='THRESH_BINARY', also_make_it_binary=True)
 ```
 #### simple_binary_image_creator
 
 + Creates a binary image from a list of points.
 + Parameters:
@@ -313,15 +314,15 @@
     + enlarge_points (optional): Whether to enlarge points.
     + smoothing (optional): Whether to apply Gaussian blur.
 
 + Example:
 
 ```python
 
-from SimpleS.basics import *
+from SimpleS.ImageRelated.basics import *
 
 binary_image = simple_binary_image_creator(points, image_size=(100, 100))
 ```
 #### advance_binary_image_creator
 
 + Creates an advanced binary image from a list of points.
 + Parameters:
```

### Comparing `simple_space-0.9.0/README.md` & `simple_space-1.0.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 
 ### Table of Contents
 
 - [Installation](#installation)
 - [Structure](#structure)
 - [Submodules](#submodules)
 + Points
-  - [dim3](#dim3)
+  - [dim3 Module](#dim3-module)
+  - dim2 Module
 + ImageRelated
   - [enhancements.py](#imagerelated-scripts--enhancementspy)
   - [basics.py](#imagerelated-scripts--basicspy)
 - [License](#license)
 - [Contact](#contact)
 
 ## Installation
@@ -28,76 +29,76 @@
 simple-space/
 │
 ├── SimpleS/
 │   ├── __init__.py
 │   ├── utils.py
 │   └── Points/
 │       ├── __init__.py
-│       ├── dimentions.py
+│       ├── dim3.py
+│       ├── dim2.py
 │   └── ImageRelated/
 │       ├── __init__.py
 │       ├── enhancements.py
 │       └── basics.py
 ├── README.md
 ├── LICENSE
 └── pyproject.toml
 ```
 ## Submodules
 1. Points
 
     - dim3.py:
-     Contains functions for 3D point data processing and visualization.
+     Contains basic functions for 3D point data processing and visualization.
     - dim2.py:
-     Contains some simple and basic functions for 2D point data processing and visualization.
+     Contains basic functions for 2D point data processing and visualization.
 2. ImageRelated
 
     - enhancements.py: Provides functions for image enhancement, including erosion and dilation.
     - basics.py: Contains basic image processing utilities like edge detection and color inversion.
 
-## dim3
+## dim3 Module
 
-The dim3 script offers tools for visualizing and processing 3D point data in Python, using libraries such as numpy, matplotlib, and scipy.
+The dim3 module offers tools for visualizing and processing 3D point data in Python, using libraries such as numpy, matplotlib, and scipy.
 
 ### Features
 
 - **Rotate 3D Points:** Rotate points around a specified axis by a given angle in degrees.
 - **Plot 3D Points/Mesh:** Visualize 3D points or a mesh, with customizable visual attributes.
 - **Create Grayscale Image from 3D Points:** Project 3D points onto a 2D plane using the z-coordinate for intensity.
 - **Fill Points in Binary Image:** Use morphological dilation to fill gaps in binary images.
 
 ### Usage
 
-#### Initializing the Class
+#### Importing
 
 ```python
 
 from SimpleS.Points import dim3
-
 ```
 ```python
 # But I recommend You Simply Use this one:
 
 from SimpleS.Points.dim3 import *
 
-# This one Lets you use all the functions inside dim3 script without any initialize word;
+# This one Lets you use all the functions inside dim3 module without any initialize word;
 # FOR EXAMPLE:
 
 dim3.rotate_points()
 
 # WOULD BE JUST:
 
-rotate_points()
+rotate_3d_points()
 ```
 **If you encounter any trouble determining the specifics of an import, such as which functions it includes, simply use the dir() function:**
 ```python
 from SimpleS.Points import dim3
 
-dir(dim3)
+dir(Dim3)
 ```
-This will show you the names of all functions inside the dim3 script.
+This will show you the names of all functions inside the dim3 module.
 
 After that, we will return to our simpler method:
 
 ```python
 from SimpleS.Points.dim3 import *
 ```
 
@@ -122,15 +123,15 @@
 
 
 #### Filling Points in a Binary Image
 
 ```python
 filled_image = fill_points(binary_image)
 ```
-For more detailed information on each method, please refer to the inline documentation within the class methods.
+For more detailed information on each method, please refer to the inline documentation within the module methods.
 
 
 ## ImageRelated Scripts : enhancements.py
 
 ### Introduction
 This Python script, titled "enhancements", is an enhanced version of the original image processing examples provided by OpenCV. It includes functionalities for applying erosion and dilatation transformations to images. This script can be used for educational purposes or integrated into larger image processing projects.
 
@@ -145,15 +146,15 @@
 
 ### Usage
 
 To use this script, you need to create an instance of the ErosAndDilat class with either a path to an image file or an image object. Here's a quick example on how to use the class:
 
 ```python
 
-from SimpleS.enhancements import ErosAndDilat
+from SimpleS.ImageRelated.enhancements import ErosAndDilat
 
 # Initialize with an image path
 image_processor = ErosAndDilat('path/to/your/image.jpg')
 
 # Perform erosion and dilatation, display results, and save them
 image_processor.main(eros=True, dilate=True, show=True, save=True)
 ```
@@ -187,23 +188,23 @@
     - save_path (optional): Directory to save the result.
     - file_name (optional): Name of the saved file.
 
 - Example:
 
 ```python
 
-from SimpleS import basics
+from SimpleS.ImageRelated import basics
 
 # Or :
 
-from SimpleS.basics import invert_image_color
+from SimpleS.ImageRelated.basics import invert_image_color
 
 #Or:
 
-from SimpleS.basics import * # Access to all
+from SimpleS.ImageRelated.basics import * # Access to all
 
 ```
 
 #### show_image
 
 - Displays an image using matplotlib.
 - Parameters:
@@ -215,15 +216,15 @@
     - save (optional): Whether to save the result.
     - save_path (optional): Directory to save the result.
     - file_name (optional): Name of the saved file.
 
 - Example:
 
 ```python
-from SimpleS.basics import *
+from SimpleS.ImageRelated.basics import *
 
 show_image('path_to_image.png', title="Example Image", save=True, save_path='./', file_name='example_image.png')
 ```
 
 #### fill_shape
 
 - Fills an area of a shape in an image based on the points defining the edges of the shape.
@@ -232,30 +233,30 @@
     - image: The image where the shape is to be filled.
     - points: A list of (x, y) tuples defining the vertices of the shape.
     - color: A tuple defining the color to fill the shape.
 
 - Example:
 
 ```python
-from SimpleS.basics import *
+from SimpleS.ImageRelated.basics import *
 
 filled_image = fill_shape(image, points, color=(255, 0, 0))
 ```
 
 #### force_image_to_GRAYSCALE
 
 + Converts a color image to grayscale.
 + Parameters:
 
     - image: The color image.
 
 + Example:
 
 ```python
-from SimpleS.basics import *
+from SimpleS.ImageRelated.basics import *
 
 grayscale_image = force_image_to_GRAYSCALE(color_image)
 ```
 
 #### read_image_in_grayscale
 
 + Reads an image in grayscale mode and optionally converts it to binary.
@@ -266,15 +267,15 @@
     + type (optional): Thresholding type.
     + also_make_it_binary (optional): Whether to convert to binary.
     + binary_image_color (optional): Color for binary conversion.
 
 + Example:
 
 ```python
-from SimpleS.basics import *
+from SimpleS.ImageRelated.basics import *
 
 binary_image = read_image_in_grayscale('path_to_image.png', thrhold=127, type='THRESH_BINARY', also_make_it_binary=True)
 ```
 #### simple_binary_image_creator
 
 + Creates a binary image from a list of points.
 + Parameters:
@@ -286,15 +287,15 @@
     + enlarge_points (optional): Whether to enlarge points.
     + smoothing (optional): Whether to apply Gaussian blur.
 
 + Example:
 
 ```python
 
-from SimpleS.basics import *
+from SimpleS.ImageRelated.basics import *
 
 binary_image = simple_binary_image_creator(points, image_size=(100, 100))
 ```
 #### advance_binary_image_creator
 
 + Creates an advanced binary image from a list of points.
 + Parameters:
```

### Comparing `simple_space-0.9.0/SimpleS/ImageRelated/basics.py` & `simple_space-1.0.0/SimpleS/ImageRelated/basics.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import tempfile
 import numpy as np
 from skimage import draw
 import scipy.ndimage as ndi
 import matplotlib.pyplot as plt
 from PIL import Image, ImageDraw
 from SimpleS.utils import save_path_generator
+from scipy.ndimage import binary_dilation
 
 
 
 def invert_image_color(image, save = False, save_path = None, file_name = None):
     
     if isinstance(image, str):
         with Image.open(image) as img:
@@ -67,14 +68,32 @@
         path_to_save = save_path_generator(file_name,save_path,flag=None )
         plt.imsave(path_to_save, image, cmap=c_map)
     plt.imshow(image, cmap=c_map, interpolation=interpolation)
     
     plt.show()
 
 
+def fill_inside_3d_image(image, iterations=5, structure=None, structure_like = (3,3) , save = False, save_path = None, file_name = None):
+        """Fill in the gaps in a binary image using morphological dilation."""
+        if structure is None:
+                structure = np.ones(structure_like)
+        try:
+                filled_image = binary_dilation(image, structure=structure, iterations=iterations)
+        except Exception as e:
+                try:
+                        filled_image = binary_dilation(image, structure=(3,3,3), iterations=iterations)
+                except:
+                        raise ValueError(f"{e}")
+        if save:
+                path_to_save = save_path_generator(file_name, save_path, flag=None)
+                plt.imsave(path_to_save, image )
+        
+        return filled_image
+
+
 def fill_shape_in_image(image, points, color = (255, 0, 0)):
     """
     Fill an area of a shape in an image based on the points defining the edges of the shape.
     Parameters:
     image (numpy.ndarray): The image where the shape is to be filled.
     points (list of tuples): A list of (x, y) tuples defining the vertices of the shape.
     color (tuple): A tuple defining the color to fill the shape. For grayscale, use one value; for color, use (B, G, R).
```

### Comparing `simple_space-0.9.0/SimpleS/ImageRelated/enhancements.py` & `simple_space-1.0.0/SimpleS/ImageRelated/enhancements.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.9.0/SimpleS/Points/dim2.py` & `simple_space-1.0.0/SimpleS/Points/dim2.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.9.0/SimpleS/Points/dim3.py` & `simple_space-1.0.0/SimpleS/Points/dim3.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import numpy as np
 import matplotlib.pyplot as plt
 from mpl_toolkits.mplot3d.art3d import Poly3DCollection
-from scipy.ndimage import binary_dilation
 from SimpleS.utils import save_path_generator
 
 
 
 def read_off_file(file_path):
         """ It will return 2Object  Vertices  and  Faces. """
         with open(file_path, 'r') as file:
@@ -135,33 +134,15 @@
         for (point, intensity) in zip(scaled_points.astype(int), z_scaled.astype(np.uint8)):
                 current_intensity = image[point[1], point[0]]
                 image[point[1], point[0]] = max(current_intensity, intensity)  # Use the maximum intensity if overlapping
         if save:
                 path_to_save = save_path_generator(file_name,save_path, flag=None)
                 plt.imsave(path_to_save, image )
         return image
-    
-    
 
-def fill_inside_3d_points(image, iterations=5, structure=None, structure_like = (3,3) , save = False, save_path = None, file_name = None):
-        """Fill in the gaps in a binary image using morphological dilation."""
-        if structure is None:
-                structure = np.ones(structure_like)
-        try:
-                filled_image = binary_dilation(image, structure=structure, iterations=iterations)
-        except Exception as e:
-                try:
-                        filled_image = binary_dilation(image, structure=(3,3,3), iterations=iterations)
-                except:
-                        raise ValueError(f"{e}")
-        if save:
-                save_path_generator(file_name, save_path, flag=None)
-        return filled_image
-    
-    
 
 def plot_3d_points(points, title = '3D Points Plot', labels = 'on', elev=None, azim=None,save = False,save_path=None, file_name = None):
         """
         Plot and optionally save a 3D plot of points with specified view angles.
         Args:
         - points (array-like): A list or array of points where each point is a list or tuple of three floats (x, y, z).
         - save_path (str, optional): Path to save the plot image. If None, the plot will not be saved.
```

### Comparing `simple_space-0.9.0/SimpleS/utils.py` & `simple_space-1.0.0/SimpleS/utils.py`

 * *Files identical despite different names*

### Comparing `simple_space-0.9.0/Simple_Space.egg-info/PKG-INFO` & `simple_space-1.0.0/Simple_Space.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Simple-Space
-Version: 0.9.0
+Version: 1.0.0
 Summary: A Try at Better Understanding Space.
 Author-email: Hamed Hajipour <cloner174.org@gmail.com>
 Project-URL: Homepage, https://github.com/cloner174/Simple-Space
 Project-URL: Documentation, https://github.com/cloner174/Simple-Space#readme
 Project-URL: Repository, https://github.com/cloner174/Simple-Space.git
 Project-URL: Issues, https://github.com/cloner174/Simple-Space/issues
 Classifier: Programming Language :: Python :: 3.6
@@ -30,15 +30,16 @@
 
 ### Table of Contents
 
 - [Installation](#installation)
 - [Structure](#structure)
 - [Submodules](#submodules)
 + Points
-  - [dim3](#dim3)
+  - [dim3 Module](#dim3-module)
+  - dim2 Module
 + ImageRelated
   - [enhancements.py](#imagerelated-scripts--enhancementspy)
   - [basics.py](#imagerelated-scripts--basicspy)
 - [License](#license)
 - [Contact](#contact)
 
 ## Installation
@@ -55,76 +56,76 @@
 simple-space/
 │
 ├── SimpleS/
 │   ├── __init__.py
 │   ├── utils.py
 │   └── Points/
 │       ├── __init__.py
-│       ├── dimentions.py
+│       ├── dim3.py
+│       ├── dim2.py
 │   └── ImageRelated/
 │       ├── __init__.py
 │       ├── enhancements.py
 │       └── basics.py
 ├── README.md
 ├── LICENSE
 └── pyproject.toml
 ```
 ## Submodules
 1. Points
 
     - dim3.py:
-     Contains functions for 3D point data processing and visualization.
+     Contains basic functions for 3D point data processing and visualization.
     - dim2.py:
-     Contains some simple and basic functions for 2D point data processing and visualization.
+     Contains basic functions for 2D point data processing and visualization.
 2. ImageRelated
 
     - enhancements.py: Provides functions for image enhancement, including erosion and dilation.
     - basics.py: Contains basic image processing utilities like edge detection and color inversion.
 
-## dim3
+## dim3 Module
 
-The dim3 script offers tools for visualizing and processing 3D point data in Python, using libraries such as numpy, matplotlib, and scipy.
+The dim3 module offers tools for visualizing and processing 3D point data in Python, using libraries such as numpy, matplotlib, and scipy.
 
 ### Features
 
 - **Rotate 3D Points:** Rotate points around a specified axis by a given angle in degrees.
 - **Plot 3D Points/Mesh:** Visualize 3D points or a mesh, with customizable visual attributes.
 - **Create Grayscale Image from 3D Points:** Project 3D points onto a 2D plane using the z-coordinate for intensity.
 - **Fill Points in Binary Image:** Use morphological dilation to fill gaps in binary images.
 
 ### Usage
 
-#### Initializing the Class
+#### Importing
 
 ```python
 
 from SimpleS.Points import dim3
-
 ```
 ```python
 # But I recommend You Simply Use this one:
 
 from SimpleS.Points.dim3 import *
 
-# This one Lets you use all the functions inside dim3 script without any initialize word;
+# This one Lets you use all the functions inside dim3 module without any initialize word;
 # FOR EXAMPLE:
 
 dim3.rotate_points()
 
 # WOULD BE JUST:
 
-rotate_points()
+rotate_3d_points()
 ```
 **If you encounter any trouble determining the specifics of an import, such as which functions it includes, simply use the dir() function:**
 ```python
 from SimpleS.Points import dim3
 
-dir(dim3)
+dir(Dim3)
 ```
-This will show you the names of all functions inside the dim3 script.
+This will show you the names of all functions inside the dim3 module.
 
 After that, we will return to our simpler method:
 
 ```python
 from SimpleS.Points.dim3 import *
 ```
 
@@ -149,15 +150,15 @@
 
 
 #### Filling Points in a Binary Image
 
 ```python
 filled_image = fill_points(binary_image)
 ```
-For more detailed information on each method, please refer to the inline documentation within the class methods.
+For more detailed information on each method, please refer to the inline documentation within the module methods.
 
 
 ## ImageRelated Scripts : enhancements.py
 
 ### Introduction
 This Python script, titled "enhancements", is an enhanced version of the original image processing examples provided by OpenCV. It includes functionalities for applying erosion and dilatation transformations to images. This script can be used for educational purposes or integrated into larger image processing projects.
 
@@ -172,15 +173,15 @@
 
 ### Usage
 
 To use this script, you need to create an instance of the ErosAndDilat class with either a path to an image file or an image object. Here's a quick example on how to use the class:
 
 ```python
 
-from SimpleS.enhancements import ErosAndDilat
+from SimpleS.ImageRelated.enhancements import ErosAndDilat
 
 # Initialize with an image path
 image_processor = ErosAndDilat('path/to/your/image.jpg')
 
 # Perform erosion and dilatation, display results, and save them
 image_processor.main(eros=True, dilate=True, show=True, save=True)
 ```
@@ -214,23 +215,23 @@
     - save_path (optional): Directory to save the result.
     - file_name (optional): Name of the saved file.
 
 - Example:
 
 ```python
 
-from SimpleS import basics
+from SimpleS.ImageRelated import basics
 
 # Or :
 
-from SimpleS.basics import invert_image_color
+from SimpleS.ImageRelated.basics import invert_image_color
 
 #Or:
 
-from SimpleS.basics import * # Access to all
+from SimpleS.ImageRelated.basics import * # Access to all
 
 ```
 
 #### show_image
 
 - Displays an image using matplotlib.
 - Parameters:
@@ -242,15 +243,15 @@
     - save (optional): Whether to save the result.
     - save_path (optional): Directory to save the result.
     - file_name (optional): Name of the saved file.
 
 - Example:
 
 ```python
-from SimpleS.basics import *
+from SimpleS.ImageRelated.basics import *
 
 show_image('path_to_image.png', title="Example Image", save=True, save_path='./', file_name='example_image.png')
 ```
 
 #### fill_shape
 
 - Fills an area of a shape in an image based on the points defining the edges of the shape.
@@ -259,30 +260,30 @@
     - image: The image where the shape is to be filled.
     - points: A list of (x, y) tuples defining the vertices of the shape.
     - color: A tuple defining the color to fill the shape.
 
 - Example:
 
 ```python
-from SimpleS.basics import *
+from SimpleS.ImageRelated.basics import *
 
 filled_image = fill_shape(image, points, color=(255, 0, 0))
 ```
 
 #### force_image_to_GRAYSCALE
 
 + Converts a color image to grayscale.
 + Parameters:
 
     - image: The color image.
 
 + Example:
 
 ```python
-from SimpleS.basics import *
+from SimpleS.ImageRelated.basics import *
 
 grayscale_image = force_image_to_GRAYSCALE(color_image)
 ```
 
 #### read_image_in_grayscale
 
 + Reads an image in grayscale mode and optionally converts it to binary.
@@ -293,15 +294,15 @@
     + type (optional): Thresholding type.
     + also_make_it_binary (optional): Whether to convert to binary.
     + binary_image_color (optional): Color for binary conversion.
 
 + Example:
 
 ```python
-from SimpleS.basics import *
+from SimpleS.ImageRelated.basics import *
 
 binary_image = read_image_in_grayscale('path_to_image.png', thrhold=127, type='THRESH_BINARY', also_make_it_binary=True)
 ```
 #### simple_binary_image_creator
 
 + Creates a binary image from a list of points.
 + Parameters:
@@ -313,15 +314,15 @@
     + enlarge_points (optional): Whether to enlarge points.
     + smoothing (optional): Whether to apply Gaussian blur.
 
 + Example:
 
 ```python
 
-from SimpleS.basics import *
+from SimpleS.ImageRelated.basics import *
 
 binary_image = simple_binary_image_creator(points, image_size=(100, 100))
 ```
 #### advance_binary_image_creator
 
 + Creates an advanced binary image from a list of points.
 + Parameters:
```

### Comparing `simple_space-0.9.0/pyproject.toml` & `simple_space-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "Simple-Space"
-version = "0.9.0"
+version = "1.0.0"
 description = "A Try at Better Understanding Space."
 readme = "README.md"
 requires-python = ">=3.6"
 authors = [
     { name = "Hamed Hajipour", email = "cloner174.org@gmail.com" },
 ]
 classifiers = [
```

