# Comparing `tmp/echowarp-0.2.9-py3-none-any.whl.zip` & `tmp/echowarp-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,28 +1,31 @@
-Zip file size: 26789 bytes, number of entries: 26
--rw-r--r--  2.0 unx      477 b- defN 24-Apr-25 22:35 echowarp/__init__.py
--rw-r--r--  2.0 unx      603 b- defN 24-Apr-25 22:35 echowarp/logging_config.py
--rw-r--r--  2.0 unx     2297 b- defN 24-Apr-25 22:35 echowarp/main.py
--rw-r--r--  2.0 unx     2470 b- defN 24-Apr-25 22:35 echowarp/settings.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 22:35 echowarp/auth_and_heartbeat/__init__.py
--rw-r--r--  2.0 unx     7070 b- defN 24-Apr-25 22:35 echowarp/auth_and_heartbeat/transport_base.py
--rw-r--r--  2.0 unx     6932 b- defN 24-Apr-25 22:35 echowarp/auth_and_heartbeat/transport_client.py
--rw-r--r--  2.0 unx     7540 b- defN 24-Apr-25 22:35 echowarp/auth_and_heartbeat/transport_server.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 22:35 echowarp/models/__init__.py
--rw-r--r--  2.0 unx     5480 b- defN 24-Apr-25 22:35 echowarp/models/audio_device.py
--rw-r--r--  2.0 unx     3420 b- defN 24-Apr-25 22:35 echowarp/models/default_values_and_options.py
--rw-r--r--  2.0 unx     6464 b- defN 24-Apr-25 22:35 echowarp/models/json_message.py
--rw-r--r--  2.0 unx      579 b- defN 24-Apr-25 22:35 echowarp/models/options_data_creater.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 22:35 echowarp/services/__init__.py
--rw-r--r--  2.0 unx     9205 b- defN 24-Apr-25 22:35 echowarp/services/crypto_manager.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 22:35 echowarp/start_modes/__init__.py
--rw-r--r--  2.0 unx     3741 b- defN 24-Apr-25 22:35 echowarp/start_modes/args_mode.py
--rw-r--r--  2.0 unx     6007 b- defN 24-Apr-25 22:35 echowarp/start_modes/interactive_mode.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-25 22:35 echowarp/streamer/__init__.py
--rw-r--r--  2.0 unx     3815 b- defN 24-Apr-25 22:35 echowarp/streamer/audio_client.py
--rw-r--r--  2.0 unx     3855 b- defN 24-Apr-25 22:35 echowarp/streamer/audio_server.py
--rw-r--r--  2.0 unx     5782 b- defN 24-Apr-25 22:36 echowarp-0.2.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-25 22:36 echowarp-0.2.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       52 b- defN 24-Apr-25 22:36 echowarp-0.2.9.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        9 b- defN 24-Apr-25 22:36 echowarp-0.2.9.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2273 b- defN 24-Apr-25 22:36 echowarp-0.2.9.dist-info/RECORD
-26 files, 78163 bytes uncompressed, 23051 bytes compressed:  70.5%
+Zip file size: 35818 bytes, number of entries: 29
+-rw-r--r--  2.0 unx       58 b- defN 24-May-31 22:12 version.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-31 22:12 echowarp/__init__.py
+-rw-r--r--  2.0 unx     1904 b- defN 24-May-31 22:12 echowarp/logging_config.py
+-rw-r--r--  2.0 unx     2757 b- defN 24-May-31 22:12 echowarp/main.py
+-rw-r--r--  2.0 unx     3187 b- defN 24-May-31 22:12 echowarp/settings.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-31 22:12 echowarp/auth_and_heartbeat/__init__.py
+-rw-r--r--  2.0 unx    13369 b- defN 24-May-31 22:12 echowarp/auth_and_heartbeat/transport_base.py
+-rw-r--r--  2.0 unx     5731 b- defN 24-May-31 22:12 echowarp/auth_and_heartbeat/transport_client.py
+-rw-r--r--  2.0 unx     8621 b- defN 24-May-31 22:12 echowarp/auth_and_heartbeat/transport_server.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-31 22:12 echowarp/models/__init__.py
+-rw-r--r--  2.0 unx     7326 b- defN 24-May-31 22:12 echowarp/models/audio_device.py
+-rw-r--r--  2.0 unx     4575 b- defN 24-May-31 22:12 echowarp/models/ban_list.py
+-rw-r--r--  2.0 unx     6327 b- defN 24-May-31 22:12 echowarp/models/default_values_and_options.py
+-rw-r--r--  2.0 unx     7590 b- defN 24-May-31 22:12 echowarp/models/json_message.py
+-rw-r--r--  2.0 unx      579 b- defN 24-May-31 22:12 echowarp/models/options_data_creater.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-31 22:12 echowarp/services/__init__.py
+-rw-r--r--  2.0 unx     9334 b- defN 24-May-31 22:12 echowarp/services/crypto_manager.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-31 22:12 echowarp/start_modes/__init__.py
+-rw-r--r--  2.0 unx     7556 b- defN 24-May-31 22:12 echowarp/start_modes/args_mode.py
+-rw-r--r--  2.0 unx    12914 b- defN 24-May-31 22:12 echowarp/start_modes/config_parser.py
+-rw-r--r--  2.0 unx    11350 b- defN 24-May-31 22:12 echowarp/start_modes/interactive_mode.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-31 22:12 echowarp/streamer/__init__.py
+-rw-r--r--  2.0 unx     2831 b- defN 24-May-31 22:12 echowarp/streamer/audio_client.py
+-rw-r--r--  2.0 unx     3286 b- defN 24-May-31 22:12 echowarp/streamer/audio_server.py
+-rw-r--r--  2.0 unx     8945 b- defN 24-May-31 22:13 echowarp-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-31 22:13 echowarp-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       48 b- defN 24-May-31 22:13 echowarp-0.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        9 b- defN 24-May-31 22:13 echowarp-0.3.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2518 b- defN 24-May-31 22:13 echowarp-0.3.0.dist-info/RECORD
+29 files, 120907 bytes uncompressed, 31704 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -1,7 +1,10 @@
+Filename: version.py
+Comment: 
+
 Filename: echowarp/__init__.py
 Comment: 
 
 Filename: echowarp/logging_config.py
 Comment: 
 
 Filename: echowarp/main.py
@@ -24,14 +27,17 @@
 
 Filename: echowarp/models/__init__.py
 Comment: 
 
 Filename: echowarp/models/audio_device.py
 Comment: 
 
+Filename: echowarp/models/ban_list.py
+Comment: 
+
 Filename: echowarp/models/default_values_and_options.py
 Comment: 
 
 Filename: echowarp/models/json_message.py
 Comment: 
 
 Filename: echowarp/models/options_data_creater.py
@@ -45,35 +51,38 @@
 
 Filename: echowarp/start_modes/__init__.py
 Comment: 
 
 Filename: echowarp/start_modes/args_mode.py
 Comment: 
 
+Filename: echowarp/start_modes/config_parser.py
+Comment: 
+
 Filename: echowarp/start_modes/interactive_mode.py
 Comment: 
 
 Filename: echowarp/streamer/__init__.py
 Comment: 
 
 Filename: echowarp/streamer/audio_client.py
 Comment: 
 
 Filename: echowarp/streamer/audio_server.py
 Comment: 
 
-Filename: echowarp-0.2.9.dist-info/METADATA
+Filename: echowarp-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: echowarp-0.2.9.dist-info/WHEEL
+Filename: echowarp-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: echowarp-0.2.9.dist-info/entry_points.txt
+Filename: echowarp-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: echowarp-0.2.9.dist-info/top_level.txt
+Filename: echowarp-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: echowarp-0.2.9.dist-info/RECORD
+Filename: echowarp-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## echowarp/__init__.py

```diff
@@ -1,30 +0,0 @@
-00000000: 6672 6f6d 2065 6368 6f77 6172 702e 7374  from echowarp.st
-00000010: 7265 616d 6572 2e61 7564 696f 5f63 6c69  reamer.audio_cli
-00000020: 656e 7420 696d 706f 7274 2043 6c69 656e  ent import Clien
-00000030: 7453 7472 6561 6d52 6563 6569 7665 720a  tStreamReceiver.
-00000040: 6672 6f6d 2065 6368 6f77 6172 702e 7374  from echowarp.st
-00000050: 7265 616d 6572 2e61 7564 696f 5f73 6572  reamer.audio_ser
-00000060: 7665 7220 696d 706f 7274 2053 6572 7665  ver import Serve
-00000070: 7253 7472 6561 6d65 720a 6672 6f6d 2065  rStreamer.from e
-00000080: 6368 6f77 6172 702e 7365 7276 6963 6573  chowarp.services
-00000090: 2e63 7279 7074 6f5f 6d61 6e61 6765 7220  .crypto_manager 
-000000a0: 696d 706f 7274 2043 7279 7074 6f4d 616e  import CryptoMan
-000000b0: 6167 6572 0a66 726f 6d20 6563 686f 7761  ager.from echowa
-000000c0: 7270 2e6d 6f64 656c 732e 6175 6469 6f5f  rp.models.audio_
-000000d0: 6465 7669 6365 2069 6d70 6f72 7420 4175  device import Au
-000000e0: 6469 6f44 6576 6963 650a 0a66 726f 6d20  dioDevice..from 
-000000f0: 6563 686f 7761 7270 2e6d 6169 6e20 696d  echowarp.main im
-00000100: 706f 7274 206d 6169 6e0a 6672 6f6d 2065  port main.from e
-00000110: 6368 6f77 6172 702e 7365 7474 696e 6773  chowarp.settings
-00000120: 2069 6d70 6f72 7420 5365 7474 696e 6773   import Settings
-00000130: 0a0a 5f5f 616c 6c5f 5f20 3d20 5b0a 2020  ..__all__ = [.  
-00000140: 2020 2743 6c69 656e 7453 7472 6561 6d52    'ClientStreamR
-00000150: 6563 6569 7665 7227 2c0a 2020 2020 2753  eceiver',.    'S
-00000160: 6572 7665 7253 7472 6561 6d65 7227 2c0a  erverStreamer',.
-00000170: 2020 2020 2743 7279 7074 6f4d 616e 6167      'CryptoManag
-00000180: 6572 272c 0a20 2020 2027 4175 6469 6f44  er',.    'AudioD
-00000190: 6576 6963 6527 2c0a 2020 2020 276d 6169  evice',.    'mai
-000001a0: 6e27 2c0a 2020 2020 2753 6574 7469 6e67  n',.    'Setting
-000001b0: 7327 2c0a 5d0a 0a69 6620 5f5f 6e61 6d65  s',.]..if __name
-000001c0: 5f5f 203d 3d20 225f 5f6d 6169 6e5f 5f22  __ == "__main__"
-000001d0: 3a0a 2020 2020 6d61 696e 2829 0a         :.    main().
```

## echowarp/logging_config.py

```diff
@@ -1,15 +1,47 @@
+import datetime
 import logging
 
 
-def setup_logging():
-    """
+class Logger:
+    IS_CORE_LOGGER_ENABLED: bool = False
+    IS_WARNING_LOGGER_ENABLED: bool = False
+
+    @staticmethod
+    def init_core_logger():
+        """
         Configures the logging settings for the application.
         Sets the logging level to INFO and specifies the format for log messages,
         including timestamp, log level, module, function name, and message.
-    """
-    logging.basicConfig(level=logging.INFO,
-                        format='[%(asctime)s] %(levelname)s | '
-                               'module: %(module)s | '
-                               'funcName: %(funcName)s | '
-                               'message: %(message)s',
-                        datefmt='%Y-%m-%d %H:%M:%S')
+        """
+        if not Logger.IS_CORE_LOGGER_ENABLED:
+            logging.basicConfig(level=logging.INFO,
+                                format='[%(asctime)s] %(levelname)s | '
+                                       'module: %(module)s | '
+                                       'funcName: %(funcName)s | '
+                                       '%(message)s',
+                                datefmt='%Y-%m-%d %H:%M:%S')
+
+            Logger.IS_CORE_LOGGER_ENABLED = True
+
+    @staticmethod
+    def init_warning_logger():
+        """
+        Configures an additional file handler for logging warnings.
+        Log messages with level WARNING or higher will be written to the specified file.
+        """
+        if not Logger.IS_WARNING_LOGGER_ENABLED:
+            current_date = datetime.datetime.now().strftime('%Y-%m-%d')
+            file_handler = logging.FileHandler(f"echowarp_errors_{current_date}.log")
+            file_handler.setLevel(logging.WARNING)
+
+            formatter = logging.Formatter('[%(asctime)s] %(levelname)s | '
+                                          'module: %(module)s | '
+                                          'funcName: %(funcName)s | '
+                                          '%(message)s',
+                                          datefmt='%Y-%m-%d %H:%M:%S')
+            file_handler.setFormatter(formatter)
+
+            logger = logging.getLogger()
+            logger.addHandler(file_handler)
+
+            Logger.IS_WARNING_LOGGER_ENABLED = True
```

## echowarp/main.py

```diff
@@ -1,61 +1,84 @@
 import sys
 import threading
 import logging
 import signal
+import time
 from functools import partial
 
-from echowarp.start_modes import args_mode
-from echowarp.logging_config import setup_logging
+from echowarp.logging_config import Logger
+from echowarp.start_modes.args_mode import ArgsParser
 from echowarp.start_modes.interactive_mode import InteractiveSettings
 
 from echowarp.streamer.audio_client import ClientStreamReceiver
 from echowarp.streamer.audio_server import ServerStreamer
 
 
-def graceful_shutdown(signum, frame, stop_util_event: threading.Event, stop_stream_event: threading.Event):
+def graceful_shutdown(signum, frame, stop_util_event: threading.Event):
     """
     Handles graceful shutdown of the application when a SIGINT signal is received.
 
     Args:
         signum (int): Signal number.
         frame (frame): Current stack frame.
         stop_util_event (threading.Event): Event to signal the utility to stop.
-        stop_stream_event (threading.Event): Event to signal the streaming to stop.
     """
     logging.info("Gracefully shutting down...")
-    stop_stream_event.set()
     stop_util_event.set()
 
 
-def main():
-    setup_logging()
-
-    stop_util_event = threading.Event()
-    stop_stream_event = threading.Event()
-
-    signal.signal(signal.SIGINT,
-                  partial(graceful_shutdown, stop_util_event=stop_util_event, stop_stream_event=stop_stream_event))
+def run_app(stop_util_event: threading.Event(), stop_stream_event: threading.Event()):
+    """
+        Runs the EchoWarp application in either server or client mode based on provided settings.
 
-    if len(sys.argv) == 1:
-        settings = InteractiveSettings.get_settings_interactive()
+        Args:
+            stop_util_event (threading.Event): Event to signal the utility to stop.
+            stop_stream_event (threading.Event): Event to signal the stream to stop.
+        """
+    if len(sys.argv) <= 1:
+        settings = InteractiveSettings.get_settings_in_interactive_mode()
     else:
-        settings = args_mode.get_settings_by_args()
+        settings = ArgsParser.get_settings_from_cli_args()
 
     if settings.is_server:
         logging.info("Start EchoWarp in server mode")
-        streamer = ServerStreamer(settings.udp_port, settings.heartbeat_attempt, stop_util_event, stop_stream_event,
-                                  settings.crypto_manager, settings.audio_device, settings.executor)
+        streamer = ServerStreamer(settings, stop_util_event, stop_stream_event)
 
         streamer_thread = threading.Thread(target=streamer.encode_audio_and_send_to_client, daemon=True)
-        streamer.start_heartbeat(streamer_thread)
+        streamer.start_streaming(streamer_thread)
     else:
         logging.info("Start EchoWarp in client mode")
-        receiver = ClientStreamReceiver(settings.server_addr, settings.udp_port, stop_util_event, stop_stream_event,
-                                        settings.crypto_manager, settings.audio_device, settings.executor)
+        receiver = ClientStreamReceiver(settings, stop_util_event, stop_stream_event)
 
         receiver_thread = threading.Thread(target=receiver.receive_audio_and_decode, daemon=True)
-        receiver.start_heartbeat(receiver_thread)
+        receiver.start_streaming(receiver_thread)
+
+
+def main():
+    """
+        Entry point of the EchoWarp application. Initializes logging, handles signals,
+        and runs the application.
+        """
+    Logger.init_core_logger()
+
+    stop_util_event = threading.Event()
+    stop_stream_event = threading.Event()
+
+    signal.signal(signal.SIGINT,
+                  partial(graceful_shutdown, stop_util_event=stop_util_event))
+
+    try:
+        run_app(stop_util_event, stop_stream_event)
+    except RuntimeError as e:
+        logging.error(e)
+    except Exception as e:
+        logging.critical(f"An error occurred: {e}", exc_info=True)
+
+        stop_stream_event.set()
+        stop_util_event.set()
+    finally:
+        time.sleep(1)
+        input("Press Enter to exit...")
 
 
 if __name__ == "__main__":
     main()
```

