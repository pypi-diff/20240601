# Comparing `tmp/dwd_global_radiation-1.1.0rc4.tar.gz` & `tmp/dwd_global_radiation-1.1.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dwd_global_radiation-1.1.0rc4.tar", last modified: Thu May 30 17:03:37 2024, max compression
+gzip compressed data, was "dwd_global_radiation-1.1.0rc5.tar", last modified: Sat Jun  1 11:02:44 2024, max compression
```

## Comparing `dwd_global_radiation-1.1.0rc4.tar` & `dwd_global_radiation-1.1.0rc5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-30 17:03:37.540764 dwd_global_radiation-1.1.0rc4/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1065 2024-05-05 09:59:58.000000 dwd_global_radiation-1.1.0rc4/LICENSE
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-30 17:03:37.540764 dwd_global_radiation-1.1.0rc4/PKG-INFO
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    21423 2024-05-30 17:02:04.000000 dwd_global_radiation-1.1.0rc4/README.md
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-30 17:03:37.536764 dwd_global_radiation-1.1.0rc4/dwd_global_radiation/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       45 2024-05-27 15:10:26.000000 dwd_global_radiation-1.1.0rc4/dwd_global_radiation/__init__.py
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    27369 2024-05-30 17:02:04.000000 dwd_global_radiation-1.1.0rc4/dwd_global_radiation/global_radiation.py
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)     7298 2024-05-30 17:02:04.000000 dwd_global_radiation-1.1.0rc4/dwd_global_radiation/global_radiation_printer.py
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    20227 2024-05-30 17:02:04.000000 dwd_global_radiation-1.1.0rc4/dwd_global_radiation/utils.py
-drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-05-30 17:03:37.540764 dwd_global_radiation-1.1.0rc4/dwd_global_radiation.egg-info/
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-05-30 17:03:37.000000 dwd_global_radiation-1.1.0rc4/dwd_global_radiation.egg-info/PKG-INFO
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)      398 2024-05-30 17:03:37.000000 dwd_global_radiation-1.1.0rc4/dwd_global_radiation.egg-info/SOURCES.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)        1 2024-05-30 17:03:37.000000 dwd_global_radiation-1.1.0rc4/dwd_global_radiation.egg-info/dependency_links.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)      128 2024-05-30 17:03:37.000000 dwd_global_radiation-1.1.0rc4/dwd_global_radiation.egg-info/requires.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       21 2024-05-30 17:03:37.000000 dwd_global_radiation-1.1.0rc4/dwd_global_radiation.egg-info/top_level.txt
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)       38 2024-05-30 17:03:37.540764 dwd_global_radiation-1.1.0rc4/setup.cfg
--rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1656 2024-05-30 17:02:04.000000 dwd_global_radiation-1.1.0rc4/setup.py
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-06-01 11:02:44.310955 dwd_global_radiation-1.1.0rc5/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1065 2024-05-05 09:59:58.000000 dwd_global_radiation-1.1.0rc5/LICENSE
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-06-01 11:02:44.310955 dwd_global_radiation-1.1.0rc5/PKG-INFO
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    21423 2024-05-30 17:02:04.000000 dwd_global_radiation-1.1.0rc5/README.md
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-06-01 11:02:44.306955 dwd_global_radiation-1.1.0rc5/dwd_global_radiation/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       45 2024-05-27 15:10:26.000000 dwd_global_radiation-1.1.0rc5/dwd_global_radiation/__init__.py
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    29091 2024-06-01 10:32:57.000000 dwd_global_radiation-1.1.0rc5/dwd_global_radiation/global_radiation.py
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)     7298 2024-05-30 17:02:04.000000 dwd_global_radiation-1.1.0rc5/dwd_global_radiation/global_radiation_printer.py
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    20227 2024-05-30 17:02:04.000000 dwd_global_radiation-1.1.0rc5/dwd_global_radiation/utils.py
+drwxr-xr-x   0 piadmin   (1000) piadmin   (1000)        0 2024-06-01 11:02:44.310955 dwd_global_radiation-1.1.0rc5/dwd_global_radiation.egg-info/
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)    22430 2024-06-01 11:02:44.000000 dwd_global_radiation-1.1.0rc5/dwd_global_radiation.egg-info/PKG-INFO
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)      398 2024-06-01 11:02:44.000000 dwd_global_radiation-1.1.0rc5/dwd_global_radiation.egg-info/SOURCES.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)        1 2024-06-01 11:02:44.000000 dwd_global_radiation-1.1.0rc5/dwd_global_radiation.egg-info/dependency_links.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)      128 2024-06-01 11:02:44.000000 dwd_global_radiation-1.1.0rc5/dwd_global_radiation.egg-info/requires.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       21 2024-06-01 11:02:44.000000 dwd_global_radiation-1.1.0rc5/dwd_global_radiation.egg-info/top_level.txt
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)       38 2024-06-01 11:02:44.310955 dwd_global_radiation-1.1.0rc5/setup.cfg
+-rw-r--r--   0 piadmin   (1000) piadmin   (1000)     1656 2024-06-01 10:53:19.000000 dwd_global_radiation-1.1.0rc5/setup.py
```

### Comparing `dwd_global_radiation-1.1.0rc4/LICENSE` & `dwd_global_radiation-1.1.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.1.0rc4/PKG-INFO` & `dwd_global_radiation-1.1.0rc5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwd_global_radiation
-Version: 1.1.0rc4
+Version: 1.1.0rc5
 Summary: Access and analyze DWD global radiation data and forecasts
 Home-page: https://github.com/aschmere/dwd_global_radiation
 Author: Arno Schmerer
 License: MIT
 Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dwd_global_radiation-1.1.0rc4/README.md` & `dwd_global_radiation-1.1.0rc5/README.md`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.1.0rc4/dwd_global_radiation/global_radiation.py` & `dwd_global_radiation-1.1.0rc5/dwd_global_radiation/global_radiation.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 """
 
 import datetime as dtbase
 import logging
 from dataclasses import dataclass, field
 from datetime import datetime, timedelta, timezone
 from typing import Any
+import json
 
 import numpy as np
 import tzlocal
 
 from . import utils
 from .global_radiation_printer import (
     FormatConfig,
@@ -110,14 +111,55 @@
             "name": self.name,
             "measurements": [
                 measurement.to_dict() for measurement in self.measurements
             ],
             "forecasts": [forecast.to_dict() for forecast in self.forecasts],
         }
 
+    def get_forecast_for_future_hour(self, datetime_input, number_of_hours):
+        """
+        Retrieves the forecast for a specific hour in the future.
+
+        Args:
+            datetime_input (datetime): The base datetime from which to calculate the future hour.
+            number_of_hours (int): The number of hours into the future for which to
+            retrieve the forecast.
+
+        Returns:
+            str: A JSON string containing the forecast timestamp in UTC and sis (Global Radiation)
+                 value, or an error message if no forecast is found for the specified time.
+        """
+        # Ensure datetime_input is in UTC
+        datetime_input = datetime_input.astimezone(timezone.utc)
+
+        # Find the index of the forecast entry that is at or just after datetime_input
+        start_index = 0
+        while (
+            start_index < len(self.forecasts[0].entries)
+            and self.forecasts[0].entries[start_index].timestamp
+            < datetime_input.timestamp()
+        ):
+            start_index += 1
+
+        # Calculate the target index
+        target_index = start_index + number_of_hours - 1
+
+        if target_index < len(self.forecasts[0].entries):
+            forecast_entry = self.forecasts[0].entries[target_index]
+            return json.dumps(
+                {
+                    "timestamp": datetime.fromtimestamp(
+                        forecast_entry.timestamp, tz=timezone.utc
+                    ).strftime("%Y-%m-%dT%H:%M:%S%z"),
+                    "sis": round(forecast_entry.sis),
+                }
+            )
+
+        return json.dumps({"error": "No forecast found for the specified time"})
+
 
 @dataclass
 class MeasurementEntry:
     """Class for storing DWD global radiation measurement data."""
 
     timestamp: float  # assuming timestamp is a Unix time float
     sis: float  # Solar Irradiance in W/m^2
@@ -260,14 +302,16 @@
 
     def to_dict(self):
         """Convert ForecastEntry to a dictionary."""
         return {
             "timestamp": float(self.timestamp),  # Explicit conversion to float
             "sis": float(self.sis),  # Explicit conversion to float
         }
+
+
 @dataclass
 class GlobalRadiation:
     """This is the main class of the DWD Global Radiation Observation and Forecast Data Library
     It gets instantiated by every program using this library. It stores the whole dataclass
     hierarchy for storing the DWD forecast and measurement data. It also provides the main methods
     for retrieving the data from DWD servers via http file download."""
 
@@ -314,17 +358,20 @@
         title, labels, dt_format = get_language_details(language)
         format_config = FormatConfig(dt_format=dt_format, local_tz=local_tz)
         config = PrintConfig(labels=labels, format_config=format_config)
 
         print_header(title)
         for location in self.locations:
             print(f"{config.labels['location']}: {location.name}")
-            print(f"{config.indent_config.indent}{config.labels['latitude']}: {location.latitude}")
             print(
-                f"{config.indent_config.indent}{config.labels['longitude']}: {location.longitude}")
+                f"{config.indent_config.indent}{config.labels['latitude']}: {location.latitude}"
+            )
+            print(
+                f"{config.indent_config.indent}{config.labels['longitude']}: {location.longitude}"
+            )
 
             if location.measurements:
                 print_measurements(location.measurements, config)
             if location.forecasts:
                 print_forecasts(location.forecasts, config)
 
     def add_location(self, *, latitude=None, longitude=None, name=None):
```

