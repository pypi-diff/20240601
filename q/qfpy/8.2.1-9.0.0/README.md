# Comparing `tmp/qfpy-8.2.1.tar.gz` & `tmp/qfpy-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfpy-8.2.1.tar", last modified: Wed May 22 17:43:21 2024, max compression
+gzip compressed data, was "qfpy-9.0.0.tar", last modified: Sat Jun  1 17:11:23 2024, max compression
```

## Comparing `qfpy-8.2.1.tar` & `qfpy-9.0.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 17:43:21.745240 qfpy-8.2.1/
--rw-rw-rw-   0        0        0      251 2024-05-22 17:43:21.743284 qfpy-8.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      335 2024-05-22 17:42:44.000000 qfpy-8.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-22 17:43:21.745240 qfpy-8.2.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-22 17:43:21.719850 qfpy-8.2.1/src/
-drwxrwxrwx   0        0        0        0 2024-05-22 17:43:21.733519 qfpy-8.2.1/src/qfpy/
--rw-rw-rw-   0        0        0       90 2024-04-30 18:19:38.000000 qfpy-8.2.1/src/qfpy/__init__.py
--rw-rw-rw-   0        0        0      210 2024-04-29 16:48:36.000000 qfpy-8.2.1/src/qfpy/character.py
--rw-rw-rw-   0        0        0      794 2024-05-22 17:43:04.000000 qfpy-8.2.1/src/qfpy/crypto.py
--rw-rw-rw-   0        0        0     1528 2024-04-29 16:50:05.000000 qfpy-8.2.1/src/qfpy/exif.py
--rw-rw-rw-   0        0        0     2988 2024-05-02 05:54:03.000000 qfpy-8.2.1/src/qfpy/ffmpeg.py
--rw-rw-rw-   0        0        0      700 2024-04-29 16:53:48.000000 qfpy-8.2.1/src/qfpy/folder.py
--rw-rw-rw-   0        0        0      881 2024-04-29 16:55:19.000000 qfpy-8.2.1/src/qfpy/function.py
--rw-rw-rw-   0        0        0     1170 2024-04-30 18:20:15.000000 qfpy-8.2.1/src/qfpy/process.py
--rw-rw-rw-   0        0        0      525 2024-04-30 18:24:38.000000 qfpy-8.2.1/src/qfpy/system.py
-drwxrwxrwx   0        0        0        0 2024-05-22 17:43:21.742308 qfpy-8.2.1/src/qfpy.egg-info/
--rw-rw-rw-   0        0        0      251 2024-05-22 17:43:21.000000 qfpy-8.2.1/src/qfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      350 2024-05-22 17:43:21.000000 qfpy-8.2.1/src/qfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 17:43:21.000000 qfpy-8.2.1/src/qfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2024-05-22 17:43:21.000000 qfpy-8.2.1/src/qfpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-22 17:43:21.000000 qfpy-8.2.1/src/qfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 17:11:23.751454 qfpy-9.0.0/
+-rw-rw-rw-   0        0        0      251 2024-06-01 17:11:23.749499 qfpy-9.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0      335 2024-06-01 17:11:02.000000 qfpy-9.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-01 17:11:23.751454 qfpy-9.0.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-01 17:11:23.715728 qfpy-9.0.0/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 17:11:23.736809 qfpy-9.0.0/src/qfpy/
+-rw-rw-rw-   0        0        0      100 2024-06-01 17:10:50.000000 qfpy-9.0.0/src/qfpy/__init__.py
+-rw-rw-rw-   0        0        0      212 2024-06-01 17:05:01.000000 qfpy-9.0.0/src/qfpy/character.py
+-rw-rw-rw-   0        0        0      794 2024-05-22 17:43:04.000000 qfpy-9.0.0/src/qfpy/crypto.py
+-rw-rw-rw-   0        0        0     1528 2024-04-29 16:50:05.000000 qfpy-9.0.0/src/qfpy/exif.py
+-rw-rw-rw-   0        0        0     2988 2024-05-02 05:54:03.000000 qfpy-9.0.0/src/qfpy/ffmpeg.py
+-rw-rw-rw-   0        0        0      700 2024-04-29 16:53:48.000000 qfpy-9.0.0/src/qfpy/folder.py
+-rw-rw-rw-   0        0        0      881 2024-04-29 16:55:19.000000 qfpy-9.0.0/src/qfpy/function.py
+-rw-rw-rw-   0        0        0      329 2024-06-01 17:10:13.000000 qfpy-9.0.0/src/qfpy/output.py
+-rw-rw-rw-   0        0        0     1170 2024-04-30 18:20:15.000000 qfpy-9.0.0/src/qfpy/process.py
+-rw-rw-rw-   0        0        0      525 2024-04-30 18:24:38.000000 qfpy-9.0.0/src/qfpy/system.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:11:23.748523 qfpy-9.0.0/src/qfpy.egg-info/
+-rw-rw-rw-   0        0        0      251 2024-06-01 17:11:23.000000 qfpy-9.0.0/src/qfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2024-06-01 17:11:23.000000 qfpy-9.0.0/src/qfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 17:11:23.000000 qfpy-9.0.0/src/qfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2024-06-01 17:11:23.000000 qfpy-9.0.0/src/qfpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-06-01 17:11:23.000000 qfpy-9.0.0/src/qfpy.egg-info/top_level.txt
```

### Comparing `qfpy-8.2.1/src/qfpy/crypto.py` & `qfpy-9.0.0/src/qfpy/crypto.py`

 * *Files identical despite different names*

### Comparing `qfpy-8.2.1/src/qfpy/exif.py` & `qfpy-9.0.0/src/qfpy/exif.py`

 * *Files identical despite different names*

### Comparing `qfpy-8.2.1/src/qfpy/ffmpeg.py` & `qfpy-9.0.0/src/qfpy/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `qfpy-8.2.1/src/qfpy/folder.py` & `qfpy-9.0.0/src/qfpy/folder.py`

 * *Files identical despite different names*

### Comparing `qfpy-8.2.1/src/qfpy/function.py` & `qfpy-9.0.0/src/qfpy/function.py`

 * *Files identical despite different names*

### Comparing `qfpy-8.2.1/src/qfpy/process.py` & `qfpy-9.0.0/src/qfpy/process.py`

 * *Files identical despite different names*

### Comparing `qfpy-8.2.1/src/qfpy/system.py` & `qfpy-9.0.0/src/qfpy/system.py`

 * *Files identical despite different names*