## echowarp/settings.py

```diff
@@ -8,43 +8,56 @@
 class Settings:
     """
     Configuration settings for the EchoWarp application, which can run in either server or client mode.
 
     Attributes:
         is_server (bool): True if the instance is configured as a server, otherwise False for a client.
         udp_port (int): The UDP port used for audio streaming.
-        server_addr (Optional[str]): The address of the server (only relevant in client mode).
-        heartbeat_attempt (int): The number of allowed missed heartbeats before the connection is considered lost.
+        server_address (Optional[str]): The address of the server (only relevant in client mode).
+        reconnect_attempt (int): The number of allowed missed reconnects before the connection is considered lost.
         audio_device (AudioDevice): The audio device configuration.
+        password (Optional[str]): The password for authentication.
         crypto_manager (Optional[CryptoManager]): Manages cryptographic operations, optional for non-secure mode.
         executor (ThreadPoolExecutor): Executor for managing concurrent tasks.
+        is_error_log (bool): Indicates if error logging is enabled.
+        socket_buffer_size (int): The buffer size for the socket.
     """
     is_server: bool
     udp_port: int
-    server_addr: Optional[str]
-    heartbeat_attempt: int
+    server_address: Optional[str]
+    reconnect_attempt: int
     audio_device: AudioDevice
+    password: Optional[str]
     crypto_manager: Optional[CryptoManager]
     executor: ThreadPoolExecutor
+    is_error_log: bool
+    socket_buffer_size: int
 
-    def __init__(self, is_server_mode: bool, udp_port: int, server_addr: Optional[str], heartbeat_attempt: int,
-                 is_ssl: bool, is_hash_control: bool, workers: int, audio_device: AudioDevice):
+    def __init__(self, is_server: bool, udp_port: int, server_address: Optional[str], reconnect_attempt: int,
+                 is_ssl: bool, is_integrity_control: bool, workers: int, audio_device: AudioDevice,
+                 password: Optional[str], is_error_log: bool, socket_buffer_size: int):
         """
         Initializes the settings for the EchoWarp application.
 
         Args:
-            is_server_mode (bool): Specifies if the settings are for a server.
+            is_server (bool): Specifies if the settings are for a server.
             udp_port (int): Port number for UDP communication.
-            server_addr (Optional[str]): Server address, necessary in client mode.
-            heartbeat_attempt (int): Number of heartbeat attempts before considering a disconnect.
+            server_address (Optional[str]): Server address, necessary in client mode.
+            reconnect_attempt (int): Number of reconnect attempts before considering a disconnect.
             is_ssl (bool): Enables SSL for secure communication.
-            is_hash_control (bool): Enables integrity control using hashing.
+            is_integrity_control (bool): Enables integrity control using hashing.
             workers (int): Number of worker threads for handling concurrent operations.
             audio_device (AudioDevice): Configured audio device.
+            password (Optional[str]): Password for authentication.
+            is_error_log (bool): Indicates if error logging is enabled.
+            socket_buffer_size (int): Buffer size for the socket.
         """
-        self.is_server = is_server_mode
+        self.is_server = is_server
         self.udp_port = udp_port
-        self.server_addr = server_addr
-        self.heartbeat_attempt = heartbeat_attempt
+        self.server_address = server_address
+        self.reconnect_attempt = reconnect_attempt
         self.audio_device = audio_device
-        self.crypto_manager = CryptoManager(self.is_server, is_hash_control, is_ssl)
+        self.password = password
+        self.crypto_manager = CryptoManager(self.is_server, is_integrity_control, is_ssl)
         self.executor = ThreadPoolExecutor(max_workers=workers)
+        self.is_error_log = is_error_log
+        self.socket_buffer_size = socket_buffer_size
```

## echowarp/auth_and_heartbeat/transport_base.py

```diff
@@ -1,163 +1,362 @@
+import base64
 import logging
+import os
 import socket
 import threading
 import time
 from abc import abstractmethod
 from typing import Optional
 
+from echowarp.models.default_values_and_options import DefaultValuesAndOptions
 from echowarp.services.crypto_manager import CryptoManager
 from echowarp.models.json_message import JSONMessage
-from echowarp.models.default_values_and_options import DefaultValuesAndOptions
+from echowarp.settings import Settings
 
 
 class TransportBase:
     """
-        Provides base TCP functionality for both client and server sides of the EchoWarp application.
-        Manages TCP connections, including sending heartbeats to maintain the connection and handling reconnections.
+    Provides base TCP functionality for both client and server sides of the EchoWarp application.
+    Manages TCP connections, including sending heartbeats to maintain the connection and handling reconnections.
 
-        Attributes:
-            _client_tcp_socket (socket.socket): Socket for TCP communication.
-            _tcp_port (int): TCP port used for communication, derived from UDP port.
-            _udp_port (int): UDP port used for audio streaming.
-            _stop_util_event (threading.Event): Event to signal when to terminate the application.
-            _stop_stream_event (threading.Event): Event to signal when to stop streaming.
-            _crypto_manager (CryptoManager): Manages cryptographic operations.
-            _heartbeat_attempt (int, optional): Allowed missed heartbeats before connection is considered lost.
-        """
+    Attributes:
+        _is_server (bool): Indicates if the instance is running as a server.
+        _client_tcp_socket (Optional[socket.socket]): Socket for TCP communication.
+        _udp_socket (socket.socket): Socket for UDP communication.
+        _tcp_port (int): TCP port used for communication, derived from UDP port.
+        _udp_port (int): UDP port used for audio streaming.
+        _stop_util_event (threading.Event): Event to signal when to terminate the application.
+        _stop_stream_event (threading.Event): Event to signal when to stop streaming.
+        _crypto_manager (CryptoManager): Manages cryptographic operations.
+        _reconnect_attempt (int, optional): Allowed missed heartbeats before connection is considered lost.
+        _password_base64 (Optional[str]): Base64 encoded password for authentication.
+        _socket_buffer_size (int): Buffer size for the socket.
+    """
+    _is_server: bool
     _client_tcp_socket: Optional[socket.socket]
+    _udp_socket: socket.socket
     _tcp_port: int
     _udp_port: int
     _stop_util_event: threading.Event
     _stop_stream_event: threading.Event
     _crypto_manager: CryptoManager
-    _heartbeat_attempt: Optional[int]
+    _reconnect_attempt: int
+    _password_base64: Optional[str]
+    _socket_buffer_size: int
 
-    def __init__(self, udp_port: int, stop_util_event: threading.Event, stop_stream_event: threading.Event,
-                 heartbeat_attempt: Optional[int], crypto_manager: CryptoManager):
+    def __init__(self, settings: Settings, stop_util_event: threading.Event(), stop_stream_event: threading.Event()):
         """
         Initializes the TransportBase with provided configuration.
 
         Args:
-            udp_port (int): UDP port for audio data streaming.
-            stop_util_event (threading.Event): Event to manage application lifecycle.
-            stop_stream_event (threading.Event): Event to manage streaming lifecycle.
-            heartbeat_attempt (int, optional): Number of heartbeat attempts before termination.
-            crypto_manager (CryptoManager): Manager for cryptographic operations.
+            settings (Settings): Settings object.
+            stop_util_event (threading.Event): Event to signal when to terminate the application.
+            stop_stream_event (threading.Event): Event to signal when to stop streaming.
         """
-        self._tcp_port = udp_port - 1
-        self._udp_port = udp_port
+        self._is_server = settings.is_server
+        self._tcp_port = settings.udp_port - 1
+        self._udp_port = settings.udp_port
         self._stop_util_event = stop_util_event
         self._stop_stream_event = stop_stream_event
-        self._heartbeat_attempt = heartbeat_attempt
-        self._crypto_manager = crypto_manager
+        self._reconnect_attempt = settings.reconnect_attempt
+        self._crypto_manager = settings.crypto_manager
+
         self._client_tcp_socket = None
+        self.__initialize_udp_socket()
+
+        self._password_base64 = self.__get_base64_password(settings.password)
 
-    def start_heartbeat(self, audio_thread: threading.Thread):
+        self._socket_buffer_size = settings.socket_buffer_size
+
+        self.__stop_message_send = False
+
+    def start_streaming(self, audio_thread: threading.Thread):
         """
-        Continuously sends heartbeat messages to maintain the connection alive. If the heartbeat fails consecutively
-        beyond a specified limit, the connection is considered lost and the thread signals the application to stop.
+        Starts the streaming process by continuously sending heartbeat messages to maintain the connection alive.
+        If the heartbeat fails consecutively beyond a specified limit, the connection is considered lost and the thread signals the application to stop.
+
+        Args:
+            audio_thread (threading.Thread): Thread for handling audio streaming.
 
         Raises:
             RuntimeError: Raised if too many consecutive heartbeat messages are missed, indicating a connection issue.
         """
         audio_thread.start()
-        heartbeat_interval = 5
+        heartbeat_delay = DefaultValuesAndOptions.get_heartbeat_delay()
 
         while not self._stop_util_event.is_set():
             try:
-                heartbeat_message = JSONMessage.encode_message_to_json_bytes(JSONMessage.HEARTBEAT_MESSAGE, 200)
-                self._client_tcp_socket.sendall(self._crypto_manager.encrypt_aes_and_sign_data(heartbeat_message))
-
-                encrypted_response = self._client_tcp_socket.recv(DefaultValuesAndOptions.SOCKET_BUFFER_SIZE)
-                decrypt_response = self._crypto_manager.decrypt_aes_and_verify_data(encrypted_response)
-                response_message = JSONMessage(decrypt_response)
-
-                if response_message.message != JSONMessage.HEARTBEAT_MESSAGE or response_message.response_code != 200:
-                    raise ValueError(
-                        f"Response heartbeat message: {response_message.response_code} {response_message.message}")
+                self.__send_and_get_heartbeat_message()
 
-                time.sleep(heartbeat_interval)
+                time.sleep(heartbeat_delay)
             except ValueError as e:
                 logging.error(e)
                 self.__reconnect()
-            except socket.error as e:
+            except RuntimeError as e:
+                logging.info(e)
+
+                if self._is_server:
+                    self.__reconnect(True)
+                else:
+                    break
+
+            except (socket.error, socket.timeout) as e:
                 logging.error(f"Heartbeat failed due to network error: {e}")
                 self.__reconnect()
             except Exception as e:
                 logging.error(f"Unexpected error during heartbeat: {e}")
                 self.__reconnect()
 
-    def __reconnect(self):
+        self._shutdown()
+
+    def __send_and_get_heartbeat_message(self):
+        """
+        Sends and receives heartbeat messages for connection validation.
+        """
+        if self._is_server:
+            self.__receive_heartbeat_and_validate()
+            self.__format_and_send_heartbeat()
+        else:
+            self.__format_and_send_heartbeat()
+            self.__receive_heartbeat_and_validate()
+
+    @staticmethod
+    def __get_base64_password(password: Optional[str]) -> Optional[str]:
+        """
+        Encodes the password to Base64 format.
+
+        Args:
+            password (Optional[str]): The password to encode.
+
+        Returns:
+            Optional[str]: The Base64 encoded password.
+        """
+        if password is None:
+            return password
+        else:
+            return base64.b64encode(password.encode("utf-8")).decode("utf-8")
+
+    def __receive_heartbeat_and_validate(self):
+        """
+        Receives and validates the heartbeat message.
+        """
+        encrypted_response = self._client_tcp_socket.recv(self._socket_buffer_size)
+        if encrypted_response == b'':
+            raise ValueError('Heartbeat message from client is NULL')
+
+        decrypt_response = self._crypto_manager.decrypt_aes_and_verify_data(encrypted_response)
+        response_message = JSONMessage(decrypt_response)
+
+        if (response_message.message == JSONMessage.LOCKED_MESSAGE.response_message and
+                response_message.response_code == JSONMessage.LOCKED_MESSAGE.response_code):
+            raise RuntimeError("Received shutdown event. Close connection.")
+
+        elif (response_message.message != JSONMessage.ACCEPTED_MESSAGE.response_message or
+              response_message.response_code != JSONMessage.ACCEPTED_MESSAGE.response_code):
+            raise ValueError(
+                f"Response heartbeat message: {response_message.response_code} {response_message.message}")
+
+    def __format_and_send_heartbeat(self):
+        """
+        Formats and sends a heartbeat message.
+        """
+        if self._stop_util_event.is_set():
+            message = JSONMessage.encode_message_to_json_bytes(
+                JSONMessage.LOCKED_MESSAGE.response_message,
+                JSONMessage.LOCKED_MESSAGE.response_code,
+                None,
+                None
+            )
+            self.__stop_message_send = True
+        else:
+            message = JSONMessage.encode_message_to_json_bytes(
+                JSONMessage.ACCEPTED_MESSAGE.response_message,
+                JSONMessage.ACCEPTED_MESSAGE.response_code,
+                None,
+                None
+            )
+
+        self._client_tcp_socket.sendall(self._crypto_manager.encrypt_aes_and_sign_data(message))
+
+    def __reconnect(self, is_client_exit=False):
+        """
+        Handles the reconnection logic for the transport layer.
+
+        Args:
+            is_client_exit (bool): Indicates if the client should exit.
+        """
+        self._print_pause_udp_listener_and_pause_stream()
+
         try:
-            logging.info("Attempting to stabilize the connection...")
-            if self.__try_send_heartbeat():
-                return
+            if not is_client_exit:
+                logging.info("Attempting to stabilize the connection...")
+                if self.__retry_send_heartbeat():
+                    return
 
-            self._cleanup_client_sockets()
-            self._initialize_socket()
+            self._cleanup_tcp_socket()
 
-            self.__perform_reconnect_attempts()
+            if self._is_server:
+                self._established_connection()
+            else:
+                self._initialize_socket()
+                self.__perform_reconnect_attempts()
+
+            if not self._stop_util_event.is_set():
+                self._print_udp_listener_and_start_stream()
+            else:
+                self._shutdown()
+        except RuntimeError as e:
+            logging.error(e)
+            self._shutdown()
         except Exception as e:
-            logging.error(f"Critical error during heartbeat: {e}")
-            self._stop_util_event.set()
-            raise
+            raise Exception(f"Critical error during reconnect: {e}")
 
-    def __try_send_heartbeat(self):
+    def __retry_send_heartbeat(self) -> bool:
+        """
+        Retries sending the heartbeat message.
+
+        Returns:
+            bool: True if the heartbeat was successfully sent, False otherwise.
+        """
         try:
-            heartbeat_message = JSONMessage.encode_message_to_json_bytes(JSONMessage.HEARTBEAT_MESSAGE, 200)
-            self._client_tcp_socket.sendall(self._crypto_manager.encrypt_aes_and_sign_data(heartbeat_message))
+            self.__send_and_get_heartbeat_message()
             logging.info("Connection stabilized with heartbeat.")
+
             return True
-        except socket.error:
-            logging.warning("Failed to send heartbeat.")
+        except ValueError as e:
+            logging.error(e)
+
             return False
+        except (socket.error, socket.timeout) as e:
+            logging.error(f"Failed to retry send heartbeat due socket exception: {e}")
 
-    def _cleanup_client_sockets(self):
-        try:
-            if self._client_tcp_socket:
-                self._client_tcp_socket.shutdown(socket.SHUT_RDWR)
-                self._client_tcp_socket.close()
-                self._client_tcp_socket = None
-        except socket.error as e:
-            logging.error(f"Error closing client TCP socket: {e}")
+            return False
         except Exception as e:
-            logging.error(f"Unhandled exception during TCP socket cleanup: {e}")
+            logging.error(f"Unexpected exception due retry sending heartbeat: {e}")
+
+            return False
 
     def __perform_reconnect_attempts(self):
+        """
+        Performs reconnection attempts until the maximum allowed attempts are reached.
+        """
         attempt = 0
-        while not self._stop_util_event.is_set() and attempt < self._heartbeat_attempt:
+        reconnect_delay = DefaultValuesAndOptions.get_heartbeat_delay()
+
+        while not self._stop_util_event.is_set() and attempt < self._reconnect_attempt:
             try:
                 self._established_connection()
                 logging.info(f"Reconnection successful on attempt {attempt + 1}")
+
                 break
-            except socket.error as e:
+            except (socket.error, socket.timeout) as e:
                 attempt += 1
-                logging.warning(
-                    f"Reconnect failed due to socket error: {e}, retrying... "
-                    f"(Attempt {attempt}/{self._heartbeat_attempt})")
-                time.sleep(5)
-            except Exception as e:
+                logging.error(f"Reconnect failed due to socket error:{os.linesep}{e}"
+                              f"{self.__get_str_reconnect_attempt(attempt)}")
+                time.sleep(reconnect_delay)
+            except ValueError as e:
                 attempt += 1
-                logging.error(
-                    f"Reconnect failed due to an unexpected error: {e}, retrying... "
-                    f"(Attempt {attempt}/{self._heartbeat_attempt})")
-                time.sleep(5)
-
-        if attempt >= self._heartbeat_attempt:
-            self._stop_util_event.set()
-            logging.error("Maximum reconnect attempts reached, terminating connection.")
-            raise RuntimeError("Connection lost due to missed reconnect attempts")
+                logging.error(f"Reconnect failed due:{os.linesep}{e}"
+                              f"{self.__get_str_reconnect_attempt(attempt)}")
+                time.sleep(reconnect_delay)
+
+        if attempt >= self._reconnect_attempt:
+            self._shutdown()
+            raise RuntimeError("Maximum reconnect attempts reached, terminating connection.")
+
+    def __get_str_reconnect_attempt(self, attempt: int) -> str:
+        """
+        Returns a formatted string representing the reconnect attempt.
+
+        Args:
+            attempt (int): The current attempt number.
+
+        Returns:
+            str: Formatted string representing the reconnect attempt.
+        """
+        if self._reconnect_attempt == 0:
+            return f"{os.linesep}Retrying connection... (Reconnect attempt: {attempt})"
+        else:
+            return f"{os.linesep}Retrying connection... (Reconnect attempt: {attempt}/{self._reconnect_attempt})"
 
-        self._print_listener()
+    def _cleanup_tcp_socket(self):
+        """
+        Cleans up the TCP socket.
+        """
+        try:
+            if self._client_tcp_socket:
+                self._client_tcp_socket.shutdown(socket.SHUT_RDWR)
+                self._client_tcp_socket.close()
+        except socket.error as e:
+            logging.error(f"Error closing client TCP socket: {e}")
+        except Exception as e:
+            logging.error(f"Unhandled exception during TCP socket cleanup: {e}")
+
+    def _cleanup_udp_socket(self):
+        """
+        Cleans up the UDP socket.
+        """
+        try:
+            if self._udp_socket:
+                self._udp_socket.close()
+        except socket.error as e:
+            logging.error(f"Error closing client UDP socket: {e}")
+        except Exception as e:
+            logging.error(f"Unhandled exception during UDP socket cleanup: {e}")
+
+    def _shutdown(self):
+        """
+        Shuts down the transport, signaling stop events and cleaning up sockets.
+        """
+        if not self.__stop_message_send:
+            shutdown_message = JSONMessage.encode_message_to_json_bytes(
+                JSONMessage.LOCKED_MESSAGE.response_message,
+                JSONMessage.LOCKED_MESSAGE.response_code,
+                None,
+                None
+            )
+            self._client_tcp_socket.sendall(self._crypto_manager.encrypt_aes_and_sign_data(shutdown_message))
+
+        self._stop_util_event.set()
+        self._stop_stream_event.set()
+
+        time.sleep(5)
+
+        self._cleanup_tcp_socket()
+        self._cleanup_udp_socket()
+
+    def __initialize_udp_socket(self):
+        """
+        Initializes the UDP socket.
+        """
+        self._udp_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
+        self._udp_socket.settimeout(DefaultValuesAndOptions.get_timeout())
+
+    def _init_tcp_connection(self):
+        """
+        Initializes the TCP connection.
+        """
+        self._initialize_socket()
+        try:
+            self._established_connection()
+        except (socket.error, socket.timeout, RuntimeError, ValueError) as e:
+            self._shutdown()
+            raise RuntimeError(e)
+        except Exception as e:
+            self._shutdown()
+            raise Exception(f"TCP connection failed: {e}")
+
+    @abstractmethod
+    def _print_udp_listener_and_start_stream(self):
+        pass
 
     @abstractmethod
-    def _print_listener(self):
+    def _print_pause_udp_listener_and_pause_stream(self):
         pass
 
     @abstractmethod
     def _initialize_socket(self):
         pass
 
     @abstractmethod
-    def _established_connection(self, is_reconnect=True):
+    def _established_connection(self):
         pass
```

