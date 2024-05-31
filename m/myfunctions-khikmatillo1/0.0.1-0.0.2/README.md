# Comparing `tmp/myfunctions_khikmatillo1-0.0.1.tar.gz` & `tmp/myfunctions_khikmatillo1-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/khikmatillo1/python-class/evolvecyber/class5/dist/tmp0rjf6iho/myfunctions_khikmatillo1-0.0.1.tar", last modified: Fri May 31 22:37:38 2024, max compression
+gzip compressed data, was "/mnt/khikmatillo1/python-class/evolvecyber/class5/dist/tmpbiryf39g/myfunctions_khikmatillo1-0.0.2.tar", last modified: Fri May 31 23:01:32 2024, max compression
```

## Comparing `myfunctions_khikmatillo1-0.0.1.tar` & `myfunctions_khikmatillo1-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 22:37:38.000000 myfunctions_khikmatillo1-0.0.1/
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      653 2024-05-31 22:37:11.000000 myfunctions_khikmatillo1-0.0.1/setup.py
-drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 22:37:38.000000 myfunctions_khikmatillo1-0.0.1/myfunctions_khikmatillo1/
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      107 2024-05-31 22:34:14.000000 myfunctions_khikmatillo1-0.0.1/myfunctions_khikmatillo1/math.py
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 22:26:26.000000 myfunctions_khikmatillo1-0.0.1/myfunctions_khikmatillo1/__init__.py
-drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 22:37:38.000000 myfunctions_khikmatillo1-0.0.1/myfunctions_khikmatillo1.egg-info/
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)       25 2024-05-31 22:37:38.000000 myfunctions_khikmatillo1-0.0.1/myfunctions_khikmatillo1.egg-info/top_level.txt
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      280 2024-05-31 22:37:38.000000 myfunctions_khikmatillo1-0.0.1/myfunctions_khikmatillo1.egg-info/SOURCES.txt
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)        1 2024-05-31 22:37:38.000000 myfunctions_khikmatillo1-0.0.1/myfunctions_khikmatillo1.egg-info/dependency_links.txt
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      469 2024-05-31 22:37:38.000000 myfunctions_khikmatillo1-0.0.1/myfunctions_khikmatillo1.egg-info/PKG-INFO
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 22:25:28.000000 myfunctions_khikmatillo1-0.0.1/README.md
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      469 2024-05-31 22:37:38.000000 myfunctions_khikmatillo1-0.0.1/PKG-INFO
--rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)       38 2024-05-31 22:37:38.000000 myfunctions_khikmatillo1-0.0.1/setup.cfg
+drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 23:01:32.000000 myfunctions_khikmatillo1-0.0.2/
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      653 2024-05-31 23:01:01.000000 myfunctions_khikmatillo1-0.0.2/setup.py
+drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 23:01:31.000000 myfunctions_khikmatillo1-0.0.2/myfunctions_khikmatillo1/
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      176 2024-05-31 23:00:55.000000 myfunctions_khikmatillo1-0.0.2/myfunctions_khikmatillo1/math.py
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 22:26:26.000000 myfunctions_khikmatillo1-0.0.2/myfunctions_khikmatillo1/__init__.py
+drwxrwxr-x   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 23:01:31.000000 myfunctions_khikmatillo1-0.0.2/myfunctions_khikmatillo1.egg-info/
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)       25 2024-05-31 23:01:31.000000 myfunctions_khikmatillo1-0.0.2/myfunctions_khikmatillo1.egg-info/top_level.txt
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      280 2024-05-31 23:01:31.000000 myfunctions_khikmatillo1-0.0.2/myfunctions_khikmatillo1.egg-info/SOURCES.txt
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)        1 2024-05-31 23:01:31.000000 myfunctions_khikmatillo1-0.0.2/myfunctions_khikmatillo1.egg-info/dependency_links.txt
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      469 2024-05-31 23:01:31.000000 myfunctions_khikmatillo1-0.0.2/myfunctions_khikmatillo1.egg-info/PKG-INFO
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)        0 2024-05-31 22:25:28.000000 myfunctions_khikmatillo1-0.0.2/README.md
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)      469 2024-05-31 23:01:32.000000 myfunctions_khikmatillo1-0.0.2/PKG-INFO
+-rw-rw-r--   0 khikmatillo1  (1682) khikmatillo1  (1683)       38 2024-05-31 23:01:32.000000 myfunctions_khikmatillo1-0.0.2/setup.cfg
```

### Comparing `myfunctions_khikmatillo1-0.0.1/setup.py` & `myfunctions_khikmatillo1-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='myfunctions_khikmatillo1',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(),
     install_requires=[],
     url='https://github.com/khikmatillo1/',
     license='MIT',
     author='Hikmatillo Lutfullaev',
     author_email='twaravancargo@gmail.com',
     description='A description of your package',
```

