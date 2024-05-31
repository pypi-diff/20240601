# Comparing `tmp/myfunction_ilonaserg-0.0.1.tar.gz` & `tmp/myfunction_ilonaserg-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/ilonaserg/python-class/evolve-cyber/class5/dist/tmpgj4c6i12/myfunction_ilonaserg-0.0.1.tar", last modified: Fri May 31 22:59:09 2024, max compression
+gzip compressed data, was "/mnt/ilonaserg/python-class/evolve-cyber/class5/dist/tmp9x8ue6ev/myfunction_ilonaserg-0.0.2.tar", last modified: Fri May 31 23:13:42 2024, max compression
```

## Comparing `myfunction_ilonaserg-0.0.1.tar` & `myfunction_ilonaserg-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 22:59:09.000000 myfunction_ilonaserg-0.0.1/
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)      642 2024-05-31 22:57:46.000000 myfunction_ilonaserg-0.0.1/setup.py
-drwxrwxr-x   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 22:59:09.000000 myfunction_ilonaserg-0.0.1/myfunctions_ilonaserg/
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)      439 2024-05-31 22:51:19.000000 myfunction_ilonaserg-0.0.1/myfunctions_ilonaserg/math.py
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 22:45:01.000000 myfunction_ilonaserg-0.0.1/myfunctions_ilonaserg/__init__.py
-drwxrwxr-x   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 22:59:09.000000 myfunction_ilonaserg-0.0.1/myfunction_ilonaserg.egg-info/
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)       22 2024-05-31 22:59:09.000000 myfunction_ilonaserg-0.0.1/myfunction_ilonaserg.egg-info/top_level.txt
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)      258 2024-05-31 22:59:09.000000 myfunction_ilonaserg-0.0.1/myfunction_ilonaserg.egg-info/SOURCES.txt
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)        1 2024-05-31 22:59:09.000000 myfunction_ilonaserg-0.0.1/myfunction_ilonaserg.egg-info/dependency_links.txt
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)      458 2024-05-31 22:59:09.000000 myfunction_ilonaserg-0.0.1/myfunction_ilonaserg.egg-info/PKG-INFO
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 22:44:42.000000 myfunction_ilonaserg-0.0.1/README.md
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)      458 2024-05-31 22:59:09.000000 myfunction_ilonaserg-0.0.1/PKG-INFO
--rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)       38 2024-05-31 22:59:09.000000 myfunction_ilonaserg-0.0.1/setup.cfg
+drwxrwxr-x   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 23:13:42.000000 myfunction_ilonaserg-0.0.2/
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)      642 2024-05-31 23:13:05.000000 myfunction_ilonaserg-0.0.2/setup.py
+drwxrwxr-x   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 23:13:42.000000 myfunction_ilonaserg-0.0.2/myfunctions_ilonaserg/
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)      439 2024-05-31 22:51:19.000000 myfunction_ilonaserg-0.0.2/myfunctions_ilonaserg/math.py
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 22:45:01.000000 myfunction_ilonaserg-0.0.2/myfunctions_ilonaserg/__init__.py
+drwxrwxr-x   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 23:13:42.000000 myfunction_ilonaserg-0.0.2/myfunction_ilonaserg.egg-info/
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)       22 2024-05-31 23:13:41.000000 myfunction_ilonaserg-0.0.2/myfunction_ilonaserg.egg-info/top_level.txt
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)      258 2024-05-31 23:13:41.000000 myfunction_ilonaserg-0.0.2/myfunction_ilonaserg.egg-info/SOURCES.txt
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)        1 2024-05-31 23:13:41.000000 myfunction_ilonaserg-0.0.2/myfunction_ilonaserg.egg-info/dependency_links.txt
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)      458 2024-05-31 23:13:41.000000 myfunction_ilonaserg-0.0.2/myfunction_ilonaserg.egg-info/PKG-INFO
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)        0 2024-05-31 22:44:42.000000 myfunction_ilonaserg-0.0.2/README.md
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)      458 2024-05-31 23:13:42.000000 myfunction_ilonaserg-0.0.2/PKG-INFO
+-rw-rw-r--   0 ilonaserg  (1639) ilonaserg  (1640)       38 2024-05-31 23:13:42.000000 myfunction_ilonaserg-0.0.2/setup.cfg
```

### Comparing `myfunction_ilonaserg-0.0.1/setup.py` & `myfunction_ilonaserg-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunction_ilonaserg',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/ilonaserg/',
     license='MIT',
     author='Ilona Sergeeva',
     author_email='asteria2009scorp@gmail.com',
     description='A description of your package',
```