## echowarp/auth_and_heartbeat/transport_client.py

```diff
@@ -1,147 +1,122 @@
+import os
 import socket
 import logging
 import threading
-import time
 from abc import ABC
-from typing import Optional
 
 from echowarp.auth_and_heartbeat.transport_base import TransportBase
-from echowarp.services.crypto_manager import CryptoManager
 from echowarp.models.json_message import JSONMessage, JSONMessageServer
 from echowarp.models.default_values_and_options import DefaultValuesAndOptions
+from echowarp.settings import Settings
 
 
 class TransportClient(TransportBase, ABC):
     """
     Manages TCP client operations for EchoWarp, including connection establishment,
     server authentication, and secure data exchange.
 
     Attributes:
         _server_address (str): The IP address or hostname of the server.
     """
-    _client_udp_socket: Optional[socket.socket]
     _server_address: str
 
-    def __init__(self, server_address: str, udp_port: int, stop_util_event: threading.Event,
-                 stop_stream_event: threading.Event, crypto_manager: CryptoManager):
+    def __init__(self, settings: Settings, stop_util_event: threading.Event(), stop_stream_event: threading.Event()):
         """
         Initializes the TCP client with the necessary configuration to establish a connection.
 
         Args:
-            server_address (str): The server's IP address or hostname.
-            udp_port (int): The TCP port on the server to connect to.
-            stop_util_event (threading.Event): An event to signal the thread to stop operations.
-            stop_stream_event (threading.Event): An event to signal the thread to stop operations.
-            crypto_manager (CryptoManager): An instance to manage cryptographic operations.
+            settings (Settings): Settings object.
         """
-        super().__init__(udp_port, stop_util_event, stop_stream_event, None, crypto_manager)
-        self._server_address = server_address
-        self._client_udp_socket = None
+        super().__init__(settings, stop_util_event, stop_stream_event)
+        self._server_address = settings.server_address
+        self._udp_socket.bind((self._server_address, self._udp_port))
 
-        self._start_tcp_client()
+        self._init_tcp_connection()
 
-    def _start_tcp_client(self):
-        """
-        Establishes a TCP connection to the server, authenticates and sets up the secure communication channel.
-
-        Raises:
-            ConnectionError: If there is an issue with connecting to the server.
-            ValueError: If the server's response during authentication is invalid.
-        """
-        self._initialize_socket()
-
-        try:
-            self._established_connection(False)
-        except socket.error as e:
-            logging.error(f"Failed to establish connection to {self._server_address}:{self._tcp_port}: {e}")
-            self._cleanup_client_sockets()
-            raise ConnectionError(f"Failed to establish connection to {self._server_address}:{self._tcp_port}")
-        except Exception as e:
-            logging.error(f"Authentication or encryption setup failed: {e}")
-            self._cleanup_client_sockets()
-
-    def __authenticate_with_server(self):
+    def __authenticate_on_server(self):
         """
         Performs authentication with the server using RSA encryption for the exchange of credentials.
 
         Raises:
             ValueError: If the authentication with the server fails or if versions mismatch.
         """
-        try:
-            self._client_tcp_socket.sendall(self._crypto_manager.get_serialized_public_key())
-            server_public_key_pem = self._client_tcp_socket.recv(DefaultValuesAndOptions.SOCKET_BUFFER_SIZE)
-            self._crypto_manager.load_peer_public_key(server_public_key_pem)
-
-            client_auth_message_bytes = JSONMessage.encode_message_to_json_bytes(
-                JSONMessage.AUTH_CLIENT_MESSAGE,
-                200
-            )
 
-            self._client_tcp_socket.sendall(self._crypto_manager.encrypt_rsa_message(client_auth_message_bytes))
+        self._client_tcp_socket.sendall(self._crypto_manager.get_serialized_public_key())
+        server_public_key_pem = self._client_tcp_socket.recv(self._socket_buffer_size)
+        self._crypto_manager.load_peer_public_key(server_public_key_pem)
+
+        client_auth_message_bytes = JSONMessage.encode_message_to_json_bytes(
+            self._password_base64,
+            JSONMessage.OK_MESSAGE.response_code,
+            None,
+            None
+        )
+
+        self._client_tcp_socket.sendall(self._crypto_manager.encrypt_rsa_message(client_auth_message_bytes))
+
+        encrypted_message_from_server = self._client_tcp_socket.recv(self._socket_buffer_size)
+        message_from_server = self._crypto_manager.decrypt_rsa_message(encrypted_message_from_server)
+        server_message = JSONMessage(message_from_server)
+        config_server_message = None
+
+        client_failed_connects = server_message.failed_connections
+        reconnect_attempts = server_message.reconnect_attempts
+        if reconnect_attempts is not None:
+            client_failed_connects = f'{client_failed_connects}/{reconnect_attempts}'
+
+        client_failed_connect_str = f'Client failed connect attempts on server: {client_failed_connects}'
 
-            encrypted_message_from_server = self._client_tcp_socket.recv(DefaultValuesAndOptions.SOCKET_BUFFER_SIZE)
-            message_from_server = self._crypto_manager.decrypt_rsa_message(encrypted_message_from_server)
+        if (server_message.message == JSONMessage.OK_MESSAGE.response_message
+                and server_message.response_code == JSONMessage.OK_MESSAGE.response_code):
             config_server_message = JSONMessageServer(message_from_server)
 
-            if (config_server_message.message != JSONMessageServer.AUTH_SERVER_MESSAGE
-                    or config_server_message.response_code != 200):
-                logging.error(
-                    f"Failed to authenticate server. Message from server: "
-                    f"{config_server_message.response_code} {config_server_message.message}")
-                raise ValueError("Server authentication failed.")
-
-            if config_server_message.version != DefaultValuesAndOptions.get_util_version():
-                logging.error(f"Client version not equal server version: "
-                              f"{DefaultValuesAndOptions.get_util_version()} - Client, "
-                              f"{config_server_message.version} - Server")
-                raise ValueError("Version mismatch between client and server.")
-
-            self._crypto_manager.load_aes_key_and_iv(config_server_message.aes_key,
-                                                     config_server_message.aes_iv)
-            self._crypto_manager.load_encryption_config_for_client(config_server_message.is_encrypt,
-                                                                   config_server_message.is_integrity_control)
-            self._heartbeat_attempt = config_server_message.heartbeat_attempt
+        elif (server_message.message == JSONMessage.FORBIDDEN_MESSAGE.response_message
+              or server_message.response_code == JSONMessage.FORBIDDEN_MESSAGE.response_code):
+            raise RuntimeError(f"Client is banned! Message from server: "
+                               f"{server_message.response_code} {server_message.message}"
+                               f"{os.linesep}{client_failed_connect_str}")
+
+        elif (server_message.message == JSONMessage.UNAUTHORIZED_MESSAGE.response_message
+              or server_message.response_code == JSONMessage.UNAUTHORIZED_MESSAGE.response_code):
+            raise ValueError(f"Invalid password! Message from server: "
+                             f"{server_message.response_code} {server_message.message}"
+                             f"{os.linesep}{client_failed_connect_str}")
+
+        if server_message.version != DefaultValuesAndOptions.get_util_comparability_version():
+            raise ValueError(f"Client comparability version not equal server version: "
+                             f"{DefaultValuesAndOptions.get_util_comparability_version()} - Client, "
+                             f"{server_message.version} - Server"
+                             f"{os.linesep}{client_failed_connect_str}")
+
+        self._crypto_manager.load_aes_key_and_iv(config_server_message.aes_key_base64,
+                                                 config_server_message.aes_iv_base64)
+        self._crypto_manager.load_encryption_config_for_client(config_server_message.is_encrypt,
+                                                               config_server_message.is_integrity_control)
 
-            logging.info("Authentication and load config from server completed successfully.")
-        except socket.error as e:
-            logging.error(f"Failed to send/receive data: {e}")
-            self._stop_util_event.set()
-        except RuntimeError as e:
-            logging.error(f"Failed to maintain connection: {e}")
-            self._stop_util_event.set()
-        except Exception as e:
-            logging.error(f"Error during authentication: {e}")
-            self._stop_util_event.set()
+        logging.info(f"Authentication on server completed.")
 
     def _initialize_socket(self):
         self._client_tcp_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self._client_tcp_socket.settimeout(DefaultValuesAndOptions.get_timeout())
 
-        self._client_udp_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-        self._client_udp_socket.bind((self._server_address, self._udp_port))
-        self._client_udp_socket.settimeout(5.0)
-
-    def _established_connection(self, is_reconnect=True):
-        self._stop_stream_event.clear()
-        if is_reconnect:
-            self._client_tcp_socket.connect((self._server_address, self._tcp_port))
-        else:
-            while not self._stop_util_event.is_set():
-                try:
-                    self._client_tcp_socket.connect((self._server_address, self._tcp_port))
-                    break
-                except socket.error as e:
-                    logging.error(f"Failed to connect to {self._server_address}:{self._tcp_port}: {e}")
-                    time.sleep(5)
-
-        logging.info(f"TCP connection to {self._server_address}:{self._tcp_port} established.")
-        self.__authenticate_with_server()
-        self._stop_stream_event.set()
+    def _established_connection(self):
+        self._client_tcp_socket.connect((self._server_address, self._tcp_port))
 
-    def _cleanup_client_sockets(self):
-        super()._cleanup_client_sockets()
+        logging.info(f"TCP connection to {self._server_address} established.")
 
         try:
-            if self._client_udp_socket:
-                self._client_udp_socket.close()
+            self.__authenticate_on_server()
+        except socket.timeout as e:
+            raise socket.timeout(f"Timeout from server socket while authenticating: {e}")
         except socket.error as e:
-            logging.error(f"Error closing client UDP socket: {e}")
+            raise socket.error(f"Failed to send/receive data: {e}")
+        except ValueError as e:
+            raise ValueError(e)
+
+    def _print_udp_listener_and_start_stream(self):
+        logging.info(f'UDP listening started from {self._server_address}:{self._udp_port}')
+        self._stop_stream_event.set()
+
+    def _print_pause_udp_listener_and_pause_stream(self):
+        logging.warning(f'Audio listening paused!')
+        self._stop_stream_event.clear()
```

## echowarp/auth_and_heartbeat/transport_server.py

