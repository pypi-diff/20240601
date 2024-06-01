# Comparing `tmp/almax_common-0.9.6.tar.gz` & `tmp/almax_common-1.0.0.dev20240601161442.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "almax_common-0.9.6.tar", last modified: Sat Jun  1 13:49:42 2024, max compression
+gzip compressed data, was "almax_common-1.0.0.dev20240601161442.tar", last modified: Sat Jun  1 16:15:06 2024, max compression
```

## Comparing `almax_common-0.9.6.tar` & `almax_common-1.0.0.dev20240601161442.tar`

### file list

```diff
@@ -1,17 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:49:42.961400 almax_common-0.9.6/
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-06-01 13:49:42.961400 almax_common-0.9.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-01 13:49:16.000000 almax_common-0.9.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:49:42.961400 almax_common-0.9.6/Utils/
--rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 13:49:16.000000 almax_common-0.9.6/Utils/FileSystem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-01 13:49:16.000000 almax_common-0.9.6/Utils/Generic.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 13:49:16.000000 almax_common-0.9.6/Utils/Time.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-06-01 13:49:16.000000 almax_common-0.9.6/Utils/Xml.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-01 13:49:16.000000 almax_common-0.9.6/Utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 13:49:42.961400 almax_common-0.9.6/almax_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-06-01 13:49:42.000000 almax_common-0.9.6/almax_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-06-01 13:49:42.000000 almax_common-0.9.6/almax_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 13:49:42.000000 almax_common-0.9.6/almax_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1345 2024-06-01 13:49:42.000000 almax_common-0.9.6/almax_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-01 13:49:42.000000 almax_common-0.9.6/almax_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 13:49:42.961400 almax_common-0.9.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-06-01 13:49:16.000000 almax_common-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:15:06.578672 almax_common-1.0.0.dev20240601161442/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:15:06.574672 almax_common-1.0.0.dev20240601161442/AlmaxClasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/AlmaxClasses/Result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/AlmaxClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:15:06.574672 almax_common-1.0.0.dev20240601161442/AlmaxGraphics/
+-rw-r--r--   0 runner    (1001) docker     (127)     5872 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/AlmaxGraphics/FrameManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5018 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/AlmaxGraphics/PdfManager.py
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/AlmaxGraphics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:15:06.574672 almax_common-1.0.0.dev20240601161442/AlmaxLogs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/AlmaxLogs/LoggerService.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/AlmaxLogs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:15:06.574672 almax_common-1.0.0.dev20240601161442/AlmaxSystemManagment/
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/AlmaxSystemManagment/CustomSubprocess.py
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/AlmaxSystemManagment/CustomThread.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/AlmaxSystemManagment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:15:06.574672 almax_common-1.0.0.dev20240601161442/AlmaxUtils/
+-rw-r--r--   0 runner    (1001) docker     (127)     4398 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/AlmaxUtils/FileSystem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/AlmaxUtils/Generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/AlmaxUtils/Time.py
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/AlmaxUtils/Xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/AlmaxUtils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-06-01 16:15:06.578672 almax_common-1.0.0.dev20240601161442/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:15:06.578672 almax_common-1.0.0.dev20240601161442/almax_common.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2789 2024-06-01 16:15:06.000000 almax_common-1.0.0.dev20240601161442/almax_common.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-06-01 16:15:06.000000 almax_common-1.0.0.dev20240601161442/almax_common.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 16:15:06.000000 almax_common-1.0.0.dev20240601161442/almax_common.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-06-01 16:15:06.000000 almax_common-1.0.0.dev20240601161442/almax_common.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 16:15:06.000000 almax_common-1.0.0.dev20240601161442/almax_common.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 16:15:06.578672 almax_common-1.0.0.dev20240601161442/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-06-01 16:14:41.000000 almax_common-1.0.0.dev20240601161442/setup.py
```

### Comparing `almax_common-0.9.6/PKG-INFO` & `almax_common-1.0.0.dev20240601161442/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 0.9.6
+Version: 1.0.0.dev20240601161442
 Summary: A common library with some of my implementations
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: appnope==0.1.4
 Requires-Dist: asttokens==2.4.1
 Requires-Dist: attrs==23.2.0
