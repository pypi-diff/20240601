# Comparing `tmp/datastew-0.1.5.tar.gz` & `tmp/datastew-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datastew-0.1.5.tar", last modified: Wed May 29 09:34:38 2024, max compression
+gzip compressed data, was "datastew-0.1.6.tar", last modified: Sat Jun  1 14:53:38 2024, max compression
```

## Comparing `datastew-0.1.5.tar` & `datastew-0.1.6.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:34:38.522670 datastew-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)    11371 2024-05-29 09:34:34.000000 datastew-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-29 09:34:38.522670 datastew-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-05-29 09:34:34.000000 datastew-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:34:38.522670 datastew-0.1.5/datastew/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-29 09:34:34.000000 datastew-0.1.5/datastew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-05-29 09:34:34.000000 datastew-0.1.5/datastew/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-05-29 09:34:34.000000 datastew-0.1.5/datastew/embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)    13109 2024-05-29 09:34:34.000000 datastew-0.1.5/datastew/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-05-29 09:34:34.000000 datastew-0.1.5/datastew/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-05-29 09:34:34.000000 datastew-0.1.5/datastew/visualisation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:34:38.522670 datastew-0.1.5/datastew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      429 2024-05-29 09:34:38.000000 datastew-0.1.5/datastew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-29 09:34:38.000000 datastew-0.1.5/datastew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 09:34:38.000000 datastew-0.1.5/datastew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-29 09:34:38.000000 datastew-0.1.5/datastew.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 09:34:38.522670 datastew-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-29 09:34:36.000000 datastew-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 09:34:38.522670 datastew-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-29 09:34:34.000000 datastew-0.1.5/tests/test_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-05-29 09:34:34.000000 datastew-0.1.5/tests/test_evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-05-29 09:34:34.000000 datastew-0.1.5/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-05-29 09:34:34.000000 datastew-0.1.5/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-29 09:34:34.000000 datastew-0.1.5/tests/test_repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-05-29 09:34:34.000000 datastew-0.1.5/tests/test_system.py
--rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-05-29 09:34:34.000000 datastew-0.1.5/tests/test_visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:53:38.879066 datastew-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    11371 2024-06-01 14:53:35.000000 datastew-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-06-01 14:53:38.879066 datastew-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5959 2024-06-01 14:53:35.000000 datastew-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:53:38.875065 datastew-0.1.6/datastew/
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-06-01 14:53:35.000000 datastew-0.1.6/datastew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-06-01 14:53:35.000000 datastew-0.1.6/datastew/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2563 2024-06-01 14:53:35.000000 datastew-0.1.6/datastew/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13109 2024-06-01 14:53:35.000000 datastew-0.1.6/datastew/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7388 2024-06-01 14:53:35.000000 datastew-0.1.6/datastew/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11364 2024-06-01 14:53:35.000000 datastew-0.1.6/datastew/visualisation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:53:38.879066 datastew-0.1.6/datastew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      429 2024-06-01 14:53:38.000000 datastew-0.1.6/datastew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-06-01 14:53:38.000000 datastew-0.1.6/datastew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 14:53:38.000000 datastew-0.1.6/datastew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 14:53:38.000000 datastew-0.1.6/datastew.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 14:53:38.879066 datastew-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-06-01 14:53:37.000000 datastew-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:53:38.879066 datastew-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-06-01 14:53:35.000000 datastew-0.1.6/tests/test_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4850 2024-06-01 14:53:35.000000 datastew-0.1.6/tests/test_evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-06-01 14:53:35.000000 datastew-0.1.6/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1852 2024-06-01 14:53:35.000000 datastew-0.1.6/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-06-01 14:53:35.000000 datastew-0.1.6/tests/test_repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2377 2024-06-01 14:53:35.000000 datastew-0.1.6/tests/test_system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5303 2024-06-01 14:53:35.000000 datastew-0.1.6/tests/test_visualisation.py
```

### Comparing `datastew-0.1.5/LICENSE` & `datastew-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datastew-0.1.5/README.md` & `datastew-0.1.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 ### From source
 
 Clone the repository:
 
 ```bash
 git clone https://github.com/SCAI-BIO/index
-cd datastew
+cd index
 ```
 
 Install python requirements:
 
 ```bash
 pip install -r requirements.txt
 ```
```

### Comparing `datastew-0.1.5/datastew/conf.py` & `datastew-0.1.6/datastew/conf.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.5/datastew/embedding.py` & `datastew-0.1.6/datastew/embedding.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.5/datastew/evaluation.py` & `datastew-0.1.6/datastew/evaluation.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.5/datastew/mapping.py` & `datastew-0.1.6/datastew/mapping.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.5/datastew/visualisation.py` & `datastew-0.1.6/datastew/visualisation.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.5/setup.py` & `datastew-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = DESCRIPTION
 
 setup(
     name='datastew',
-    version='v0.1.5',
+    version='v0.1.6',
     packages=['datastew'],
     url='https://github.com/SCAI-BIO/index',
     license='Apache-2.0 license"',
     author='Tim Adams',
     author_email='tim.adams@scai.fraunhofer.de',
     description=DESCRIPTION,
     long_description=DESCRIPTION,
```

### Comparing `datastew-0.1.5/tests/test_embedding.py` & `datastew-0.1.6/tests/test_embedding.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.5/tests/test_evaluation.py` & `datastew-0.1.6/tests/test_evaluation.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.5/tests/test_mapping.py` & `datastew-0.1.6/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.5/tests/test_parser.py` & `datastew-0.1.6/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.5/tests/test_repository.py` & `datastew-0.1.6/tests/test_repository.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.5/tests/test_system.py` & `datastew-0.1.6/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `datastew-0.1.5/tests/test_visualisation.py` & `datastew-0.1.6/tests/test_visualisation.py`

 * *Files identical despite different names*