```diff
@@ -1,170 +1,201 @@
 import logging
+import os
 import socket
 import threading
 from abc import ABC
 from typing import Optional
 
 from echowarp.auth_and_heartbeat.transport_base import TransportBase
-from echowarp.services.crypto_manager import CryptoManager
+from echowarp.models.ban_list import BanList
 from echowarp.models.json_message import JSONMessageServer, JSONMessage
 from echowarp.models.default_values_and_options import DefaultValuesAndOptions
+from echowarp.settings import Settings
 
 
 class TransportServer(TransportBase, ABC):
     """
     Manages TCP server operations for EchoWarp, including handling client connections,
     authentication, and setting up a secure communication channel.
 
     Attributes:
-        _client_addr (Optional[str]): IP address of the connected client.
-        _tcp_server_socket (Optional[socket.socket]): Server TCP socket for accepting client connections.
-        _udp_server_socket (Optional[socket.socket]): Server UDP socket for accepting client connections.
+        _client_address (Optional[str]): IP address of the connected client.
         _stop_util_event (threading.Event): Event to signal util to stop.
         _stop_stream_event (threading.Event): Event to signal stream to stop.
     """
-    _client_addr: Optional[str]
-    _tcp_server_socket: Optional[socket.socket]
-    _udp_server_socket: Optional[socket.socket]
+    _server_tcp_socket: socket.socket
+    _client_address: Optional[str]
+    __ban_list: BanList
 
-    def __init__(self, udp_port, heartbeat_attempt: int, stop_util_event: threading.Event,
-                 stop_stream_event: threading.Event, crypto_manager: CryptoManager):
+    def __init__(self, settings: Settings, stop_util_event: threading.Event(), stop_stream_event: threading.Event()):
         """
         Initializes the TCPServer with specified configuration parameters.
 
         Args:
-            udp_port (int): The port number on which the server listens for incoming TCP connections.
-            heartbeat_attempt (int): The number of allowed missed heartbeats before considering the connection lost.
-            stop_util_event (threading.Event): An event to signal the server to stop operations.
-            stop_stream_event (threading.Event): An event to signal the server to stop operations.
-            crypto_manager (CryptoManager): An instance to manage cryptographic operations.
+            settings (Settings): Settings object.
         """
-        super().__init__(udp_port, stop_util_event, stop_stream_event, heartbeat_attempt, crypto_manager)
+        super().__init__(settings, stop_util_event, stop_stream_event)
 
-        self._client_addr = None
-        self._tcp_server_socket = None
-        self._udp_server_socket = None
+        self._client_address = None
+        self.__ban_list = BanList(settings.reconnect_attempt)
 
-        self._start_tcp_server()
-
-    def _start_tcp_server(self):
-        """
-        Starts the TCP server, listens for incoming connections, and handles client authentication and setup.
-        """
-        self._tcp_server_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self._udp_server_socket = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
-
-        self._tcp_server_socket.bind(('0.0.0.0', self._tcp_port))
-        self._tcp_server_socket.listen(1)
-
-        logging.info(f'TCP server started on port "{self._tcp_port}" awaiting client connection')
-
-        try:
-            self._established_connection(False)
-        except Exception as e:
-            logging.error(f"Server encountered an error: {e}")
-            self._cleanup_client_sockets()
-            self._cleanup_server_socket()
+        self._init_tcp_connection()
 
     def __authenticate_client(self):
         """
         Handles the authentication sequence with the client by exchanging encrypted messages and
         establishing encryption settings.
 
         Raises:
             ValueError: If client authentication fails or there is a version mismatch.
         """
-        try:
-            self._client_tcp_socket.sendall(self._crypto_manager.get_serialized_public_key())
-
-            client_public_key_pem = self._client_tcp_socket.recv(DefaultValuesAndOptions.SOCKET_BUFFER_SIZE)
-            self._crypto_manager.load_peer_public_key(client_public_key_pem)
-
-            encrypted_message_from_client = self._client_tcp_socket.recv(DefaultValuesAndOptions.SOCKET_BUFFER_SIZE)
-            message_from_client = self._crypto_manager.decrypt_rsa_message(encrypted_message_from_client)
-
-            client_auth_message = JSONMessage(message_from_client)
 
-            if (client_auth_message.message != JSONMessage.AUTH_CLIENT_MESSAGE
-                    or client_auth_message.response_code != 200):
-                error_message = "Forbidden"
-                error_message_bytes = JSONMessage.encode_message_to_json_bytes(error_message, 403)
+        self._client_tcp_socket.sendall(self._crypto_manager.get_serialized_public_key())
 
-                self._client_tcp_socket.sendall(self._crypto_manager.encrypt_rsa_message(error_message_bytes))
+        client_public_key_pem = self._client_tcp_socket.recv(self._socket_buffer_size)
+        self._crypto_manager.load_peer_public_key(client_public_key_pem)
 
-                logging.error(f"Failed to authenticate client. Client sent message: {client_auth_message.message}")
-                raise ValueError("Client authentication failed.")
+        encrypted_message_from_client = self._client_tcp_socket.recv(self._socket_buffer_size)
+        message_from_client = self._crypto_manager.decrypt_rsa_message(encrypted_message_from_client)
 
-            logging.info("Client authenticated")
-
-            if client_auth_message.version != DefaultValuesAndOptions.get_util_version():
-                error_message = (f"Client version not equal server version: "
-                                 f"{client_auth_message.version} - Client, "
-                                 f"{DefaultValuesAndOptions.get_util_version()} - Server")
-                error_message_bytes = JSONMessage.encode_message_to_json_bytes(error_message, 500)
-
-                self._client_tcp_socket.sendall(self._crypto_manager.encrypt_rsa_message(error_message_bytes))
+        client_auth_message = JSONMessage(message_from_client)
+
+        if self.__ban_list.is_banned(self._client_address):
+            self.__form_error_message(
+                JSONMessage.FORBIDDEN_MESSAGE.response_message,
+                JSONMessage.FORBIDDEN_MESSAGE.response_code,
+                f"Failed to authenticate client: {self._client_address}. "
+                f"Client is {JSONMessage.FORBIDDEN_MESSAGE.response_message}"
+            )
+
+        if client_auth_message.message != self._password_base64:
+            self.__form_error_message(
+                JSONMessage.UNAUTHORIZED_MESSAGE.response_message,
+                JSONMessage.UNAUTHORIZED_MESSAGE.response_code,
+                f"Failed to authenticate client: {self._client_address}. "
+                f"Client is {JSONMessage.UNAUTHORIZED_MESSAGE.response_message}"
+            )
+
+        if client_auth_message.version != DefaultValuesAndOptions.get_util_comparability_version():
+            self.__form_error_message(
+                JSONMessage.CONFLICT_MESSAGE.response_message,
+                JSONMessage.CONFLICT_MESSAGE.response_code,
+                f"Client version not equal server version: "
+                f"{client_auth_message.version} - Client, "
+                f"{DefaultValuesAndOptions.get_util_comparability_version()} - Server"
+            )
+
+        logging.info(f"Client {self._client_address} authenticated.")
+        self.__ban_list.success_connect_attempt(self._client_address)
+        self.__print_client_info()
+
+        self.__send_configuration()
+
+    def __form_error_message(self, response_message: str, response_code: int, exception_message: str):
+        self.__ban_list.fail_connect_attempt(self._client_address)
+
+        error_message_bytes = JSONMessage.encode_message_to_json_bytes(
+            response_message,
+            response_code,
+            self.__ban_list.get_failed_connect_attempts(self._client_address),
+            self._reconnect_attempt
+        )
 
-                logging.error(error_message)
-                raise ValueError("Version mismatch between client and server.")
-
-            self.__send_configuration()
-        except socket.error as e:
-            logging.error(f"Failed to send/receive data: {e}")
-            self._stop_util_event.set()
-        except RuntimeError as e:
-            logging.error(f"Failed to maintain connection: {e}")
-            self._stop_util_event.set()
-        except Exception as e:
-            logging.error(f"Error during authentication: {e}")
-            self._stop_util_event.set()
+        self._client_tcp_socket.sendall(self._crypto_manager.encrypt_rsa_message(error_message_bytes))
+        raise ValueError(exception_message)
 
     def __send_configuration(self):
         """
         Sends the configuration settings to the connected client, including security settings and AES keys.
 
         The configuration is sent as an encrypted JSON string.
         """
         config_json = JSONMessageServer.encode_server_config_to_json_bytes(
-            self._heartbeat_attempt, self._crypto_manager.is_encrypt, self._crypto_manager.is_hash_control,
-            self._crypto_manager.get_aes_key(), self._crypto_manager.get_aes_iv()
+            self._crypto_manager.is_ssl, self._crypto_manager.is_integrity_control,
+            self._crypto_manager.get_aes_key_base64(), self._crypto_manager.get_aes_iv_base64(),
+            self.__ban_list.get_failed_connect_attempts(self._client_address), self._reconnect_attempt
         )
 
         self._client_tcp_socket.sendall(self._crypto_manager.encrypt_rsa_message(config_json))
         logging.info("Configuration sent to client.")
 
     def _initialize_socket(self):
-        pass
+        self._server_tcp_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+        self._server_tcp_socket.bind(('0.0.0.0', self._tcp_port))
+        self._server_tcp_socket.settimeout(DefaultValuesAndOptions.get_timeout())
+        self._server_tcp_socket.listen(1)
 
-    def _established_connection(self, is_reconnect=True):
-        self._tcp_server_socket.settimeout(5.0)
-        is_connected = False
+    def _established_connection(self):
+        is_log = True
         while not self._stop_util_event.is_set():
+            if is_log:
+                logging.info(f'Authenticate server started and awaiting client connection')
+
             try:
-                self._stop_stream_event.clear()
-                self._client_tcp_socket, client_addr = self._tcp_server_socket.accept()
-            except socket.timeout:
+                self._client_tcp_socket, client_address = self._server_tcp_socket.accept()
+            except (socket.error, socket.timeout):
+                is_log = False
                 continue
 
-            self._client_addr = client_addr[0]
+            is_log = True
+            self._client_address = client_address[0]
+            self.__ban_list.add_client_to_ban_list(self._client_address)
+
+            if self.__ban_list.is_banned(self._client_address) and not self.__ban_list.is_first_time_message(
+                    self._client_address):
+                logging.error(f'Client {self._client_address} banned!')
+                self.__ban_list.fail_connect_attempt(self._client_address)
+                continue
 
-            logging.info(f"Client connected from {self._client_addr}")
+            logging.info(f"Client connected from {self._client_address}")
 
-            self.__authenticate_client()
-            is_connected = True
-            break
+            try:
+                self.__authenticate_client()
+            except ValueError as e:
+                logging.error(e)
+                self.__print_client_info()
+                continue
+            except (socket.error, socket.timeout) as e:
+                logging.error(f"Failed to send/receive data: {e}")
+                self.__print_client_info()
+                continue
+            except Exception as e:
+                logging.error(f"Error during authentication: {e}")
+                self.__print_client_info()
+                continue
+            finally:
+                self.__ban_list.update_ban_list_file()
 
-        self._stop_stream_event.set()
+            break
 
-        if not is_connected:
-            raise RuntimeError
+    def __print_client_info(self):
+        success_connections = self.__ban_list.get_success_connect_attempts(self._client_address)
+        failed_connections = self.__ban_list.get_failed_connect_attempts(self._client_address)
+        all_failed_connections = self.__ban_list.get_all_failed_connect_attempts(self._client_address)
+
+        failed_connections_attempts = f'{failed_connections}/{self._reconnect_attempt}' if self._reconnect_attempt > 0 \
+            else failed_connections
+
+        logging.info(
+            f"Client {self._client_address} info:{os.linesep}"
+            f"Success client connections: {success_connections}{os.linesep}"
+            f"Failed client connection attempts after last success: {failed_connections_attempts}{os.linesep}"
+            f"Count of failed client connections: {all_failed_connections}"
+        )
 
-    def _cleanup_server_socket(self):
+    def _shutdown(self):
+        super()._shutdown()
         try:
-            if self._tcp_server_socket:
-                self._tcp_server_socket.shutdown(socket.SHUT_RDWR)
-                self._tcp_server_socket.close()
-                self._tcp_server_socket = None
+            if self._server_tcp_socket:
+                self._server_tcp_socket.close()
         except socket.error as e:
-            logging.error(f"Error closing server socket: {e}")
+            logging.error(f"Error closing server TCP socket: {e}")
         except Exception as e:
-            logging.error(f"Unhandled exception during server socket cleanup: {e}")
+            logging.error(f"Unhandled exception during TCP socket cleanup: {e}")
+
+    def _print_udp_listener_and_start_stream(self):
+        logging.info(f"Start UDP audio streaming to client {self._client_address}:{self._udp_port}")
+        self._stop_stream_event.set()
+
+    def _print_pause_udp_listener_and_pause_stream(self):
+        logging.warning(f'Audio streaming paused!')
+        self._stop_stream_event.clear()
```

## echowarp/models/audio_device.py

