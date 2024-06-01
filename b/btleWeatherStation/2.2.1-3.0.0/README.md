# Comparing `tmp/btleWeatherStation-2.2.1.tar.gz` & `tmp/btleWeatherStation-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "btleWeatherStation-2.2.1.tar", last modified: Thu Mar 30 23:13:19 2023, max compression
+gzip compressed data, was "btleWeatherStation-3.0.0.tar", last modified: Sat Jun  1 18:08:42 2024, max compression
```

## Comparing `btleWeatherStation-2.2.1.tar` & `btleWeatherStation-3.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 rcf       (1000) rcf       (1000)        0 2023-03-30 23:13:19.761038 btleWeatherStation-2.2.1/
--rw-r--r--   0 rcf       (1000) rcf       (1000)     1097 2023-03-30 21:50:31.000000 btleWeatherStation-2.2.1/LICENSE
--rw-r--r--   0 rcf       (1000) rcf       (1000)      964 2023-03-30 23:13:19.757038 btleWeatherStation-2.2.1/PKG-INFO
--rw-r--r--   0 rcf       (1000) rcf       (1000)      487 2023-03-30 21:50:31.000000 btleWeatherStation-2.2.1/README.md
-drwxr-xr-x   0 rcf       (1000) rcf       (1000)        0 2023-03-30 23:13:19.749038 btleWeatherStation-2.2.1/btleWeatherStation/
--rw-r--r--   0 rcf       (1000) rcf       (1000)      332 2023-03-30 23:12:06.000000 btleWeatherStation-2.2.1/btleWeatherStation/__init__.py
--rw-r--r--   0 rcf       (1000) rcf       (1000)     5984 2023-03-30 22:07:32.000000 btleWeatherStation-2.2.1/btleWeatherStation/__main__.py
--rw-r--r--   0 rcf       (1000) rcf       (1000)     4087 2023-03-30 22:02:04.000000 btleWeatherStation-2.2.1/btleWeatherStation/scan.py
--rw-r--r--   0 rcf       (1000) rcf       (1000)    19204 2023-03-30 21:50:31.000000 btleWeatherStation-2.2.1/btleWeatherStation/station.py
-drwxr-xr-x   0 rcf       (1000) rcf       (1000)        0 2023-03-30 23:13:19.757038 btleWeatherStation-2.2.1/btleWeatherStation.egg-info/
--rw-r--r--   0 rcf       (1000) rcf       (1000)      964 2023-03-30 23:13:19.000000 btleWeatherStation-2.2.1/btleWeatherStation.egg-info/PKG-INFO
--rw-r--r--   0 rcf       (1000) rcf       (1000)      354 2023-03-30 23:13:19.000000 btleWeatherStation-2.2.1/btleWeatherStation.egg-info/SOURCES.txt
--rw-r--r--   0 rcf       (1000) rcf       (1000)        1 2023-03-30 23:13:19.000000 btleWeatherStation-2.2.1/btleWeatherStation.egg-info/dependency_links.txt
--rw-r--r--   0 rcf       (1000) rcf       (1000)        7 2023-03-30 23:13:19.000000 btleWeatherStation-2.2.1/btleWeatherStation.egg-info/requires.txt
--rw-r--r--   0 rcf       (1000) rcf       (1000)       19 2023-03-30 23:13:19.000000 btleWeatherStation-2.2.1/btleWeatherStation.egg-info/top_level.txt
--rw-r--r--   0 rcf       (1000) rcf       (1000)       38 2023-03-30 23:13:19.761038 btleWeatherStation-2.2.1/setup.cfg
--rwxr-xr-x   0 rcf       (1000) rcf       (1000)      830 2023-03-30 21:50:31.000000 btleWeatherStation-2.2.1/setup.py
+drwxr-xr-x   0 rcf       (1000) rcf       (1000)        0 2024-06-01 18:08:42.676631 btleWeatherStation-3.0.0/
+-rw-r--r--   0 rcf       (1000) rcf       (1000)     1097 2023-03-30 21:50:31.000000 btleWeatherStation-3.0.0/LICENSE
+-rw-r--r--   0 rcf       (1000) rcf       (1000)      964 2024-06-01 18:08:42.672631 btleWeatherStation-3.0.0/PKG-INFO
+-rw-r--r--   0 rcf       (1000) rcf       (1000)      487 2023-03-30 21:50:31.000000 btleWeatherStation-3.0.0/README.md
+drwxr-xr-x   0 rcf       (1000) rcf       (1000)        0 2024-06-01 18:08:42.664631 btleWeatherStation-3.0.0/btleWeatherStation/
+-rw-r--r--   0 rcf       (1000) rcf       (1000)      332 2024-06-01 18:08:26.000000 btleWeatherStation-3.0.0/btleWeatherStation/__init__.py
+-rw-r--r--   0 rcf       (1000) rcf       (1000)     5276 2024-06-01 18:08:26.000000 btleWeatherStation-3.0.0/btleWeatherStation/__main__.py
+-rw-r--r--   0 rcf       (1000) rcf       (1000)     4087 2024-06-01 18:08:26.000000 btleWeatherStation-3.0.0/btleWeatherStation/scan.py
+-rw-r--r--   0 rcf       (1000) rcf       (1000)    20400 2024-06-01 18:05:38.000000 btleWeatherStation-3.0.0/btleWeatherStation/station.py
+drwxr-xr-x   0 rcf       (1000) rcf       (1000)        0 2024-06-01 18:08:42.672631 btleWeatherStation-3.0.0/btleWeatherStation.egg-info/
+-rw-r--r--   0 rcf       (1000) rcf       (1000)      964 2024-06-01 18:08:42.000000 btleWeatherStation-3.0.0/btleWeatherStation.egg-info/PKG-INFO
+-rw-r--r--   0 rcf       (1000) rcf       (1000)      354 2024-06-01 18:08:42.000000 btleWeatherStation-3.0.0/btleWeatherStation.egg-info/SOURCES.txt
+-rw-r--r--   0 rcf       (1000) rcf       (1000)        1 2024-06-01 18:08:42.000000 btleWeatherStation-3.0.0/btleWeatherStation.egg-info/dependency_links.txt
+-rw-r--r--   0 rcf       (1000) rcf       (1000)        7 2024-06-01 18:08:42.000000 btleWeatherStation-3.0.0/btleWeatherStation.egg-info/requires.txt
+-rw-r--r--   0 rcf       (1000) rcf       (1000)       19 2024-06-01 18:08:42.000000 btleWeatherStation-3.0.0/btleWeatherStation.egg-info/top_level.txt
+-rw-r--r--   0 rcf       (1000) rcf       (1000)       38 2024-06-01 18:08:42.676631 btleWeatherStation-3.0.0/setup.cfg
+-rwxr-xr-x   0 rcf       (1000) rcf       (1000)      830 2023-03-30 21:50:31.000000 btleWeatherStation-3.0.0/setup.py
```

### Comparing `btleWeatherStation-2.2.1/LICENSE` & `btleWeatherStation-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `btleWeatherStation-2.2.1/PKG-INFO` & `btleWeatherStation-3.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btleWeatherStation
-Version: 2.2.1
+Version: 3.0.0
 Summary: Scan for and get data from an Oregon Scientific BtLE weather station
 Home-page: https://github.com/mincebert/bleWeatherStation
 Author: Arnaud Balmelle & Robert Franklin
 Author-email: rcf@mince.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `btleWeatherStation-2.2.1/btleWeatherStation/scan.py` & `btleWeatherStation-3.0.0/btleWeatherStation/scan.py`

 * *Files identical despite different names*

### Comparing `btleWeatherStation-2.2.1/btleWeatherStation/station.py` & `btleWeatherStation-3.0.0/btleWeatherStation/station.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,18 +42,129 @@
     "Exception raised when no data was received from a weather station."
 
     def __init__(self, message):
         self.message = message
 
 
 
