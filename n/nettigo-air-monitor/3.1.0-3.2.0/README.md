# Comparing `tmp/nettigo_air_monitor-3.1.0.tar.gz` & `tmp/nettigo_air_monitor-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nettigo_air_monitor-3.1.0.tar", last modified: Mon May 27 08:15:03 2024, max compression
+gzip compressed data, was "nettigo_air_monitor-3.2.0.tar", last modified: Sat Jun  1 09:06:33 2024, max compression
```

## Comparing `nettigo_air_monitor-3.1.0.tar` & `nettigo_air_monitor-3.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:15:03.498492 nettigo_air_monitor-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-27 08:15:03.498492 nettigo_air_monitor-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:15:03.494492 nettigo_air_monitor-3.1.0/nettigo_air_monitor/
--rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor/const.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor/model.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:15:03.498492 nettigo_air_monitor-3.1.0/nettigo_air_monitor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-05-27 08:15:03.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-27 08:15:03.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-27 08:15:03.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 08:15:03.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-27 08:15:03.000000 nettigo_air_monitor-3.1.0/nettigo_air_monitor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-27 08:15:03.498492 nettigo_air_monitor-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-27 08:15:03.498492 nettigo_air_monitor-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-05-27 08:14:53.000000 nettigo_air_monitor-3.1.0/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:06:33.284689 nettigo_air_monitor-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-06-01 09:06:25.000000 nettigo_air_monitor-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-06-01 09:06:25.000000 nettigo_air_monitor-3.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-06-01 09:06:33.284689 nettigo_air_monitor-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-06-01 09:06:25.000000 nettigo_air_monitor-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:06:33.284689 nettigo_air_monitor-3.2.0/nettigo_air_monitor/
+-rw-r--r--   0 runner    (1001) docker     (127)     7105 2024-06-01 09:06:25.000000 nettigo_air_monitor-3.2.0/nettigo_air_monitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-01 09:06:25.000000 nettigo_air_monitor-3.2.0/nettigo_air_monitor/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-06-01 09:06:25.000000 nettigo_air_monitor-3.2.0/nettigo_air_monitor/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-06-01 09:06:25.000000 nettigo_air_monitor-3.2.0/nettigo_air_monitor/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 09:06:25.000000 nettigo_air_monitor-3.2.0/nettigo_air_monitor/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:06:33.284689 nettigo_air_monitor-3.2.0/nettigo_air_monitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3378 2024-06-01 09:06:33.000000 nettigo_air_monitor-3.2.0/nettigo_air_monitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-06-01 09:06:33.000000 nettigo_air_monitor-3.2.0/nettigo_air_monitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 09:06:33.000000 nettigo_air_monitor-3.2.0/nettigo_air_monitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-01 09:06:33.000000 nettigo_air_monitor-3.2.0/nettigo_air_monitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-06-01 09:06:33.000000 nettigo_air_monitor-3.2.0/nettigo_air_monitor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-06-01 09:06:25.000000 nettigo_air_monitor-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-06-01 09:06:25.000000 nettigo_air_monitor-3.2.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-06-01 09:06:25.000000 nettigo_air_monitor-3.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 09:06:33.284689 nettigo_air_monitor-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-06-01 09:06:25.000000 nettigo_air_monitor-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:06:33.284689 nettigo_air_monitor-3.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13036 2024-06-01 09:06:25.000000 nettigo_air_monitor-3.2.0/tests/test_init.py
```

### Comparing `nettigo_air_monitor-3.1.0/LICENSE` & `nettigo_air_monitor-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-3.1.0/PKG-INFO` & `nettigo_air_monitor-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nettigo_air_monitor
-Version: 3.1.0
+Version: 3.2.0
 Summary: Python wrapper for getting air quality data from Nettigo Air Monitor devices.
 Home-page: https://github.com/bieniu/nettigo-air-monitor
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `nettigo_air_monitor-3.1.0/README.md` & `nettigo_air_monitor-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-3.1.0/nettigo_air_monitor/__init__.py` & `nettigo_air_monitor-3.2.0/nettigo_air_monitor/__init__.py`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-3.1.0/nettigo_air_monitor/const.py` & `nettigo_air_monitor-3.2.0/nettigo_air_monitor/const.py`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-3.1.0/nettigo_air_monitor/exceptions.py` & `nettigo_air_monitor-3.2.0/nettigo_air_monitor/exceptions.py`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-3.1.0/nettigo_air_monitor/model.py` & `nettigo_air_monitor-3.2.0/nettigo_air_monitor/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,14 +34,15 @@
     bme280_temperature: float | None
     bmp180_pressure: float | None
     bmp180_temperature: float | None
     bmp280_pressure: float | None
     bmp280_temperature: float | None
     dht22_humidity: float | None
     dht22_temperature: float | None
+    ds18b20_temperature: float | None
     heca_humidity: float | None
     heca_temperature: float | None
     mhz14a_carbon_dioxide: float | None
     pms_caqi: int | None
     pms_caqi_level: str | None
     pms_p0: float | None
     pms_p1: float | None
```

### Comparing `nettigo_air_monitor-3.1.0/nettigo_air_monitor.egg-info/PKG-INFO` & `nettigo_air_monitor-3.2.0/nettigo_air_monitor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nettigo_air_monitor
-Version: 3.1.0
+Version: 3.2.0
 Summary: Python wrapper for getting air quality data from Nettigo Air Monitor devices.
 Home-page: https://github.com/bieniu/nettigo-air-monitor
 Author: Maciej Bieniek
 License: Apache-2.0 License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `nettigo_air_monitor-3.1.0/pyproject.toml` & `nettigo_air_monitor-3.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `nettigo_air_monitor-3.1.0/setup.py` & `nettigo_air_monitor-3.2.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 
 from setuptools import setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "3.1.0"
+VERSION = "3.2.0"
 
 setup(
     name="nettigo_air_monitor",
     version=VERSION,
     author="Maciej Bieniek",
     description=(
         "Python wrapper for getting air quality data from Nettigo Air Monitor devices."
```

### Comparing `nettigo_air_monitor-3.1.0/tests/test_init.py` & `nettigo_air_monitor-3.2.0/tests/test_init.py`

 * *Files identical despite different names*