```diff
@@ -1,156 +1,201 @@
-import locale
 import logging
 import os
 import platform
 import subprocess
-from typing import List, Optional
+from dataclasses import dataclass
+from typing import List, Optional, Mapping
 
+import chardet
 import pyaudio
 
 
+@dataclass
+class Device:
+    id: int
+    dev: Mapping
+    device_name: str
+    audio_devices_str: str
+
+
 class AudioDevice:
     """
     Represents an audio device for recording or playback, handling device selection and configuration.
 
     Attributes:
         py_audio (pyaudio.PyAudio): Instance of PyAudio used to interface with audio hardware.
         device_name (str): The name of the device.
         device_index (int): The index of the device as used by PyAudio.
         channels (int): Number of audio channels supported by the device.
         sample_rate (int): The sample rate (in Hz) of the device.
     """
     py_audio: pyaudio.PyAudio
     device_name: str
+    device_id: Optional[int]
     device_index: int
     channels: int
     sample_rate: int
+    ignore_device_encoding_names: bool
+    device_encoding_names: str
 
-    def __init__(self, is_input_device: bool, device_id: Optional[int]):
+    def __init__(self, is_input_device: bool, device_id: Optional[int], ignore_device_encoding_names: bool,
+                 device_encoding_names: str):
         """
         Initializes an audio device, either for input or output, based on the provided parameters.
 
         Args:
             is_input_device (bool): Set to True to initialize as an input device, False for output.
             device_id (Optional[int]): Specific device ID to use. If None, the user will select a device interactively.
         """
-        self.__is_input_device = is_input_device
-        self.__device_id = device_id
+        self.is_input_device = is_input_device
+        self.device_id = device_id
         self.py_audio = pyaudio.PyAudio()
 
-        if self.__device_id is None:
+        self.ignore_device_encoding_names = ignore_device_encoding_names
+        self.device_encoding_names = device_encoding_names
+
+        if self.device_id is None:
             self.__select_audio_device()
         else:
             self.__select_audio_device_by_device_id()
 
     def __select_audio_device_by_device_id(self):
-        self.device_index = self.__device_id
-        dev = self.py_audio.get_device_info_by_index(self.device_index)
+        self.device_index = self.device_id
+        try:
+            dev = self.py_audio.get_device_info_by_index(self.device_index)
+        except Exception as e:
+            raise Exception(f"Selected invalid device id - {self.device_index}: {e}")
+
         self.device_name = self.__decode_string(dev['name'])
         self.sample_rate = int(dev['defaultSampleRate'])
 
         if dev['maxInputChannels'] > 0:
             self.channels = dev['maxInputChannels']
         else:
             self.channels = dev['maxOutputChannels']
 
     def __select_audio_device(self):
         """
                 Prompts the user to select an audio device from the list of available devices.
         """
-        if self.__is_input_device:
+        if self.is_input_device:
             device_type = 'Input'
         else:
             device_type = 'Output'
 
-        logging.info(f"Select id of {device_type} audio device:")
+        device_list = self.__get_id_list_of_devices(device_type)
+        if len(device_list) == 0:
+            raise Exception(f"No connected {device_type} audio devices found!")
 
-        id_list = self.__get_id_list_of_devices(device_type)
+        self.__print_list_of_audio_devices(device_type, device_list)
+        device_indexes = [device.id for device in device_list]
         device_index = None
 
-        while device_index not in id_list:
+        while device_index not in device_indexes:
             try:
                 device_index = input()
                 device_index = int(device_index)
             except Exception as e:
                 logging.error(f'Selected invalid device id: {device_index}{os.linesep}{e}')
 
         self.device_index = device_index
+        self.device_id = device_index
         dev = self.py_audio.get_device_info_by_index(self.device_index)
         self.device_name = self.__decode_string(dev['name'])
         self.channels = dev[f'max{device_type}Channels']
         self.sample_rate = int(dev['defaultSampleRate'])
 
-    def __get_id_list_of_devices(self, device_type: str) -> List[int]:
-        id_list = []
-
-        is_windows = platform.system() == 'Windows'
-        result_from_powershell = None
-
-        if is_windows:
-            result_from_powershell = self.__get_data_from_powershell()
+    @staticmethod
+    def __print_list_of_audio_devices(audio_device_type: str, device_list: List[Device]):
+        logging.info(
+            f"Select id of {audio_device_type} audio devices:{os.linesep}"
+            f"{os.linesep.join(device.audio_devices_str for device in device_list)}")
+
+    def __get_id_list_of_devices(self, device_type: str) -> List[Device]:
+        device_list = []
+        device_count = self.py_audio.get_device_count()
 
-        audio_devices_str = ""
+        if device_count == 0:
+            raise Exception(f"No connected audio devices found!")
 
-        for i in range(self.py_audio.get_device_count()):
+        for i in range(device_count):
             dev = self.py_audio.get_device_info_by_index(i)
 
             device_name = self.__decode_string(dev['name'])
 
-            if self.__is_needed_audio_device(dev, device_name, device_type, is_windows, result_from_powershell):
-                id_list.append(i)
-                audio_devices_str += (
+            if dev[f'max{device_type}Channels'] > 0:
+                audio_devices_str = (
                     f"{i}: {device_name}, "
                     f"Channels: {dev[f'max{device_type}Channels']}, "
-                    f"Sample rate: {int(dev['defaultSampleRate'])}Hz{os.linesep}"
+                    f"Sample rate: {int(dev['defaultSampleRate'])}Hz"
                 )
+                device_list.append(Device(i, dev, device_name, audio_devices_str))
 
-        logging.info(os.linesep + audio_devices_str)
-
-        return id_list
+        if platform.system() == 'Windows':
+            device_list = self.__get_data_from_powershell(device_list)
 
-    @staticmethod
-    def __is_needed_audio_device(dev, device_name: str, device_type: str, is_windows: bool,
-                                 result_from_powershell):
-        if is_windows:
-            return dev[f'max{device_type}Channels'] > 0 and device_name in result_from_powershell
-        else:
-            return dev[f'max{device_type}Channels'] > 0
+        return device_list
 
-    def __get_data_from_powershell(self) -> List[str]:
+    def __get_data_from_powershell(self, device_list: List[Device]) -> List[Device]:
         command = """
             $OutputEncoding = [Console]::OutputEncoding = [System.Text.Encoding]::UTF8;
             Get-PnpDevice | 
             Where-Object { $_.Class -eq 'AudioEndpoint' -and $_.Status -eq 'OK' } | 
             Select-Object Name | 
             Out-String
             """
 
-        result = subprocess.run(["powershell", "-Command", command], capture_output=True, text=True, encoding='utf-8')
+        try:
+            result = subprocess.run(["powershell", "-Command", command], capture_output=True, text=True,
+                                    encoding='utf-8')
+            ps_device_names = self.__parse_powershell_stdout(result.stdout)
+        except Exception as e:
+            logging.warning(f"Failed to get device names from PowerShell: {e}")
 
-        device_names = self.__parse_powershell_stdout(result.stdout)
+            return device_list
 
-        return device_names
+        py_audio_device_names = [device.device_name for device in device_list]
+        is_ps_device_names_exists = any(ps_device_name in py_audio_device_names for ps_device_name in ps_device_names)
+
+        if not is_ps_device_names_exists:
+            logging.warning("Failed to size list of Windows audio devices!")
+
+            return device_list
+        else:
+            sized_device_list = device_list.copy()
+            for id_device in device_list:
+                if id_device.device_name not in ps_device_names:
+                    sized_device_list.remove(id_device)
+
+            return sized_device_list
 
     @staticmethod
     def __parse_powershell_stdout(stdout: str) -> List[str]:
         lines = stdout.split('\n')
         device_names = []
         collect_names = False
 
         for line in lines:
             if '----' in line:
                 collect_names = True
                 continue
+
             if collect_names and line.strip():
                 device_names.append(line.strip())
 
         return device_names
 
-    @staticmethod
-    def __decode_string(string: str) -> str:
+    def __decode_string(self, string: str) -> str:
+        if self.ignore_device_encoding_names:
+            return string
+
         try:
-            device_name = string.encode(locale.getpreferredencoding()).decode('utf-8')
-        except UnicodeEncodeError:
-            device_name = string
+            return string.encode(self.device_encoding_names).decode('utf-8')
+        except (UnicodeEncodeError, UnicodeDecodeError):
+            try:
+                return string.encode(self.device_encoding_names).decode(
+                    chardet.detect(string.encode(self.device_encoding_names))['encoding']
+                )
+            except (UnicodeEncodeError, UnicodeDecodeError):
+                pass
 
-        return device_name
+        return string
```

## echowarp/models/default_values_and_options.py

```diff
@@ -1,59 +1,111 @@
+import locale
+
 from echowarp.models.options_data_creater import OptionsData
 import version
 
 
 class DefaultValuesAndOptions:
     """
     Provides default configuration values and options for various settings within the EchoWarp project.
     This class facilitates the retrieval of default values and options for user interface and setup configurations.
 
     Attributes:
         __DEFAULT_PORT (int): Default port number used for UDP and TCP communication.
         __DEFAULT_WORKERS_COUNT (int): Default number of worker threads or processes.
-        __DEFAULT_HEARTBEAT_ATTEMPT (int): Default number of heartbeat attempts before considering the connection lost.
+        __DEFAULT_RECONNECT_ATTEMPT (int): Default number of heartbeat attempts before considering the connection lost.
         __DEFAULT_SERVER_MODE (list): Default server mode option and its boolean value.
         __SERVER_MODE_OPTIONS (list of lists): Available server mode options.
         __DEFAULT_AUDIO_DEVICE_TYPE (list): Default audio device type option and its boolean value.
         __AUDIO_DEVICE_OPTIONS (list of lists): Available audio device options.
         __DEFAULT_SSL (list): Default SSL option and its boolean value.
         __SSL_OPTIONS (list of lists): Available SSL options.
         __DEFAULT_HASH_CONTROL (list): Default hash control option and its boolean value.
         __HASH_CONTROL_OPTIONS (list of lists): Available integrity control options.
     """
     __DEFAULT_PORT = 4415
     __DEFAULT_WORKERS_COUNT = 1
-    __DEFAULT_HEARTBEAT_ATTEMPT = 5
+    __DEFAULT_RECONNECT_ATTEMPT = 5
+    __DEFAULT_BUFFER_SIZE = 6144
+    __DEFAULT_TIMEOUT = 5
+    __DEFAULT_HEARTBEAT_DELAY = 2
 
-    SOCKET_BUFFER_SIZE = 6144
+    CONFIG_TITLE = 'echowarp_conf'
+    BAN_LIST_FILE = 'echowarp_ban_list.txt'
 
     __DEFAULT_SERVER_MODE = ['Server mode', True]
     __SERVER_MODE_OPTIONS = [
         __DEFAULT_SERVER_MODE,
         ['Client mode', False]
     ]
 
+    __DEFAULT_SOCKET_BUFFER_SIZE = [f'{__DEFAULT_BUFFER_SIZE}', __DEFAULT_BUFFER_SIZE]
+    __SOCKET_BUFFER_SIZE_OPTIONS = [
+        __DEFAULT_SOCKET_BUFFER_SIZE,
+        ['Custom size', False]
+    ]
+
     __DEFAULT_AUDIO_DEVICE_TYPE = ['Input audio device', True]
     __AUDIO_DEVICE_OPTIONS = [
         __DEFAULT_AUDIO_DEVICE_TYPE,
         ['Output audio device', False]
     ]
 
+    __DEFAULT_DEVICE_ENCODING_NAMES = [f'Locale of OS - {locale.getpreferredencoding()}', locale.getpreferredencoding()]
+    __DEVICE_ENCODING_NAMES_OPTIONS = [
+        __DEFAULT_DEVICE_ENCODING_NAMES,
+        ['Use custom encoding', True]
+    ]
+
+    __DEFAULT_IGNORE_DEVICE_ENCODING_NAMES = ['Enable encoding', False]
+    __IGNORE_DEVICE_ENCODING_NAMES_OPTIONS = [
+        __DEFAULT_IGNORE_DEVICE_ENCODING_NAMES,
+        ['Disable encoding', True]
+    ]
+
+    __DEFAULT_IS_ERROR_LOG = ['Disable error file log', False]
+    __IS_ERROR_LOG_OPTIONS = [
+        __DEFAULT_IS_ERROR_LOG,
+        ['Enable error file log', True]]
+
     __DEFAULT_SSL = ['Disable SSL', False]
     __SSL_OPTIONS = [
         ['Enable SSL', True],
         __DEFAULT_SSL
     ]
 
     __DEFAULT_HASH_CONTROL = ['Disable integrity control', False]
     __HASH_CONTROL_OPTIONS = [
         ['Enable integrity control', True],
         __DEFAULT_HASH_CONTROL
     ]
 
+    __DEFAULT_SAVE_PROFILE = ['Skip saving params', False]
+    __SAVE_PROFILE_OPTIONS = [
+        ['Save values to config file', True],
+        __DEFAULT_SAVE_PROFILE
+    ]
+
+    @staticmethod
+    def get_variants_config_load_options_data() -> OptionsData:
+        return OptionsData(
+            ["Load config", True],
+            [
+                ["Load config", True],
+                ["Skip config", False]
+            ]
+        )
+
+    @staticmethod
+    def get_socket_buffer_size_options_data() -> OptionsData:
+        return OptionsData(
+            DefaultValuesAndOptions.__DEFAULT_SOCKET_BUFFER_SIZE,
+            DefaultValuesAndOptions.__SOCKET_BUFFER_SIZE_OPTIONS
+        )
+
     @staticmethod
     def get_util_mods_options_data() -> OptionsData:
         return OptionsData(
             DefaultValuesAndOptions.__DEFAULT_SERVER_MODE,
             DefaultValuesAndOptions.__SERVER_MODE_OPTIONS
         )
 
@@ -61,35 +113,71 @@
     def get_audio_device_type_options_data() -> OptionsData:
         return OptionsData(
             DefaultValuesAndOptions.__DEFAULT_AUDIO_DEVICE_TYPE,
             DefaultValuesAndOptions.__AUDIO_DEVICE_OPTIONS
         )
 
     @staticmethod
+    def get_encoding_charset_options_data() -> OptionsData:
+        return OptionsData(
+            DefaultValuesAndOptions.__DEFAULT_DEVICE_ENCODING_NAMES,
+            DefaultValuesAndOptions.__DEVICE_ENCODING_NAMES_OPTIONS
+        )
+
+    @staticmethod
+    def get_ignore_encoding_options_data() -> OptionsData:
+        return OptionsData(
+            DefaultValuesAndOptions.__DEFAULT_IGNORE_DEVICE_ENCODING_NAMES,
+            DefaultValuesAndOptions.__IGNORE_DEVICE_ENCODING_NAMES_OPTIONS
+        )
+
+    @staticmethod
+    def get_error_log_options_data() -> OptionsData:
+        return OptionsData(
+            DefaultValuesAndOptions.__DEFAULT_IS_ERROR_LOG,
+            DefaultValuesAndOptions.__IS_ERROR_LOG_OPTIONS
+        )
+
+    @staticmethod
     def get_ssl_options_data() -> OptionsData:
         return OptionsData(
             DefaultValuesAndOptions.__DEFAULT_SSL,
             DefaultValuesAndOptions.__SSL_OPTIONS
         )
 
     @staticmethod
     def get_hash_control_options_data() -> OptionsData:
         return OptionsData(
             DefaultValuesAndOptions.__DEFAULT_HASH_CONTROL,
             DefaultValuesAndOptions.__HASH_CONTROL_OPTIONS
         )
 
     @staticmethod
+    def get_save_profile_options_data() -> OptionsData:
+        return OptionsData(
+            DefaultValuesAndOptions.__DEFAULT_SAVE_PROFILE,
+            DefaultValuesAndOptions.__SAVE_PROFILE_OPTIONS
+        )
+
+    @staticmethod
     def get_default_port() -> int:
         return DefaultValuesAndOptions.__DEFAULT_PORT
 
     @staticmethod
-    def get_default_heartbeat_attempt() -> int:
-        return DefaultValuesAndOptions.__DEFAULT_HEARTBEAT_ATTEMPT
+    def get_default_reconnect_attempt() -> int:
+        return DefaultValuesAndOptions.__DEFAULT_RECONNECT_ATTEMPT
 
     @staticmethod
     def get_default_workers() -> int:
         return DefaultValuesAndOptions.__DEFAULT_WORKERS_COUNT
 
     @staticmethod
-    def get_util_version() -> str:
-        return version.__version__
+    def get_util_comparability_version() -> str:
+        return version.__comparability_version__
+
+    @staticmethod
+    def get_heartbeat_delay() -> float:
+        return DefaultValuesAndOptions.__DEFAULT_HEARTBEAT_DELAY
+
+    @staticmethod
+    def get_timeout() -> int:
+        return DefaultValuesAndOptions.__DEFAULT_TIMEOUT
```

## echowarp/models/json_message.py