+# --- functions ---
+
+
+
+def _default(s, default="--"):
+    """Returns the supplied string 's' if it is not None.  If 's' is
+    None, the 'default' value is returned.
+
+    It's typically used for debugging messages, to show undefined or
+    unavailable values.
+    """
+
+    if s is None:
+        return default
+
+    return s
+
+
+
 # --- classes ---
 
 
 
+class WeatherStationSensor(object):
+    """This class represents a measured status for a sensor on the
+    weather station.  It is typically used by the WeatherStationData
+    class.
+
+    Attributes contain the various measured values:
+
+    temp_current, temp_min, temp_max -- the current, minimum and
+    maximum temperatures in celcius
+
+    humidity_current, humidity_min, humidity_max -- the current, minimum
+    and maximum humidities as a percentage (0-100)
+
+    low_battery -- a boolean indicating if the sensor has a low battery
+    state
+    """
+
+    def __init__(
+            self, temp_current=None, temp_min=None, temp_max=None,
+            humidity_current=None, humidity_min=None, humidity_max=None,
+            low_battery=None):
+
+        "The constructor just stores the supplied values."
+
+        super().__init__()
+
+        self.temp_current = temp_current
+        self.temp_min = temp_min
+        self.temp_max = temp_max
+
+        self.humidity_current = humidity_current
+        self.humidity_min = humidity_min
+        self.humidity_max = humidity_max
+
+        self.low_battery = low_battery
+
+
+    def __str__(self):
+        """Returns a simple string representation of the sensor data,
+        primarily for debugging purposes and the format should not be
+        relied upon.
+        """
+
+        return (
+            "TEMP ('C): "
+            f"min: { _default(self.temp_min) }, "
+            f"current: { _default(self.temp_current) }, "
+            f"max: { _default(self.temp_max) }; "
+            "HUMIDITY (%): "
+            f"min: { _default(self.humidity_min) }, "
+            f"current: { _default(self.humidity_current) }, "
+            f"max: { _default(self.humidity_max) }, "
+            f"BATTERY: { 'low' if self.low_battery else 'ok' }")
+
+
+
+class WeatherStationData(object):
+    """Snapshot of all measured data from a WeatherStation, as returned
+    by WeatherStation.measure() (and measure_retry()).
+
+    There are two attributes:
+
+    clock -- a datetime object containing the time set in the station
+
+    sensors -- a dictionary, keyed on the sensor number, containing
+    WeatherStationSensor objects giving data for that sensor
+    """
+
+    def __init__(self, clock=None, sensors=None):
+        """The constructor just stores the supplied clock and sensor
+        data.
+        """
+
+        super().__init__()
+
+        self.clock = clock
+        self.sensors = sensors
+
+
+    def __str__(self):
+        """Print the station data as a multiline string.  This is
+        primarily used for debugging and the format should not be
+        relied upon.
+        """
+
+        s = "clock: " + str(self.clock)
+        for sensor in sorted(self.sensors):
+            s += "\n" + f"sensor[{ sensor }]: { self.sensors[sensor] }"
+        return s
+
+
+
 class WeatherStation(object):
     """This class models a weather station and has methods to connect
     and retrieve data from it.
     """
 
 
     def __init__(self, mac):
