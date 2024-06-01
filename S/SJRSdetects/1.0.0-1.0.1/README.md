# Comparing `tmp/sjrsdetects-1.0.0.tar.gz` & `tmp/sjrsdetects-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sjrsdetects-1.0.0.tar", last modified: Sat Jun  1 15:19:18 2024, max compression
+gzip compressed data, was "sjrsdetects-1.0.1.tar", last modified: Sat Jun  1 15:27:46 2024, max compression
```

## Comparing `sjrsdetects-1.0.0.tar` & `sjrsdetects-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 15:19:18.493682 sjrsdetects-1.0.0/
--rw-rw-rw-   0        0        0      585 2024-06-01 15:19:18.489125 sjrsdetects-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       58 2024-05-27 08:29:42.000000 sjrsdetects-1.0.0/README.md
--rw-rw-rw-   0        0        0       42 2024-06-01 15:19:18.493682 sjrsdetects-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      857 2024-06-01 15:17:32.000000 sjrsdetects-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:19:18.379111 sjrsdetects-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2024-06-01 15:19:18.433606 sjrsdetects-1.0.0/src/SJRS-detect/
--rw-rw-rw-   0        0        0     1602 2024-05-27 09:36:31.000000 sjrsdetects-1.0.0/src/SJRS-detect/DetectaFormas.py
--rw-rw-rw-   0        0        0     2206 2024-06-01 14:30:15.000000 sjrsdetects-1.0.0/src/SJRS-detect/DetectaMovCamara.py
--rw-rw-rw-   0        0        0     2568 2024-05-27 09:28:51.000000 sjrsdetects-1.0.0/src/SJRS-detect/DetectaMovFotos.py
--rw-rw-rw-   0        0        0     3010 2024-05-27 09:31:31.000000 sjrsdetects-1.0.0/src/SJRS-detect/DetectaMovVideo.py
--rw-rw-rw-   0        0        0      530 2024-06-01 14:14:18.000000 sjrsdetects-1.0.0/src/SJRS-detect/TestDetectaMovCamara.py
--rw-rw-rw-   0        0        0      180 2024-05-27 07:55:51.000000 sjrsdetects-1.0.0/src/SJRS-detect/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:19:18.484240 sjrsdetects-1.0.0/src/SJRSdetects.egg-info/
--rw-rw-rw-   0        0        0      585 2024-06-01 15:19:18.000000 sjrsdetects-1.0.0/src/SJRSdetects.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2024-06-01 15:19:18.000000 sjrsdetects-1.0.0/src/SJRSdetects.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:19:18.000000 sjrsdetects-1.0.0/src/SJRSdetects.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-06-01 15:19:18.000000 sjrsdetects-1.0.0/src/SJRSdetects.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 15:27:46.535636 sjrsdetects-1.0.1/
+-rw-rw-rw-   0        0        0      588 2024-06-01 15:27:46.523704 sjrsdetects-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       58 2024-05-27 08:29:42.000000 sjrsdetects-1.0.1/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:27:46.536146 sjrsdetects-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      860 2024-06-01 15:27:18.000000 sjrsdetects-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:27:46.442015 sjrsdetects-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 15:27:46.467787 sjrsdetects-1.0.1/src/SJRS-detect/
+-rw-rw-rw-   0        0        0     1602 2024-05-27 09:36:31.000000 sjrsdetects-1.0.1/src/SJRS-detect/DetectaFormas.py
+-rw-rw-rw-   0        0        0     2206 2024-06-01 14:30:15.000000 sjrsdetects-1.0.1/src/SJRS-detect/DetectaMovCamara.py
+-rw-rw-rw-   0        0        0     2568 2024-05-27 09:28:51.000000 sjrsdetects-1.0.1/src/SJRS-detect/DetectaMovFotos.py
+-rw-rw-rw-   0        0        0     3010 2024-05-27 09:31:31.000000 sjrsdetects-1.0.1/src/SJRS-detect/DetectaMovVideo.py
+-rw-rw-rw-   0        0        0      180 2024-05-27 07:55:51.000000 sjrsdetects-1.0.1/src/SJRS-detect/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:27:46.523704 sjrsdetects-1.0.1/src/SJRSdetects.egg-info/
+-rw-rw-rw-   0        0        0      588 2024-06-01 15:27:46.000000 sjrsdetects-1.0.1/src/SJRSdetects.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2024-06-01 15:27:46.000000 sjrsdetects-1.0.1/src/SJRSdetects.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:27:46.000000 sjrsdetects-1.0.1/src/SJRSdetects.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 15:27:46.000000 sjrsdetects-1.0.1/src/SJRSdetects.egg-info/top_level.txt
```

### Comparing `sjrsdetects-1.0.0/PKG-INFO` & `sjrsdetects-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: SJRSdetects
-Version: 1.0.0
+Version: 1.0.1
 Summary: Detecta movimiento en fotos, video y camara
