# Comparing `tmp/qfpy-9.0.1.tar.gz` & `tmp/qfpy-9.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qfpy-9.0.1.tar", last modified: Sat Jun  1 17:13:23 2024, max compression
+gzip compressed data, was "qfpy-9.0.2.tar", last modified: Sat Jun  1 17:15:54 2024, max compression
```

## Comparing `qfpy-9.0.1.tar` & `qfpy-9.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 17:13:23.823913 qfpy-9.0.1/
--rw-rw-rw-   0        0        0      227 2024-06-01 17:13:23.822942 qfpy-9.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      321 2024-06-01 17:13:06.000000 qfpy-9.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-06-01 17:13:23.823913 qfpy-9.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-06-01 17:13:23.779848 qfpy-9.0.1/src/
-drwxrwxrwx   0        0        0        0 2024-06-01 17:13:23.810675 qfpy-9.0.1/src/qfpy/
--rw-rw-rw-   0        0        0      100 2024-06-01 17:10:50.000000 qfpy-9.0.1/src/qfpy/__init__.py
--rw-rw-rw-   0        0        0      212 2024-06-01 17:05:01.000000 qfpy-9.0.1/src/qfpy/character.py
--rw-rw-rw-   0        0        0      794 2024-05-22 17:43:04.000000 qfpy-9.0.1/src/qfpy/crypto.py
--rw-rw-rw-   0        0        0     1528 2024-04-29 16:50:05.000000 qfpy-9.0.1/src/qfpy/exif.py
--rw-rw-rw-   0        0        0     1992 2024-06-01 17:12:53.000000 qfpy-9.0.1/src/qfpy/ffmpeg.py
--rw-rw-rw-   0        0        0      700 2024-04-29 16:53:48.000000 qfpy-9.0.1/src/qfpy/folder.py
--rw-rw-rw-   0        0        0      881 2024-04-29 16:55:19.000000 qfpy-9.0.1/src/qfpy/function.py
--rw-rw-rw-   0        0        0      329 2024-06-01 17:10:13.000000 qfpy-9.0.1/src/qfpy/output.py
--rw-rw-rw-   0        0        0     1170 2024-04-30 18:20:15.000000 qfpy-9.0.1/src/qfpy/process.py
--rw-rw-rw-   0        0        0      525 2024-04-30 18:24:38.000000 qfpy-9.0.1/src/qfpy/system.py
-drwxrwxrwx   0        0        0        0 2024-06-01 17:13:23.821960 qfpy-9.0.1/src/qfpy.egg-info/
--rw-rw-rw-   0        0        0      227 2024-06-01 17:13:23.000000 qfpy-9.0.1/src/qfpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      369 2024-06-01 17:13:23.000000 qfpy-9.0.1/src/qfpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 17:13:23.000000 qfpy-9.0.1/src/qfpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-06-01 17:13:23.000000 qfpy-9.0.1/src/qfpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-06-01 17:13:23.000000 qfpy-9.0.1/src/qfpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 17:15:54.841266 qfpy-9.0.2/
+-rw-rw-rw-   0        0        0      227 2024-06-01 17:15:54.840288 qfpy-9.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      321 2024-06-01 17:14:14.000000 qfpy-9.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-06-01 17:15:54.842244 qfpy-9.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-06-01 17:15:54.812430 qfpy-9.0.2/src/
+drwxrwxrwx   0        0        0        0 2024-06-01 17:15:54.832476 qfpy-9.0.2/src/qfpy/
+-rw-rw-rw-   0        0        0      100 2024-06-01 17:10:50.000000 qfpy-9.0.2/src/qfpy/__init__.py
+-rw-rw-rw-   0        0        0      212 2024-06-01 17:05:01.000000 qfpy-9.0.2/src/qfpy/character.py
+-rw-rw-rw-   0        0        0      794 2024-05-22 17:43:04.000000 qfpy-9.0.2/src/qfpy/crypto.py
+-rw-rw-rw-   0        0        0     1528 2024-04-29 16:50:05.000000 qfpy-9.0.2/src/qfpy/exif.py
+-rw-rw-rw-   0        0        0     1992 2024-06-01 17:12:53.000000 qfpy-9.0.2/src/qfpy/ffmpeg.py
+-rw-rw-rw-   0        0        0      700 2024-04-29 16:53:48.000000 qfpy-9.0.2/src/qfpy/folder.py
+-rw-rw-rw-   0        0        0      881 2024-04-29 16:55:19.000000 qfpy-9.0.2/src/qfpy/function.py
+-rw-rw-rw-   0        0        0      334 2024-06-01 17:14:05.000000 qfpy-9.0.2/src/qfpy/output.py
+-rw-rw-rw-   0        0        0     1170 2024-04-30 18:20:15.000000 qfpy-9.0.2/src/qfpy/process.py
+-rw-rw-rw-   0        0        0      525 2024-04-30 18:24:38.000000 qfpy-9.0.2/src/qfpy/system.py
+drwxrwxrwx   0        0        0        0 2024-06-01 17:15:54.839313 qfpy-9.0.2/src/qfpy.egg-info/
+-rw-rw-rw-   0        0        0      227 2024-06-01 17:15:54.000000 qfpy-9.0.2/src/qfpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      369 2024-06-01 17:15:54.000000 qfpy-9.0.2/src/qfpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 17:15:54.000000 qfpy-9.0.2/src/qfpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-06-01 17:15:54.000000 qfpy-9.0.2/src/qfpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-06-01 17:15:54.000000 qfpy-9.0.2/src/qfpy.egg-info/top_level.txt
```

### Comparing `qfpy-9.0.1/src/qfpy/crypto.py` & `qfpy-9.0.2/src/qfpy/crypto.py`

 * *Files identical despite different names*

### Comparing `qfpy-9.0.1/src/qfpy/exif.py` & `qfpy-9.0.2/src/qfpy/exif.py`

 * *Files identical despite different names*

### Comparing `qfpy-9.0.1/src/qfpy/ffmpeg.py` & `qfpy-9.0.2/src/qfpy/ffmpeg.py`

 * *Files identical despite different names*

### Comparing `qfpy-9.0.1/src/qfpy/folder.py` & `qfpy-9.0.2/src/qfpy/folder.py`

 * *Files identical despite different names*

### Comparing `qfpy-9.0.1/src/qfpy/function.py` & `qfpy-9.0.2/src/qfpy/function.py`

 * *Files identical despite different names*

### Comparing `qfpy-9.0.1/src/qfpy/process.py` & `qfpy-9.0.2/src/qfpy/process.py`

 * *Files identical despite different names*

### Comparing `qfpy-9.0.1/src/qfpy/system.py` & `qfpy-9.0.2/src/qfpy/system.py`

 * *Files identical despite different names*

