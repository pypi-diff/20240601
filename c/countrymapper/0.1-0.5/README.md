# Comparing `tmp/countrymapper-0.1.tar.gz` & `tmp/countrymapper-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "countrymapper-0.1.tar", last modified: Fri May 31 06:01:52 2024, max compression
+gzip compressed data, was "countrymapper-0.5.tar", last modified: Sat Jun  1 16:54:21 2024, max compression
```

## Comparing `countrymapper-0.1.tar` & `countrymapper-0.5.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxr-x   0 arfat     (1000) arfat     (1000)        0 2024-05-31 06:01:52.384810 countrymapper-0.1/
--rw-rw-r--   0 arfat     (1000) arfat     (1000)      243 2024-05-31 06:01:52.384810 countrymapper-0.1/PKG-INFO
--rw-rw-r--   0 arfat     (1000) arfat     (1000)     9087 2024-05-31 05:43:30.000000 countrymapper-0.1/README.md
-drwxrwxr-x   0 arfat     (1000) arfat     (1000)        0 2024-05-31 06:01:52.380810 countrymapper-0.1/countrymapper/
--rw-rw-r--   0 arfat     (1000) arfat     (1000)      182 2024-05-31 02:59:56.000000 countrymapper-0.1/countrymapper/__init__.py
--rw-rw-r--   0 arfat     (1000) arfat     (1000)    35707 2024-05-31 03:03:40.000000 countrymapper-0.1/countrymapper/countrymapper.py
--rw-rw-r--   0 arfat     (1000) arfat     (1000)       19 2024-05-31 05:58:43.000000 countrymapper-0.1/countrymapper/version.py
-drwxrwxr-x   0 arfat     (1000) arfat     (1000)        0 2024-05-31 06:01:52.384810 countrymapper-0.1/countrymapper.egg-info/
--rw-rw-r--   0 arfat     (1000) arfat     (1000)      243 2024-05-31 06:01:52.000000 countrymapper-0.1/countrymapper.egg-info/PKG-INFO
--rw-rw-r--   0 arfat     (1000) arfat     (1000)      248 2024-05-31 06:01:52.000000 countrymapper-0.1/countrymapper.egg-info/SOURCES.txt
--rw-rw-r--   0 arfat     (1000) arfat     (1000)        1 2024-05-31 06:01:52.000000 countrymapper-0.1/countrymapper.egg-info/dependency_links.txt
--rw-rw-r--   0 arfat     (1000) arfat     (1000)       14 2024-05-31 06:01:52.000000 countrymapper-0.1/countrymapper.egg-info/top_level.txt
--rw-rw-r--   0 arfat     (1000) arfat     (1000)       38 2024-05-31 06:01:52.384810 countrymapper-0.1/setup.cfg
--rw-rw-r--   0 arfat     (1000) arfat     (1000)      268 2024-05-31 06:01:34.000000 countrymapper-0.1/setup.py
+drwxrwxr-x   0 arfat     (1000) arfat     (1000)        0 2024-06-01 16:54:21.322737 countrymapper-0.5/
+-rw-r--r--   0 arfat     (1000) arfat     (1000)     9307 2024-06-01 16:54:21.322737 countrymapper-0.5/PKG-INFO
+-rw-rw-r--   0 arfat     (1000) arfat     (1000)     9087 2024-05-31 05:43:30.000000 countrymapper-0.5/README.md
+drwxrwxr-x   0 arfat     (1000) arfat     (1000)        0 2024-06-01 16:54:21.318737 countrymapper-0.5/countrymapper/
+-rw-rw-r--   0 arfat     (1000) arfat     (1000)      148 2024-06-01 16:52:51.000000 countrymapper-0.5/countrymapper/__init__.py
+-rw-rw-r--   0 arfat     (1000) arfat     (1000)    35615 2024-06-01 16:52:51.000000 countrymapper-0.5/countrymapper/countrymapper.py
+drwxrwxr-x   0 arfat     (1000) arfat     (1000)        0 2024-06-01 16:54:21.322737 countrymapper-0.5/countrymapper.egg-info/
+-rw-r--r--   0 arfat     (1000) arfat     (1000)     9307 2024-06-01 16:54:21.000000 countrymapper-0.5/countrymapper.egg-info/PKG-INFO
+-rw-rw-r--   0 arfat     (1000) arfat     (1000)      223 2024-06-01 16:54:21.000000 countrymapper-0.5/countrymapper.egg-info/SOURCES.txt
+-rw-rw-r--   0 arfat     (1000) arfat     (1000)        1 2024-06-01 16:54:21.000000 countrymapper-0.5/countrymapper.egg-info/dependency_links.txt
+-rw-rw-r--   0 arfat     (1000) arfat     (1000)       14 2024-06-01 16:54:21.000000 countrymapper-0.5/countrymapper.egg-info/top_level.txt
+-rw-rw-r--   0 arfat     (1000) arfat     (1000)       38 2024-06-01 16:54:21.322737 countrymapper-0.5/setup.cfg
+-rw-rw-r--   0 arfat     (1000) arfat     (1000)      421 2024-06-01 16:54:09.000000 countrymapper-0.5/setup.py
```

### Comparing `countrymapper-0.1/README.md` & `countrymapper-0.5/README.md`

 * *Files identical despite different names*

### Comparing `countrymapper-0.1/countrymapper/countrymapper.py` & `countrymapper-0.5/countrymapper/countrymapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import pprint
 import re
 import sys
 from collections import OrderedDict
 
 import pandas as pd
 
-from countrymapper.version import __version__
 
 COUNTRY_DATA_FILE = os.path.join(
     os.path.split(os.path.abspath(__file__))[0], "country_mapper_data.tsv"
 )
 
 log = logging.getLogger(__name__)
 
@@ -884,15 +883,14 @@
     """
 
     parser = argparse.ArgumentParser(
         description=(
             "The country converter (coco): a Python package for "
             "converting country names between "
             "different classifications schemes. "
-            "Version: {}".format(__version__)
         ),
         prog="coco",
         usage=("%(prog)s names --src --to]"),
     )
 
     parser.add_argument(
         "names",
```

