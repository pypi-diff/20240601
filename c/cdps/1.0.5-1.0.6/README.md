# Comparing `tmp/cdps-1.0.5.tar.gz` & `tmp/cdps-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdps-1.0.5.tar", last modified: Sat Jun  1 15:23:37 2024, max compression
+gzip compressed data, was "cdps-1.0.6.tar", last modified: Sat Jun  1 15:27:07 2024, max compression
```

## Comparing `cdps-1.0.5.tar` & `cdps-1.0.6.tar`

### file list

```diff
@@ -1,13 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 15:23:37.744772 cdps-1.0.5/
--rw-rw-rw-   0        0        0    35184 2024-06-01 14:18:34.000000 cdps-1.0.5/LICENSE
--rw-rw-rw-   0        0        0     1835 2024-06-01 15:23:37.743785 cdps-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2024-06-01 14:23:15.000000 cdps-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 15:23:37.742806 cdps-1.0.5/cdps.egg-info/
--rw-rw-rw-   0        0        0     1835 2024-06-01 15:23:37.000000 cdps-1.0.5/cdps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2024-06-01 15:23:37.000000 cdps-1.0.5/cdps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:23:37.000000 cdps-1.0.5/cdps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2024-06-01 15:23:37.000000 cdps-1.0.5/cdps.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      172 2024-06-01 15:23:37.000000 cdps-1.0.5/cdps.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:23:37.000000 cdps-1.0.5/cdps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 15:23:37.744772 cdps-1.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1720 2024-06-01 15:23:17.000000 cdps-1.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:27:07.406601 cdps-1.0.6/
+-rw-rw-rw-   0        0        0    35184 2024-06-01 14:18:34.000000 cdps-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1835 2024-06-01 15:27:07.405611 cdps-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1036 2024-06-01 14:23:15.000000 cdps-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 15:27:07.363858 cdps-1.0.6/cdps/
+-rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/__main__.py
+-rw-rw-rw-   0        0        0      393 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/boostrap.py
+-rw-rw-rw-   0        0        0     1708 2024-06-01 15:18:23.000000 cdps-1.0.6/cdps/cdps_server.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:27:07.398595 cdps-1.0.6/cdps/cli/
+-rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/cli/__init__.py
+-rw-rw-rw-   0        0        0     2353 2024-05-23 16:49:32.000000 cdps-1.0.6/cdps/cli/cli_entry.py
+-rw-rw-rw-   0        0        0      231 2024-06-01 15:19:05.000000 cdps-1.0.6/cdps/cli/cli_gendefault.py
+-rw-rw-rw-   0        0        0      348 2024-06-01 15:19:01.000000 cdps-1.0.6/cdps/cli/cli_init.py
+-rw-rw-rw-   0        0        0      326 2024-06-01 15:18:55.000000 cdps-1.0.6/cdps/cli/cli_run.py
+-rw-rw-rw-   0        0        0      190 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/cli/cli_version.py
+-rw-rw-rw-   0        0        0     1215 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/config.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:27:07.399637 cdps-1.0.6/cdps/constants/
+-rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/constants/__init__.py
+-rw-rw-rw-   0        0        0      112 2024-06-01 15:26:51.000000 cdps-1.0.6/cdps/constants/core_constant.py
+-rw-rw-rw-   0        0        0      598 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/entrypoint.py
+-rw-rw-rw-   0        0        0      401 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/state.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:27:07.405611 cdps-1.0.6/cdps/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/utils/__init__.py
+-rw-rw-rw-   0        0        0     1233 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/utils/file_util.py
+-rw-rw-rw-   0        0        0      344 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/utils/lazy_item.py
+-rw-rw-rw-   0        0        0      265 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/utils/level.py
+-rw-rw-rw-   0        0        0      554 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/utils/line.py
+-rw-rw-rw-   0        0        0     4397 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/utils/logger.py
+-rw-rw-rw-   0        0        0      765 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/utils/resources_util.py
+-rw-rw-rw-   0        0        0     1663 2024-05-21 07:25:40.000000 cdps-1.0.6/cdps/utils/yaml_data_storage.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:27:07.393890 cdps-1.0.6/cdps.egg-info/
+-rw-rw-rw-   0        0        0     1835 2024-06-01 15:27:07.000000 cdps-1.0.6/cdps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      701 2024-06-01 15:27:07.000000 cdps-1.0.6/cdps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:27:07.000000 cdps-1.0.6/cdps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-06-01 15:27:07.000000 cdps-1.0.6/cdps.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      172 2024-06-01 15:27:07.000000 cdps-1.0.6/cdps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-06-01 15:27:07.000000 cdps-1.0.6/cdps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:27:07.406601 cdps-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1710 2024-06-01 15:27:04.000000 cdps-1.0.6/setup.py
```

### Comparing `cdps-1.0.5/LICENSE` & `cdps-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cdps-1.0.5/PKG-INFO` & `cdps-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdps
-Version: 1.0.5
+Version: 1.0.6
 Summary: Composite Disaster Prevention Server
 Home-page: UNKNOWN
 Author: ExpTechTW
 Author-email: exptech.tw@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `cdps-1.0.5/README.md` & `cdps-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cdps-1.0.5/cdps.egg-info/PKG-INFO` & `cdps-1.0.6/cdps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdps
-Version: 1.0.5
+Version: 1.0.6
 Summary: Composite Disaster Prevention Server
 Home-page: UNKNOWN
 Author: ExpTechTW
 Author-email: exptech.tw@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `cdps-1.0.5/setup.py` & `cdps-1.0.6/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cdps.core.constants import core_constant
+from cdps.constants import core_constant
 
 import os
 from setuptools import setup, find_packages
 
 NAME = core_constant.PACKAGE_NAME
 VERSION = core_constant.VERSION
 DESCRIPTION = 'Composite Disaster Prevention Server'
@@ -20,15 +20,15 @@
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
 ]
 
 ENTRY_POINTS = {
 	'console_scripts': [
-		'{} = {}.core.entrypoint:entrypoint'.format(core_constant.CLI_COMMAND, core_constant.PACKAGE_NAME)
+		'{} = {}.entrypoint:entrypoint'.format(core_constant.CLI_COMMAND, core_constant.PACKAGE_NAME)
 	]
 }
 print('ENTRY_POINTS = {}'.format(ENTRY_POINTS))
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, 'requirements.txt')) as f:
```

