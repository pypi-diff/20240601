# Comparing `tmp/cdps-1.0.7.tar.gz` & `tmp/cdps-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdps-1.0.7.tar", last modified: Sat Jun  1 15:31:54 2024, max compression
+gzip compressed data, was "cdps-1.0.8.tar", last modified: Sat Jun  1 15:33:40 2024, max compression
```

## Comparing `cdps-1.0.7.tar` & `cdps-1.0.8.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 15:31:54.530191 cdps-1.0.7/
--rw-rw-rw-   0        0        0    35184 2024-06-01 14:18:34.000000 cdps-1.0.7/LICENSE
--rw-rw-rw-   0        0        0     1835 2024-06-01 15:31:54.529167 cdps-1.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1036 2024-06-01 14:23:15.000000 cdps-1.0.7/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 15:31:54.495981 cdps-1.0.7/cdps/
--rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/__init__.py
--rw-rw-rw-   0        0        0      116 2024-06-01 15:30:54.000000 cdps-1.0.7/cdps/__main__.py
--rw-rw-rw-   0        0        0      393 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/boostrap.py
--rw-rw-rw-   0        0        0     1688 2024-06-01 15:30:46.000000 cdps-1.0.7/cdps/cdps_server.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:31:54.521497 cdps-1.0.7/cdps/cli/
--rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/cli/__init__.py
--rw-rw-rw-   0        0        0     2328 2024-06-01 15:31:23.000000 cdps-1.0.7/cdps/cli/cli_entry.py
--rw-rw-rw-   0        0        0      226 2024-06-01 15:31:26.000000 cdps-1.0.7/cdps/cli/cli_gendefault.py
--rw-rw-rw-   0        0        0      338 2024-06-01 15:31:31.000000 cdps-1.0.7/cdps/cli/cli_init.py
--rw-rw-rw-   0        0        0      316 2024-06-01 15:31:37.000000 cdps-1.0.7/cdps/cli/cli_run.py
--rw-rw-rw-   0        0        0      185 2024-06-01 15:31:40.000000 cdps-1.0.7/cdps/cli/cli_version.py
--rw-rw-rw-   0        0        0     1210 2024-06-01 15:30:38.000000 cdps-1.0.7/cdps/config.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:31:54.522517 cdps-1.0.7/cdps/constants/
--rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/constants/__init__.py
--rw-rw-rw-   0        0        0      112 2024-06-01 15:31:49.000000 cdps-1.0.7/cdps/constants/core_constant.py
--rw-rw-rw-   0        0        0      588 2024-06-01 15:30:33.000000 cdps-1.0.7/cdps/entrypoint.py
--rw-rw-rw-   0        0        0      401 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/state.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:31:54.529167 cdps-1.0.7/cdps/utils/
--rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/utils/__init__.py
--rw-rw-rw-   0        0        0     1233 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/utils/file_util.py
--rw-rw-rw-   0        0        0      344 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/utils/lazy_item.py
--rw-rw-rw-   0        0        0      265 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/utils/level.py
--rw-rw-rw-   0        0        0      554 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/utils/line.py
--rw-rw-rw-   0        0        0     4397 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/utils/logger.py
--rw-rw-rw-   0        0        0      765 2024-05-21 07:25:40.000000 cdps-1.0.7/cdps/utils/resources_util.py
--rw-rw-rw-   0        0        0     1653 2024-06-01 15:31:08.000000 cdps-1.0.7/cdps/utils/yaml_data_storage.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:31:54.517801 cdps-1.0.7/cdps.egg-info/
--rw-rw-rw-   0        0        0     1835 2024-06-01 15:31:54.000000 cdps-1.0.7/cdps.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      701 2024-06-01 15:31:54.000000 cdps-1.0.7/cdps.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:31:54.000000 cdps-1.0.7/cdps.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       53 2024-06-01 15:31:54.000000 cdps-1.0.7/cdps.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      172 2024-06-01 15:31:54.000000 cdps-1.0.7/cdps.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-06-01 15:31:54.000000 cdps-1.0.7/cdps.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 15:31:54.530191 cdps-1.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1710 2024-06-01 15:27:04.000000 cdps-1.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:33:40.019934 cdps-1.0.8/
+-rw-rw-rw-   0        0        0    35184 2024-06-01 14:18:34.000000 cdps-1.0.8/LICENSE
+-rw-rw-rw-   0        0        0     1835 2024-06-01 15:33:40.018934 cdps-1.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1036 2024-06-01 14:23:15.000000 cdps-1.0.8/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 15:33:39.989606 cdps-1.0.8/cdps/
+-rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/__init__.py
+-rw-rw-rw-   0        0        0      116 2024-06-01 15:30:54.000000 cdps-1.0.8/cdps/__main__.py
+-rw-rw-rw-   0        0        0      393 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/boostrap.py
+-rw-rw-rw-   0        0        0     1688 2024-06-01 15:30:46.000000 cdps-1.0.8/cdps/cdps_server.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:33:40.011902 cdps-1.0.8/cdps/cli/
+-rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/cli/__init__.py
+-rw-rw-rw-   0        0        0     2328 2024-06-01 15:31:23.000000 cdps-1.0.8/cdps/cli/cli_entry.py
+-rw-rw-rw-   0        0        0      226 2024-06-01 15:31:26.000000 cdps-1.0.8/cdps/cli/cli_gendefault.py
+-rw-rw-rw-   0        0        0      338 2024-06-01 15:31:31.000000 cdps-1.0.8/cdps/cli/cli_init.py
+-rw-rw-rw-   0        0        0      316 2024-06-01 15:31:37.000000 cdps-1.0.8/cdps/cli/cli_run.py
+-rw-rw-rw-   0        0        0      185 2024-06-01 15:31:40.000000 cdps-1.0.8/cdps/cli/cli_version.py
+-rw-rw-rw-   0        0        0     1210 2024-06-01 15:30:38.000000 cdps-1.0.8/cdps/config.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:33:40.012902 cdps-1.0.8/cdps/constants/
+-rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/constants/__init__.py
+-rw-rw-rw-   0        0        0      112 2024-06-01 15:33:33.000000 cdps-1.0.8/cdps/constants/core_constant.py
+-rw-rw-rw-   0        0        0      583 2024-06-01 15:32:25.000000 cdps-1.0.8/cdps/entrypoint.py
+-rw-rw-rw-   0        0        0      401 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/state.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:33:40.018934 cdps-1.0.8/cdps/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/utils/__init__.py
+-rw-rw-rw-   0        0        0     1233 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/utils/file_util.py
+-rw-rw-rw-   0        0        0      344 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/utils/lazy_item.py
+-rw-rw-rw-   0        0        0      265 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/utils/level.py
+-rw-rw-rw-   0        0        0      554 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/utils/line.py
+-rw-rw-rw-   0        0        0     4397 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/utils/logger.py
+-rw-rw-rw-   0        0        0      765 2024-05-21 07:25:40.000000 cdps-1.0.8/cdps/utils/resources_util.py
+-rw-rw-rw-   0        0        0     1653 2024-06-01 15:31:08.000000 cdps-1.0.8/cdps/utils/yaml_data_storage.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:33:40.006890 cdps-1.0.8/cdps.egg-info/
+-rw-rw-rw-   0        0        0     1835 2024-06-01 15:33:39.000000 cdps-1.0.8/cdps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      701 2024-06-01 15:33:39.000000 cdps-1.0.8/cdps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:33:39.000000 cdps-1.0.8/cdps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       53 2024-06-01 15:33:39.000000 cdps-1.0.8/cdps.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      172 2024-06-01 15:33:39.000000 cdps-1.0.8/cdps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-06-01 15:33:39.000000 cdps-1.0.8/cdps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:33:40.019934 cdps-1.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1745 2024-06-01 15:33:14.000000 cdps-1.0.8/setup.py
```

### Comparing `cdps-1.0.7/LICENSE` & `cdps-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `cdps-1.0.7/PKG-INFO` & `cdps-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdps
-Version: 1.0.7
+Version: 1.0.8
 Summary: Composite Disaster Prevention Server
 Home-page: UNKNOWN
 Author: ExpTechTW
 Author-email: exptech.tw@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `cdps-1.0.7/README.md` & `cdps-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `cdps-1.0.7/cdps/cdps_server.py` & `cdps-1.0.8/cdps/cdps_server.py`

 * *Files identical despite different names*

