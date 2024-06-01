# Comparing `tmp/simple_out-0.1.tar.gz` & `tmp/simple_out-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_out-0.1.tar", last modified: Sun May 19 17:01:16 2024, max compression
+gzip compressed data, was "simple_out-0.3.tar", last modified: Sat Jun  1 15:42:23 2024, max compression
```

## Comparing `simple_out-0.1.tar` & `simple_out-0.3.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:01:16.596866 simple_out-0.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-19 17:01:08.000000 simple_out-0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-19 17:01:16.592866 simple_out-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-19 17:01:08.000000 simple_out-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:01:16.592866 simple_out-0.1/out/
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-19 17:01:08.000000 simple_out-0.1/out/out.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 17:01:16.596866 simple_out-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-19 17:01:08.000000 simple_out-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 17:01:16.592866 simple_out-0.1/simple_out.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-19 17:01:16.000000 simple_out-0.1/simple_out.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-19 17:01:16.000000 simple_out-0.1/simple_out.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 17:01:16.000000 simple_out-0.1/simple_out.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-19 17:01:16.000000 simple_out-0.1/simple_out.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:42:23.370056 simple_out-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 15:42:19.000000 simple_out-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-06-01 15:42:23.370056 simple_out-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-01 15:42:19.000000 simple_out-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:42:23.370056 simple_out-0.3/out/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 15:42:19.000000 simple_out-0.3/out/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-06-01 15:42:19.000000 simple_out-0.3/out/out.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 15:42:23.370056 simple_out-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-06-01 15:42:19.000000 simple_out-0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 15:42:23.370056 simple_out-0.3/simple_out.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-06-01 15:42:23.000000 simple_out-0.3/simple_out.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-06-01 15:42:23.000000 simple_out-0.3/simple_out.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 15:42:23.000000 simple_out-0.3/simple_out.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-06-01 15:42:23.000000 simple_out-0.3/simple_out.egg-info/top_level.txt
```

### Comparing `simple_out-0.1/LICENSE` & `simple_out-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_out-0.1/setup.py` & `simple_out-0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 with open("README.md", "r") as read:
     long_description = read.read()
 
 setup(
-    name="simple-out",
-    version="0.1",
+    name="simple_out",
+    version="0.3",
     description="A simple way to print colored text in the terminal.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords=["print", "output", "input"],
     author="2Bor3d",
     packages=["out"],
     classifiers=[
```

