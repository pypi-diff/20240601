# Comparing `tmp/gooeypie-0.8.1.tar.gz` & `tmp/gooeypie-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gooeypie-0.8.1.tar", last modified: Sun Jan 15 23:46:46 2023, max compression
+gzip compressed data, was "gooeypie-0.9.0.tar", last modified: Wed Mar 15 07:24:48 2023, max compression
```

## Comparing `gooeypie-0.8.1.tar` & `gooeypie-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-01-15 23:46:46.538656 gooeypie-0.8.1/
--rw-rw-rw-   0        0        0     1088 2022-10-29 00:44:21.000000 gooeypie-0.8.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1017 2023-01-15 23:46:46.538155 gooeypie-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0      360 2021-09-14 23:46:40.000000 gooeypie-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2023-01-15 23:46:46.531149 gooeypie-0.8.1/gooeypie/
--rw-rw-rw-   0        0        0    48870 2023-01-15 23:45:56.000000 gooeypie-0.8.1/gooeypie/__init__.py
--rw-rw-rw-   0        0        0   108554 2023-01-03 22:33:49.000000 gooeypie-0.8.1/gooeypie/widgets.py
-drwxrwxrwx   0        0        0        0 2023-01-15 23:46:46.536654 gooeypie-0.8.1/gooeypie.egg-info/
--rw-rw-rw-   0        0        0     1017 2023-01-15 23:46:46.000000 gooeypie-0.8.1/gooeypie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      230 2023-01-15 23:46:46.000000 gooeypie-0.8.1/gooeypie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-15 23:46:46.000000 gooeypie-0.8.1/gooeypie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-01-15 23:46:46.000000 gooeypie-0.8.1/gooeypie.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-01-15 23:46:46.000000 gooeypie-0.8.1/gooeypie.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-15 23:46:46.538656 gooeypie-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0     1012 2023-01-15 23:43:15.000000 gooeypie-0.8.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-03-15 07:24:48.642015 gooeypie-0.9.0/
+-rw-rw-rw-   0        0        0     1088 2022-10-29 00:44:21.000000 gooeypie-0.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     1017 2023-03-15 07:24:48.641514 gooeypie-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2021-09-14 23:46:40.000000 gooeypie-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2023-03-15 07:24:48.635014 gooeypie-0.9.0/gooeypie/
+-rw-rw-rw-   0        0        0    48870 2023-03-15 07:24:23.000000 gooeypie-0.9.0/gooeypie/__init__.py
+-rw-rw-rw-   0        0        0   110599 2023-03-12 03:34:33.000000 gooeypie-0.9.0/gooeypie/widgets.py
+drwxrwxrwx   0        0        0        0 2023-03-15 07:24:48.640014 gooeypie-0.9.0/gooeypie.egg-info/
+-rw-rw-rw-   0        0        0     1017 2023-03-15 07:24:48.000000 gooeypie-0.9.0/gooeypie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      230 2023-03-15 07:24:48.000000 gooeypie-0.9.0/gooeypie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-15 07:24:48.000000 gooeypie-0.9.0/gooeypie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-03-15 07:24:48.000000 gooeypie-0.9.0/gooeypie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-03-15 07:24:48.000000 gooeypie-0.9.0/gooeypie.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-03-15 07:24:48.642015 gooeypie-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     1012 2023-03-15 07:24:23.000000 gooeypie-0.9.0/setup.py
```

### Comparing `gooeypie-0.8.1/LICENSE.txt` & `gooeypie-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gooeypie-0.8.1/PKG-INFO` & `gooeypie-0.9.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gooeypie
-Version: 0.8.1
+Version: 0.9.0
 Summary: Designed for beginners, GooeyPie is a simple but powerful GUI library.
 Home-page: https://gooeypie.dev
 Author: Adam Antonio
 Author-email: adam@gooeypie.dev
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gooeypie-0.8.1/gooeypie/__init__.py` & `gooeypie-0.9.0/gooeypie/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from tkinter import messagebox
 from tkinter import filedialog
 import base64
 from io import BytesIO
 
 from .widgets import *
 
-__version__ = "0.8.1"
+__version__ = "0.9.0"
 
 
 class WindowBase(Container):
     """Base class for GooeyPieApp and Window classes
     Provides functions for window options like size, title and menus
     """
     def __init__(self, root, title, *args):
```

### Comparing `gooeypie-0.8.1/gooeypie/widgets.py` & `gooeypie-0.9.0/gooeypie/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -2759,7 +2759,71 @@
         self._orientation = orientation
 
     def __str__(self):
         return f"<{self._orientation} Separator>"
 
     def __repr__(self):
         return self.__str__()
+
+
+class Progressbar(ttk.Progressbar, GooeyPieWidget):
+    """Put a description here later
+
+     """
+
+    def __init__(self, container, mode='determinate'):
+        """Creates a new ProgressBar widget
+
+        Args
+            container: The window or container to which the widget will be added
+            mode (str): Optional - the mode of the progress bar, either 'determinate' or 'indeterminate'
+        """
+        GooeyPieWidget.__init__(self, container)
+
+        self._value = tk.IntVar()
+        ttk.Progressbar.__init__(self, container, variable=self._value)
+        self.mode = mode
+
+    def __str__(self):
+        return f"<Progressbar widget>"
+
+    def __repr__(self):
+        return self.__str__()
+
+    @property
+    def value(self):
+        """Gets or sets the value of the progress bar as a number between 0 and 100"""
+        return self._value.get()
+
+    @value.setter
+    def value(self, value):
+        if type(value) not in (int, float):
+            raise ValueError('Progressbar value must be an integer')
+        if not (0 <= value <= 100):
+            raise ValueError('Progressbar value must be an integer between 0 and 100 (inclusive)')
+
+        self._value.set(value)
+
+    @property
+    def mode(self):
+        """Gets or sets the mode of the progress bar - either 'determinate' or 'indeterminate'"""
+        return self.cget('mode')
+
+    @mode.setter
+    def mode(self, mode):
+        if mode not in ('determinate', 'indeterminate'):
+            raise ValueError("mode must be either 'determinate' or 'indeterminate'")
+        self.config(mode=mode)
+
+    @property
+    def width(self):
+        """Gets or sets the width of the progress bar in pixels"""
+        return self.cget('length')
+
+    @width.setter
+    def width(self, width):
+        if type(width) != int:
+            raise ValueError('width must be a positive integer')
+        if width <= 0:
+            raise ValueError('width must be a positive integer')
+
+        self.config(length=width)
```

### Comparing `gooeypie-0.8.1/gooeypie.egg-info/PKG-INFO` & `gooeypie-0.9.0/gooeypie.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gooeypie
-Version: 0.8.1
+Version: 0.9.0
 Summary: Designed for beginners, GooeyPie is a simple but powerful GUI library.
 Home-page: https://gooeypie.dev
 Author: Adam Antonio
 Author-email: adam@gooeypie.dev
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `gooeypie-0.8.1/setup.py` & `gooeypie-0.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # README
 HERE = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(HERE, "README.md")) as fid:
     README = fid.read()
 
 setup(
     name="gooeypie",
-    version="0.8.1",
+    version="0.9.0",
     description="Designed for beginners, GooeyPie is a simple but powerful GUI library.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://gooeypie.dev",
     author="Adam Antonio",
     author_email="adam@gooeypie.dev",
     license="MIT",
```