```diff
@@ -1,37 +1,52 @@
-import base64
 import json
 import logging
+from dataclasses import dataclass
+from typing import Optional
 
 from echowarp.models.default_values_and_options import DefaultValuesAndOptions
 
 
+@dataclass
+class ResponseMessage:
+    response_code: int
+    response_message: str
+
+
 class JSONMessage:
     """
-    Encapsulates the structure of JSON messages used for communication between the client and server in the EchoWarp application.
+    Encapsulates the structure of JSON messages used for communication between the client and server
+    in the EchoWarp application.
     Provides methods for encoding and decoding these messages.
 
     Attributes:
         message (str): The main content of the message.
         response_code (int): An HTTP-like response code indicating the status of the message.
         version (float): The version of the utility compatible with this message format.
     """
     _json_message: dict
 
     message: str
     response_code: int
     version: str
+    failed_connections: int
+    reconnect_attempts: Optional[int]
 
-    AUTH_CLIENT_MESSAGE = "EchoWarpClient"
-    AUTH_SERVER_MESSAGE = "EchoWarpServer"
-    HEARTBEAT_MESSAGE = "heartbeat"
+    OK_MESSAGE = ResponseMessage(200, "OK")
+    ACCEPTED_MESSAGE = ResponseMessage(202, "Accepted")
+    UNAUTHORIZED_MESSAGE = ResponseMessage(401, "Unauthorized")
+    FORBIDDEN_MESSAGE = ResponseMessage(403, "Forbidden")
+    CONFLICT_MESSAGE = ResponseMessage(409, "Conflict")
+    LOCKED_MESSAGE = ResponseMessage(423, "Locked")
 
     _MESSAGE_KEY = "message"
     _RESPONSE_CODE = "response_code"
-    _VERSION_KEY = "version"
+    _COMPARABILITY_VERSION_KEY = "comparability_version"
+    _FAILED_CONNECTIONS_KEY = "failed_connections"
+    _RECONNECT_ATTEMPTS_KEY = "reconnect_attempts"
 
     def __init__(self, json_bytes: bytes):
         """
                 Initializes a new instance of JSONMessage from a byte array containing a JSON string.
 
                 Args:
                     json_bytes (bytes): A byte array containing the JSON-encoded string.
@@ -40,58 +55,67 @@
                     Exception: If there is an error decoding the JSON data.
         """
         try:
             self._json_message = json.loads(json_bytes.decode('utf-8'))
 
             self.message = self._json_message[self._MESSAGE_KEY]
             self.response_code = self._json_message[self._RESPONSE_CODE]
-            self.version = self._json_message[self._VERSION_KEY]
+            self.version = self._json_message[self._COMPARABILITY_VERSION_KEY]
+            self.failed_connections = self._json_message[self._FAILED_CONNECTIONS_KEY]
+            self.reconnect_attempts = self._json_message[self._RECONNECT_ATTEMPTS_KEY]
         except Exception as e:
             logging.error(f"Decode json message error: {e}")
             raise
 
     @staticmethod
-    def encode_message_to_json_bytes(message: str, response_code: int) -> bytes:
+    def encode_message_to_json_bytes(message: str, response_code: int,
+                                     failed_connections: Optional[int], reconnect_attempts: Optional[int]) -> bytes:
         """
                 Encodes a message with its response code and version into a byte array containing JSON data.
 
                 Args:
                     message (str): The main content of the message.
                     response_code (int): The HTTP-like response code.
+                    failed_connections (int): Failed connections.
+                    reconnect_attempts (int): Reconnect attempts.
 
                 Returns:
                     bytes: A byte array containing the JSON-encoded message.
         """
+        if reconnect_attempts is not None and reconnect_attempts <= 0:
+            reconnect_attempts = None
+
         message = {
             JSONMessage._MESSAGE_KEY: message,
             JSONMessage._RESPONSE_CODE: response_code,
-            JSONMessage._VERSION_KEY: DefaultValuesAndOptions.get_util_version(),
+            JSONMessage._COMPARABILITY_VERSION_KEY: DefaultValuesAndOptions.get_util_comparability_version(),
+            JSONMessageServer._FAILED_CONNECTIONS_KEY: failed_connections,
+            JSONMessageServer._RECONNECT_ATTEMPTS_KEY: reconnect_attempts,
         }
 
         return json.dumps(message).encode('utf-8')
 
 
 class JSONMessageServer(JSONMessage):
     """
     Extends JSONMessage to include server-specific configuration settings such as heartbeat attempts,
     encryption status, and integrity control settings.
 
     Attributes:
-        heartbeat_attempt (int): The number of allowed missed heartbeats before the server considers the connection lost.
         is_encrypt (bool): Indicates if encryption is enabled for the communication.
         is_integrity_control (bool): Indicates if data integrity checks are enabled.
-        aes_key (bytes): AES key used for encryption, provided as a base64-encoded string.
-        aes_iv (bytes): AES initialization vector used for encryption, provided as a base64-encoded string.
+        aes_key_base64 (bytes): AES key used for encryption, provided as a base64-encoded string.
+        aes_iv_base64 (bytes): AES initialization vector used for encryption, provided as a base64-encoded string.
     """
-    heartbeat_attempt: int
     is_encrypt: bool
     is_integrity_control: bool
+    aes_key_base64: str
+    aes_iv_base64: str
 
     _CONFIGS_KEY = "config"
-    _HEARTBEAT_ATTEMPT_KEY = "heartbeat_attempt"
     _IS_ENCRYPT_KEY = "is_encrypt"
     _IS_INTEGRITY_CONTROL_KEY = "is_integrity_control"
     _AES_KEY = "aes_key"
     _AES_IV_KEY = "aes_iv"
 
     def __init__(self, json_bytes: bytes):
         """
@@ -104,56 +128,53 @@
             ValueError: If the configuration keys are missing in the JSON data.
             Exception: If there is an error decoding the JSON data.
         """
         super().__init__(json_bytes)
 
         if self._CONFIGS_KEY in self._json_message:
             try:
-                self.heartbeat_attempt = self._json_message[self._CONFIGS_KEY][self._HEARTBEAT_ATTEMPT_KEY]
                 self.is_encrypt = self._json_message[self._CONFIGS_KEY][self._IS_ENCRYPT_KEY]
                 self.is_integrity_control = self._json_message[self._CONFIGS_KEY][self._IS_INTEGRITY_CONTROL_KEY]
-                aes_key = self._json_message[self._CONFIGS_KEY][self._AES_KEY]
-                aes_iv = self._json_message[self._CONFIGS_KEY][self._AES_IV_KEY]
-
-                self.aes_key = base64.b64decode(aes_key)
-                self.aes_iv = base64.b64decode(aes_iv)
+                self.aes_key_base64 = self._json_message[self._CONFIGS_KEY][self._AES_KEY]
+                self.aes_iv_base64 = self._json_message[self._CONFIGS_KEY][self._AES_IV_KEY]
             except Exception as e:
-                logging.error(f"Decode json message error: {e}")
-                raise
+                raise Exception(f"Decode json message error: {e}")
         else:
-            logging.error(self._CONFIGS_KEY + " not in json config message")
-            raise ValueError
+            raise ValueError(self._CONFIGS_KEY + " not in json config message")
 
     @staticmethod
-    def encode_server_config_to_json_bytes(heartbeat_attempt: int, is_encrypt: bool, is_hash_control: bool,
-                                           aes_key: bytes, aes_iv: bytes) -> bytes:
+    def encode_server_config_to_json_bytes(is_encrypt: bool, is_hash_control: bool,
+                                           aes_key_base64: str, aes_iv_base64: str,
+                                           failed_connections: int, reconnect_attempts: int) -> bytes:
         """
         Encodes server configuration into a byte array containing JSON data.
 
         Args:
-            heartbeat_attempt (int): Number of heartbeat attempts before disconnect.
             is_encrypt (bool): Enable or disable encryption.
             is_hash_control (bool): Enable or disable integrity control.
-            aes_key (bytes): AES key for encryption.
-            aes_iv (bytes): AES initialization vector.
+            aes_key_base64 (str): AES key in Base64 for encryption.
+            aes_iv_base64 (str): AES initialization vector in Base64.
+            failed_connections (int): Failed connections if client.
+            reconnect_attempts (int): Max reconnect attempts on server.
 
         Returns:
             bytes: A byte array containing the JSON-encoded server configuration.
         """
-        encoded_aes_key = base64.b64encode(aes_key).decode('utf-8')
-        encoded_aes_iv = base64.b64encode(aes_iv).decode('utf-8')
+        if reconnect_attempts <= 0:
+            reconnect_attempts = None
 
         config = {
-            JSONMessageServer._MESSAGE_KEY: JSONMessageServer.AUTH_SERVER_MESSAGE,
-            JSONMessageServer._RESPONSE_CODE: 200,
-            JSONMessageServer._VERSION_KEY: DefaultValuesAndOptions.get_util_version(),
+            JSONMessageServer._MESSAGE_KEY: JSONMessageServer.OK_MESSAGE.response_message,
+            JSONMessageServer._RESPONSE_CODE: JSONMessageServer.OK_MESSAGE.response_code,
+            JSONMessageServer._COMPARABILITY_VERSION_KEY: DefaultValuesAndOptions.get_util_comparability_version(),
+            JSONMessageServer._FAILED_CONNECTIONS_KEY: failed_connections,
+            JSONMessageServer._RECONNECT_ATTEMPTS_KEY: reconnect_attempts,
 
             JSONMessageServer._CONFIGS_KEY: {
-                JSONMessageServer._HEARTBEAT_ATTEMPT_KEY: heartbeat_attempt,
                 JSONMessageServer._IS_ENCRYPT_KEY: is_encrypt,
                 JSONMessageServer._IS_INTEGRITY_CONTROL_KEY: is_hash_control,
-                JSONMessageServer._AES_KEY: encoded_aes_key,
-                JSONMessageServer._AES_IV_KEY: encoded_aes_iv,
+                JSONMessageServer._AES_KEY: aes_key_base64,
+                JSONMessageServer._AES_IV_KEY: aes_iv_base64,
             }
         }
 
         return json.dumps(config).encode('utf-8')
```

## echowarp/services/crypto_manager.py

```diff
@@ -1,7 +1,8 @@
+import base64
 import logging
 import os
 import hashlib
 from typing import Tuple, Optional
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.asymmetric import rsa, padding
@@ -12,54 +13,54 @@
 
 class CryptoManager:
     """
     Manages cryptographic operations such as RSA and AES encryption/decryption for secure communication in EchoWarp.
 
     Attributes:
         __is_server (bool): True if this instance is configured for server-side operations.
-        is_encrypt (bool): Determines if encryption is enabled.
-        is_hash_control (bool): Determines if integrity control via hashing is enabled.
+        is_ssl (bool): Determines if encryption is enabled.
+        is_integrity_control (bool): Determines if integrity control via hashing is enabled.
         __private_key (rsa.RSAPrivateKey): The RSA private key for decryption.
         __public_key (rsa.RSAPublicKey): The RSA public key for encryption.
         __aes_key (Optional[bytes]): The AES key for symmetric encryption, used if encryption is enabled.
         __aes_iv (Optional[bytes]): The AES IV for symmetric encryption.
         __peer_public_key (Optional[rsa.RSAPublicKey]): The public key of the communication peer,
         for encrypted communications.
     """
     __is_server: bool
-    is_encrypt: Optional[bool]
-    is_hash_control: Optional[bool]
+    is_ssl: Optional[bool]
+    is_integrity_control: Optional[bool]
     __private_key: rsa.RSAPrivateKey
     __public_key: rsa.RSAPublicKey
     __aes_key: Optional[bytes]
     __aes_iv: Optional[bytes]
     __peer_public_key: rsa.RSAPublicKey
 
-    def __init__(self, is_server: bool, is_hash_control: bool, is_encrypt: bool):
+    def __init__(self, is_server: bool, is_integrity_control: bool, is_ssl: bool):
         """
                 Initializes a new CryptoManager instance with the specified settings.
 
                 Args:
                     is_server (bool): Indicates if this instance is used by a server.
-                    is_hash_control (bool): Enable or disable integrity control via hashing.
-                    is_encrypt (bool): Enable or disable encryption.
+                    is_integrity_control (bool): Enable or disable integrity control via hashing.
+                    is_ssl (bool): Enable or disable encryption.
         """
         self.__is_server = is_server
-        self.is_encrypt = is_encrypt
-        self.is_hash_control = is_hash_control
+        self.is_ssl = is_ssl
+        self.is_integrity_control = is_integrity_control
 
         self.__private_key, self.__public_key = self.__generate_and_get_rsa_keys()
         self.__aes_key, self.__aes_iv = self.__generate_and_get_aes_key_and_iv() if is_server else (None, None)
 
     def load_encryption_config_for_client(self, is_encrypt: bool, is_hash_control: bool):
         if self.__is_server:
             raise ValueError("Load encryption config applied only for client")
 
-        self.is_encrypt = is_encrypt
-        self.is_hash_control = is_hash_control
+        self.is_ssl = is_encrypt
+        self.is_integrity_control = is_hash_control
 
     def encrypt_aes_and_sign_data(self, data: bytes) -> bytes:
         """
         Encrypts and optionally signs data with a hash for integrity.
 
         Args:
             data (bytes): Data to encrypt and sign.
@@ -70,18 +71,18 @@
         Raises:
             ValueError: If data is None.
             Exception: General exceptions during encryption, logged as an error.
         """
         if data is None:
             raise ValueError("Data to encrypt and sign cannot be None")
 
-        if self.is_hash_control:
+        if self.is_integrity_control:
             data = self.__calculate_hash_to_data(data)
 
-        if self.is_encrypt:
+        if self.is_ssl:
             try:
                 data = self.__encrypt_data_aes(data)
             except Exception as e:
                 logging.error(f"Failed to encrypt data: {e}")
                 raise
 
         return data
@@ -99,22 +100,22 @@
         Raises:
             ValueError: If data is None.
             Exception: General exceptions during decryption, logged as an error.
         """
         if data is None:
             raise ValueError("Data to decrypt and verify cannot be None")
 
-        if self.is_encrypt:
+        if self.is_ssl:
             try:
                 data = self.__decrypt_data_aes(data)
             except Exception as e:
                 logging.error(f"Failed to decrypt data: {e}")
                 raise
 
-        if self.is_hash_control:
+        if self.is_integrity_control:
             data = self.__compare_hash_and_get_data(data)
 
         return data
 
     @staticmethod
     def __generate_and_get_rsa_keys() -> Tuple[rsa.RSAPrivateKey, rsa.RSAPublicKey]:
         """
@@ -195,69 +196,67 @@
         Generates a new AES key and IV for symmetric encryption.
         """
         aes_key = os.urandom(32)
         aes_iv = os.urandom(16)
 
         return aes_key, aes_iv
 
-    def get_aes_key(self) -> bytes:
+    def get_aes_key_base64(self) -> str:
         """
-        Returns the AES key in bytes.
+        Returns the AES key in Base64.
         """
 
-        return self.__aes_key
+        return base64.b64encode(self.__aes_key).decode('utf-8')
 
-    def get_aes_iv(self) -> bytes:
+    def get_aes_iv_base64(self) -> str:
         """
-        Returns the AES IV in bytes.
+        Returns the AES IV in Base64.
         """
 
-        return self.__aes_iv
+        return base64.b64encode(self.__aes_iv).decode('utf-8')
 
-    def load_aes_key_and_iv(self, aes_key, aes_iv):
+    def load_aes_key_and_iv(self, aes_key_base64: str, aes_iv_base64: str):
         """
         Loads the AES key and IV from peer.
         """
         if self.__is_server:
             logging.error("Only client can load AES key and IV")
             raise ValueError
 
-        self.__aes_key = aes_key
-        self.__aes_iv = aes_iv
+        self.__aes_key = base64.b64decode(aes_key_base64)
+        self.__aes_iv = base64.b64decode(aes_iv_base64)
 
     def __encrypt_data_aes(self, data):
         """
         Encrypts data using AES.
 
         Args:
             data: The plaintext data to encrypt.
 
         Returns:
             The encrypted data.
         """
         padder = sym_padding.PKCS7(128).padder()
         padded_data = padder.update(data) + padder.finalize()
 
-        cipher = Cipher(algorithms.AES(self.__aes_key), modes.CBC(self.__aes_iv))
-        encryptor = cipher.encryptor()
+        encryptor = Cipher(algorithms.AES(self.__aes_key), modes.CBC(self.__aes_iv)).encryptor()
 
         return encryptor.update(padded_data) + encryptor.finalize()
 
     def __decrypt_data_aes(self, encrypted_data):
         """
         Decrypts data using AES.
 
         Args:
             encrypted_data: The encrypted data to decrypt.
 
         Returns:
             The decrypted plaintext data.
         """
-        cipher = Cipher(algorithms.AES(self.__aes_key), modes.CBC(self.__aes_iv))
-        decryptor = cipher.decryptor()
+        decryptor = Cipher(algorithms.AES(self.__aes_key), modes.CBC(self.__aes_iv)).decryptor()
         padded_data = decryptor.update(encrypted_data) + decryptor.finalize()
 
         unpadder = sym_padding.PKCS7(128).unpadder()
 
         return unpadder.update(padded_data) + unpadder.finalize()
 
     @staticmethod
```

## echowarp/start_modes/args_mode.py

