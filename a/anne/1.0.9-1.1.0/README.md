# Comparing `tmp/anne-1.0.9.tar.gz` & `tmp/anne-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anne-1.0.9.tar", last modified: Sat Jun  1 08:25:30 2024, max compression
+gzip compressed data, was "anne-1.1.0.tar", last modified: Sat Jun  1 10:23:51 2024, max compression
```

## Comparing `anne-1.0.9.tar` & `anne-1.1.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 08:25:30.244944 anne-1.0.9/
--rw-rw-rw-   0        0        0     1090 2024-05-28 14:49:46.000000 anne-1.0.9/LICENSE
--rw-rw-rw-   0        0        0     1731 2024-06-01 08:25:30.244944 anne-1.0.9/PKG-INFO
--rw-rw-rw-   0        0        0       45 2024-05-28 15:27:28.000000 anne-1.0.9/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 08:25:30.240958 anne-1.0.9/app/
-drwxrwxrwx   0        0        0        0 2024-06-01 08:25:30.241954 anne-1.0.9/app/anne/
--rw-rw-rw-   0        0        0       64 2024-05-31 00:19:07.000000 anne-1.0.9/app/anne/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 08:25:30.243947 anne-1.0.9/app/anne/browser/
--rw-rw-rw-   0        0        0    18825 2024-05-31 00:58:51.000000 anne-1.0.9/app/anne/browser/AnneBrowser.py
--rw-rw-rw-   0        0        0       38 2024-05-31 00:17:53.000000 anne-1.0.9/app/anne/browser/__init__.py
--rw-rw-rw-   0        0        0      692 2024-05-28 16:07:51.000000 anne-1.0.9/app/anne/browser/utils.py
-drwxrwxrwx   0        0        0        0 2024-06-01 08:25:30.243947 anne-1.0.9/app/anne/proxy/
--rw-rw-rw-   0        0        0     1441 2024-06-01 08:25:02.000000 anne-1.0.9/app/anne/proxy/AnneProxy.py
--rw-rw-rw-   0        0        0       32 2024-05-31 00:19:01.000000 anne-1.0.9/app/anne/proxy/__init__.py
--rw-rw-rw-   0        0        0        2 2024-06-01 08:18:38.000000 anne-1.0.9/app/anne/proxy/utils.py
-drwxrwxrwx   0        0        0        0 2024-06-01 08:25:30.242951 anne-1.0.9/app/anne.egg-info/
--rw-rw-rw-   0        0        0     1731 2024-06-01 08:25:30.000000 anne-1.0.9/app/anne.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-06-01 08:25:30.000000 anne-1.0.9/app/anne.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 08:25:30.000000 anne-1.0.9/app/anne.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-06-01 08:25:30.000000 anne-1.0.9/app/anne.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-06-01 08:25:30.000000 anne-1.0.9/app/anne.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 08:25:30.244944 anne-1.0.9/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-06-01 08:25:29.000000 anne-1.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:23:51.044412 anne-1.1.0/
+-rw-rw-rw-   0        0        0     1090 2024-05-28 14:49:46.000000 anne-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     1731 2024-06-01 10:23:51.044412 anne-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2024-05-28 15:27:28.000000 anne-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 10:23:51.040425 anne-1.1.0/app/
+drwxrwxrwx   0        0        0        0 2024-06-01 10:23:51.041422 anne-1.1.0/app/anne/
+-rw-rw-rw-   0        0        0       90 2024-06-01 09:09:16.000000 anne-1.1.0/app/anne/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:23:51.043415 anne-1.1.0/app/anne/browser/
+-rw-rw-rw-   0        0        0    18825 2024-05-31 00:58:51.000000 anne-1.1.0/app/anne/browser/AnneBrowser.py
+-rw-rw-rw-   0        0        0       38 2024-05-31 00:17:53.000000 anne-1.1.0/app/anne/browser/__init__.py
+-rw-rw-rw-   0        0        0      692 2024-05-28 16:07:51.000000 anne-1.1.0/app/anne/browser/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:23:51.043415 anne-1.1.0/app/anne/info/
+-rw-rw-rw-   0        0        0     5935 2024-06-01 10:22:47.000000 anne-1.1.0/app/anne/info/AnneInfo.py
+-rw-rw-rw-   0        0        0       32 2024-06-01 09:09:05.000000 anne-1.1.0/app/anne/info/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:23:51.044412 anne-1.1.0/app/anne/proxy/
+-rw-rw-rw-   0        0        0     5495 2024-06-01 09:07:50.000000 anne-1.1.0/app/anne/proxy/AnneProxy.py
+-rw-rw-rw-   0        0        0       32 2024-05-31 00:19:01.000000 anne-1.1.0/app/anne/proxy/__init__.py
+-rw-rw-rw-   0        0        0        2 2024-06-01 09:07:41.000000 anne-1.1.0/app/anne/proxy/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 10:23:51.042418 anne-1.1.0/app/anne.egg-info/
+-rw-rw-rw-   0        0        0     1731 2024-06-01 10:23:50.000000 anne-1.1.0/app/anne.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      424 2024-06-01 10:23:50.000000 anne-1.1.0/app/anne.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 10:23:50.000000 anne-1.1.0/app/anne.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-06-01 10:23:50.000000 anne-1.1.0/app/anne.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-06-01 10:23:50.000000 anne-1.1.0/app/anne.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 10:23:51.045408 anne-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-06-01 10:23:50.000000 anne-1.1.0/setup.py
```

### Comparing `anne-1.0.9/LICENSE` & `anne-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anne-1.0.9/PKG-INFO` & `anne-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anne
-Version: 1.0.9
+Version: 1.1.0
 Summary: Lib for lazy dev
 Home-page: https://github.com/mrship666/anne-lib
 Author: AnneHouman
 Author-email: annehouman01@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `anne-1.0.9/app/anne/browser/AnneBrowser.py` & `anne-1.1.0/app/anne/browser/AnneBrowser.py`

 * *Files identical despite different names*

### Comparing `anne-1.0.9/app/anne/browser/utils.py` & `anne-1.1.0/app/anne/browser/utils.py`

 * *Files identical despite different names*

### Comparing `anne-1.0.9/app/anne.egg-info/PKG-INFO` & `anne-1.1.0/app/anne.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anne
-Version: 1.0.9
+Version: 1.1.0
 Summary: Lib for lazy dev
 Home-page: https://github.com/mrship666/anne-lib
 Author: AnneHouman
 Author-email: annehouman01@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