@@ -30,14 +30,15 @@
 Requires-Dist: Jinja2==3.1.4
 Requires-Dist: jsonschema==4.22.0
 Requires-Dist: jsonschema-specifications==2023.12.1
 Requires-Dist: jupyter_client==8.6.2
 Requires-Dist: jupyter_core==5.7.2
 Requires-Dist: jupyterlab_pygments==0.3.0
 Requires-Dist: keyring==25.1.0
+Requires-Dist: lxml==5.2.2
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: MarkupSafe==2.1.5
 Requires-Dist: matplotlib-inline==0.1.7
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: mistune==3.0.2
 Requires-Dist: more-itertools==10.2.0
 Requires-Dist: nbclient==0.10.0
```

### Comparing `almax_common-0.9.6/Utils/FileSystem.py` & `almax_common-1.0.0.dev20240601161442/AlmaxUtils/FileSystem.py`

 * *Files identical despite different names*

### Comparing `almax_common-0.9.6/Utils/Generic.py` & `almax_common-1.0.0.dev20240601161442/AlmaxUtils/Generic.py`

 * *Files identical despite different names*

### Comparing `almax_common-0.9.6/Utils/Time.py` & `almax_common-1.0.0.dev20240601161442/AlmaxUtils/Time.py`

 * *Files identical despite different names*

### Comparing `almax_common-0.9.6/almax_common.egg-info/PKG-INFO` & `almax_common-1.0.0.dev20240601161442/almax_common.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: almax_common
-Version: 0.9.6
+Version: 1.0.0.dev20240601161442
 Summary: A common library with some of my implementations
 Author: AlMax98
 Author-email: alihaider.maqsood@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: appnope==0.1.4
 Requires-Dist: asttokens==2.4.1
 Requires-Dist: attrs==23.2.0
@@ -30,14 +30,15 @@
 Requires-Dist: Jinja2==3.1.4
 Requires-Dist: jsonschema==4.22.0
 Requires-Dist: jsonschema-specifications==2023.12.1
 Requires-Dist: jupyter_client==8.6.2
 Requires-Dist: jupyter_core==5.7.2
 Requires-Dist: jupyterlab_pygments==0.3.0
 Requires-Dist: keyring==25.1.0
+Requires-Dist: lxml==5.2.2
 Requires-Dist: markdown-it-py==3.0.0
 Requires-Dist: MarkupSafe==2.1.5
 Requires-Dist: matplotlib-inline==0.1.7
 Requires-Dist: mdurl==0.1.2
 Requires-Dist: mistune==3.0.2
 Requires-Dist: more-itertools==10.2.0
 Requires-Dist: nbclient==0.10.0
```

### Comparing `almax_common-0.9.6/almax_common.egg-info/requires.txt` & `almax_common-1.0.0.dev20240601161442/almax_common.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 Jinja2==3.1.4
 jsonschema==4.22.0
 jsonschema-specifications==2023.12.1
 jupyter_client==8.6.2
 jupyter_core==5.7.2
 jupyterlab_pygments==0.3.0
 keyring==25.1.0
+lxml==5.2.2
 markdown-it-py==3.0.0
 MarkupSafe==2.1.5
 matplotlib-inline==0.1.7
 mdurl==0.1.2
 mistune==3.0.2
 more-itertools==10.2.0
 nbclient==0.10.0
```

### Comparing `almax_common-0.9.6/setup.py` & `almax_common-1.0.0.dev20240601161442/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,21 @@
-from setuptools import setup, find_packages
+from setuptools import setup, find_packages;
 
 with open("README.md", "r") as fh:
     readMe = fh.read();
 
 with open("requirements.txt") as f:
     required = f.read().splitlines();
 
+with open("version.txt", "r") as fh:
+    versionFile = fh.read().strip();
+
 setup(
     name='almax_common',
-    version='0.9.6',
+    version=versionFile,
     description='A common library with some of my implementations',
     long_description=readMe,
     long_description_content_type='text/markdown',
     author='AlMax98',
     author_email='alihaider.maqsood@gmail.com',
     packages=find_packages(),
     package_dir={'': '.'},
```

