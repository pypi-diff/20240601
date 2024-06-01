# Comparing `tmp/almax_common-1.0.1.dev20240601164303.tar.gz` & `tmp/almax_common-1.0.2.dev20240601170049.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-1.0.1.dev20240601164303.tar", last modified: Sat Jun  1 16:43:25 2024, max compression
+gzip compressed data, was "almax_common-1.0.2.dev20240601170049.tar", last modified: Sat Jun  1 17:01:15 2024, max compression
```

## Comparing `almax_common-1.0.1.dev20240601164303.tar` & `almax_common-1.0.2.dev20240601170049.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:43:25.693725 almax_common-1.0.1.dev20240601164303/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:43:25.689725 almax_common-1.0.1.dev20240601164303/AlmaxClasses/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/AlmaxClasses/Result.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/AlmaxClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:43:25.693725 almax_common-1.0.1.dev20240601164303/AlmaxGraphics/
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/AlmaxGraphics/FrameManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/AlmaxGraphics/PdfManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/AlmaxGraphics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:43:25.693725 almax_common-1.0.1.dev20240601164303/AlmaxLogs/
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/AlmaxLogs/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/AlmaxLogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:43:25.693725 almax_common-1.0.1.dev20240601164303/AlmaxSystemManagment/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/AlmaxSystemManagment/CustomSubprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/AlmaxSystemManagment/CustomThread.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/AlmaxSystemManagment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:43:25.693725 almax_common-1.0.1.dev20240601164303/AlmaxUtils/
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/AlmaxUtils/FileSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/AlmaxUtils/Generic.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/AlmaxUtils/Time.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/AlmaxUtils/Xml.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/AlmaxUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-06-01 16:43:25.693725 almax_common-1.0.1.dev20240601164303/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:43:25.693725 almax_common-1.0.1.dev20240601164303/almax_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-06-01 16:43:25.000000 almax_common-1.0.1.dev20240601164303/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-06-01 16:43:25.000000 almax_common-1.0.1.dev20240601164303/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 16:43:25.000000 almax_common-1.0.1.dev20240601164303/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-06-01 16:43:25.000000 almax_common-1.0.1.dev20240601164303/almax_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 16:43:25.000000 almax_common-1.0.1.dev20240601164303/almax_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 16:43:25.693725 almax_common-1.0.1.dev20240601164303/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-06-01 16:43:02.000000 almax_common-1.0.1.dev20240601164303/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:01:15.119331 almax_common-1.0.2.dev20240601170049/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:01:15.115331 almax_common-1.0.2.dev20240601170049/AlmaxClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/AlmaxClasses/Result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/AlmaxClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:01:15.115331 almax_common-1.0.2.dev20240601170049/AlmaxGraphics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/AlmaxGraphics/FrameManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/AlmaxGraphics/PdfManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/AlmaxGraphics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:01:15.115331 almax_common-1.0.2.dev20240601170049/AlmaxLogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/AlmaxLogs/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/AlmaxLogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:01:15.115331 almax_common-1.0.2.dev20240601170049/AlmaxSystemManagment/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/AlmaxSystemManagment/CustomSubprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/AlmaxSystemManagment/CustomThread.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/AlmaxSystemManagment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:01:15.115331 almax_common-1.0.2.dev20240601170049/AlmaxUtils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/AlmaxUtils/FileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/AlmaxUtils/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/AlmaxUtils/Time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/AlmaxUtils/Xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/AlmaxUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-06-01 17:01:15.119331 almax_common-1.0.2.dev20240601170049/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:01:15.115331 almax_common-1.0.2.dev20240601170049/almax_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-06-01 17:01:15.000000 almax_common-1.0.2.dev20240601170049/almax_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-06-01 17:01:15.000000 almax_common-1.0.2.dev20240601170049/almax_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 17:01:15.000000 almax_common-1.0.2.dev20240601170049/almax_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-06-01 17:01:15.000000 almax_common-1.0.2.dev20240601170049/almax_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 17:01:15.000000 almax_common-1.0.2.dev20240601170049/almax_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 17:01:15.119331 almax_common-1.0.2.dev20240601170049/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-06-01 17:00:48.000000 almax_common-1.0.2.dev20240601170049/setup.py
```

### Comparing `almax_common-1.0.1.dev20240601164303/AlmaxClasses/__init__.py` & `almax_common-1.0.2.dev20240601170049/AlmaxClasses/__init__.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.1.dev20240601164303/AlmaxGraphics/FrameManager.py` & `almax_common-1.0.2.dev20240601170049/AlmaxGraphics/FrameManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.1.dev20240601164303/AlmaxGraphics/PdfManager.py` & `almax_common-1.0.2.dev20240601170049/AlmaxGraphics/PdfManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.1.dev20240601164303/AlmaxLogs/LoggerService.py` & `almax_common-1.0.2.dev20240601170049/AlmaxLogs/LoggerService.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.1.dev20240601164303/AlmaxSystemManagment/CustomSubprocess.py` & `almax_common-1.0.2.dev20240601170049/AlmaxSystemManagment/CustomSubprocess.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.1.dev20240601164303/AlmaxSystemManagment/CustomThread.py` & `almax_common-1.0.2.dev20240601170049/AlmaxSystemManagment/CustomThread.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.1.dev20240601164303/AlmaxUtils/FileSystem.py` & `almax_common-1.0.2.dev20240601170049/AlmaxUtils/FileSystem.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.1.dev20240601164303/AlmaxUtils/Generic.py` & `almax_common-1.0.2.dev20240601170049/AlmaxUtils/Generic.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.1.dev20240601164303/AlmaxUtils/Time.py` & `almax_common-1.0.2.dev20240601170049/AlmaxUtils/Time.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.1.dev20240601164303/PKG-INFO` & `almax_common-1.0.2.dev20240601170049/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 1.0.1.dev20240601164303
+Version: 1.0.2.dev20240601170049
 Summary: A common library with some of my implementations
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: appnope==0.1.4
 Requires-Dist: asttokens==2.4.1
 Requires-Dist: attrs==23.2.0
```

### Comparing `almax_common-1.0.1.dev20240601164303/almax_common.egg-info/PKG-INFO` & `almax_common-1.0.2.dev20240601170049/almax_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 1.0.1.dev20240601164303
+Version: 1.0.2.dev20240601170049
 Summary: A common library with some of my implementations
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: appnope==0.1.4
 Requires-Dist: asttokens==2.4.1
 Requires-Dist: attrs==23.2.0
```

### Comparing `almax_common-1.0.1.dev20240601164303/almax_common.egg-info/SOURCES.txt` & `almax_common-1.0.2.dev20240601170049/almax_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.1.dev20240601164303/almax_common.egg-info/requires.txt` & `almax_common-1.0.2.dev20240601170049/almax_common.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.1.dev20240601164303/setup.py` & `almax_common-1.0.2.dev20240601170049/setup.py`

 * *Files identical despite different names*