### Comparing `dwd_global_radiation-1.1.0rc4/dwd_global_radiation/global_radiation_printer.py` & `dwd_global_radiation-1.1.0rc5/dwd_global_radiation/global_radiation_printer.py`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.1.0rc4/dwd_global_radiation/utils.py` & `dwd_global_radiation-1.1.0rc5/dwd_global_radiation/utils.py`

 * *Files identical despite different names*

### Comparing `dwd_global_radiation-1.1.0rc4/dwd_global_radiation.egg-info/PKG-INFO` & `dwd_global_radiation-1.1.0rc5/dwd_global_radiation.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dwd_global_radiation
-Version: 1.1.0rc4
+Version: 1.1.0rc5
 Summary: Access and analyze DWD global radiation data and forecasts
 Home-page: https://github.com/aschmere/dwd_global_radiation
 Author: Arno Schmerer
 License: MIT
 Keywords: weather meteorology radiation solar forecasting DWD data environmental data climate studies solar energy forecasting
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `dwd_global_radiation-1.1.0rc4/setup.py` & `dwd_global_radiation-1.1.0rc5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='dwd_global_radiation',
-    version='1.1.0rc4',
+    version='1.1.0rc5',
     packages=find_packages(),
     description='Access and analyze DWD global radiation data and forecasts',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/aschmere/dwd_global_radiation',
     author='Arno Schmerer',
     license='MIT',
```

