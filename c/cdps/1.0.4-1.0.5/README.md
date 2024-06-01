# Comparing `tmp/cdps-1.0.4.tar.gz` & `tmp/cdps-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdps-1.0.4.tar", last modified: Sat Jun  1 15:19:34 2024, max compression
+gzip compressed data, was "cdps-1.0.5.tar", last modified: Sat Jun  1 15:23:37 2024, max compression
```

## Comparing `cdps-1.0.4.tar` & `cdps-1.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 15:19:34.810805 cdps-1.0.4/
--rw-rw-rw-   0        0        0    35184 2024-06-01 14:18:34.000000 cdps-1.0.4/LICENSE
--rw-rw-rw-   0        0        0     1835 2024-06-01 15:19:34.810805 cdps-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2024-06-01 14:23:15.000000 cdps-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 15:19:34.809805 cdps-1.0.4/cdps.egg-info/
--rw-rw-rw-   0        0        0     1835 2024-06-01 15:19:34.000000 cdps-1.0.4/cdps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2024-06-01 15:19:34.000000 cdps-1.0.4/cdps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:19:34.000000 cdps-1.0.4/cdps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-06-01 15:19:34.000000 cdps-1.0.4/cdps.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      172 2024-06-01 15:19:34.000000 cdps-1.0.4/cdps.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:19:34.000000 cdps-1.0.4/cdps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 15:19:34.811805 cdps-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1715 2024-06-01 15:18:12.000000 cdps-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:23:37.744772 cdps-1.0.5/
+-rw-rw-rw-   0        0        0    35184 2024-06-01 14:18:34.000000 cdps-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1835 2024-06-01 15:23:37.743785 cdps-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     1036 2024-06-01 14:23:15.000000 cdps-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 15:23:37.742806 cdps-1.0.5/cdps.egg-info/
+-rw-rw-rw-   0        0        0     1835 2024-06-01 15:23:37.000000 cdps-1.0.5/cdps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2024-06-01 15:23:37.000000 cdps-1.0.5/cdps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:23:37.000000 cdps-1.0.5/cdps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2024-06-01 15:23:37.000000 cdps-1.0.5/cdps.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      172 2024-06-01 15:23:37.000000 cdps-1.0.5/cdps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:23:37.000000 cdps-1.0.5/cdps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:23:37.744772 cdps-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1720 2024-06-01 15:23:17.000000 cdps-1.0.5/setup.py
```

### Comparing `cdps-1.0.4/LICENSE` & `cdps-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cdps-1.0.4/PKG-INFO` & `cdps-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdps
-Version: 1.0.4
+Version: 1.0.5
 Summary: Composite Disaster Prevention Server
 Home-page: UNKNOWN
 Author: ExpTechTW
 Author-email: exptech.tw@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `cdps-1.0.4/README.md` & `cdps-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cdps-1.0.4/cdps.egg-info/PKG-INFO` & `cdps-1.0.5/cdps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdps
-Version: 1.0.4
+Version: 1.0.5
 Summary: Composite Disaster Prevention Server
 Home-page: UNKNOWN
 Author: ExpTechTW
 Author-email: exptech.tw@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `cdps-1.0.4/setup.py` & `cdps-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3.12',
 ]
 
 ENTRY_POINTS = {
 	'console_scripts': [
-		'{} = {}.entrypoint:entrypoint'.format(core_constant.CLI_COMMAND, core_constant.PACKAGE_NAME)
+		'{} = {}.core.entrypoint:entrypoint'.format(core_constant.CLI_COMMAND, core_constant.PACKAGE_NAME)
 	]
 }
 print('ENTRY_POINTS = {}'.format(ENTRY_POINTS))
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with open(os.path.join(here, 'requirements.txt')) as f:
```

