# Comparing `tmp/almax_common-1.0.4.tar.gz` & `tmp/almax_common-1.0.4.dev20240601201036.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-1.0.4.tar", last modified: Sat Jun  1 20:27:29 2024, max compression
+gzip compressed data, was "almax_common-1.0.4.dev20240601201036.tar", last modified: Sat Jun  1 20:10:41 2024, max compression
```

## Comparing `almax_common-1.0.4.tar` & `almax_common-1.0.4.dev20240601201036.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:27:29.108872 almax_common-1.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:27:29.104872 almax_common-1.0.4/AlmaxClasses/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 20:27:19.000000 almax_common-1.0.4/AlmaxClasses/Result.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 20:27:19.000000 almax_common-1.0.4/AlmaxClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:27:29.104872 almax_common-1.0.4/AlmaxGraphics/
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 20:27:19.000000 almax_common-1.0.4/AlmaxGraphics/FrameManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 20:27:19.000000 almax_common-1.0.4/AlmaxGraphics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:27:29.104872 almax_common-1.0.4/AlmaxLogs/
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-01 20:27:19.000000 almax_common-1.0.4/AlmaxLogs/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 20:27:19.000000 almax_common-1.0.4/AlmaxLogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:27:29.104872 almax_common-1.0.4/AlmaxSystemManagment/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 20:27:19.000000 almax_common-1.0.4/AlmaxSystemManagment/CustomSubprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 20:27:19.000000 almax_common-1.0.4/AlmaxSystemManagment/CustomThread.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:27:19.000000 almax_common-1.0.4/AlmaxSystemManagment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:27:29.104872 almax_common-1.0.4/AlmaxUtils/
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 20:27:19.000000 almax_common-1.0.4/AlmaxUtils/FileSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-06-01 20:27:19.000000 almax_common-1.0.4/AlmaxUtils/Generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-06-01 20:27:19.000000 almax_common-1.0.4/AlmaxUtils/PdfManager.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 20:27:19.000000 almax_common-1.0.4/AlmaxUtils/Time.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 20:27:19.000000 almax_common-1.0.4/AlmaxUtils/Xml.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 20:27:19.000000 almax_common-1.0.4/AlmaxUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-06-01 20:27:29.108872 almax_common-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-01 20:27:19.000000 almax_common-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:27:29.108872 almax_common-1.0.4/almax_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-06-01 20:27:29.000000 almax_common-1.0.4/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-06-01 20:27:29.000000 almax_common-1.0.4/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 20:27:29.000000 almax_common-1.0.4/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 20:27:29.000000 almax_common-1.0.4/almax_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 20:27:29.108872 almax_common-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 20:27:19.000000 almax_common-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:10:41.484402 almax_common-1.0.4.dev20240601201036/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:10:41.480402 almax_common-1.0.4.dev20240601201036/AlmaxClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxClasses/Result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:10:41.480402 almax_common-1.0.4.dev20240601201036/AlmaxGraphics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxGraphics/FrameManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxGraphics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:10:41.480402 almax_common-1.0.4.dev20240601201036/AlmaxLogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxLogs/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxLogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:10:41.480402 almax_common-1.0.4.dev20240601201036/AlmaxSystemManagment/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxSystemManagment/CustomSubprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxSystemManagment/CustomThread.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxSystemManagment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:10:41.480402 almax_common-1.0.4.dev20240601201036/AlmaxUtils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxUtils/FileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1926 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxUtils/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxUtils/PdfManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxUtils/Time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxUtils/Xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/AlmaxUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 20:10:41.484402 almax_common-1.0.4.dev20240601201036/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:10:41.484402 almax_common-1.0.4.dev20240601201036/almax_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 20:10:41.000000 almax_common-1.0.4.dev20240601201036/almax_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-06-01 20:10:41.000000 almax_common-1.0.4.dev20240601201036/almax_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 20:10:41.000000 almax_common-1.0.4.dev20240601201036/almax_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 20:10:41.000000 almax_common-1.0.4.dev20240601201036/almax_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 20:10:41.484402 almax_common-1.0.4.dev20240601201036/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 20:10:30.000000 almax_common-1.0.4.dev20240601201036/setup.py
```

### Comparing `almax_common-1.0.4/AlmaxClasses/__init__.py` & `almax_common-1.0.4.dev20240601201036/AlmaxClasses/__init__.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.4/AlmaxGraphics/FrameManager.py` & `almax_common-1.0.4.dev20240601201036/AlmaxGraphics/FrameManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.4/AlmaxLogs/LoggerService.py` & `almax_common-1.0.4.dev20240601201036/AlmaxLogs/LoggerService.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.4/AlmaxSystemManagment/CustomSubprocess.py` & `almax_common-1.0.4.dev20240601201036/AlmaxSystemManagment/CustomSubprocess.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.4/AlmaxSystemManagment/CustomThread.py` & `almax_common-1.0.4.dev20240601201036/AlmaxSystemManagment/CustomThread.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.4/AlmaxUtils/FileSystem.py` & `almax_common-1.0.4.dev20240601201036/AlmaxUtils/FileSystem.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.4/AlmaxUtils/Generic.py` & `almax_common-1.0.4.dev20240601201036/AlmaxUtils/Generic.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.4/AlmaxUtils/PdfManager.py` & `almax_common-1.0.4.dev20240601201036/AlmaxUtils/PdfManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.4/AlmaxUtils/Time.py` & `almax_common-1.0.4.dev20240601201036/AlmaxUtils/Time.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.4/almax_common.egg-info/SOURCES.txt` & `almax_common-1.0.4.dev20240601201036/almax_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

