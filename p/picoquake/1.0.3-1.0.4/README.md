# Comparing `tmp/picoquake-1.0.3.tar.gz` & `tmp/picoquake-1.0.4.tar.gz`

## Comparing `picoquake-1.0.3.tar` & `picoquake-1.0.4.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 picoquake-1.0.3/.python-version
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 picoquake-1.0.3/.vscode/settings.json
--rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 picoquake-1.0.3/examples/acquire.py
--rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 picoquake-1.0.3/examples/continuous.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 picoquake-1.0.3/picoquake/__init__.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 picoquake-1.0.3/picoquake/__main__.py
--rw-r--r--   0        0        0    16259 2020-02-02 00:00:00.000000 picoquake-1.0.3/picoquake/cli.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 picoquake-1.0.3/picoquake/configuration.py
--rw-r--r--   0        0        0     7888 2020-02-02 00:00:00.000000 picoquake-1.0.3/picoquake/data.py
--rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 picoquake-1.0.3/picoquake/exceptions.py
--rw-r--r--   0        0        0    19055 2020-02-02 00:00:00.000000 picoquake-1.0.3/picoquake/interface.py
--rw-r--r--   0        0        0     8987 2020-02-02 00:00:00.000000 picoquake-1.0.3/picoquake/plot.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 picoquake-1.0.3/picoquake/msg/__init__.py
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 picoquake-1.0.3/picoquake/msg/messages_pb2.py
--rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 picoquake-1.0.3/picoquake/msg/nanopb_pb2.py
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 picoquake-1.0.3/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 picoquake-1.0.3/LICENSE.txt
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 picoquake-1.0.3/README.md
--rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 picoquake-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 picoquake-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 picoquake-1.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 picoquake-1.0.4/examples/acquire.py
+-rw-r--r--   0        0        0     1140 2020-02-02 00:00:00.000000 picoquake-1.0.4/examples/continuous.py
+-rw-r--r--   0        0        0      188 2020-02-02 00:00:00.000000 picoquake-1.0.4/picoquake/__init__.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 picoquake-1.0.4/picoquake/__main__.py
+-rw-r--r--   0        0        0    17171 2020-02-02 00:00:00.000000 picoquake-1.0.4/picoquake/cli.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 picoquake-1.0.4/picoquake/configuration.py
+-rw-r--r--   0        0        0     7888 2020-02-02 00:00:00.000000 picoquake-1.0.4/picoquake/data.py
+-rw-r--r--   0        0        0      697 2020-02-02 00:00:00.000000 picoquake-1.0.4/picoquake/exceptions.py
+-rw-r--r--   0        0        0    20585 2020-02-02 00:00:00.000000 picoquake-1.0.4/picoquake/interface.py
+-rw-r--r--   0        0        0     8987 2020-02-02 00:00:00.000000 picoquake-1.0.4/picoquake/plot.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 picoquake-1.0.4/picoquake/msg/__init__.py
+-rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 picoquake-1.0.4/picoquake/msg/messages_pb2.py
+-rw-r--r--   0        0        0     4385 2020-02-02 00:00:00.000000 picoquake-1.0.4/picoquake/msg/nanopb_pb2.py
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 picoquake-1.0.4/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 picoquake-1.0.4/LICENSE.txt
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 picoquake-1.0.4/README.md
+-rw-r--r--   0        0        0     1148 2020-02-02 00:00:00.000000 picoquake-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 picoquake-1.0.4/PKG-INFO
```

### Comparing `picoquake-1.0.3/examples/acquire.py` & `picoquake-1.0.4/examples/acquire.py`

 * *Files identical despite different names*

### Comparing `picoquake-1.0.3/examples/continuous.py` & `picoquake-1.0.4/examples/continuous.py`

 * *Files identical despite different names*

### Comparing `picoquake-1.0.3/picoquake/cli.py` & `picoquake-1.0.4/picoquake/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -237,20 +237,24 @@
         sys.exit(1)
 
 
 
 def _list_devices(args):
     all_ports = args.all
     ports = comports()
+    devices = []
     for p in ports:
         if p.vid == VID and p.pid == PID and p.serial_number:
             short_id = DeviceInfo.unique_id_to_short_id(p.serial_number)
+            devices.append((short_id, p))
             print(f"PicoQuake {short_id}: {p.device}")
         elif all_ports:
             print(f"Unknown device: {p.device}, description: {p.description}")
+    if not devices:
+        print("No PicoQuake devices found.")
 
 
 def _info(args):
     short_id: str = args.short_id
     try:
         device = PicoQuake(short_id)
     except DeviceNotFound:
@@ -316,14 +320,34 @@
         logger.exception(e)
         print(f"Error: {e}")
         sys.exit(1)
     finally:
         device.stop()
 
 