@@ -67,19 +178,14 @@
         # the MAC address of the weather station we're connecting to
         self._mac = mac
 
         # the btle.Peripheral object for the station, set by a call to
         # _connect()
         self._station = None
 
-        # the station clock and weather data binary blobs, if received
-        # (or blank if none) - these are filled in by measure()
-        self._clock = None
-        self._sensors = {}
-
 
     def _connect(self):
         """This method connects to the weather station.
 
         If the weather station is already connected, it will be
         disconnected (to avoid jamming up a station's Bluetooth stack)
         and a btle.BTLEDisconnectError exception raised.
@@ -216,15 +322,15 @@
         # missing data has a percentage greater than 100%
         if b[o] > 100:
             return None
 
         return b[o]
 
 
-    def _decode_clock(self, b):
+    def _decode_clock(self, c):
         """Decode the weather station clock from the supplied
         clock notification data.
 
         The bytes at the positions below have the following meaning:
 
         00    = clock: year - 2000
         01    = clock: month
@@ -235,52 +341,52 @@
         06    = unknown (always seems to be 0xff)
         07-10 = unknown (vary)
         11-18 = unknown (always seem to be 0xff)
 
         Note: there is always a clock time present - it's just
         incorrect, if not set.
 
-        b -- the clock notification data as a block of bytes
+        c -- the clock notification data as a block of bytes
+        """
+
+        return datetime(year=2000 + c[0], month=c[1], day=c[2],
+                        hour=c[3], minute=c[4], second=c[5])
+
+
+    def _decode_low_battery(self, t):
+        """Return a set of the numbers of the sensors which currently
+        have the 'low battery' alarm.  This includes sensor 0 - the
+        display.
+
+        t -- the status notification data as a block of bytes
         """
 
-        return datetime(
-                   year=2000 + b[0], month=b[1], day=b[2],
-                   hour=b[3], minute=b[4], second=b[5])
+        # the display's low battery is the MSB of the first byte; each
+        # sensor's low battery state is a bitfield in the sixth byte
+        return ({ 0 } if t[0] & 0x80
+                    else set().union({ sensor for sensor in range(1, 4)
+                                           if t[5] & (1 << (sensor - 1)) }))
 
 
-    def _decode_sensors_present(self, b):
+    def _decode_sensors_present(self, t):
         """Return a set of the numbers of the sensors which are
         present.  Sensor 0 (internal) is always assumed to be
         present, for convenience (you can't detect this, but it's
         clearly the case!).
 
