# Comparing `tmp/almax_common-1.0.2.dev20240601170258.tar.gz` & `tmp/almax_common-1.0.2.dev20240601170722.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-1.0.2.dev20240601170258.tar", last modified: Sat Jun  1 17:03:20 2024, max compression
+gzip compressed data, was "almax_common-1.0.2.dev20240601170722.tar", last modified: Sat Jun  1 17:07:44 2024, max compression
```

## Comparing `almax_common-1.0.2.dev20240601170258.tar` & `almax_common-1.0.2.dev20240601170722.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:03:20.373415 almax_common-1.0.2.dev20240601170258/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:03:20.369415 almax_common-1.0.2.dev20240601170258/AlmaxClasses/
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/AlmaxClasses/Result.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/AlmaxClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:03:20.369415 almax_common-1.0.2.dev20240601170258/AlmaxGraphics/
--rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/AlmaxGraphics/FrameManager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/AlmaxGraphics/PdfManager.py
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/AlmaxGraphics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:03:20.369415 almax_common-1.0.2.dev20240601170258/AlmaxLogs/
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/AlmaxLogs/LoggerService.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/AlmaxLogs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:03:20.369415 almax_common-1.0.2.dev20240601170258/AlmaxSystemManagment/
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/AlmaxSystemManagment/CustomSubprocess.py
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/AlmaxSystemManagment/CustomThread.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/AlmaxSystemManagment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:03:20.373415 almax_common-1.0.2.dev20240601170258/AlmaxUtils/
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/AlmaxUtils/FileSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/AlmaxUtils/Generic.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/AlmaxUtils/Time.py
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/AlmaxUtils/Xml.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/AlmaxUtils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-06-01 17:03:20.373415 almax_common-1.0.2.dev20240601170258/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:03:20.373415 almax_common-1.0.2.dev20240601170258/almax_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-06-01 17:03:20.000000 almax_common-1.0.2.dev20240601170258/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-06-01 17:03:20.000000 almax_common-1.0.2.dev20240601170258/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 17:03:20.000000 almax_common-1.0.2.dev20240601170258/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-06-01 17:03:20.000000 almax_common-1.0.2.dev20240601170258/almax_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 17:03:20.000000 almax_common-1.0.2.dev20240601170258/almax_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 17:03:20.373415 almax_common-1.0.2.dev20240601170258/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-06-01 17:02:57.000000 almax_common-1.0.2.dev20240601170258/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:07:44.686884 almax_common-1.0.2.dev20240601170722/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:07:44.682884 almax_common-1.0.2.dev20240601170722/AlmaxClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/AlmaxClasses/Result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/AlmaxClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:07:44.682884 almax_common-1.0.2.dev20240601170722/AlmaxGraphics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/AlmaxGraphics/FrameManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/AlmaxGraphics/PdfManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/AlmaxGraphics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:07:44.682884 almax_common-1.0.2.dev20240601170722/AlmaxLogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/AlmaxLogs/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/AlmaxLogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:07:44.682884 almax_common-1.0.2.dev20240601170722/AlmaxSystemManagment/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/AlmaxSystemManagment/CustomSubprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/AlmaxSystemManagment/CustomThread.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/AlmaxSystemManagment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:07:44.682884 almax_common-1.0.2.dev20240601170722/AlmaxUtils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/AlmaxUtils/FileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/AlmaxUtils/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/AlmaxUtils/Time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/AlmaxUtils/Xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/AlmaxUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-06-01 17:07:44.686884 almax_common-1.0.2.dev20240601170722/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 17:07:44.686884 almax_common-1.0.2.dev20240601170722/almax_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-06-01 17:07:44.000000 almax_common-1.0.2.dev20240601170722/almax_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-06-01 17:07:44.000000 almax_common-1.0.2.dev20240601170722/almax_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 17:07:44.000000 almax_common-1.0.2.dev20240601170722/almax_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-06-01 17:07:44.000000 almax_common-1.0.2.dev20240601170722/almax_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 17:07:44.000000 almax_common-1.0.2.dev20240601170722/almax_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 17:07:44.686884 almax_common-1.0.2.dev20240601170722/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-06-01 17:07:20.000000 almax_common-1.0.2.dev20240601170722/setup.py
```

### Comparing `almax_common-1.0.2.dev20240601170258/AlmaxClasses/__init__.py` & `almax_common-1.0.2.dev20240601170722/AlmaxClasses/__init__.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601170258/AlmaxGraphics/FrameManager.py` & `almax_common-1.0.2.dev20240601170722/AlmaxGraphics/FrameManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601170258/AlmaxGraphics/PdfManager.py` & `almax_common-1.0.2.dev20240601170722/AlmaxGraphics/PdfManager.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601170258/AlmaxLogs/LoggerService.py` & `almax_common-1.0.2.dev20240601170722/AlmaxLogs/LoggerService.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601170258/AlmaxSystemManagment/CustomSubprocess.py` & `almax_common-1.0.2.dev20240601170722/AlmaxSystemManagment/CustomSubprocess.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601170258/AlmaxSystemManagment/CustomThread.py` & `almax_common-1.0.2.dev20240601170722/AlmaxSystemManagment/CustomThread.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601170258/AlmaxUtils/FileSystem.py` & `almax_common-1.0.2.dev20240601170722/AlmaxUtils/FileSystem.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601170258/AlmaxUtils/Generic.py` & `almax_common-1.0.2.dev20240601170722/AlmaxUtils/Generic.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601170258/AlmaxUtils/Time.py` & `almax_common-1.0.2.dev20240601170722/AlmaxUtils/Time.py`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601170258/PKG-INFO` & `almax_common-1.0.2.dev20240601170722/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 1.0.2.dev20240601170258
+Version: 1.0.2.dev20240601170722
 Summary: A common library with some of my implementations
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: appnope==0.1.4
 Requires-Dist: asttokens==2.4.1
 Requires-Dist: attrs==23.2.0
@@ -59,15 +59,15 @@
 Requires-Dist: pure-eval==0.2.2
 Requires-Dist: Pygments==2.17.2
 Requires-Dist: python-dateutil==2.9.0.post0
 Requires-Dist: pyzmq==26.0.3
 Requires-Dist: readme_renderer==43.0
 Requires-Dist: referencing==0.35.1
 Requires-Dist: reportlab==4.1.0
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.0
 Requires-Dist: requests-toolbelt==1.0.0
 Requires-Dist: rfc3986==2.0.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: rpds-py==0.18.1
 Requires-Dist: setuptools==69.5.1
 Requires-Dist: six==1.16.0
 Requires-Dist: soupsieve==2.5
```

