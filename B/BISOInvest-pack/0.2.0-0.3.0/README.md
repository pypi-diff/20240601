# Comparing `tmp/BISOInvest_pack-0.2.0.tar.gz` & `tmp/BISOInvest_pack-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BISOInvest_pack-0.2.0.tar", last modified: Sat Jun  1 19:17:44 2024, max compression
+gzip compressed data, was "BISOInvest_pack-0.3.0.tar", last modified: Sat Jun  1 19:21:36 2024, max compression
```

## Comparing `BISOInvest_pack-0.2.0.tar` & `BISOInvest_pack-0.3.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 oliverokstadekeberg   (501) staff       (20)        0 2024-06-01 19:17:44.802663 BISOInvest_pack-0.2.0/
-drwxr-xr-x   0 oliverokstadekeberg   (501) staff       (20)        0 2024-06-01 19:17:44.793482 BISOInvest_pack-0.2.0/BISOInvest_pack/
--rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)       24 2024-06-01 19:15:31.000000 BISOInvest_pack-0.2.0/BISOInvest_pack/__init__.py
--rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)     1124 2024-05-29 09:11:46.000000 BISOInvest_pack-0.2.0/BISOInvest_pack/nordnetAPI.py
-drwxr-xr-x   0 oliverokstadekeberg   (501) staff       (20)        0 2024-06-01 19:17:44.799206 BISOInvest_pack-0.2.0/BISOInvest_pack.egg-info/
--rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)      288 2024-06-01 19:17:44.000000 BISOInvest_pack-0.2.0/BISOInvest_pack.egg-info/PKG-INFO
--rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)      312 2024-06-01 19:17:44.000000 BISOInvest_pack-0.2.0/BISOInvest_pack.egg-info/SOURCES.txt
--rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)        1 2024-06-01 19:17:44.000000 BISOInvest_pack-0.2.0/BISOInvest_pack.egg-info/dependency_links.txt
--rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)       63 2024-06-01 19:17:44.000000 BISOInvest_pack-0.2.0/BISOInvest_pack.egg-info/entry_points.txt
--rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)       32 2024-06-01 19:17:44.000000 BISOInvest_pack-0.2.0/BISOInvest_pack.egg-info/requires.txt
--rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)       16 2024-06-01 19:17:44.000000 BISOInvest_pack-0.2.0/BISOInvest_pack.egg-info/top_level.txt
--rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)      288 2024-06-01 19:17:44.801237 BISOInvest_pack-0.2.0/PKG-INFO
--rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)        0 2024-06-01 18:55:50.000000 BISOInvest_pack-0.2.0/README.md
--rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)       38 2024-06-01 19:17:44.802980 BISOInvest_pack-0.2.0/setup.cfg
--rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)      629 2024-06-01 19:17:26.000000 BISOInvest_pack-0.2.0/setup.py
+drwxr-xr-x   0 oliverokstadekeberg   (501) staff       (20)        0 2024-06-01 19:21:36.075623 BISOInvest_pack-0.3.0/
+drwxr-xr-x   0 oliverokstadekeberg   (501) staff       (20)        0 2024-06-01 19:21:36.067237 BISOInvest_pack-0.3.0/BISOInvest_pack/
+-rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)       24 2024-06-01 19:15:31.000000 BISOInvest_pack-0.3.0/BISOInvest_pack/__init__.py
+-rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)     1124 2024-05-29 09:11:46.000000 BISOInvest_pack-0.3.0/BISOInvest_pack/nordnetAPI.py
+drwxr-xr-x   0 oliverokstadekeberg   (501) staff       (20)        0 2024-06-01 19:21:36.073412 BISOInvest_pack-0.3.0/BISOInvest_pack.egg-info/
+-rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)      288 2024-06-01 19:21:35.000000 BISOInvest_pack-0.3.0/BISOInvest_pack.egg-info/PKG-INFO
+-rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)      312 2024-06-01 19:21:36.000000 BISOInvest_pack-0.3.0/BISOInvest_pack.egg-info/SOURCES.txt
+-rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)        1 2024-06-01 19:21:35.000000 BISOInvest_pack-0.3.0/BISOInvest_pack.egg-info/dependency_links.txt
+-rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)       63 2024-06-01 19:21:35.000000 BISOInvest_pack-0.3.0/BISOInvest_pack.egg-info/entry_points.txt
+-rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)       32 2024-06-01 19:21:35.000000 BISOInvest_pack-0.3.0/BISOInvest_pack.egg-info/requires.txt
+-rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)       16 2024-06-01 19:21:35.000000 BISOInvest_pack-0.3.0/BISOInvest_pack.egg-info/top_level.txt
+-rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)      288 2024-06-01 19:21:36.074522 BISOInvest_pack-0.3.0/PKG-INFO
+-rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)        0 2024-06-01 18:55:50.000000 BISOInvest_pack-0.3.0/README.md
+-rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)       38 2024-06-01 19:21:36.075899 BISOInvest_pack-0.3.0/setup.cfg
+-rw-r--r--   0 oliverokstadekeberg   (501) staff       (20)      629 2024-06-01 19:21:23.000000 BISOInvest_pack-0.3.0/setup.py
```

### Comparing `BISOInvest_pack-0.2.0/BISOInvest_pack/nordnetAPI.py` & `BISOInvest_pack-0.3.0/BISOInvest_pack/nordnetAPI.py`

 * *Files identical despite different names*

### Comparing `BISOInvest_pack-0.2.0/setup.py` & `BISOInvest_pack-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pathlib
 import setuptools
 
 setuptools.setup(
 	name ="BISOInvest_pack",
-	version = "0.2.0",
+	version = "0.3.0",
 	description = "Brief description",
 	long_description = pathlib.Path("README.md").read_text(),
 	long_description_content_type = "text/markdown",
 	author = "Oliver Ekeberg",
 	author_email = "ekebergoliver@gmail.com",
 	python_requires = ">=3.10",
 	install_requires = ["requests", "pandas>=2.0", "numpy>=1.0"],
```

