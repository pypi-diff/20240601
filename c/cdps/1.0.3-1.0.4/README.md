# Comparing `tmp/cdps-1.0.3.tar.gz` & `tmp/cdps-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdps-1.0.3.tar", last modified: Sat Jun  1 15:15:32 2024, max compression
+gzip compressed data, was "cdps-1.0.4.tar", last modified: Sat Jun  1 15:19:34 2024, max compression
```

## Comparing `cdps-1.0.3.tar` & `cdps-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 15:15:32.795112 cdps-1.0.3/
--rw-rw-rw-   0        0        0    35184 2024-06-01 14:18:34.000000 cdps-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1835 2024-06-01 15:15:32.794112 cdps-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2024-06-01 14:23:15.000000 cdps-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 15:15:32.793112 cdps-1.0.3/cdps.egg-info/
--rw-rw-rw-   0        0        0     1835 2024-06-01 15:15:32.000000 cdps-1.0.3/cdps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2024-06-01 15:15:32.000000 cdps-1.0.3/cdps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:15:32.000000 cdps-1.0.3/cdps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-06-01 15:15:32.000000 cdps-1.0.3/cdps.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      172 2024-06-01 15:15:32.000000 cdps-1.0.3/cdps.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:15:32.000000 cdps-1.0.3/cdps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 15:15:32.795112 cdps-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1715 2024-06-01 15:11:18.000000 cdps-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:19:34.810805 cdps-1.0.4/
+-rw-rw-rw-   0        0        0    35184 2024-06-01 14:18:34.000000 cdps-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1835 2024-06-01 15:19:34.810805 cdps-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1036 2024-06-01 14:23:15.000000 cdps-1.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 15:19:34.809805 cdps-1.0.4/cdps.egg-info/
+-rw-rw-rw-   0        0        0     1835 2024-06-01 15:19:34.000000 cdps-1.0.4/cdps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2024-06-01 15:19:34.000000 cdps-1.0.4/cdps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:19:34.000000 cdps-1.0.4/cdps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-06-01 15:19:34.000000 cdps-1.0.4/cdps.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      172 2024-06-01 15:19:34.000000 cdps-1.0.4/cdps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:19:34.000000 cdps-1.0.4/cdps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:19:34.811805 cdps-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1715 2024-06-01 15:18:12.000000 cdps-1.0.4/setup.py
```

### Comparing `cdps-1.0.3/LICENSE` & `cdps-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdps-1.0.3/PKG-INFO` & `cdps-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdps
-Version: 1.0.3
+Version: 1.0.4
 Summary: Composite Disaster Prevention Server
 Home-page: UNKNOWN
 Author: ExpTechTW
 Author-email: exptech.tw@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `cdps-1.0.3/README.md` & `cdps-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cdps-1.0.3/cdps.egg-info/PKG-INFO` & `cdps-1.0.4/cdps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdps
-Version: 1.0.3
+Version: 1.0.4
 Summary: Composite Disaster Prevention Server
 Home-page: UNKNOWN
 Author: ExpTechTW
 Author-email: exptech.tw@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `cdps-1.0.3/setup.py` & `cdps-1.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from CDPS.core.constants import core_constant
+from cdps.core.constants import core_constant
 
 import os
 from setuptools import setup, find_packages
 
 NAME = core_constant.PACKAGE_NAME
 VERSION = core_constant.VERSION
 DESCRIPTION = 'Composite Disaster Prevention Server'
```

