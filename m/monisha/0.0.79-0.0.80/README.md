# Comparing `tmp/monisha-0.0.79.tar.gz` & `tmp/monisha-0.0.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monisha-0.0.79.tar", last modified: Fri May 31 20:26:00 2024, max compression
+gzip compressed data, was "monisha-0.0.80.tar", last modified: Fri May 31 22:13:53 2024, max compression
```

## Comparing `monisha-0.0.79.tar` & `monisha-0.0.80.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:26:00.586716 monisha-0.0.79/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-31 20:25:55.000000 monisha-0.0.79/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:26:00.578716 monisha-0.0.79/Monisha/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:26:00.582716 monisha-0.0.79/Monisha/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/collections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function01.py
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function02.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function03.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function04.py
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function05.py
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function06.py
--rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function07.py
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function08.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function09.py
--rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function10.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function11.py
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function12.py
--rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function13.py
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function14.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function15.py
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function16.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function17.py
--rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function18.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function19.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function20.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function21.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/functions/function22.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:26:00.582716 monisha-0.0.79/Monisha/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/scripts/en.py
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/scripts/eo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/scripts/es.py
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-31 20:25:55.000000 monisha-0.0.79/Monisha/scripts/eu.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-31 20:26:00.586716 monisha-0.0.79/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-31 20:25:55.000000 monisha-0.0.79/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 20:26:00.586716 monisha-0.0.79/monisha.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-31 20:26:00.000000 monisha-0.0.79/monisha.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-31 20:26:00.000000 monisha-0.0.79/monisha.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 20:26:00.000000 monisha-0.0.79/monisha.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-31 20:26:00.000000 monisha-0.0.79/monisha.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 20:26:00.000000 monisha-0.0.79/monisha.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 20:26:00.586716 monisha-0.0.79/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-31 20:25:55.000000 monisha-0.0.79/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:13:53.185448 monisha-0.0.80/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-31 22:13:49.000000 monisha-0.0.80/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:13:53.177448 monisha-0.0.80/Monisha/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:13:53.181448 monisha-0.0.80/Monisha/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/collections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2722 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function01.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function02.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function03.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function04.py
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function05.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function06.py
+-rw-r--r--   0 runner    (1001) docker     (127)      517 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function07.py
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function08.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function09.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60666 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function10.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function11.py
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function12.py
+-rw-r--r--   0 runner    (1001) docker     (127)      422 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function13.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function14.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function15.py
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function16.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function17.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2937 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function18.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function19.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function20.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function21.py
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/functions/function22.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:13:53.185448 monisha-0.0.80/Monisha/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/scripts/en.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/scripts/eo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/scripts/es.py
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-05-31 22:13:49.000000 monisha-0.0.80/Monisha/scripts/eu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-31 22:13:53.185448 monisha-0.0.80/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-31 22:13:49.000000 monisha-0.0.80/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:13:53.185448 monisha-0.0.80/monisha.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-31 22:13:53.000000 monisha-0.0.80/monisha.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-31 22:13:53.000000 monisha-0.0.80/monisha.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:13:53.000000 monisha-0.0.80/monisha.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-31 22:13:53.000000 monisha-0.0.80/monisha.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 22:13:53.000000 monisha-0.0.80/monisha.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 22:13:53.185448 monisha-0.0.80/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-31 22:13:49.000000 monisha-0.0.80/setup.py
```

### Comparing `monisha-0.0.79/LICENSE` & `monisha-0.0.80/LICENSE`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/Monisha/__init__.py` & `monisha-0.0.80/Monisha/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 appname = "monisha"
-version = "0.0.79"
+version = "0.0.80"
 
 install = ["hachoir",
            "requests",
            "beautifulsoup4"]
 
 DATA01 = "clintonabrahamc@gmail.com"
 DATA02 = ['Natural Language :: English',
```

### Comparing `monisha-0.0.79/Monisha/functions/__init__.py` & `monisha-0.0.80/Monisha/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/Monisha/functions/collections.py` & `monisha-0.0.80/Monisha/functions/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 class SMessage:
 
     def __init__(self, **kwargs):
         self.errors = kwargs.get("errors", None)
         self.result = kwargs.get("result", None)
         self.numfiles = kwargs.get('numfiles', 0)
         self.filesize = kwargs.get('filesize', 0)
+        self.allfiles = kwargs.get('allfiles', [])
         self.filename = kwargs.get("filename", None)
         self.taskcode = kwargs.get("taskcode", 5000)
-        self.allfiles = kwargs.get('allfiles', None)
         self.location = kwargs.get('location', None)
         self.filetype = kwargs.get("filetype", None)
         self.extension = kwargs.get("extension", None)
```

### Comparing `monisha-0.0.79/Monisha/functions/function01.py` & `monisha-0.0.80/Monisha/functions/function01.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/Monisha/functions/function02.py` & `monisha-0.0.80/Monisha/functions/function02.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/Monisha/functions/function03.py` & `monisha-0.0.80/Monisha/functions/function03.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/Monisha/functions/function04.py` & `monisha-0.0.80/Monisha/functions/function04.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/Monisha/functions/function06.py` & `monisha-0.0.80/Monisha/functions/function06.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/Monisha/functions/function07.py` & `monisha-0.0.80/Monisha/functions/function07.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/Monisha/functions/function10.py` & `monisha-0.0.80/Monisha/functions/function10.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/Monisha/functions/function15.py` & `monisha-0.0.80/Monisha/functions/function15.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/Monisha/functions/function16.py` & `monisha-0.0.80/Monisha/functions/function16.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/Monisha/functions/function17.py` & `monisha-0.0.80/Monisha/functions/function17.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/Monisha/functions/function18.py` & `monisha-0.0.80/Monisha/functions/function18.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/Monisha/functions/function19.py` & `monisha-0.0.80/Monisha/functions/function19.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/Monisha/functions/function20.py` & `monisha-0.0.80/Monisha/functions/function20.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/Monisha/scripts/es.py` & `monisha-0.0.80/Monisha/scripts/es.py`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/PKG-INFO` & `monisha-0.0.80/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.79
+Version: 0.0.80
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.79 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.80 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.79/monisha.egg-info/PKG-INFO` & `monisha-0.0.80/monisha.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monisha
-Version: 0.0.79
+Version: 0.0.80
 Summary: ㅤ
 Home-page: https://github.com/Clinton-Abraham
 Author: Clinton-Abraham
 Author-email: clintonabrahamc@gmail.com
 License: MIT
 Keywords: python,clinton,abraham
 Classifier: Natural Language :: English
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: monisha Version: 0.0.79 Summary: ã¤ Home-page:
+Metadata-Version: 2.1 Name: monisha Version: 0.0.80 Summary: ã¤ Home-page:
 https://github.com/Clinton-Abraham Author: Clinton-Abraham Author-email:
 clintonabrahamc@gmail.com License: MIT Keywords: python,clinton,abraham
 Classifier: Natural Language :: English Classifier: Intended Audience ::
 Developers Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Topic :: Software Development :: Libraries Classifier: Topic :: Software
```

### Comparing `monisha-0.0.79/monisha.egg-info/SOURCES.txt` & `monisha-0.0.80/monisha.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `monisha-0.0.79/setup.py` & `monisha-0.0.80/setup.py`

 * *Files identical despite different names*