+def _reboot_to_bootsel(args):
+    short_id: str = args.short_id
+    try:
+        device = PicoQuake(short_id)
+    except DeviceNotFound:
+        print(f"Device with short_id {short_id} not found.")
+        sys.exit(1)
+    except Exception as e:
+        logger.exception(e)
+        print(f"Error: {e}")
+        sys.exit(1)
+    try:
+        device.reboot_to_bootsel()
+        print("Device rebooted to BOOTSEL.")
+    except Exception as e:
+        logger.exception(e)
+        print(f"Error: {e}")
+        sys.exit(1)
+
+
 def main():
     main_parser = argparse.ArgumentParser(description="PicoQuake CLI.")
     main_parser.add_argument("-v", "--version", action="version", version=f"picoquake {__version__}")
     main_parser.add_argument("--verbose", action="store_true", help="Print log messages to console.")
     main_parser.add_argument("--debug", action="store_true", help="Set log level to debug.")
     subparsers = main_parser.add_subparsers(required=True, dest="command")
 
@@ -365,14 +389,19 @@
     info_parser.set_defaults(func=_info)
 
     # test
     test_parser = subparsers.add_parser("test", help="Test device.")
     test_parser.add_argument("short_id", help="The 4 character ID of the device. Found on the label.")
     test_parser.set_defaults(func=_test)
 
+    # reboot to bootsel
+    reboot_bootsel = subparsers.add_parser("bootsel", help="Reboot device to BOOTSEL.")
+    reboot_bootsel.add_argument("short_id", help="The 4 character ID of the device. Found on the label.")
+    reboot_bootsel.set_defaults(func=_reboot_to_bootsel)
+
     # plot PSD
     fftplot_parser = subparsers.add_parser("plot_psd", help="Plot Power Spectral Density of acquired data.")
     fftplot_parser.add_argument("csv_path", help="The CSV file containing the acquired data.")
     fftplot_parser.add_argument("output", help="The output file to save the plot to. '.' to save next to the data file.")
     fftplot_parser.add_argument("-a", "--axis", default="xyz", help="Axis to plot, must be 'x', 'y', 'z', or a combination")
     fftplot_parser.add_argument("--fmin", type=float, default=0.0, help="Minimum frequency to plot.")
     fftplot_parser.add_argument("--fmax", type=float, default=1000.0, help="Maximum frequency to plot.")
@@ -397,15 +426,14 @@
     plot_parser.add_argument("output", help="The output file to save the plot to. '.' to save next to the data file.")
     plot_parser.add_argument("-a", "--axis", default="xyz", help="Axis to plot, must be 'x', 'y', 'z', or a combination")
     plot_parser.add_argument("--tstart", type=float, default=0.0, help="Start time of the plot.")
     plot_parser.add_argument("--tend", type=float, default=None, help="End time of the plot.")
     plot_parser.add_argument("--title", help="Title of the plot.", default=None)
     plot_parser.set_defaults(func=_plot)
 