```diff
@@ -1,73 +1,149 @@
 import argparse
+import os
 
+from echowarp.logging_config import Logger
 from echowarp.models.audio_device import AudioDevice
 from echowarp.models.default_values_and_options import DefaultValuesAndOptions
 from echowarp.settings import Settings
+from echowarp.start_modes.config_parser import ConfigParser
 
 
-def get_settings_by_args() -> Settings:
-    """
-        Parses command line arguments to configure the EchoWarp utility settings. This function
-        constructs the settings based on the provided command line arguments, handling different modes
-        and configurations such as server/client mode, audio device selection, and network settings.
-
-        Returns:
-            Settings: An instance of the Settings class populated with values derived from parsed command line arguments.
-
-        Raises:
-            argparse.ArgumentError: If there are issues with the provided arguments, such as missing required arguments
-                                    or invalid values.
-    """
-    parser = argparse.ArgumentParser(description="EchoWarp Audio Streamer")
-
-    parser.add_argument("-c", "--client", action='store_false',
-                        help=f"Start util in client mode. "
-                             f"(default={DefaultValuesAndOptions.get_util_mods_options_data().default_descr})")
-    parser.add_argument("-o", "--output", action='store_false',
-                        help=f"Use output audio device. "
-                             f"(default={DefaultValuesAndOptions.get_audio_device_type_options_data().default_descr})")
-    parser.add_argument("-p", "--udp_port", type=int, default=DefaultValuesAndOptions.get_default_port(),
-                        help="UDP port for audio streaming.")
-    parser.add_argument("-d", "--device_id", type=int,
-                        help="Specify the device ID to bypass interactive selection.")
-
-    client_args = parser.add_argument_group('Client Only Options')
-    client_args.add_argument("-a", "--server_addr", type=str, help="Server address.")
-
-    server_args = parser.add_argument_group('Server Only Options')
-    server_args.add_argument("-b", "--heartbeat", type=int,
-                             default=DefaultValuesAndOptions.get_default_heartbeat_attempt(),
-                             help="Number of heartbeat attempts before disconnect (server mode only).")
-    server_args.add_argument("--ssl", action='store_true',
-                             help=f"Init SSL mode (server mode only). "
-                                  f"(default={DefaultValuesAndOptions.get_ssl_options_data().default_descr})")
-    server_args.add_argument("-i", "--integrity_control", action='store_true',
-                             help=f"Init integrity control by hash (server mode only). "
-                                  f"(default={DefaultValuesAndOptions.get_hash_control_options_data().default_descr})")
-    server_args.add_argument("-w", "--workers", type=int,
-                             help="Max workers in multithreading (server mode only).",
-                             default=DefaultValuesAndOptions.get_default_workers())
-
-    args = parser.parse_args()
-
-    if not args.client:
-        if any([args.ssl, args.integrity_control]) and args.workers != 1:
-            parser.error("Options --ssl, --integrity_control and --workers are only available in server mode.")
-        if not args.server_addr:
-            parser.error("The --server_addr argument is required in client mode.")
-    else:
-        if args.server_addr:
-            parser.error("The --server_addr argument is only valid in client mode.")
-
-    audio_device = AudioDevice(args.output, args.device_id)
-
-    return Settings(
-        args.client,
-        args.udp_port,
-        args.server_addr,
-        args.heartbeat,
-        args.ssl,
-        args.integrity_control,
-        args.workers,
-        audio_device
-    )
+class ArgsParser:
+    @staticmethod
+    def get_settings_from_cli_args() -> Settings:
+        """
+            Parses command line arguments to configure the EchoWarp utility settings. This function
+            constructs the settings based on the provided command line arguments, handling different modes
+            and configurations such as server/client mode, audio device selection, and network settings.
+
+            Returns:
+                Settings: An instance of the Settings class populated with values derived from parsed command line arguments.
+
+            Raises:
+                argparse.ArgumentError: If there are issues with the provided arguments, such as missing required arguments
+                                        or invalid values.
+        """
+        parser = argparse.ArgumentParser(description="EchoWarp Audio Streamer")
+
+        parser.add_argument("-c", "--client", action='store_false',
+                            help=f"Start util in client mode. "
+                                 f"(default={DefaultValuesAndOptions.get_util_mods_options_data().default_descr})")
+        parser.add_argument(
+            "-o", "--output", action='store_false',
+            help=f"Use output audio device.{os.linesep}"
+                 f"(default={DefaultValuesAndOptions.get_audio_device_type_options_data().default_descr})"
+        )
+        parser.add_argument("-u", "--udp_port", type=int, default=DefaultValuesAndOptions.get_default_port(),
+                            help=f"UDP port for audio streaming. "
+                                 f"(default={DefaultValuesAndOptions.get_default_port()})")
+        parser.add_argument(
+            "-b", "--socket_buffer_size", type=int,
+            default=DefaultValuesAndOptions.get_socket_buffer_size_options_data().default_value,
+            help=f"Size of socket buffer. "
+                 f"(default={DefaultValuesAndOptions.get_socket_buffer_size_options_data().default_value})"
+        )
+        parser.add_argument("-d", "--device_id", type=int,
+                            help="Specify the device ID to bypass interactive selection.")
+        parser.add_argument("-p", "--password", type=str, help="Password, if needed.")
+        parser.add_argument("-f", "--config_file", type=str, help="Path to config file "
+                                                                  "(Ignoring other args, if they added).")
+        parser.add_argument("-e", "--device_encoding_names", type=str,
+                            help=f"Charset encoding for audio device. "
+                                 f"(default=preferred system encoding - "
+                                 f"{DefaultValuesAndOptions.get_encoding_charset_options_data().default_value})",
+                            default=DefaultValuesAndOptions.get_encoding_charset_options_data().default_value)
+        parser.add_argument("--ignore_device_encoding_names", action='store_true',
+                            help="Ignoring device names encoding.")
+
+        parser.add_argument("-l", "--is_error_log", action='store_true', help="Init error file logger.")
+        parser.add_argument("-r", "--reconnect", type=int,
+                            default=DefaultValuesAndOptions.get_default_reconnect_attempt(),
+                            help=f"The number of failed connections in client mode before closing the application. "
+                                 f"The number of failed client authorization attempts in server mode "
+                                 f"before banning the client. (0 = infinite). "
+                                 f"(default={DefaultValuesAndOptions.get_default_reconnect_attempt()})")
+
+        parser.add_argument("-s", "--save_config", type=str, help="Save config file from selected args "
+                                                                  "(Ignored default values)")
+
+        client_args = parser.add_argument_group('Client Only Options')
+        client_args.add_argument("-a", "--server_address", type=str, help="Server address.")
+
+        server_args = parser.add_argument_group('Server Only Options')
+        server_args.add_argument("--ssl", action='store_true',
+                                 help=f"Init SSL mode (server mode only). "
+                                      f"(default={DefaultValuesAndOptions.get_ssl_options_data().default_descr})")
+        server_args.add_argument(
+            "-i", "--integrity_control", action='store_true',
+            help=f"Init integrity control by hash (server mode only). "
+                 f"(default={DefaultValuesAndOptions.get_hash_control_options_data().default_descr})"
+        )
+        server_args.add_argument("-w", "--workers", type=int,
+                                 help="Max workers in multithreading (server mode only).",
+                                 default=DefaultValuesAndOptions.get_default_workers())
+
+        args = parser.parse_args()
+
+        if args.is_error_log:
+            Logger.init_warning_logger()
+
+        if args.config_file is not None:
+            return ArgsParser.__load_from_config(args.config_file)
+
+        if not args.client:
+            if any([args.ssl, args.integrity_control]) and args.workers != 1:
+                parser.error("Options --ssl, --integrity_control and --workers are only available in server mode.")
+            if not args.server_address:
+                parser.error("The --server_address argument is required in client mode.")
+        else:
+            if args.server_address:
+                parser.error("The --server_address argument is only valid in client mode.")
+
+        if args.ignore_device_encoding_names:
+            args.device_encoding_names = DefaultValuesAndOptions.get_encoding_charset_options_data().default_value
+
+        audio_device = AudioDevice(args.output,
+                                   args.device_id,
+                                   args.ignore_device_encoding_names,
+                                   args.device_encoding_names)
+
+        settings = Settings(
+            args.client,
+            args.udp_port,
+            args.server_address,
+            args.reconnect,
+            args.ssl,
+            args.integrity_control,
+            args.workers,
+            audio_device,
+            args.password,
+            args.is_error_log,
+            args.socket_buffer_size
+        )
+
+        if args.save_config is not None:
+            ConfigParser(filename=args.save_config, settings=settings)
+
+        return settings
+
+    @staticmethod
+    def __load_from_config(filepath: str) -> Settings:
+        configs = ConfigParser(filename=filepath)
+        audio_device = AudioDevice(configs.is_input_audio_device,
+                                   configs.device_id,
+                                   configs.ignore_device_encoding_names,
+                                   configs.device_encoding_names)
+
+        return Settings(
+            configs.is_server,
+            configs.udp_port,
+            configs.server_address,
+            configs.reconnect_attempt,
+            configs.is_ssl,
+            configs.is_integrity_control,
+            configs.workers,
+            audio_device,
+            configs.password,
+            configs.is_error_log,
+            configs.socket_buffer_size
+        )
```

## echowarp/start_modes/interactive_mode.py

```diff
@@ -1,15 +1,18 @@
+import itertools
 import os
 
 import logging
 
+from echowarp.logging_config import Logger
 from echowarp.models.audio_device import AudioDevice
 from echowarp.models.default_values_and_options import DefaultValuesAndOptions
 from echowarp.settings import Settings
 from echowarp.models.options_data_creater import OptionsData
+from echowarp.start_modes.config_parser import ConfigParser
 
 
 class NumberValidator:
     """
         A custom validator for prompt_toolkit that ensures user input is a valid number within a specified range.
 
         Attributes:
@@ -45,67 +48,171 @@
     """
     Handles the interactive configuration of EchoWarp settings through command line prompts.
     Allows users to configure settings such as server/client mode, audio device selection, and network options
     by answering interactive questions.
     """
 
     @staticmethod
-    def get_settings_interactive() -> Settings:
+    def get_settings_in_interactive_mode() -> Settings:
         """
         Prompts the user interactively to configure the EchoWarp settings and returns the configured settings object.
 
         Returns:
             Settings: A fully configured Settings object based on user input.
         """
         server_address = None
-        heartbeat_attempt = None
         is_ssl = None
-        is_hash_control = None
-        workers_count = 1
+        is_integrity_control = None
+        workers = 1
+
+        conf_files = []
+        for filename in os.listdir():
+            if os.path.isfile(os.path.join(filename)) and filename.endswith('.conf'):
+                file_str = ConfigParser.get_file_str(filename)
+                if file_str.split('\n')[0] == f'[{DefaultValuesAndOptions.CONFIG_TITLE}]':
+                    conf_files.append(filename)
+
+        if len(conf_files) == 1:
+            is_load_config = InteractiveSettings.__select_in_interactive_from_values(
+                f'load config from "{conf_files[0]}" file',
+                DefaultValuesAndOptions.get_variants_config_load_options_data()
+            )
+
+            if is_load_config:
+                return InteractiveSettings.__get_settings_from_config(conf_files[0])
+        elif len(conf_files) > 1:
+            config_files_num_list = [[value, i] for i, value in zip(itertools.count(), conf_files)]
+            config_file_num = InteractiveSettings.__select_in_interactive_from_values(
+                'founded config files',
+                OptionsData(
+                    ["Skip configs", False],
+                    config_files_num_list
+                )
+            )
+
+            if type(config_file_num) is int:
+                selected_file_name = config_files_num_list[config_file_num][0]
+
+                # noinspection PyTypeChecker
+                return InteractiveSettings.__get_settings_from_config(selected_file_name)
+        else:
+            config_file_path = input("Input path to config file (empty field to skip): ")
+            if config_file_path.strip() != '':
+                return InteractiveSettings.__get_settings_from_config(config_file_path.strip())
+
+        is_error_log = InteractiveSettings.__select_in_interactive_from_values(
+            'error file logger switcher',
+            DefaultValuesAndOptions.get_error_log_options_data()
+        )
+
+        if is_error_log:
+            Logger.init_warning_logger()
 
         is_server_mode = InteractiveSettings.__select_in_interactive_from_values(
             'util mode',
             DefaultValuesAndOptions.get_util_mods_options_data()
         )
 
+        socket_buffer_size = InteractiveSettings.__select_in_interactive_from_values(
+            'size of socket buffer',
+            DefaultValuesAndOptions.get_socket_buffer_size_options_data()
+        )
+
+        if type(socket_buffer_size) is bool:
+            socket_buffer_size = InteractiveSettings.__get_not_null_int_input("custom buffer size in KB")
+
         is_input_device = InteractiveSettings.__select_in_interactive_from_values(
             'capture audio device type',
             DefaultValuesAndOptions.get_audio_device_type_options_data()
         )
 
         udp_port = InteractiveSettings.__input_in_interactive_int_value(
             DefaultValuesAndOptions.get_default_port(),
             'UDP port for audio streaming'
         )
 
+        password = input("Input password, if needed: ")
+        if password.strip() == '':
+            password = None
+
+        reconnect_attempt = InteractiveSettings.__input_in_interactive_int_value(
+            DefaultValuesAndOptions.get_default_reconnect_attempt(),
+            'count of reconnect attempt'
+        )
+
+        ignore_device_encoding_names = InteractiveSettings.__select_in_interactive_from_values(
+            'ignore audio device encoding names',
+            DefaultValuesAndOptions.get_ignore_encoding_options_data()
+        )
+
+        if ignore_device_encoding_names:
+            device_encoding_names = InteractiveSettings.__select_in_interactive_from_values(
+                'audio device charset encoding names',
+                DefaultValuesAndOptions.get_encoding_charset_options_data()
+            )
+
+            if type(device_encoding_names) is bool:
+                device_encoding_names = InteractiveSettings.__get_not_null_str_input('custom charset encoding')
+        else:
+            device_encoding_names = DefaultValuesAndOptions.get_encoding_charset_options_data().default_value
+
         if not is_server_mode:
             server_address = input("Select server host: ")
         else:
-            heartbeat_attempt = InteractiveSettings.__input_in_interactive_int_value(
-                DefaultValuesAndOptions.get_default_heartbeat_attempt(),
-                'count of heartbeat attempt'
-            )
-
             is_ssl = InteractiveSettings.__select_in_interactive_from_values(
                 'init ssl mode',
                 DefaultValuesAndOptions.get_ssl_options_data()
             )
 
-            is_hash_control = InteractiveSettings.__select_in_interactive_from_values(
+            is_integrity_control = InteractiveSettings.__select_in_interactive_from_values(
                 'init integrity control',
                 DefaultValuesAndOptions.get_hash_control_options_data()
             )
 
-            workers_count = InteractiveSettings.__input_in_interactive_int_value(
+            workers = InteractiveSettings.__input_in_interactive_int_value(
                 DefaultValuesAndOptions.get_default_workers(), 'thread workers count')
 
-        audio_device = AudioDevice(is_input_device, None)
+        audio_device = AudioDevice(is_input_device, None, ignore_device_encoding_names, device_encoding_names)
+        settings = Settings(is_server_mode, udp_port, server_address, reconnect_attempt, is_ssl,
+                            is_integrity_control, workers, audio_device, password, is_error_log, socket_buffer_size)
+
+        save_to_config_file = InteractiveSettings.__select_in_interactive_from_values(
+            'save selected values to config file',
+            DefaultValuesAndOptions.get_save_profile_options_data()
+        )
+
+        if save_to_config_file:
+            config_file_name = InteractiveSettings.__get_not_null_str_input('config file name')
+            ConfigParser(filename=config_file_name, settings=settings)
 
-        return Settings(is_server_mode, udp_port, server_address, heartbeat_attempt, is_ssl,
-                        is_hash_control, workers_count, audio_device)
+        return settings
+
+    @staticmethod
+    def __get_not_null_str_input(descr: str) -> str:
+        str_input = ''
+        while str_input == '':
+            str_input = input(f"Input {descr}: ").strip()
+            if str_input == '':
+                logging.error(f"Selected {descr} is NULL!")
+
+        return str_input
+
+    @staticmethod
+    def __get_not_null_int_input(descr: str) -> str:
+        int_input = ''
+        while type(int_input) is not int:
+            try:
+                int_input = input(f'Input {descr}: ').strip()
+                if int_input == '':
+                    raise Exception
+                int_input = int(int_input)
+            except Exception:
+                logging.error(f"Invalid {descr}: {int_input}")
+
+        return int_input
 
     @staticmethod
     def __select_in_interactive_from_values(descr: str, options_data: OptionsData):
         """
         Displays a list of options to the user and allows them to select one interactively.
 
         Args:
@@ -116,15 +223,15 @@
             Any: The value of the selected option.
         """
         options_dict = {index: opt for index, opt in enumerate(options_data.options, start=1)}
 
         choices = os.linesep.join([f"{num}. {desc.option_descr}" for num, desc in options_dict.items()])
         prompt_text = (f"Select id of {descr}:"
                        f"{os.linesep + choices + os.linesep}"
-                       f"Your choice (default={options_data.default_descr}): {os.linesep}")
+                       f"Empty field for default value (default={options_data.default_descr}): {os.linesep}")
 
         number_validator = NumberValidator(list(options_dict.keys()))
         while True:
             try:
                 choice = input(prompt_text)
                 is_validating = number_validator.validate(choice)
 
@@ -152,9 +259,30 @@
         """
         while True:
             try:
                 value = input(f"Select {descr} (default={default_value}): ")
 
                 return int(value) if value else default_value
             except ValueError as ve:
-                logging.error(f"Error: {ve}")
-                print("Invalid input, please enter a valid integer.")
+                logging.error(f"Invalid input, please enter a valid integer: {ve}")
+
+    @staticmethod
+    def __get_settings_from_config(filepath: str) -> Settings:
+        configs = ConfigParser(filepath)
+        audio_device = AudioDevice(configs.is_input_audio_device,
+                                   configs.device_id,
+                                   configs.ignore_device_encoding_names,
+                                   configs.device_encoding_names)
+
+        return Settings(
+            configs.is_server,
+            configs.udp_port,
+            configs.server_address,
+            configs.reconnect_attempt,
+            configs.is_ssl,
+            configs.is_integrity_control,
+            configs.workers,
+            audio_device,
+            configs.password,
+            configs.is_error_log,
+            configs.socket_buffer_size
+        )
```