-Home-page: https://github.com/Stevenjoelrs/SJRdetect
+Home-page: https://github.com/Stevenjoelrs/SJRSdetects
 Author: Stevenjoelrs
 Author-email: Stevenjramossalazar@gmail.com
-Project-URL: Bug Tracker, https://github.com/Stevenjoelrs/SJRdetect/issues
+Project-URL: Bug Tracker, https://github.com/Stevenjoelrs/SJRSdetect/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # SJRdetect
```

### Comparing `sjrsdetects-1.0.0/setup.py` & `sjrsdetects-1.0.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="SJRSdetects",
-    version="1.0.0",
+    version="1.0.1",
     author="Stevenjoelrs",
     author_email="Stevenjramossalazar@gmail.com",
     description="Detecta movimiento en fotos, video y camara",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/Stevenjoelrs/SJRdetect",
+    url="https://github.com/Stevenjoelrs/SJRSdetects",
     project_urls={
-        "Bug Tracker": "https://github.com/Stevenjoelrs/SJRdetect/issues",
+        "Bug Tracker": "https://github.com/Stevenjoelrs/SJRSdetect/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     package_dir={"": "src"},
```

### Comparing `sjrsdetects-1.0.0/src/SJRS-detect/DetectaFormas.py` & `sjrsdetects-1.0.1/src/SJRS-detect/DetectaFormas.py`

 * *Files identical despite different names*

### Comparing `sjrsdetects-1.0.0/src/SJRS-detect/DetectaMovCamara.py` & `sjrsdetects-1.0.1/src/SJRS-detect/DetectaMovCamara.py`

 * *Files identical despite different names*

### Comparing `sjrsdetects-1.0.0/src/SJRS-detect/DetectaMovFotos.py` & `sjrsdetects-1.0.1/src/SJRS-detect/DetectaMovFotos.py`

 * *Files identical despite different names*

### Comparing `sjrsdetects-1.0.0/src/SJRS-detect/DetectaMovVideo.py` & `sjrsdetects-1.0.1/src/SJRS-detect/DetectaMovVideo.py`

 * *Files identical despite different names*

### Comparing `sjrsdetects-1.0.0/src/SJRSdetects.egg-info/PKG-INFO` & `sjrsdetects-1.0.1/src/SJRSdetects.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: SJRSdetects
-Version: 1.0.0
+Version: 1.0.1
 Summary: Detecta movimiento en fotos, video y camara
-Home-page: https://github.com/Stevenjoelrs/SJRdetect
+Home-page: https://github.com/Stevenjoelrs/SJRSdetects
 Author: Stevenjoelrs
 Author-email: Stevenjramossalazar@gmail.com
-Project-URL: Bug Tracker, https://github.com/Stevenjoelrs/SJRdetect/issues
+Project-URL: Bug Tracker, https://github.com/Stevenjoelrs/SJRSdetect/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # SJRdetect
```

