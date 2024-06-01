# Comparing `tmp/myfunctions_Adnan-IT-0.0.13.tar.gz` & `tmp/myfunctions_Adnan-IT-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/Adnan-IT/python-class/class5/dist/tmp3pqe7d7t/myfunctions_Adnan-IT-0.0.13.tar", last modified: Fri May 31 23:58:55 2024, max compression
+gzip compressed data, was "/mnt/Adnan-IT/python-class/class5/dist/tmpsu77kz6c/myfunctions_Adnan-IT-0.0.9.tar", last modified: Fri May 31 20:56:37 2024, max compression
```

## Comparing `myfunctions_Adnan-IT-0.0.13.tar` & `myfunctions_Adnan-IT-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,10 @@
-drwxrwxr-x   0 Adnan-IT  (1633) Adnan-IT  (1634)        0 2024-05-31 23:58:55.000000 myfunctions_Adnan-IT-0.0.13/
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)      634 2024-05-31 23:58:45.000000 myfunctions_Adnan-IT-0.0.13/setup.py
-drwxrwxr-x   0 Adnan-IT  (1633) Adnan-IT  (1634)        0 2024-05-31 23:58:55.000000 myfunctions_Adnan-IT-0.0.13/myfunctions_Adnan_IT.egg-info/
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)        1 2024-05-31 23:58:55.000000 myfunctions_Adnan-IT-0.0.13/myfunctions_Adnan_IT.egg-info/top_level.txt
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)      237 2024-05-31 23:58:55.000000 myfunctions_Adnan-IT-0.0.13/myfunctions_Adnan_IT.egg-info/SOURCES.txt
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)        3 2024-05-31 23:58:55.000000 myfunctions_Adnan-IT-0.0.13/myfunctions_Adnan_IT.egg-info/requires.txt
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)        1 2024-05-31 23:58:55.000000 myfunctions_Adnan-IT-0.0.13/myfunctions_Adnan_IT.egg-info/dependency_links.txt
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)     3432 2024-05-31 23:58:55.000000 myfunctions_Adnan-IT-0.0.13/myfunctions_Adnan_IT.egg-info/PKG-INFO
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)     2994 2024-05-31 21:32:41.000000 myfunctions_Adnan-IT-0.0.13/README.md
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)     3432 2024-05-31 23:58:55.000000 myfunctions_Adnan-IT-0.0.13/PKG-INFO
--rw-rw-r--   0 Adnan-IT  (1633) Adnan-IT  (1634)       38 2024-05-31 23:58:55.000000 myfunctions_Adnan-IT-0.0.13/setup.cfg
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

### Comparing `myfunctions_Adnan-IT-0.0.13/setup.py` & `myfunctions_Adnan-IT-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_Adnan-IT',
-    version='0.0.13',
+    version='0.0.9',
     packages=find_packages(),
-    install_requires=["os"],
+    install_requires=[],
     url='https://github.com/Adnan-IT',
     license='MIT',
     author='Adnan-IT',
     author_email='adnan123it@gmail.com',
     description='A description of your package',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
```

