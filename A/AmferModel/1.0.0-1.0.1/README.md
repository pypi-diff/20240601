# Comparing `tmp/AmferModel-1.0.0.tar.gz` & `tmp/AmferModel-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AmferModel-1.0.0.tar", last modified: Fri May 31 09:01:48 2024, max compression
+gzip compressed data, was "AmferModel-1.0.1.tar", last modified: Fri May 31 09:17:17 2024, max compression
```

## Comparing `AmferModel-1.0.0.tar` & `AmferModel-1.0.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 09:01:48.656931 AmferModel-1.0.0/
-drwxrwxrwx   0        0        0        0 2024-05-31 09:01:48.654931 AmferModel-1.0.0/AmferModel.egg-info/
--rw-rw-rw-   0        0        0      451 2024-05-31 09:01:48.000000 AmferModel-1.0.0/AmferModel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2024-05-31 09:01:48.000000 AmferModel-1.0.0/AmferModel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 09:01:48.000000 AmferModel-1.0.0/AmferModel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-05-31 09:01:48.000000 AmferModel-1.0.0/AmferModel.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-31 09:01:48.000000 AmferModel-1.0.0/AmferModel.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      451 2024-05-31 09:01:48.655931 AmferModel-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-31 09:01:48.656931 AmferModel-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      584 2024-05-31 09:01:01.000000 AmferModel-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-31 09:17:17.247071 AmferModel-1.0.1/
+drwxrwxrwx   0        0        0        0 2024-05-31 09:17:17.245071 AmferModel-1.0.1/AmferModel.egg-info/
+-rw-rw-rw-   0        0        0      451 2024-05-31 09:17:17.000000 AmferModel-1.0.1/AmferModel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      191 2024-05-31 09:17:17.000000 AmferModel-1.0.1/AmferModel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-31 09:17:17.000000 AmferModel-1.0.1/AmferModel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-31 09:17:17.000000 AmferModel-1.0.1/AmferModel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-31 09:17:17.000000 AmferModel-1.0.1/AmferModel.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    38745 2024-05-31 09:11:27.000000 AmferModel-1.0.1/AmferModel.py
+-rw-rw-rw-   0        0        0      451 2024-05-31 09:17:17.246071 AmferModel-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-31 09:17:17.247071 AmferModel-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      584 2024-05-31 09:17:13.000000 AmferModel-1.0.1/setup.py
```

### Comparing `AmferModel-1.0.0/setup.py` & `AmferModel-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='AmferModel',
-    version='1.0.0',
+    version='1.0.1',
     author='aertsimon90',
     author_email='simon.scap090@gmail.com',
     description='A Python module for artificial intelligence infrastructure, including chatbots, image-drawing bots, and text-to-speech conversion.',
     py_modules=['AmferModel'],
     install_requires=[
         'Pillow',
         'gtts'
```

