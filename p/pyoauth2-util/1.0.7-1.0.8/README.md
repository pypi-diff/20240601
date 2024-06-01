# Comparing `tmp/pyoauth2_util-1.0.7.tar.gz` & `tmp/pyoauth2_util-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoauth2_util-1.0.7.tar", last modified: Wed May  1 13:50:17 2024, max compression
+gzip compressed data, was "pyoauth2_util-1.0.8.tar", last modified: Sat Jun  1 16:12:41 2024, max compression
```

## Comparing `pyoauth2_util-1.0.7.tar` & `pyoauth2_util-1.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:50:17.460578 pyoauth2_util-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-01 13:50:02.000000 pyoauth2_util-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-01 13:50:17.460578 pyoauth2_util-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       94 2024-05-01 13:50:02.000000 pyoauth2_util-1.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:50:17.460578 pyoauth2_util-1.0.7/pyoauth2_util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-01 13:50:02.000000 pyoauth2_util-1.0.7/pyoauth2_util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-05-01 13:50:02.000000 pyoauth2_util-1.0.7/pyoauth2_util/oauth2.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 13:50:17.460578 pyoauth2_util-1.0.7/pyoauth2_util.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-01 13:50:17.000000 pyoauth2_util-1.0.7/pyoauth2_util.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-01 13:50:17.000000 pyoauth2_util-1.0.7/pyoauth2_util.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:50:17.000000 pyoauth2_util-1.0.7/pyoauth2_util.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-01 13:50:17.000000 pyoauth2_util-1.0.7/pyoauth2_util.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-01 13:50:17.000000 pyoauth2_util-1.0.7/pyoauth2_util.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 13:50:17.000000 pyoauth2_util-1.0.7/pyoauth2_util.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 13:50:17.460578 pyoauth2_util-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-05-01 13:50:02.000000 pyoauth2_util-1.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:12:41.947639 pyoauth2_util-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-06-01 16:12:33.000000 pyoauth2_util-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-06-01 16:12:41.947639 pyoauth2_util-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-06-01 16:12:33.000000 pyoauth2_util-1.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:12:41.943639 pyoauth2_util-1.0.8/pyoauth2_util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 16:12:33.000000 pyoauth2_util-1.0.8/pyoauth2_util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2024-06-01 16:12:33.000000 pyoauth2_util-1.0.8/pyoauth2_util/oauth2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 16:12:41.947639 pyoauth2_util-1.0.8/pyoauth2_util.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-06-01 16:12:41.000000 pyoauth2_util-1.0.8/pyoauth2_util.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-06-01 16:12:41.000000 pyoauth2_util-1.0.8/pyoauth2_util.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 16:12:41.000000 pyoauth2_util-1.0.8/pyoauth2_util.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-06-01 16:12:41.000000 pyoauth2_util-1.0.8/pyoauth2_util.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 16:12:41.000000 pyoauth2_util-1.0.8/pyoauth2_util.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 16:12:41.000000 pyoauth2_util-1.0.8/pyoauth2_util.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 16:12:41.947639 pyoauth2_util-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-06-01 16:12:33.000000 pyoauth2_util-1.0.8/setup.py
```

### Comparing `pyoauth2_util-1.0.7/LICENSE` & `pyoauth2_util-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoauth2_util-1.0.7/pyoauth2_util/oauth2.py` & `pyoauth2_util-1.0.8/pyoauth2_util/oauth2.py`

 * *Files identical despite different names*

### Comparing `pyoauth2_util-1.0.7/setup.py` & `pyoauth2_util-1.0.8/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 with io.open("requirements.txt", 'r') as f:
     install_requires = f.read().split(os.sep)
 
 
 setup(
     name='pyoauth2_util',
-    version='1.0.7',
+    version='1.0.8',
     description='oauth2助手',
     author='buyfakett',
     author_email='buyfakett@vip.qq.com',
     license='MIT',
     url="https://github.com/buyfakett",
     packages=find_packages(),  # packages=["pytest"],
     long_description=long_description,
```

