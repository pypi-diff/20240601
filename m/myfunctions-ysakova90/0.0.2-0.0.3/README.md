# Comparing `tmp/myfunctions_ysakova90-0.0.2.tar.gz` & `tmp/myfunctions_ysakova90-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/ysakova90/python-class/class5/dist/tmp17putgkf/myfunctions_ysakova90-0.0.2.tar", last modified: Sat Jun  1 03:00:02 2024, max compression
+gzip compressed data, was "/mnt/ysakova90/python-class/class5/dist/tmpycw3rzmy/myfunctions_ysakova90-0.0.3.tar", last modified: Sat Jun  1 16:25:27 2024, max compression
```

## Comparing `myfunctions_ysakova90-0.0.2.tar` & `myfunctions_ysakova90-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 ysakova90  (1622) ysakova90  (1623)        0 2024-06-01 03:00:02.000000 myfunctions_ysakova90-0.0.2/
--rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)      634 2024-06-01 02:59:32.000000 myfunctions_ysakova90-0.0.2/setup.py
--rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)        0 2024-06-01 00:02:03.000000 myfunctions_ysakova90-0.0.2/README.md
--rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)      450 2024-06-01 03:00:02.000000 myfunctions_ysakova90-0.0.2/PKG-INFO
--rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)       38 2024-06-01 03:00:02.000000 myfunctions_ysakova90-0.0.2/setup.cfg
-drwxrwxr-x   0 ysakova90  (1622) ysakova90  (1623)        0 2024-06-01 03:00:02.000000 myfunctions_ysakova90-0.0.2/myfunctions_ysakova90.egg-info/
--rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)        1 2024-06-01 03:00:01.000000 myfunctions_ysakova90-0.0.2/myfunctions_ysakova90.egg-info/top_level.txt
--rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)      198 2024-06-01 03:00:01.000000 myfunctions_ysakova90-0.0.2/myfunctions_ysakova90.egg-info/SOURCES.txt
--rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)        1 2024-06-01 03:00:01.000000 myfunctions_ysakova90-0.0.2/myfunctions_ysakova90.egg-info/dependency_links.txt
--rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)      450 2024-06-01 03:00:01.000000 myfunctions_ysakova90-0.0.2/myfunctions_ysakova90.egg-info/PKG-INFO
+drwxrwxr-x   0 ysakova90  (1622) ysakova90  (1623)        0 2024-06-01 16:25:27.000000 myfunctions_ysakova90-0.0.3/
+-rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)      634 2024-06-01 16:23:33.000000 myfunctions_ysakova90-0.0.3/setup.py
+-rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)     2395 2024-06-01 16:22:13.000000 myfunctions_ysakova90-0.0.3/README.md
+-rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)     2838 2024-06-01 16:25:27.000000 myfunctions_ysakova90-0.0.3/PKG-INFO
+-rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)       38 2024-06-01 16:25:27.000000 myfunctions_ysakova90-0.0.3/setup.cfg
+drwxrwxr-x   0 ysakova90  (1622) ysakova90  (1623)        0 2024-06-01 16:25:27.000000 myfunctions_ysakova90-0.0.3/myfunctions_ysakova90.egg-info/
+-rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)        1 2024-06-01 16:25:27.000000 myfunctions_ysakova90-0.0.3/myfunctions_ysakova90.egg-info/top_level.txt
+-rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)      198 2024-06-01 16:25:27.000000 myfunctions_ysakova90-0.0.3/myfunctions_ysakova90.egg-info/SOURCES.txt
+-rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)        1 2024-06-01 16:25:27.000000 myfunctions_ysakova90-0.0.3/myfunctions_ysakova90.egg-info/dependency_links.txt
+-rw-rw-r--   0 ysakova90  (1622) ysakova90  (1623)     2838 2024-06-01 16:25:27.000000 myfunctions_ysakova90-0.0.3/myfunctions_ysakova90.egg-info/PKG-INFO
```

### Comparing `myfunctions_ysakova90-0.0.2/setup.py` & `myfunctions_ysakova90-0.0.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_ysakova90',
-    version='0.0.2',
+    version='0.0.3',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/ysakova90',
     license='MIT',
     author='Aigul Ysakova',
     author_email='ysakova90@gmail.com',
     description='A description of your package',
```