### Comparing `cdps-1.0.7/cdps/cli/cli_entry.py` & `cdps-1.0.8/cdps/cli/cli_entry.py`

 * *Files identical despite different names*

### Comparing `cdps-1.0.7/cdps/config.py` & `cdps-1.0.8/cdps/config.py`

 * *Files identical despite different names*

### Comparing `cdps-1.0.7/cdps/entrypoint.py` & `cdps-1.0.8/cdps/entrypoint.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,9 +17,9 @@
         sys.exit(1)
 
 
 def entrypoint():
     boostrap()
     __environment_check()
 
-    from core.cli import cli_entry
+    from cli import cli_entry
     cli_entry.cli_dispatch()
```

### Comparing `cdps-1.0.7/cdps/utils/file_util.py` & `cdps-1.0.8/cdps/utils/file_util.py`

 * *Files identical despite different names*

### Comparing `cdps-1.0.7/cdps/utils/line.py` & `cdps-1.0.8/cdps/utils/line.py`

 * *Files identical despite different names*

### Comparing `cdps-1.0.7/cdps/utils/logger.py` & `cdps-1.0.8/cdps/utils/logger.py`

 * *Files identical despite different names*

### Comparing `cdps-1.0.7/cdps/utils/resources_util.py` & `cdps-1.0.8/cdps/utils/resources_util.py`

 * *Files identical despite different names*

### Comparing `cdps-1.0.7/cdps/utils/yaml_data_storage.py` & `cdps-1.0.8/cdps/utils/yaml_data_storage.py`

 * *Files identical despite different names*

### Comparing `cdps-1.0.7/cdps.egg-info/PKG-INFO` & `cdps-1.0.8/cdps.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdps
-Version: 1.0.7
+Version: 1.0.8
 Summary: Composite Disaster Prevention Server
 Home-page: UNKNOWN
 Author: ExpTechTW
 Author-email: exptech.tw@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `cdps-1.0.7/cdps.egg-info/SOURCES.txt` & `cdps-1.0.8/cdps.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cdps-1.0.7/setup.py` & `cdps-1.0.8/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -42,14 +42,14 @@
     name=NAME,
     version=VERSION,
     description=DESCRIPTION,
 	long_description=LONG_DESCRIPTION,
 	long_description_content_type='text/markdown',
     author=AUTHOR,
     author_email='exptech.tw@gmail.com',
-    packages=find_packages(exclude=['tests']),
+    packages=find_packages(exclude=['tests', '*.tests', '*.tests.*', 'tests.*']),
     include_package_data=True,
 	python_requires=REQUIRES_PYTHON,
 	install_requires=REQUIRED,
 	classifiers=CLASSIFIERS,
 	entry_points=ENTRY_POINTS,
 )
```