-        b -- the status notification data as a block of bytes
+        t -- the status notification data as a block of bytes
         """
 
         # the 'sensor present' data is a bitfield in the second byte of
         # the status notification data
-        return { 0 }.union(
-                   { s for s in range(1, 4) if b[1] & (1 << (s - 1)) })
+        return { 0 }.union({ sensor for sensor in range(1, 4)
+                                 if t[1] & (1 << (sensor - 1)) })
 
 
-    def _decode_low_battery(self, b):
-        """Return a set of the numbers of the sensors which currently
-        have the 'low battery' alarm.  This includes sensor 0 - the
-        display.
-
-        b -- the status notification data as a block of bytes
-        """
-
-        # the display's low battery is the MSB of the first byte; each
-        # sensor's low battery state is a bitfield in the sixth byte
-        return { 0 } if b[0] & 0x80 else set().union(
-                   { s for s in range(1, 4) if b[5] & (1 << (s - 1)) })
-
-
-    def _decode_sensors(self, d):
+    def _decode_sensors_data(self, r):
         """Decode the data from the sensors from the supplied
         notification dictionary.
 
         The bytes at the positions below have the following meaning:
 
         00-01 = sensor 0 (internal): temperature - current
         02-03 = sensor 1: temperature - current
@@ -304,60 +410,61 @@
         26-27 = sensor 1: temperature - maxumum
         28-29 = sensor 1: temperature - minimum
         30-31 = sensor 2: temperature - maxumum
         32-33 = sensor 2: temperature - minimum
         34-35 = sensor 3: temperature - maxumum
         36-37 = sensor 3: temperature - minimum
 
