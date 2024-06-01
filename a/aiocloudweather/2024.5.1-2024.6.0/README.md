# Comparing `tmp/aiocloudweather-2024.5.1.tar.gz` & `tmp/aiocloudweather-2024.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiocloudweather-2024.5.1.tar", last modified: Thu May 30 21:15:10 2024, max compression
+gzip compressed data, was "aiocloudweather-2024.6.0.tar", last modified: Sat Jun  1 20:25:10 2024, max compression
```

## Comparing `aiocloudweather-2024.5.1.tar` & `aiocloudweather-2024.6.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:15:10.013999 aiocloudweather-2024.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-05-30 21:15:01.000000 aiocloudweather-2024.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-30 21:15:10.013999 aiocloudweather-2024.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-05-30 21:15:01.000000 aiocloudweather-2024.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:15:10.009999 aiocloudweather-2024.5.1/aiocloudweather/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-05-30 21:15:01.000000 aiocloudweather-2024.5.1/aiocloudweather/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-05-30 21:15:01.000000 aiocloudweather-2024.5.1/aiocloudweather/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-30 21:15:01.000000 aiocloudweather-2024.5.1/aiocloudweather/const.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-05-30 21:15:01.000000 aiocloudweather-2024.5.1/aiocloudweather/conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 21:15:01.000000 aiocloudweather-2024.5.1/aiocloudweather/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     4612 2024-05-30 21:15:01.000000 aiocloudweather-2024.5.1/aiocloudweather/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    11472 2024-05-30 21:15:01.000000 aiocloudweather-2024.5.1/aiocloudweather/station.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:15:10.013999 aiocloudweather-2024.5.1/aiocloudweather.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-05-30 21:15:09.000000 aiocloudweather-2024.5.1/aiocloudweather.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-30 21:15:09.000000 aiocloudweather-2024.5.1/aiocloudweather.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:15:09.000000 aiocloudweather-2024.5.1/aiocloudweather.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-30 21:15:09.000000 aiocloudweather-2024.5.1/aiocloudweather.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 21:15:09.000000 aiocloudweather-2024.5.1/aiocloudweather.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-30 21:15:09.000000 aiocloudweather-2024.5.1/aiocloudweather.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-30 21:15:09.000000 aiocloudweather-2024.5.1/aiocloudweather.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-05-30 21:15:10.013999 aiocloudweather-2024.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-05-30 21:15:01.000000 aiocloudweather-2024.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 21:15:10.009999 aiocloudweather-2024.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-05-30 21:15:01.000000 aiocloudweather-2024.5.1/tests/test_conversion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-30 21:15:01.000000 aiocloudweather-2024.5.1/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-30 21:15:01.000000 aiocloudweather-2024.5.1/tests/test_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:25:10.209030 aiocloudweather-2024.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11383 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-01 20:25:10.209030 aiocloudweather-2024.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:25:10.209030 aiocloudweather-2024.6.0/aiocloudweather/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/aiocloudweather/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/aiocloudweather/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/aiocloudweather/const.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/aiocloudweather/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/aiocloudweather/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     4685 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/aiocloudweather/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11388 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/aiocloudweather/station.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:25:10.209030 aiocloudweather-2024.6.0/aiocloudweather.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-06-01 20:25:10.000000 aiocloudweather-2024.6.0/aiocloudweather.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-06-01 20:25:10.000000 aiocloudweather-2024.6.0/aiocloudweather.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 20:25:10.000000 aiocloudweather-2024.6.0/aiocloudweather.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-06-01 20:25:10.000000 aiocloudweather-2024.6.0/aiocloudweather.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 20:25:10.000000 aiocloudweather-2024.6.0/aiocloudweather.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 20:25:10.000000 aiocloudweather-2024.6.0/aiocloudweather.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 20:25:10.000000 aiocloudweather-2024.6.0/aiocloudweather.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-06-01 20:25:10.209030 aiocloudweather-2024.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 20:25:10.209030 aiocloudweather-2024.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/tests/test_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-06-01 20:25:02.000000 aiocloudweather-2024.6.0/tests/test_server.py
```

### Comparing `aiocloudweather-2024.5.1/LICENSE` & `aiocloudweather-2024.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.5.1/PKG-INFO` & `aiocloudweather-2024.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocloudweather
-Version: 2024.5.1
+Version: 2024.6.0
 Summary: Python wrapper for Cloud Weather protocols
 Home-page: https://github.com/lhw/aiocloudweather
 Download-URL: https://github.com/lhw/aiocloudweather
 Author: Lennart Weller
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `aiocloudweather-2024.5.1/aiocloudweather/__main__.py` & `aiocloudweather-2024.6.0/aiocloudweather/__main__.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.5.1/aiocloudweather/const.py` & `aiocloudweather-2024.6.0/aiocloudweather/const.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.5.1/aiocloudweather/conversion.py` & `aiocloudweather-2024.6.0/aiocloudweather/conversion.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,62 +20,49 @@
     return decorator
 
 
 # imperial shenanigans
 @unit(UnitOfTemperature.CELSIUS)
 def fahrenheit_to_celsius(temp_f: float) -> float:
     """Convert Fahrenheit to Celsius."""
-    return (temp_f - 32) * 5.0 / 9.0
+    return round((temp_f - 32) * 5.0 / 9.0, 2)
 
 
 @unit(UnitOfPressure.HPA)
 def inhg_to_hpa(pressure: float) -> float:
     """Convert inches of mercury (inHg) to hectopascals (hPa)."""
-    return pressure * 33.864
+    return round(pressure * 33.864, 2)
 
 
 @unit(UnitOfPrecipitationDepth.MILLIMETERS)
 def in_to_mm(length: float) -> float:
     """Convert inches to millimeters (mm)."""
-    return length * 25.4
-
-
-@unit(UnitOfIrradiance.WATTS_PER_SQUARE_METER)
-def lux_to_wm2(lux: float) -> float:
-    """Convert lux to watts per square meter (W/m²)."""
-    return lux * 0.0079
+    return round(length * 25.4, 2)
 
 
 @unit(UnitOfSpeed.METERS_PER_SECOND)
 def mph_to_ms(speed: float) -> float:
     """Convert miles per hour (mph) to meters per second (m/s)."""
-    return speed * 0.44704
+    return round(speed * 0.44704, 2)
 
 
 @unit(UnitOfPressure.INHG)
 def hpa_to_inhg(pressure: float) -> float:
     """Convert hectopascals (hPa) to inches of mercury (inHg)."""
-    return pressure * 0.02953
+    return round(pressure * 0.02953, 2)
 
 
 @unit(UnitOfTemperature.FAHRENHEIT)
 def celsius_to_fahrenheit(temp_c: float) -> float:
     """Convert Celsius to Fahrenheit."""
-    return temp_c * 9.0 / 5.0 + 32
+    return round(temp_c * 9.0 / 5.0 + 32, 2)
 
 
 @unit(UnitOfPrecipitationDepth.INCHES)
 def mm_to_in(length: float) -> float:
     """Convert millimeters (mm) to inches."""
-    return length * 0.0393701
-
-
-@unit(LIGHT_LUX)
-def wm2_to_lux(lux: float) -> float:
-    """Convert watts per square meter (W/m²) to lux."""
-    return lux * 127
-
+    return round(length * 0.0393701, 2)
 
 @unit(UnitOfSpeed.MILES_PER_HOUR)
 def ms_to_mph(speed: float) -> float:
     """Convert meters per second (m/s) to miles per hour (mph)."""
-    return speed * 2.23694
+    return round(speed * 2.23694, 2)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aiocloudweather-2024.5.1/aiocloudweather/server.py` & `aiocloudweather-2024.6.0/aiocloudweather/server.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,21 +62,18 @@
         instance_data = {}
         for arg, field in dfields.items():
             if arg in data:
                 instance_data[field.name] = field.type(data[arg])
 
         return WeatherStation.from_wunderground(WundergroundRawSensor(**instance_data))
 
-    async def process_weathercloud(self, path: str):
+    async def process_weathercloud(self, segments: list[str]) -> WeatherStation:
         """Process WeatherCloud data."""
 
-        segments = [seg for seg in path.split("/") if seg]
-
-        data = dict(zip(segments[2::2], map(int, segments[3::2])))
-
+        data = dict(zip(segments[::2], map(int, segments[1::2])))
         dfields = {
             f.metadata["arg"]: f
             for f in fields(WeathercloudRawSensor)
             if "arg" in f.metadata
         }
         instance_data = {
             field.name: field.type(data[arg])
@@ -90,19 +87,21 @@
         """AIOHTTP handler for the API."""
 
         if request.method != "GET" or request.path is None:
             raise web.HTTPBadRequest()
 
         station_id: str = None
         dataset: WeatherStation = None
-        if request.path.startswith("/weatherstation/updateweatherstation.php"):
+        if request.path.endswith("/weatherstation/updateweatherstation.php"):
             dataset = await self.process_wunderground(request.query)
             station_id = dataset.station_id
-        elif request.path.startswith("/v01/set"):
-            dataset = await self.process_weathercloud(request.path)
+        elif "/v01/set" in request.path:
+            dataset_path = request.path.split("/v01/set/", 1)[1]
+            path_segments = dataset_path.split("/")
+            dataset = await self.process_weathercloud(path_segments)
             station_id = dataset.station_id
 
         if station_id not in self.stations:
             _LOGGER.debug("Found new station: %s", station_id)
             self.stations.append(station_id)
 
         self.last_updates[station_id] = time.monotonic()
```

