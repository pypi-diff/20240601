# Comparing `tmp/redbacktechpy-2024.5.0b1.tar.gz` & `tmp/redbacktechpy-2024.5.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbacktechpy-2024.5.0b1.tar", last modified: Fri May 31 01:52:31 2024, max compression
+gzip compressed data, was "redbacktechpy-2024.5.0b2.tar", last modified: Fri May 31 03:19:42 2024, max compression
```

## Comparing `redbacktechpy-2024.5.0b1.tar` & `redbacktechpy-2024.5.0b2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:52:31.191617 redbacktechpy-2024.5.0b1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 01:52:26.000000 redbacktechpy-2024.5.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-31 01:52:31.191617 redbacktechpy-2024.5.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-31 01:52:26.000000 redbacktechpy-2024.5.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 01:52:31.191617 redbacktechpy-2024.5.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:52:31.187617 redbacktechpy-2024.5.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:52:31.187617 redbacktechpy-2024.5.0b1/src/redbacktechpy/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-31 01:52:26.000000 redbacktechpy-2024.5.0b1/src/redbacktechpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-31 01:52:26.000000 redbacktechpy-2024.5.0b1/src/redbacktechpy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-31 01:52:26.000000 redbacktechpy-2024.5.0b1/src/redbacktechpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-31 01:52:26.000000 redbacktechpy-2024.5.0b1/src/redbacktechpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    26182 2024-05-31 01:52:26.000000 redbacktechpy-2024.5.0b1/src/redbacktechpy/redbacktech_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-31 01:52:26.000000 redbacktechpy-2024.5.0b1/src/redbacktechpy/str_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 01:52:31.187617 redbacktechpy-2024.5.0b1/src/redbacktechpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-31 01:52:31.000000 redbacktechpy-2024.5.0b1/src/redbacktechpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-31 01:52:31.000000 redbacktechpy-2024.5.0b1/src/redbacktechpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 01:52:31.000000 redbacktechpy-2024.5.0b1/src/redbacktechpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 01:52:31.000000 redbacktechpy-2024.5.0b1/src/redbacktechpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-31 01:52:31.000000 redbacktechpy-2024.5.0b1/src/redbacktechpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:19:42.642428 redbacktechpy-2024.5.0b2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 03:19:33.000000 redbacktechpy-2024.5.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-31 03:19:42.642428 redbacktechpy-2024.5.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-31 03:19:33.000000 redbacktechpy-2024.5.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 03:19:42.642428 redbacktechpy-2024.5.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:19:42.638428 redbacktechpy-2024.5.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:19:42.642428 redbacktechpy-2024.5.0b2/src/redbacktechpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-31 03:19:33.000000 redbacktechpy-2024.5.0b2/src/redbacktechpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2117 2024-05-31 03:19:33.000000 redbacktechpy-2024.5.0b2/src/redbacktechpy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-31 03:19:33.000000 redbacktechpy-2024.5.0b2/src/redbacktechpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-05-31 03:19:33.000000 redbacktechpy-2024.5.0b2/src/redbacktechpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26185 2024-05-31 03:19:33.000000 redbacktechpy-2024.5.0b2/src/redbacktechpy/redbacktech_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-31 03:19:33.000000 redbacktechpy-2024.5.0b2/src/redbacktechpy/str_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 03:19:42.642428 redbacktechpy-2024.5.0b2/src/redbacktechpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-31 03:19:42.000000 redbacktechpy-2024.5.0b2/src/redbacktechpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-31 03:19:42.000000 redbacktechpy-2024.5.0b2/src/redbacktechpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 03:19:42.000000 redbacktechpy-2024.5.0b2/src/redbacktechpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 03:19:42.000000 redbacktechpy-2024.5.0b2/src/redbacktechpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-31 03:19:42.000000 redbacktechpy-2024.5.0b2/src/redbacktechpy.egg-info/top_level.txt
```

### Comparing `redbacktechpy-2024.5.0b1/LICENSE` & `redbacktechpy-2024.5.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.0b1/PKG-INFO` & `redbacktechpy-2024.5.0b2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.0b1
+Version: 2024.5.0b2
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `redbacktechpy-2024.5.0b1/pyproject.toml` & `redbacktechpy-2024.5.0b2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "redbacktechpy"
-version = "2024.05.0b1"
+version = "2024.05.0b2"
 authors = [
   { name="Chris Abberley", email="unlisted@gmail.com" },
 ]
 description = "Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
```

### Comparing `redbacktechpy-2024.5.0b1/src/redbacktechpy/__init__.py` & `redbacktechpy-2024.5.0b2/src/redbacktechpy/__init__.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.0b1/src/redbacktechpy/constants.py` & `redbacktechpy-2024.5.0b2/src/redbacktechpy/constants.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.0b1/src/redbacktechpy/model.py` & `redbacktechpy-2024.5.0b2/src/redbacktechpy/model.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.0b1/src/redbacktechpy/redbacktech_client.py` & `redbacktechpy-2024.5.0b2/src/redbacktechpy/redbacktech_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,16 +66,16 @@
                     
                 if device['device_type'] == 'battery':
                     bat_instance, bat_id = await self._handle_battery(device)
                     battery_data[bat_id] = bat_instance
                     
         
         return RedbackTechData(
-            user_id: self.client_id
-            inverters = inverter_data
+            user_id = self.client_id,
+            inverters = inverter_data,
             batterys = battery_data
         )
         
     async def api_login(self) -> None:
         """Login to Redback API and obtain token."""
         login_url = f'{BaseUrl.API}{Endpoint.API_AUTH}'
```

### Comparing `redbacktechpy-2024.5.0b1/src/redbacktechpy/str_enum.py` & `redbacktechpy-2024.5.0b2/src/redbacktechpy/str_enum.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.0b1/src/redbacktechpy.egg-info/PKG-INFO` & `redbacktechpy-2024.5.0b2/src/redbacktechpy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.0b1
+Version: 2024.5.0b2
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