-        d -- notification dictionary (as returned by get_raw_data())
+        r -- notification dictionary (as returned by get_raw_data())
         """
 
-        sensors = {}
-
-        # get the sensors notification data
-        s = d[SENSORS_HANDLE]
+        # get the sensors notification packet data
+        sensor_data = r[SENSORS_HANDLE]
 
         # get the sensors present and which have low battery
-        sensors_present = self._decode_sensors_present(d[STATUS_HANDLE])
-        low_battery = self._decode_low_battery(d[STATUS_HANDLE])
-
-        # go through the set of sensors which are present, getting
-        # their data
-        for n in sorted(sensors_present):
-            sensor = {
-                "temp": {
-                    "current": self._decode_temp(s, n*2),
-                    "min"    : self._decode_temp(s, 24 + n*4),
-                    "max"    : self._decode_temp(s, 22 + n*4), },
-
-                "humidity": {
-                    "current": self._decode_humidity(s, 8 + n),
-                    "min"    : self._decode_humidity(s, 15 + n*2),
-                    "max"    : self._decode_humidity(s, 14 + n*2), },
-
-                "low_battery": n in low_battery,
-            }
+        sensors_present = self._decode_sensors_present(r[STATUS_HANDLE])
+        low_battery = self._decode_low_battery(r[STATUS_HANDLE])
 
-            sensors[n] = sensor
+        # initialise a dictionary of decoded sensor data - this will be
+        # return
+        sensors = {}
 
+        for sensor in sorted(sensors_present):
+            # decode the sensor values from the raw data
+            temp_current = self._decode_temp(sensor_data, sensor*2)
+            temp_min = self._decode_temp(sensor_data, 24 + sensor*4)
+            temp_max = self._decode_temp(sensor_data, 22 + sensor*4)
+            humidity_current = self._decode_humidity(sensor_data, 8 + sensor)
+            humidity_min = self._decode_humidity(sensor_data, 15 + sensor*2)
+            humidity_max = self._decode_humidity(sensor_data, 14 + sensor*2)
+
+            # store this sensor's data in a WeatherStationSensor object
+            # in the 'sensors' dictionary
+            sensors[sensor] = WeatherStationSensor(
+                temp_current=temp_current,
+                temp_min=temp_min,
+                temp_max=temp_max,
+                humidity_current=humidity_current,
+                humidity_min=humidity_min,
+                humidity_max=humidity_max,
+                low_battery=sensor in low_battery)
 
             # if we're in debug mode, we log the decoded sensor data
-
-            logging.debug("decoded sensor data: %s "
-                          "temp: %s < %s < %s, "
-                          "humidity: %s < %s < %s, "
-                          "low battery?: %s"
-                              % (n,
-                                 sensor["temp"]["min"] or "?",
-                                 sensor["temp"]["current"] or "?",
-                                 sensor["temp"]["max"] or "?",
-                                 sensor["humidity"]["min"] or "?",
-                                 sensor["humidity"]["current"] or "?",
-                                 sensor["humidity"]["max"] or "?",
-                                 sensor["low_battery"]))
+            logging.debug("decoded sensor: %s data:"
+                          " temp: %s <= %s <= %s,"
+                          " humidity: %s <= %s <= %s,"
+                          " low battery?: %s"
+                              % (sensor,
+                                 _default(temp_min),
+                                 _default(temp_current),
+                                 _default(temp_max),
+                                 _default(humidity_min),
+                                 _default(humidity_current),
+                                 _default(humidity_max),
+                                 sensor in low_battery))
 
         return sensors
 
 
     def get_raw_data(self):
         """This method connects, gets the current data from the weather
         station, disconnects and returns it as a dictionary keyed on
@@ -389,170 +496,101 @@
         data = self._station.delegate.getData()
         self._disconnect()
 
 
         return data
 
 
-    def measure(self):
+    def measure_once(self):
         """Connect to the weather station, retrieve the current weather
-        sensor data, disconnect and decode it, storing it in the
-        object.
-
-        Data includes the temperature and humidity of all the sensors,
-        included stored minima and maxima, as well as the current clock
-        time.
+        sensor data, disconnect and decode it and store it in a
+        WeatherStationData object, which is returned.
 
         If no data was received, an WeatherStationNoDataError exception
         is raised.
+
+        This is only attempted once and can fail fairly regulary.  Using
+        measure() (which can handle retries) is recommended.
         """
 
 
         # connect to the weather station, read the current data and
         # disconnect
 
-        data = self.get_raw_data()
+        raw_data = self.get_raw_data()
 
 
         # decode and store the date and time using the system data
 
-        self._clock = (self._decode_clock(data[CLOCK_HANDLE])
-                           if CLOCK_HANDLE in data
-                           else None)
+        if CLOCK_HANDLE not in raw_data:
+            raise WeatherStationNoDataError(
+                      "no clock data received from station")
 
-        if self._clock:
-            logging.debug("decoded clock data: %s", self._clock)
+        clock = self._decode_clock(raw_data[CLOCK_HANDLE])
+
+        if clock:
+            logging.debug("decoded clock data: %s", clock)
 
 
         # if the sensor data was missing, blank it out and stop with
         # failure
 
-        if SENSORS_HANDLE not in data:
-            self._sensors = {}
-            raise WeatherStationNoDataError("no data received from station")
+        if SENSORS_HANDLE not in raw_data:
+            raise WeatherStationNoDataError(
+                      "no sensor data received from station")
+
+        sensors = self._decode_sensors_data(raw_data)
+
 
-        self._sensors = self._decode_sensors(data)
+        # build a WeatherStationData object and return it
 
+        return WeatherStationData(clock=clock, sensors=sensors)
 
-    def measure_retry(self, timeout=30, interval=3):
+
+    def measure(self, max_tries=5, interval=3):
         """This method repeatedly retries measure() until it returns a
         successful result, up until the maximum time specifed,
         sleep()ing for the interval, between each retry.
 
         This is useful because sometimes the weather station connection
         fails and it's necessary to retry it a few times to get data.
+
+        As with measure(), a WeatherStationData object will be returned,
+        or an exception raised.
         """
 
