# Comparing `tmp/almax_common-1.0.2.dev20240601180721.tar.gz` & `tmp/almax_common-1.0.3.dev20240601181343.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-1.0.2.dev20240601180721.tar", last modified: Sat Jun  1 18:07:24 2024, max compression
+gzip compressed data, was "almax_common-1.0.3.dev20240601181343.tar", last modified: Sat Jun  1 18:13:45 2024, max compression
```

## Comparing `almax_common-1.0.2.dev20240601180721.tar` & `almax_common-1.0.3.dev20240601181343.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:07:24.272412 almax_common-1.0.2.dev20240601180721/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:07:24.268412 almax_common-1.0.2.dev20240601180721/AlmaxClasses/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/AlmaxClasses/Result.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/AlmaxClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:07:24.268412 almax_common-1.0.2.dev20240601180721/AlmaxGraphics/
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/AlmaxGraphics/FrameManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/AlmaxGraphics/PdfManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/AlmaxGraphics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:07:24.272412 almax_common-1.0.2.dev20240601180721/AlmaxLogs/
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/AlmaxLogs/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/AlmaxLogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:07:24.272412 almax_common-1.0.2.dev20240601180721/AlmaxSystemManagment/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/AlmaxSystemManagment/CustomSubprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/AlmaxSystemManagment/CustomThread.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/AlmaxSystemManagment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:07:24.272412 almax_common-1.0.2.dev20240601180721/AlmaxUtils/
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/AlmaxUtils/FileSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/AlmaxUtils/Generic.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/AlmaxUtils/Time.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/AlmaxUtils/Xml.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/AlmaxUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 18:07:24.272412 almax_common-1.0.2.dev20240601180721/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:07:24.272412 almax_common-1.0.2.dev20240601180721/almax_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 18:07:24.000000 almax_common-1.0.2.dev20240601180721/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-06-01 18:07:24.000000 almax_common-1.0.2.dev20240601180721/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 18:07:24.000000 almax_common-1.0.2.dev20240601180721/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 18:07:24.000000 almax_common-1.0.2.dev20240601180721/almax_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 18:07:24.272412 almax_common-1.0.2.dev20240601180721/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 18:07:19.000000 almax_common-1.0.2.dev20240601180721/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:13:45.977513 almax_common-1.0.3.dev20240601181343/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:13:45.973513 almax_common-1.0.3.dev20240601181343/AlmaxClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxClasses/Result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:13:45.973513 almax_common-1.0.3.dev20240601181343/AlmaxGraphics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxGraphics/FrameManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxGraphics/PdfManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxGraphics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:13:45.973513 almax_common-1.0.3.dev20240601181343/AlmaxLogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxLogs/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxLogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:13:45.973513 almax_common-1.0.3.dev20240601181343/AlmaxSystemManagment/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxSystemManagment/CustomSubprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxSystemManagment/CustomThread.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxSystemManagment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:13:45.973513 almax_common-1.0.3.dev20240601181343/AlmaxUtils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxUtils/FileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxUtils/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxUtils/Time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxUtils/Xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/AlmaxUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 18:13:45.977513 almax_common-1.0.3.dev20240601181343/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 18:13:45.977513 almax_common-1.0.3.dev20240601181343/almax_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 18:13:45.000000 almax_common-1.0.3.dev20240601181343/almax_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-06-01 18:13:45.000000 almax_common-1.0.3.dev20240601181343/almax_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 18:13:45.000000 almax_common-1.0.3.dev20240601181343/almax_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 18:13:45.000000 almax_common-1.0.3.dev20240601181343/almax_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 18:13:45.977513 almax_common-1.0.3.dev20240601181343/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      511 2024-06-01 18:13:41.000000 almax_common-1.0.3.dev20240601181343/setup.py
```

### Comparing `almax_common-1.0.2.dev20240601180721/AlmaxClasses/__init__.py` & `almax_common-1.0.3.dev20240601181343/AlmaxClasses/__init__.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601180721/AlmaxGraphics/FrameManager.py` & `almax_common-1.0.3.dev20240601181343/AlmaxGraphics/FrameManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601180721/AlmaxGraphics/PdfManager.py` & `almax_common-1.0.3.dev20240601181343/AlmaxGraphics/PdfManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601180721/AlmaxLogs/LoggerService.py` & `almax_common-1.0.3.dev20240601181343/AlmaxLogs/LoggerService.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601180721/AlmaxSystemManagment/CustomSubprocess.py` & `almax_common-1.0.3.dev20240601181343/AlmaxSystemManagment/CustomSubprocess.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601180721/AlmaxSystemManagment/CustomThread.py` & `almax_common-1.0.3.dev20240601181343/AlmaxSystemManagment/CustomThread.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601180721/AlmaxUtils/FileSystem.py` & `almax_common-1.0.3.dev20240601181343/AlmaxUtils/FileSystem.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601180721/AlmaxUtils/Generic.py` & `almax_common-1.0.3.dev20240601181343/AlmaxUtils/Generic.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601180721/AlmaxUtils/Time.py` & `almax_common-1.0.3.dev20240601181343/AlmaxUtils/Time.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601180721/almax_common.egg-info/SOURCES.txt` & `almax_common-1.0.3.dev20240601181343/almax_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

