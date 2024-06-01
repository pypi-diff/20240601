# Comparing `tmp/almax_common-1.0.3.dev20240601181343.tar.gz` & `tmp/almax_common-1.0.4.dev20240601201036.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-1.0.3.dev20240601181343.tar", last modified: Sat Jun  1 18:13:45 2024, max compression
+gzip compressed data, was "almax_common-1.0.4.dev20240601201036.tar", last modified: Sat Jun  1 20:10:41 2024, max compression
```

## Comparing `almax_common-1.0.3.dev20240601181343.tar` & `almax_common-1.0.4.dev20240601201036.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:13:45.977513 almax_common-1.0.3.dev20240601181343/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:13:45.973513 almax_common-1.0.3.dev20240601181343/AlmaxClasses/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxClasses/Result.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:13:45.973513 almax_common-1.0.3.dev20240601181343/AlmaxGraphics/
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxGraphics/FrameManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxGraphics/PdfManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxGraphics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:13:45.973513 almax_common-1.0.3.dev20240601181343/AlmaxLogs/
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxLogs/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxLogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:13:45.973513 almax_common-1.0.3.dev20240601181343/AlmaxSystemManagment/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxSystemManagment/CustomSubprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxSystemManagment/CustomThread.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxSystemManagment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:13:45.973513 almax_common-1.0.3.dev20240601181343/AlmaxUtils/
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxUtils/FileSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxUtils/Generic.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxUtils/Time.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxUtils/Xml.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 18:13:45.977513 almax_common-1.0.3.dev20240601181343/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:13:45.977513 almax_common-1.0.3.dev20240601181343/almax_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 18:13:45.000000 almax_common-1.0.3.dev20240601181343/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-06-01 18:13:45.000000 almax_common-1.0.3.dev20240601181343/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 18:13:45.000000 almax_common-1.0.3.dev20240601181343/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 18:13:45.000000 almax_common-1.0.3.dev20240601181343/almax_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 18:13:45.977513 almax_common-1.0.3.dev20240601181343/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/setup.py
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

### Comparing `almax_common-1.0.3.dev20240601181343/AlmaxClasses/__init__.py` & `almax_common-1.0.4.dev20240601201036/AlmaxClasses/__init__.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.3.dev20240601181343/AlmaxGraphics/FrameManager.py` & `almax_common-1.0.4.dev20240601201036/AlmaxGraphics/FrameManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.3.dev20240601181343/AlmaxLogs/LoggerService.py` & `almax_common-1.0.4.dev20240601201036/AlmaxLogs/LoggerService.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.3.dev20240601181343/AlmaxSystemManagment/CustomSubprocess.py` & `almax_common-1.0.4.dev20240601201036/AlmaxSystemManagment/CustomSubprocess.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.3.dev20240601181343/AlmaxSystemManagment/CustomThread.py` & `almax_common-1.0.4.dev20240601201036/AlmaxSystemManagment/CustomThread.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.3.dev20240601181343/AlmaxUtils/FileSystem.py` & `almax_common-1.0.4.dev20240601201036/AlmaxUtils/FileSystem.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.3.dev20240601181343/AlmaxUtils/Time.py` & `almax_common-1.0.4.dev20240601201036/AlmaxUtils/Time.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.3.dev20240601181343/almax_common.egg-info/SOURCES.txt` & `almax_common-1.0.4.dev20240601201036/almax_common.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 README.md
 setup.py
 ./AlmaxClasses/Result.py
 ./AlmaxClasses/__init__.py
 ./AlmaxGraphics/FrameManager.py
-./AlmaxGraphics/PdfManager.py
 ./AlmaxGraphics/__init__.py
 ./AlmaxLogs/LoggerService.py
 ./AlmaxLogs/__init__.py
 ./AlmaxSystemManagment/CustomSubprocess.py
 ./AlmaxSystemManagment/CustomThread.py
 ./AlmaxSystemManagment/__init__.py
 ./AlmaxUtils/FileSystem.py
 ./AlmaxUtils/Generic.py
+./AlmaxUtils/PdfManager.py
 ./AlmaxUtils/Time.py
 ./AlmaxUtils/Xml.py
 ./AlmaxUtils/__init__.py
 almax_common.egg-info/PKG-INFO
 almax_common.egg-info/SOURCES.txt
 almax_common.egg-info/dependency_links.txt
 almax_common.egg-info/top_level.txt
```