-    
     args = main_parser.parse_args()
 
     # logging
     log_path = os.path.join(_get_log_path("picoquake"), "picoquake.log")
     file_handler =RotatingFileHandler(log_path, mode='a', maxBytes=15*1024*1024, backupCount=5)
     file_handler.setFormatter(logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s'))
     logging.getLogger().addHandler(file_handler)
```

### Comparing `picoquake-1.0.3/picoquake/configuration.py` & `picoquake-1.0.4/picoquake/configuration.py`

 * *Files identical despite different names*

### Comparing `picoquake-1.0.3/picoquake/data.py` & `picoquake-1.0.4/picoquake/data.py`

 * *Files identical despite different names*

### Comparing `picoquake-1.0.3/picoquake/exceptions.py` & `picoquake-1.0.4/picoquake/exceptions.py`

 * *Files identical despite different names*

### Comparing `picoquake-1.0.3/picoquake/interface.py` & `picoquake-1.0.4/picoquake/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,34 +3,36 @@
 """
 
 import time
 from serial import Serial, SerialException
 from serial.tools.list_ports import comports
 from queue import Empty, Queue
 from time import sleep, time
-from threading import Thread, Event
+from threading import Thread, Event, Lock
 from typing import List, Optional, cast, Tuple
 import logging
 import struct
 from datetime import datetime
+from collections import deque
 
 from cobs import cobs
 
 from .msg import messages_pb2
 from .configuration import *
 from .data import *
 from .exceptions import *
 
 VID = 0x2E8A
 PID = 0xA
 
 _HANDSHAKE_TIMEOUT = 5.0
 _STATUS_TIMEOUT = 2.0
 _SAMPLE_START_TIMEOUT = 1.0
-_READ_LAST_TIMEOUT = 1.0
+
+_LEN_DEQUE = 1_000_000
 
 
 def _handle_exceptions(func):
     """
     Decorator for handling exceptions in class methods.
     Calls `_handle_exceptions` method of the class.
     """
@@ -94,23 +96,23 @@
 
         self.config: Config = Config(SampleRate.hz_100, Filter.hz_42, AccRange.g_2, GyroRange.dps_250)
         """The current configuration of the device."""
 
         self._continuos_mode = False
         self._acquire_n_samples = 0
         self._is_sampling = False
-        self._sample_list: List[IMUSample] = []
-        self._last_sample: Optional[IMUSample] = None
+        self._sample_deque: deque = deque()
 
         self._out_packet_queue = Queue()
         self._in_message_queue = Queue()
         self._stop_event = Event()
         
         self._serial_thread = Thread(target=self._serial_worker, daemon=True)
         self._handler_thread = Thread(target=self._handler, daemon=True)
+        self._lock = Lock()
 
         self._device_status = Status(State.IDLE, 0, 0, 0)
         self._last_status_time = time()
 
         self._exception: Optional[Exception] = None
 
         self._started = False
@@ -190,14 +192,15 @@
         if seconds > 0:
             n_samples = int(seconds * self.config.sample_rate.param_value)
 
         max_duration = n_samples / self.config.sample_rate.param_value * 1.2 + 1.0
         exception: Optional[Exception] = None
 
         self._logger.info(f"Acquiring {n_samples} samples, max expected duration: {max_duration:.1f}s")
+        self._sample_deque = deque(maxlen=n_samples * 2)
         self._acquire_n_samples = n_samples
         self._start_sampling(n_samples)
         # wait for sampling to start
         cmd_start_t = time()
         while True:
             if self._device_status.state == State.SAMPLING:
                 break
@@ -213,73 +216,122 @@
             if self._device_status.state == State.IDLE:
                 break
             if time() - start_t > max_duration:
                 exception = ConnectionError("Sampling timeout")
                 break
             sleep(0.001)
         stop_t = time()
+        samples = list(self._sample_deque)
         self._logger.info(f"Acquisition stopped. Took: {stop_t - start_t:.1f}s.")
-        self._logger.info(f"Received {len(self._sample_list)} samples")
+        self._logger.info(f"Received {len(samples)} samples")
 
-        data = AcquisitionData(samples=self._sample_list[0:n_samples],
+        data = AcquisitionData(samples=samples[0:n_samples],
                                device=cast(DeviceInfo, self.device_info),
                                config=self.config,
                                start_time=datetime.fromtimestamp(start_t))
 
         if exception is None:
-            if len(self._sample_list) < n_samples:
-                self._logger.warning(f"Expected {n_samples} samples, received {len(self._sample_list)}")
+            if len(samples) < n_samples:
+                self._logger.warning(f"Expected {n_samples} samples, received {len(samples)}")
                 exception = ConnectionError("Not all samples received")
             elif not data._check_integrity:
                 self._logger.warning(f"Data integrity compromised, {data.skipped_samples} samples skipped")
                 exception = ConnectionError("Data integrity compromised")
         return data, exception
 
     def start_continuos(self):
         """
         Starts the device in continuos mode. Samples can be read using `read_last()`.
         """
         self._continuos_mode = True
+        self._sample_deque = deque(maxlen=_LEN_DEQUE)
         self._start_sampling()
         self._logger.info("Continuos mode started")
 
     def stop_continuos(self):
         """
         Stops the device in continuos mode.
         """
         self._continuos_mode = False
         self._stop_sampling()
-        self._last_sample = None
         self._logger.info("Continuos mode stopped")
 
-    def read_last(self) -> IMUSample:
+    def read(self, num: int=1, timeout: Optional[float]=None) -> List[IMUSample]:
+        """
+        Reads the specified number of samples received in continuos mode.
+        Samples are returned in the same order as they were received.
+        If timeout is None, blocks until the specified number of samples are received.
+
+        Args:
+            num: The number of samples to read.
+            timeout: The maximum time to wait for the samples.
+        Returns:
+            List of samples. Might be less than `num` if timeout is set.
+
+        Raises:
+            RuntimeError: If continuos mode is not started.
+        """
+        if not self._continuos_mode:
+            raise RuntimeError("Continuos mode not started")
+        start_time = time()
+        while len(self._sample_deque) < num:
+            if timeout is not None:
+                if time() - start_time > timeout:
+                    break
+            if self._exception is not None:
+                raise self._exception
+            sleep(0.001)
+        samples = []
+        with self._lock:
+            num_ret = min(num, len(self._sample_deque))
+            for _ in range(num_ret):
+                samples.append(self._sample_deque.popleft())
+        return samples
+
+    def read_last(self, timeout: Optional[float]=None) -> Optional[IMUSample]:
         """
         Reads the last sample received in continuos mode.
+        If timeout is None, blocks until a sample is received.
+
+        Args:
+            timeout: The maximum time to wait for the sample.
 
         Returns:
-            The latest sample performed on device.
+            The latest sample received.
 
         Raises:
             RuntimeError: If continuos mode is not started.
-            ConnectionError: If no samples are received.
         """       
         if not self._continuos_mode:
             raise RuntimeError("Continuos mode not started")
 
         start_time = time()
-        while self._last_sample is None:
-            if time() - start_time > _READ_LAST_TIMEOUT:
-                if self._exception is not None:
-                    raise self._exception
-                else:
-                    raise ConnectionError("No samples received")
+        while len(self._sample_deque) < 1:
+            if timeout is not None:
+                if time() - start_time > timeout:
+                    break
+            if self._exception is not None:
+                raise self._exception
             sleep(0.001)
-        if self._exception is not None:
-            raise self._exception
-        return self._last_sample
+        with self._lock:
+            if len(self._sample_deque) > 0:
+                return self._sample_deque.pop()
+            else:
+                return None
+    
+    def reboot_to_bootsel(self):
+        """
+        Reboots the device to BOOTSEL mode.
+        """
+        if self._started:
+            self.stop()
+        self._logger.info("Rebooting to BOOTSEL...")
+        ser = Serial(self._port, 1200, timeout=0.1)
+        sleep(0.1)
+        ser.close()
 
     def _find_port(self, short_id: str) -> Optional[str]:
         """
         Finds the port to which the device is connected.
         """
         ports = comports()
         for p in ports:
@@ -307,16 +359,14 @@
         Sends start sampling command.
 
         Args:
             num_samples: The number of samples to acquire.
                 If 0, the device will sample continuously.
         """
         self._logger.debug("Starting sampling...")
-        self._sample_list = []
-        self._last_sample = None
         self._send_command(CommandID.START_SAMPLING, self.config, num_samples)
         self._is_sampling = True
 
     def _stop_sampling(self):
         """
         Sends stop sampling command.
         """
@@ -369,19 +419,15 @@
             # process messages
             try:
                 msg = self._in_message_queue.get(timeout=0.1)
             except Empty:
                 pass
             else:
                 if isinstance(msg, IMUSample):
-                    imu_data = msg
-                    if self._continuos_mode:
-                        self._last_sample = imu_data
-                    else:
-                        self._sample_list.append(imu_data)
+                    self._sample_deque.append(msg)
                 elif isinstance(msg, messages_pb2.Status):
                     status = Status(State(msg.state), msg.temperature,
                                     msg.missed_samples, msg.error_code)
                     if status.state != self._device_status.state:
                         self._logger.debug(f"Device state changed from {self._device_status.state.name} to {status.state.name}")
                     self._device_status = status
                     self._last_status_time = time()
```

### Comparing `picoquake-1.0.3/picoquake/plot.py` & `picoquake-1.0.4/picoquake/plot.py`

 * *Files identical despite different names*

### Comparing `picoquake-1.0.3/picoquake/msg/messages_pb2.py` & `picoquake-1.0.4/picoquake/msg/messages_pb2.py`

 * *Files identical despite different names*

### Comparing `picoquake-1.0.3/picoquake/msg/nanopb_pb2.py` & `picoquake-1.0.4/picoquake/msg/nanopb_pb2.py`

 * *Files identical despite different names*

### Comparing `picoquake-1.0.3/.gitignore` & `picoquake-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `picoquake-1.0.3/LICENSE.txt` & `picoquake-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `picoquake-1.0.3/README.md` & `picoquake-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `picoquake-1.0.3/pyproject.toml` & `picoquake-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "picoquake"
-version = "1.0.3"
+version = "1.0.4"
 description = "PicoQuake USB vibration sensor library."
 requires-python = ">=3.9"
 readme = "README.md"
 authors = [
     { name = "Nejc Planinsek", email = "nejc@plab.si" }
 ]
 keywords = [
```

### Comparing `picoquake-1.0.3/PKG-INFO` & `picoquake-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: picoquake
-Version: 1.0.3
+Version: 1.0.4
 Summary: PicoQuake USB vibration sensor library.
 Project-URL: Repository, https://github.com/PLab-SI/PicoQuake
 Project-URL: Documentation, https://plab-si.github.io/PicoQuake/
 Author-email: Nejc Planinsek <nejc@plab.si>
 License-File: LICENSE.txt
 Keywords: IMU,accelerometer,data acquisition,gyroscope,picoquake,vibration
 Classifier: Development Status :: 4 - Beta
```

