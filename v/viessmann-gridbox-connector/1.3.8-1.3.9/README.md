# Comparing `tmp/viessmann_gridbox_connector-1.3.8.tar.gz` & `tmp/viessmann_gridbox_connector-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viessmann_gridbox_connector-1.3.8.tar", last modified: Fri May 10 05:51:28 2024, max compression
+gzip compressed data, was "viessmann_gridbox_connector-1.3.9.tar", last modified: Sat Jun  1 00:15:31 2024, max compression
```

## Comparing `viessmann_gridbox_connector-1.3.8.tar` & `viessmann_gridbox_connector-1.3.9.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:51:28.262531 viessmann_gridbox_connector-1.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-10 05:51:24.000000 viessmann_gridbox_connector-1.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-10 05:51:28.262531 viessmann_gridbox_connector-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-10 05:51:24.000000 viessmann_gridbox_connector-1.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:51:28.262531 viessmann_gridbox_connector-1.3.8/gridbox_connector/
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-10 05:51:24.000000 viessmann_gridbox_connector-1.3.8/gridbox_connector/GridboxConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-10 05:51:24.000000 viessmann_gridbox_connector-1.3.8/gridbox_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      388 2024-05-10 05:51:24.000000 viessmann_gridbox_connector-1.3.8/gridbox_connector/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 05:51:28.262531 viessmann_gridbox_connector-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-10 05:51:24.000000 viessmann_gridbox_connector-1.3.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 05:51:28.262531 viessmann_gridbox_connector-1.3.8/viessmann_gridbox_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-10 05:51:28.000000 viessmann_gridbox_connector-1.3.8/viessmann_gridbox_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-05-10 05:51:28.000000 viessmann_gridbox_connector-1.3.8/viessmann_gridbox_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 05:51:28.000000 viessmann_gridbox_connector-1.3.8/viessmann_gridbox_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-10 05:51:28.000000 viessmann_gridbox_connector-1.3.8/viessmann_gridbox_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-10 05:51:28.000000 viessmann_gridbox_connector-1.3.8/viessmann_gridbox_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:15:31.568275 viessmann_gridbox_connector-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-06-01 00:15:27.000000 viessmann_gridbox_connector-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-06-01 00:15:31.568275 viessmann_gridbox_connector-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-06-01 00:15:27.000000 viessmann_gridbox_connector-1.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:15:31.568275 viessmann_gridbox_connector-1.3.9/gridbox_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-06-01 00:15:27.000000 viessmann_gridbox_connector-1.3.9/gridbox_connector/GridboxConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-06-01 00:15:27.000000 viessmann_gridbox_connector-1.3.9/gridbox_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 00:15:31.568275 viessmann_gridbox_connector-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-06-01 00:15:27.000000 viessmann_gridbox_connector-1.3.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:15:31.568275 viessmann_gridbox_connector-1.3.9/viessmann_gridbox_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-06-01 00:15:31.000000 viessmann_gridbox_connector-1.3.9/viessmann_gridbox_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-06-01 00:15:31.000000 viessmann_gridbox_connector-1.3.9/viessmann_gridbox_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:15:31.000000 viessmann_gridbox_connector-1.3.9/viessmann_gridbox_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 00:15:31.000000 viessmann_gridbox_connector-1.3.9/viessmann_gridbox_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 00:15:31.000000 viessmann_gridbox_connector-1.3.9/viessmann_gridbox_connector.egg-info/top_level.txt
```

### Comparing `viessmann_gridbox_connector-1.3.8/LICENSE` & `viessmann_gridbox_connector-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `viessmann_gridbox_connector-1.3.8/PKG-INFO` & `viessmann_gridbox_connector-1.3.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,13 @@
-Metadata-Version: 2.1
-Name: viessmann-gridbox-connector
-Version: 1.3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-
 # Viessmann Gridbox Connector
-**This is not an official Viessmann library**
+### **<h3 style="text-align: center;">This is not an official Viessmann library</h3>**
 
 a GridboxConnector Lib to fetch your Data from the Cloud.
 It is using the same Rest-API like the Dashboard and the App.
+![Screenshot vom mygridbox](images/screenshot.png)
 
 ## Installation
 ```script shell
 pip install viessmann-gridbox-connector
 ```
 Set your email and password in the config.json. 
 Use your Login Data from the App or from https://mygridbox.viessmann.com/login
```

### Comparing `viessmann_gridbox_connector-1.3.8/README.md` & `viessmann_gridbox_connector-1.3.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,20 @@
+Metadata-Version: 2.1
+Name: viessmann-gridbox-connector
+Version: 1.3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+
 # Viessmann Gridbox Connector
-**This is not an official Viessmann library**
+### **<h3 style="text-align: center;">This is not an official Viessmann library</h3>**
 
 a GridboxConnector Lib to fetch your Data from the Cloud.
 It is using the same Rest-API like the Dashboard and the App.
+![Screenshot vom mygridbox](images/screenshot.png)
 
 ## Installation
 ```script shell
 pip install viessmann-gridbox-connector
 ```
 Set your email and password in the config.json. 
 Use your Login Data from the App or from https://mygridbox.viessmann.com/login
```

### Comparing `viessmann_gridbox_connector-1.3.8/viessmann_gridbox_connector.egg-info/PKG-INFO` & `viessmann_gridbox_connector-1.3.9/viessmann_gridbox_connector.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: viessmann-gridbox-connector
-Version: 1.3.8
+Version: 1.3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # Viessmann Gridbox Connector
-**This is not an official Viessmann library**
+### **<h3 style="text-align: center;">This is not an official Viessmann library</h3>**
 
 a GridboxConnector Lib to fetch your Data from the Cloud.
 It is using the same Rest-API like the Dashboard and the App.
+![Screenshot vom mygridbox](images/screenshot.png)
 
 ## Installation
 ```script shell
 pip install viessmann-gridbox-connector
 ```
 Set your email and password in the config.json. 
 Use your Login Data from the App or from https://mygridbox.viessmann.com/login
```