### Comparing `aiocloudweather-2024.5.1/aiocloudweather/station.py` & `aiocloudweather-2024.6.0/aiocloudweather/station.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,23 +150,21 @@
     )
 
 
 IMPERIAL_TO_METRIC: Final = {
     UnitOfPressure.INHG: inhg_to_hpa,
     UnitOfTemperature.FAHRENHEIT: fahrenheit_to_celsius,
     UnitOfPrecipitationDepth.INCHES: in_to_mm,
-    LIGHT_LUX: lux_to_wm2,
     UnitOfSpeed.MILES_PER_HOUR: mph_to_ms,
 }
 
 METRIC_TO_IMPERIAL: Final = {
     UnitOfPressure.HPA: hpa_to_inhg,
     UnitOfTemperature.CELSIUS: celsius_to_fahrenheit,
     UnitOfPrecipitationDepth.MILLIMETERS: mm_to_in,
-    UnitOfIrradiance.WATTS_PER_SQUARE_METER: wm2_to_lux,
     UnitOfSpeed.METERS_PER_SECOND: ms_to_mph,
 }
 
 
 @dataclass
 class Sensor:
     """Represents a weather sensor."""
```

### Comparing `aiocloudweather-2024.5.1/aiocloudweather.egg-info/PKG-INFO` & `aiocloudweather-2024.6.0/aiocloudweather.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiocloudweather
-Version: 2024.5.1
+Version: 2024.6.0
 Summary: Python wrapper for Cloud Weather protocols
 Home-page: https://github.com/lhw/aiocloudweather
 Download-URL: https://github.com/lhw/aiocloudweather
 Author: Lennart Weller
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
```

### Comparing `aiocloudweather-2024.5.1/aiocloudweather.egg-info/SOURCES.txt` & `aiocloudweather-2024.6.0/aiocloudweather.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.5.1/setup.cfg` & `aiocloudweather-2024.6.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.5.1/setup.py` & `aiocloudweather-2024.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from pathlib import Path
 
 from setuptools import find_packages, setup
 
 PROJECT_DIR = Path(__file__).parent.resolve()
 README_FILE = PROJECT_DIR / "README.md"
-VERSION = "2024.5.1"
+VERSION = "2024.6.0"
 
 
 setup(
     name="aiocloudweather",
     version=VERSION,
     url="https://github.com/lhw/aiocloudweather",
     download_url="https://github.com/lhw/aiocloudweather",
```

### Comparing `aiocloudweather-2024.5.1/tests/test_conversion.py` & `aiocloudweather-2024.6.0/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.5.1/tests/test_sensor.py` & `aiocloudweather-2024.6.0/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `aiocloudweather-2024.5.1/tests/test_server.py` & `aiocloudweather-2024.6.0/tests/test_server.py`

 * *Files identical despite different names*