### Comparing `almax_common-1.0.2.dev20240601170258/almax_common.egg-info/PKG-INFO` & `almax_common-1.0.2.dev20240601170722/almax_common.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 1.0.2.dev20240601170258
+Version: 1.0.2.dev20240601170722
 Summary: A common library with some of my implementations
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: appnope==0.1.4
 Requires-Dist: asttokens==2.4.1
 Requires-Dist: attrs==23.2.0
@@ -59,15 +59,15 @@
 Requires-Dist: pure-eval==0.2.2
 Requires-Dist: Pygments==2.17.2
 Requires-Dist: python-dateutil==2.9.0.post0
 Requires-Dist: pyzmq==26.0.3
 Requires-Dist: readme_renderer==43.0
 Requires-Dist: referencing==0.35.1
 Requires-Dist: reportlab==4.1.0
-Requires-Dist: requests==2.31.0
+Requires-Dist: requests==2.32.0
 Requires-Dist: requests-toolbelt==1.0.0
 Requires-Dist: rfc3986==2.0.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: rpds-py==0.18.1
 Requires-Dist: setuptools==69.5.1
 Requires-Dist: six==1.16.0
 Requires-Dist: soupsieve==2.5
```

### Comparing `almax_common-1.0.2.dev20240601170258/almax_common.egg-info/SOURCES.txt` & `almax_common-1.0.2.dev20240601170722/almax_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `almax_common-1.0.2.dev20240601170258/almax_common.egg-info/requires.txt` & `almax_common-1.0.2.dev20240601170722/almax_common.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 pure-eval==0.2.2
 Pygments==2.17.2
 python-dateutil==2.9.0.post0
 pyzmq==26.0.3
 readme_renderer==43.0
 referencing==0.35.1
 reportlab==4.1.0
-requests==2.31.0
+requests==2.32.0
 requests-toolbelt==1.0.0
 rfc3986==2.0.0
 rich==13.7.1
 rpds-py==0.18.1
 setuptools==69.5.1
 six==1.16.0
 soupsieve==2.5
```

### Comparing `almax_common-1.0.2.dev20240601170258/setup.py` & `almax_common-1.0.2.dev20240601170722/setup.py`

 * *Files identical despite different names*

