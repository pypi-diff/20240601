# Comparing `tmp/id_card_recognition-0.2.1.tar.gz` & `tmp/id_card_recognition-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "id_card_recognition-0.2.1.tar", last modified: Sat Jun  1 12:43:18 2024, max compression
+gzip compressed data, was "id_card_recognition-0.2.2.tar", last modified: Sat Jun  1 12:46:28 2024, max compression
```

## Comparing `id_card_recognition-0.2.1.tar` & `id_card_recognition-0.2.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:43:18.272545 id_card_recognition-0.2.1/
--rw-r--r--   0 wangligang   (501) staff       (20)      517 2024-06-01 12:43:18.271963 id_card_recognition-0.2.1/PKG-INFO
--rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:18.000000 id_card_recognition-0.2.1/README.md
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:43:18.267429 id_card_recognition-0.2.1/id_card_recognition/
--rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:56.000000 id_card_recognition-0.2.1/id_card_recognition/__init__.py
--rw-r--r--   0 wangligang   (501) staff       (20)     5347 2024-06-01 12:43:13.000000 id_card_recognition-0.2.1/id_card_recognition/recognition.py
--rw-r--r--   0 wangligang   (501) staff       (20)      938 2024-06-01 10:09:42.000000 id_card_recognition-0.2.1/id_card_recognition/utils.py
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:43:18.271252 id_card_recognition-0.2.1/id_card_recognition.egg-info/
--rw-r--r--   0 wangligang   (501) staff       (20)      517 2024-06-01 12:43:18.000000 id_card_recognition-0.2.1/id_card_recognition.egg-info/PKG-INFO
--rw-r--r--   0 wangligang   (501) staff       (20)      400 2024-06-01 12:43:18.000000 id_card_recognition-0.2.1/id_card_recognition.egg-info/SOURCES.txt
--rw-r--r--   0 wangligang   (501) staff       (20)        1 2024-06-01 12:43:18.000000 id_card_recognition-0.2.1/id_card_recognition.egg-info/dependency_links.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       77 2024-06-01 12:43:18.000000 id_card_recognition-0.2.1/id_card_recognition.egg-info/entry_points.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 12:43:18.000000 id_card_recognition-0.2.1/id_card_recognition.egg-info/requires.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       20 2024-06-01 12:43:18.000000 id_card_recognition-0.2.1/id_card_recognition.egg-info/top_level.txt
--rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 12:43:18.272637 id_card_recognition-0.2.1/setup.cfg
--rw-r--r--   0 wangligang   (501) staff       (20)      847 2024-06-01 12:43:13.000000 id_card_recognition-0.2.1/setup.py
-drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:43:18.270762 id_card_recognition-0.2.1/tests/
--rw-r--r--   0 wangligang   (501) staff       (20)      485 2024-06-01 10:10:09.000000 id_card_recognition-0.2.1/tests/test_recognition.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:46:28.522873 id_card_recognition-0.2.2/
+-rw-r--r--   0 wangligang   (501) staff       (20)      517 2024-06-01 12:46:28.522265 id_card_recognition-0.2.2/PKG-INFO
+-rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:18.000000 id_card_recognition-0.2.2/README.md
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:46:28.517537 id_card_recognition-0.2.2/id_card_recognition/
+-rw-r--r--   0 wangligang   (501) staff       (20)        0 2024-06-01 10:03:56.000000 id_card_recognition-0.2.2/id_card_recognition/__init__.py
+-rw-r--r--   0 wangligang   (501) staff       (20)     5347 2024-06-01 12:43:13.000000 id_card_recognition-0.2.2/id_card_recognition/recognition.py
+-rw-r--r--   0 wangligang   (501) staff       (20)      938 2024-06-01 10:09:42.000000 id_card_recognition-0.2.2/id_card_recognition/utils.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:46:28.521502 id_card_recognition-0.2.2/id_card_recognition.egg-info/
+-rw-r--r--   0 wangligang   (501) staff       (20)      517 2024-06-01 12:46:28.000000 id_card_recognition-0.2.2/id_card_recognition.egg-info/PKG-INFO
+-rw-r--r--   0 wangligang   (501) staff       (20)      400 2024-06-01 12:46:28.000000 id_card_recognition-0.2.2/id_card_recognition.egg-info/SOURCES.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)        1 2024-06-01 12:46:28.000000 id_card_recognition-0.2.2/id_card_recognition.egg-info/dependency_links.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       77 2024-06-01 12:46:28.000000 id_card_recognition-0.2.2/id_card_recognition.egg-info/entry_points.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 12:46:28.000000 id_card_recognition-0.2.2/id_card_recognition.egg-info/requires.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       20 2024-06-01 12:46:28.000000 id_card_recognition-0.2.2/id_card_recognition.egg-info/top_level.txt
+-rw-r--r--   0 wangligang   (501) staff       (20)       38 2024-06-01 12:46:28.523084 id_card_recognition-0.2.2/setup.cfg
+-rw-r--r--   0 wangligang   (501) staff       (20)      847 2024-06-01 12:46:24.000000 id_card_recognition-0.2.2/setup.py
+drwxr-xr-x   0 wangligang   (501) staff       (20)        0 2024-06-01 12:46:28.520975 id_card_recognition-0.2.2/tests/
+-rw-r--r--   0 wangligang   (501) staff       (20)      485 2024-06-01 10:10:09.000000 id_card_recognition-0.2.2/tests/test_recognition.py
```

### Comparing `id_card_recognition-0.2.1/PKG-INFO` & `id_card_recognition-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id_card_recognition
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package for ID card recognition using OpenAI
 Home-page: https://github.com/freedak-wang/id_card_recognition
 Author: freedak Wang
 Author-email: freedak@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `id_card_recognition-0.2.1/id_card_recognition/recognition.py` & `id_card_recognition-0.2.2/id_card_recognition/recognition.py`

 * *Files identical despite different names*

### Comparing `id_card_recognition-0.2.1/id_card_recognition/utils.py` & `id_card_recognition-0.2.2/id_card_recognition/utils.py`

 * *Files identical despite different names*

### Comparing `id_card_recognition-0.2.1/id_card_recognition.egg-info/PKG-INFO` & `id_card_recognition-0.2.2/id_card_recognition.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: id_card_recognition
-Version: 0.2.1
+Version: 0.2.2
 Summary: A package for ID card recognition using OpenAI
 Home-page: https://github.com/freedak-wang/id_card_recognition
 Author: freedak Wang
 Author-email: freedak@163.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `id_card_recognition-0.2.1/setup.py` & `id_card_recognition-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='id_card_recognition',
-    version='0.2.1',
+    version='0.2.2',
     packages=find_packages(),
     install_requires=[
         'requests',
         'natsort',
         'openai',
         'python-dotenv',
     ],
```