-        total = 0
+        tries = 0
+
+        while tries < max_tries:
+            tries += 1
 
-        while True:
             try:
-                self.measure()
+                return self.measure_once()
                 break
 
             except (btle.BTLEException, WeatherStationNoDataError):
-                # stop if we've waited at least the maximum time
+                # if we have more tries left, wait for the interval time
 
-                if total >= timeout:
+                if tries >= max_tries:
                     logging.debug(
-                        "info: stopping measure after: %ds timeout: %ds",
-                        total, timeout)
+                        f"info: maximum number of tries {tries} reached -"
+                        " aborting")
 
                     raise
 
 
-            # wait for the interval time
+            # we have more tries left, so wait and then retry
 
             logging.debug(
-                "info: waited so far: %ds timeout: %ds: retrying in: %ds",
-                total, timeout, interval)
+                f"info: try {tries} failed, {max_tries - tries} left; waiting "
+                f"{interval} seconds before retry")
 
             sleep(interval)
-            total += interval
-
-
-    def sensor_present(self, n):
-        """This method returns if there is data for a particular sensor
-        present, after calling measure().
-
-        The presence can also be tested for by using get_sensors() and
-        testing if the sensor's number is present in the returned
-        dictionary.
-        """
 
-        return n in self._sensors
-
-
-    def get_sensors(self):
-        """This method returns a dictionary, keyed on the sensor number
-        and then on the type of data measured ("temp" and "humidity")
-        and then the value ("current", "min" and "max"); there is also
-        a "low_battery" key with a flag showing if that alarm is set.
-
-        A sensor's presence can be explicitly tested for with the
-        sensor_present() method or by checking if its key is in this
-        dictionary.
-
-        The returned value must not be changed: if it is to be
-        modified, it must be deepcopy()ed first.
-        """
-
-        return self._sensors
-
-
-    def get_clock(self):
-        """This method returns the clock time returned by the weather
-        station.
-
-        If the clock has not been measured or was not available, None
-        will be returned.
-        """
-
-        return self._clock
-
-
-    def get_temp(self, n=0):
-        """This method returns the temperature data from the numbered
-        sensor (with 0 being the weather station's internal sensor).
-        Temperatures are returned as floats.
-
-        The returned value is a dictionary, keyed on the "current",
-        "min" and "max" values.
-
-        If any particular sensor value is unavailable, None will be
-        returned for that.
-        """
-
-        return self._sensors[n].get("temp")
-
-
-    def get_humidity(self, n=0):
-        """This method returns the humidity data from the numbered
-        sensor (with 0 being the weather station's internal sensor).
-        Humidities are returned as an integer, giving the percentage.
-
-        The returned value is a dictionary, keyed on the "current",
-        "min" and "max" values.
-
-        If any particular sensor value is unavailable, None will be
-        returned for that.
-        """
-
-        return self._sensors[n].get("humidity")
-
-
-    def get_low_battery(self, n=0):
-        """This method returns the low battery alarm from the numbered
-        sensor (with 0 being the weather station's battery).
-
-        The return value is a boolean.  If the status is unavailable,
-        None will be returned.
-        """
 
-        return self._sensors[n].get("low_battery")
 
 
 class _WeatherStationDelegate(btle.DefaultDelegate):
     """This class handles notifications from a BtLE weather station and
     stores them for retrieval and processing by the caller..
 
     Notifications contain information about the current weather data.
```

### Comparing `btleWeatherStation-2.2.1/btleWeatherStation.egg-info/PKG-INFO` & `btleWeatherStation-3.0.0/btleWeatherStation.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: btleWeatherStation
-Version: 2.2.1
+Version: 3.0.0
 Summary: Scan for and get data from an Oregon Scientific BtLE weather station
 Home-page: https://github.com/mincebert/bleWeatherStation
 Author: Arnaud Balmelle & Robert Franklin
 Author-email: rcf@mince.net
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `btleWeatherStation-2.2.1/setup.py` & `btleWeatherStation-3.0.0/setup.py`

 * *Files identical despite different names*

