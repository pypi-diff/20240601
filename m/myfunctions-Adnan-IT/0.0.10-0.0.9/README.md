# Comparing `tmp/myfunctions_Adnan-IT-0.0.10.tar.gz` & `tmp/myfunctions_Adnan-IT-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/Adnan-IT/python-class/class5/dist/tmp2dxfm5pw/myfunctions_Adnan-IT-0.0.10.tar", last modified: Fri May 31 21:33:08 2024, max compression
+gzip compressed data, was "/mnt/Adnan-IT/python-class/class5/dist/tmpsu77kz6c/myfunctions_Adnan-IT-0.0.9.tar", last modified: Fri May 31 20:56:37 2024, max compression
```

## Comparing `myfunctions_Adnan-IT-0.0.10.tar` & `myfunctions_Adnan-IT-0.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 Adnan-IT  (1633) Adnan-IT  (1634)        0 2024-05-31 21:33:08.000000 myfunctions_Adnan-IT-0.0.10/
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)      630 2024-05-31 21:32:46.000000 myfunctions_Adnan-IT-0.0.10/setup.py
-drwxrwxr-x   0 Adnan-IT  (1633) Adnan-IT  (1634)        0 2024-05-31 21:33:08.000000 myfunctions_Adnan-IT-0.0.10/myfunctions_Adnan_IT.egg-info/
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)        1 2024-05-31 21:33:08.000000 myfunctions_Adnan-IT-0.0.10/myfunctions_Adnan_IT.egg-info/top_level.txt
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)      194 2024-05-31 21:33:08.000000 myfunctions_Adnan-IT-0.0.10/myfunctions_Adnan_IT.egg-info/SOURCES.txt
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)        1 2024-05-31 21:33:08.000000 myfunctions_Adnan-IT-0.0.10/myfunctions_Adnan_IT.egg-info/dependency_links.txt
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)     3432 2024-05-31 21:33:08.000000 myfunctions_Adnan-IT-0.0.10/myfunctions_Adnan_IT.egg-info/PKG-INFO
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)     2994 2024-05-31 21:32:41.000000 myfunctions_Adnan-IT-0.0.10/README.md
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)     3432 2024-05-31 21:33:08.000000 myfunctions_Adnan-IT-0.0.10/PKG-INFO
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)       38 2024-05-31 21:33:08.000000 myfunctions_Adnan-IT-0.0.10/setup.cfg
+drwxrwxr-x   0 Adnan-IT  (1633) Adnan-IT  (1634)        0 2024-05-31 20:56:37.000000 myfunctions_Adnan-IT-0.0.9/
+-rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)      629 2024-05-31 20:53:03.000000 myfunctions_Adnan-IT-0.0.9/setup.py
+drwxrwxr-x   0 Adnan-IT  (1633) Adnan-IT  (1634)        0 2024-05-31 20:56:37.000000 myfunctions_Adnan-IT-0.0.9/myfunctions_Adnan_IT.egg-info/
+-rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)        1 2024-05-31 20:56:36.000000 myfunctions_Adnan-IT-0.0.9/myfunctions_Adnan_IT.egg-info/top_level.txt
+-rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)      194 2024-05-31 20:56:36.000000 myfunctions_Adnan-IT-0.0.9/myfunctions_Adnan_IT.egg-info/SOURCES.txt
+-rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)        1 2024-05-31 20:56:36.000000 myfunctions_Adnan-IT-0.0.9/myfunctions_Adnan_IT.egg-info/dependency_links.txt
+-rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)      444 2024-05-31 20:56:36.000000 myfunctions_Adnan-IT-0.0.9/myfunctions_Adnan_IT.egg-info/PKG-INFO
+-rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)        0 2024-05-31 01:07:49.000000 myfunctions_Adnan-IT-0.0.9/README.md
+-rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)      444 2024-05-31 20:56:37.000000 myfunctions_Adnan-IT-0.0.9/PKG-INFO
+-rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)       38 2024-05-31 20:56:37.000000 myfunctions_Adnan-IT-0.0.9/setup.cfg
```

### Comparing `myfunctions_Adnan-IT-0.0.10/setup.py` & `myfunctions_Adnan-IT-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_Adnan-IT',
-    version='0.0.10',
+    version='0.0.9',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/Adnan-IT',
     license='MIT',
     author='Adnan-IT',
     author_email='adnan123it@gmail.com',
     description='A description of your package',
```