## echowarp/streamer/audio_client.py

```diff
@@ -1,47 +1,40 @@
-import socket
 import threading
 from concurrent.futures import ThreadPoolExecutor
 
 import pyaudio
 import logging
 
 from echowarp.auth_and_heartbeat.transport_client import TransportClient
 from echowarp.models.audio_device import AudioDevice
-from echowarp.models.default_values_and_options import DefaultValuesAndOptions
-from echowarp.services.crypto_manager import CryptoManager
+from echowarp.settings import Settings
 
 
 class ClientStreamReceiver(TransportClient):
     """
         Handles receiving and decoding audio streams on the client side over UDP.
 
         Attributes:
             _udp_port (int): The port number used for receiving UDP audio streams.
             _audio_device (AudioDevice): Audio device configuration for output.
             _executor (ThreadPoolExecutor): Executor for asynchronous task handling.
     """
     _audio_device: AudioDevice
     _executor: ThreadPoolExecutor
 
-    def __init__(self, server_address: str, udp_port: int, stop_util_event: threading.Event,
-                 stop_stream_event: threading.Event, crypto_manager: CryptoManager, audio_device: AudioDevice,
-                 executor: ThreadPoolExecutor):
+    def __init__(self, settings: Settings, stop_util_event: threading.Event(), stop_stream_event: threading.Event()):
         """
                 Initializes a UDP client to receive and play back audio streams.
 
                 Args:
-                    server_address (str): The IP address of the audio source server.
-                    udp_port (int): The UDP port to listen for incoming audio data.
-                    audio_device (AudioDevice): Configured audio device for output.
-                    executor (Executor): Executor for running tasks asynchronously.
-        """
-        super().__init__(server_address, udp_port, stop_util_event, stop_stream_event, crypto_manager)
-        self._audio_device = audio_device
-        self._executor = executor
+                    settings (Settings): Settings object.
+        """
+        super().__init__(settings, stop_util_event, stop_stream_event)
+        self._audio_device = settings.audio_device
+        self._executor = settings.executor
 
     def receive_audio_and_decode(self):
         """
         Starts the process of receiving audio data from the server over UDP, decrypting and decoding it,
         and then playing it back using the configured audio device.
 
         This method handles continuous audio streaming until a stop event is triggered.
@@ -50,46 +43,36 @@
             format=pyaudio.paInt16,
             channels=self._audio_device.channels,
             rate=self._audio_device.sample_rate,
             output=True,
             output_device_index=self._audio_device.device_index
         )
 
-        self._print_listener()
+        self._print_udp_listener_and_start_stream()
         try:
             while not self._stop_util_event.is_set():
-                self._stop_stream_event.wait()
-
                 try:
-                    data, _ = self._client_udp_socket.recvfrom(DefaultValuesAndOptions.SOCKET_BUFFER_SIZE)
-                except socket.timeout as e:
-                    logging.error(f"Timeout to receive stream: {e}")
-                    continue
-                except socket.error as e:
-                    logging.error(f"Failed to receive stream: {e}")
-                    continue
-
-                self._executor.submit(self.__decode_and_play, data, stream)
-        except Exception as e:
-            logging.error(f"Error in streaming audio: {e}")
+                    data, _ = self._udp_socket.recvfrom(self._socket_buffer_size)
+                    self._executor.submit(self.__decode_and_play, data, stream)
+                except Exception:
+                    pass
+
+                self._stop_stream_event.wait()
         finally:
+            self._executor.shutdown()
             stream.stop_stream()
             stream.close()
 
             self._audio_device.py_audio.terminate()
-            self._cleanup_client_sockets()
 
-            logging.info("UDP listening stopped")
+            logging.info("UDP listening finished...")
 
     def __decode_and_play(self, data, stream):
         """
         Decodes the received encrypted audio data and plays it back.
 
         Args:
             data (bytes): Encrypted audio data.
             stream (pyaudio.Stream): PyAudio stream for audio playback.
         """
         data = self._crypto_manager.decrypt_aes_and_verify_data(data)
         stream.write(data)
-
-    def _print_listener(self):
-        logging.info(f'UDP listening started from host {self._server_address}:{self._udp_port}')
```

## echowarp/streamer/audio_server.py

```diff
@@ -1,90 +1,79 @@
-import socket
 import threading
 from concurrent.futures import ThreadPoolExecutor
 
 import pyaudio
 import logging
 
 from echowarp.auth_and_heartbeat.transport_server import TransportServer
 from echowarp.services.crypto_manager import CryptoManager
 from echowarp.models.audio_device import AudioDevice
+from echowarp.settings import Settings
 
 
 class ServerStreamer(TransportServer):
     """
     Handles streaming audio from the server to the client over UDP.
 
     Attributes:
-        _client_addr (str): The client's IP address to send audio data to.
+        _client_address (str): The client's IP address to send audio data to.
         _udp_port (int): The port used for UDP streaming.
         _audio_device (AudioDevice): Audio device used for capturing audio.
         _stop_util_event (threading.Event): Event to signal util to stop.
         _stop_stream_event (threading.Event): Event to signal stream to stop.
         _crypto_manager (CryptoManager): Manager for cryptographic operations.
         _executor (Executor): Executor for asynchronous task execution.
     """
     _audio_device: AudioDevice
     _executor: ThreadPoolExecutor
 
-    def __init__(self, udp_port: int, heartbeat_attempt: int, stop_util_event: threading.Event,
-                 stop_stream_event: threading.Event, crypto_manager: CryptoManager, audio_device: AudioDevice,
-                 executor: ThreadPoolExecutor):
+    def __init__(self, settings: Settings, stop_util_event: threading.Event(), stop_stream_event: threading.Event()):
         """
         Initializes the UDPServerStreamer with specified client address, port, and audio settings.
 
         Args:
-            udp_port (int): UDP port to use for audio streaming.
-            audio_device (AudioDevice): Configured audio device for capturing audio.
-            executor (ThreadPoolExecutor): Executor for managing asynchronous tasks.
-        """
-        super().__init__(udp_port, heartbeat_attempt, stop_util_event, stop_stream_event, crypto_manager)
-        self._audio_device = audio_device
-        self._executor = executor
+            settings (Settings): Settings object.
+        """
+        super().__init__(settings, stop_util_event, stop_stream_event)
+        self._audio_device = settings.audio_device
+        self._executor = settings.executor
 
     def encode_audio_and_send_to_client(self):
         """
         Captures audio from the selected device, encodes it, encrypts, and sends it to the client over UDP.
         This method continuously captures and sends audio until a stop event is triggered.
         """
         stream = self._audio_device.py_audio.open(format=pyaudio.paInt16,
                                                   channels=self._audio_device.channels,
                                                   rate=self._audio_device.sample_rate,
                                                   input=True,
                                                   input_device_index=self._audio_device.device_index,
                                                   frames_per_buffer=1024)
 
-        self._print_listener()
+        self._print_udp_listener_and_start_stream()
         try:
             while not self._stop_util_event.is_set():
-                self._stop_stream_event.wait()
-
-                data = stream.read(1024, exception_on_overflow=False)
-
                 try:
+                    data = stream.read(1024, exception_on_overflow=False)
                     self._executor.submit(self.__send_stream_to_client, data)
-                except socket.error as e:
-                    logging.error(f"Failed to send stream: {e}")
+                except Exception:
+                    pass
 
-        except Exception as e:
-            logging.error(f"Error in streaming audio: {e}")
+                self._stop_stream_event.wait()
         finally:
+            self._executor.shutdown()
             stream.stop_stream()
             stream.close()
 
             self._audio_device.py_audio.terminate()
-            self._cleanup_client_sockets()
 
-            logging.info("Streaming audio stopped.")
+            logging.info("UDP streaming finished...")
 
     def __send_stream_to_client(self, data):
         """
         Encodes and encrypts audio data, then sends it to the client using UDP.
 
         Args:
             data (bytes): Raw audio data to encode and send.
         """
         encoded_data = self._crypto_manager.encrypt_aes_and_sign_data(data)
-        self._udp_server_socket.sendto(encoded_data, (self._client_addr, self._udp_port))
-
-    def _print_listener(self):
-        logging.info(f"Start audio streaming to client on host {self._client_addr}:{self._udp_port}")
+        self._udp_socket.sendto(encoded_data, (self._client_address, self._udp_port))
```

## Comparing `echowarp-0.2.9.dist-info/METADATA` & `echowarp-0.3.0.dist-info/METADATA`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: echowarp
-Version: 0.2.9
+Version: 0.3.0
 Summary: Network audio streaming tool using UDP
 Home-page: https://github.com/lHumaNl/EchoWarp
 Author: lHumaNl
 Author-email: fisher_sam@mail.ru
 License: MIT
 Keywords: audio streaming network
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
-Requires-Dist: pyaudio
+Requires-Dist: PyAudio
 Requires-Dist: cryptography
+Requires-Dist: chardet
 
 # EchoWarp
 
 EchoWarp is a versatile network audio streaming tool designed to transmit audio streams between a server and a client
 over a network. It supports both audio input and output devices, adapting to various audio streaming scenarios. EchoWarp
 can operate in either server or client mode, with robust configuration options available via command-line arguments or
 an interactive setup.
@@ -30,14 +31,16 @@
 - **Flexible Audio Device Selection**: Choose specific input or output devices for audio streaming.
 - **Real-Time Audio Streaming**: Utilizes UDP for transmitting audio data and TCP for control signals.
 - **Robust Encryption and Integrity Checks**: Supports AES encryption and SHA-256 hashing to secure data streams.
 - **Automatic Reconnection**: Implements heartbeat and authentication mechanisms to handle reconnections and ensure
   continuous streaming.
 - **Configurable through CLI and Interactive Modes**: Offers easy setup through an interactive mode or scriptable CLI
   options.
+- **Ban List Management**: Server maintains a ban list to block clients after a specified number of failed connection
+  attempts.
 
 ## Prerequisites
 
 - **Operating System**: Windows, Linux, or macOS.
 - **Python Version**: Python 3.6 or later.
 - **Dependencies**: Includes libraries like PyAudio, and Cryptography.
 
@@ -103,45 +106,110 @@
 arguments.
 
 ## Interactive Mode
 
 Simply run the main.py script without arguments to enter interactive mode:
 
 ```bash
-python main.py
+python -m echowarp.main
 ```
 
 Follow the on-screen prompts to configure the utility.
 
 ## Command-Line Arguments
 
 EchoWarp supports configuration via command-line arguments for easy integration into scripts and automation workflows.
 
 #### Arguments Table
 
-| Argument                    | Description                                                                       | Default      |
-|-----------------------------|-----------------------------------------------------------------------------------|--------------|
-| `-c`, `--client`            | Start utility in client mode.                                                     | Server mode  |
-| `-o`, `--output`            | Use the output audio device for streaming.                                        | Input device |
-| `-p`, `--udp_port`          | Specify the UDP port for audio data transmission.                                 | 4415         |
-| `-d`, `--device_id`         | Specify the device ID directly to avoid interactive selection.                    | None         |
-| `-a`, `--server_addr`       | Specify the server address (only valid in client mode).                           | None         |
-| `-b`, `--heartbeat`         | Set the number of allowed missed heartbeats before disconnect (server mode only). | 5            |
-| `--ssl`                     | Enable SSL mode for encrypted communication (server mode only).                   | False        |
-| `-i`, `--integrity_control` | Enable integrity control using hash (server mode only).                           | False        |
-| `-w`, `--workers`           | Set the maximum number of worker threads (server mode only).                      | 1            |
+| Argument                         | Description                                                     | Default                 |
+|----------------------------------|-----------------------------------------------------------------|-------------------------|
+| `-c`, `--client`                 | Start utility in client mode.                                   | Server mode             |
+| `-o`, `--output`                 | Use the output audio device for streaming.                      | Input device            |
+| `-u`, `--udp_port`               | Specify the UDP port for audio data transmission.               | 4415                    |
+| `-b`, `--socket_buffer_size`     | Size of socket buffer.                                          | 6144                    |
+| `-d`, `--device_id`              | Specify the device ID directly to avoid interactive selection.  | None                    |
+| `-p`, `--password`               | Password for authentication.                                    | None                    |
+| `-f`, `--config_file`            | Path to config file (ignoring other args, if they added).       | None                    |
+| `-e`, `--device_encoding_names`  | Charset encoding for audio device.                              | System default encoding |
+| `--ignore_device_encoding_names` | Ignoring device names encoding.                                 | False                   |
+| `-l`, `--is_error_log`           | Init error file logger.                                         | False                   |
+| `-r`, `--reconnect`              | Number of failed connections before closing the application.    | 5                       |
+| `-s`, `--save_config`            | Save config file from selected args (ignoring default values).  | None                    |
+| `-a`, `--server_address`         | Specify the server address (only valid in client mode).         | None                    |
+| `--ssl`                          | Enable SSL mode for encrypted communication (server mode only). | False                   |
+| `-i`, `--integrity_control`      | Enable integrity control using hash (server mode only).         | False                   |
+| `-w`, `--workers`                | Set the maximum number of worker threads (server mode only).    | 1                       |
 
 Use these arguments to configure the utility directly from the command line for both automation and manual setups.
 
+## Launching with Config File
+
+You can launch EchoWarp using a configuration file to avoid specifying all the arguments manually. Create a
+configuration file with the desired settings and use the --config_file argument to specify the path to this file.
+
+Example of a configuration file (config.conf):
+
+```ini
+[echowarp_conf]
+is_server=False
+udp_port=6532
+socket_buffer_size=10240
+device_id=1
+password=mysecretpassword
+device_encoding_names=cp1251
+is_error_log=True
+server_address=192.168.1.5
+reconnect_attempt=15
+is_ssl=True
+is_integrity_control=True
+```
+
+To launch EchoWarp with the configuration file with CLI args:
+
+```bash
+python -m echowarp.main --config_file path/to/config.conf
+```
+
+## Ban List Management
+
+EchoWarp server maintains a ban list to block clients after a specified number of failed connection attempts. This
+feature helps to secure the server from unauthorized access attempts and repeated failed authentications.
+
+### How Ban List Works
+
+1. **Failed Connection Attempts**: Each client connection attempt is monitored. If a client fails to authenticate multiple times (as specified by the `--reconnect` argument), the client is added to the ban list. Setting `--reconnect` to `0` in server mode disables the ban list feature.
+2. **Banning Clients**: Once a client is banned, it cannot reconnect to the server until the ban list is manually
+   cleared or the server is restarted.
+3. **Persistent Ban List**: The ban list is saved to a file (`echowarp_ban_list.txt`) to maintain the list of banned
+   clients across server restarts.
+
+### Example of Ban List File
+
+The ban list file (`echowarp_ban_list.txt`) contains the IP addresses of banned clients, one per line:
+
+```txt
+192.168.1.100
+192.168.1.101
+```
+
+## Additional Features
+
+- **Heartbeat Mechanism**: Ensures the continuous connection between client and server by periodically sending heartbeat
+  messages.
+- **Thread Pooling**: Utilizes thread pooling for handling concurrent tasks efficiently.
+- **Logging**: Comprehensive logging for both normal operations and errors, with an option to enable error logging to a
+  file.
+
 ## Examples
 
 ### Consult the help output for detailed command-line options::
 
 ```bash
-python main.py --help
+python -m echowarp.main --help
 ```
 
 ### Client Mode with Custom Server Address and Port:
 
 ```bash
-python main.py --client --server_addr 192.168.1.5 --udp_port 6555
+python -m echowarp.main --client --server_addr 192.168.1.5 --udp_port 6555
 ```
```

