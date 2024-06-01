# Comparing `tmp/diagralhomekit-0.9.8.tar.gz` & `tmp/diagralhomekit-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diagralhomekit-0.9.8.tar", max compression
+gzip compressed data, was "diagralhomekit-0.9.9.tar", max compression
```

## Comparing `diagralhomekit-0.9.8.tar` & `diagralhomekit-0.9.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0    21393 2023-04-03 19:32:16.506454 diagralhomekit-0.9.8/LICENSE
--rw-r--r--   0        0        0     3336 2023-04-06 16:01:35.043604 diagralhomekit-0.9.8/README.md
--rw-r--r--   0        0        0      455 2023-04-05 18:45:00.080586 diagralhomekit-0.9.8/diagralhomekit/__init__.py
--rw-r--r--   0        0        0      584 2023-04-06 08:43:32.341564 diagralhomekit-0.9.8/diagralhomekit/__main__.py
--rw-r--r--   0        0        0     2352 2023-04-06 12:46:44.557883 diagralhomekit-0.9.8/diagralhomekit/alarm_system.py
--rw-r--r--   0        0        0     2453 2023-04-09 07:56:45.202374 diagralhomekit-0.9.8/diagralhomekit/config.py
--rw-r--r--   0        0        0    27550 2023-08-20 16:01:57.683182 diagralhomekit-0.9.8/diagralhomekit/diagral.py
--rw-r--r--   0        0        0     7402 2023-04-09 17:37:48.827836 diagralhomekit-0.9.8/diagralhomekit/homekit_alarm.py
--rw-r--r--   0        0        0     4243 2023-04-06 14:01:59.443690 diagralhomekit-0.9.8/diagralhomekit/http_plugin.py
--rw-r--r--   0        0        0     4763 2023-09-18 12:47:42.637830 diagralhomekit-0.9.8/diagralhomekit/main.py
--rw-r--r--   0        0        0     7518 2023-04-06 15:59:40.754133 diagralhomekit-0.9.8/diagralhomekit/meteofrance.py
--rw-r--r--   0        0        0     4452 2023-04-06 15:48:02.383331 diagralhomekit-0.9.8/diagralhomekit/nut.py
--rw-r--r--   0        0        0     8870 2023-08-19 20:28:09.558662 diagralhomekit-0.9.8/diagralhomekit/plex.py
--rw-r--r--   0        0        0     1044 2023-04-06 13:50:15.159321 diagralhomekit-0.9.8/diagralhomekit/plugin.py
--rw-r--r--   0        0        0     2524 2023-04-06 13:38:00.533738 diagralhomekit-0.9.8/diagralhomekit/utils.py
--rw-r--r--   0        0        0      642 2023-09-18 12:48:18.667173 diagralhomekit-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     4423 1970-01-01 00:00:00.000000 diagralhomekit-0.9.8/setup.py
--rw-r--r--   0        0        0     4215 1970-01-01 00:00:00.000000 diagralhomekit-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    21393 2023-04-03 19:32:16.506454 diagralhomekit-0.9.9/LICENSE
+-rw-r--r--   0        0        0     3336 2023-04-06 16:01:35.043604 diagralhomekit-0.9.9/README.md
+-rw-r--r--   0        0        0      455 2023-04-05 18:45:00.080586 diagralhomekit-0.9.9/diagralhomekit/__init__.py
+-rw-r--r--   0        0        0      584 2023-04-06 08:43:32.341564 diagralhomekit-0.9.9/diagralhomekit/__main__.py
+-rw-r--r--   0        0        0     2352 2023-04-06 12:46:44.557883 diagralhomekit-0.9.9/diagralhomekit/alarm_system.py
+-rw-r--r--   0        0        0     2453 2023-04-09 07:56:45.202374 diagralhomekit-0.9.9/diagralhomekit/config.py
+-rw-r--r--   0        0        0    27550 2023-08-20 16:01:57.683182 diagralhomekit-0.9.9/diagralhomekit/diagral.py
+-rw-r--r--   0        0        0     7402 2023-04-09 17:37:48.827836 diagralhomekit-0.9.9/diagralhomekit/homekit_alarm.py
+-rw-r--r--   0        0        0     4243 2023-04-06 14:01:59.443690 diagralhomekit-0.9.9/diagralhomekit/http_plugin.py
+-rw-r--r--   0        0        0     3075 2023-09-19 13:40:59.416488 diagralhomekit-0.9.9/diagralhomekit/main.py
+-rw-r--r--   0        0        0     7518 2023-04-06 15:59:40.754133 diagralhomekit-0.9.9/diagralhomekit/meteofrance.py
+-rw-r--r--   0        0        0     4452 2023-04-06 15:48:02.383331 diagralhomekit-0.9.9/diagralhomekit/nut.py
+-rw-r--r--   0        0        0     8870 2023-08-19 20:28:09.558662 diagralhomekit-0.9.9/diagralhomekit/plex.py
+-rw-r--r--   0        0        0     1044 2023-04-06 13:50:15.159321 diagralhomekit-0.9.9/diagralhomekit/plugin.py
+-rw-r--r--   0        0        0     2524 2023-04-06 13:38:00.533738 diagralhomekit-0.9.9/diagralhomekit/utils.py
+-rw-r--r--   0        0        0      612 2023-09-19 13:40:57.242047 diagralhomekit-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     4386 1970-01-01 00:00:00.000000 diagralhomekit-0.9.9/setup.py
+-rw-r--r--   0        0        0     4164 1970-01-01 00:00:00.000000 diagralhomekit-0.9.9/PKG-INFO
```

### Comparing `diagralhomekit-0.9.8/LICENSE` & `diagralhomekit-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.8/README.md` & `diagralhomekit-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.8/diagralhomekit/__main__.py` & `diagralhomekit-0.9.9/diagralhomekit/__main__.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.8/diagralhomekit/alarm_system.py` & `diagralhomekit-0.9.9/diagralhomekit/alarm_system.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.8/diagralhomekit/config.py` & `diagralhomekit-0.9.9/diagralhomekit/config.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.8/diagralhomekit/diagral.py` & `diagralhomekit-0.9.9/diagralhomekit/diagral.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.8/diagralhomekit/homekit_alarm.py` & `diagralhomekit-0.9.9/diagralhomekit/homekit_alarm.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.8/diagralhomekit/http_plugin.py` & `diagralhomekit-0.9.9/diagralhomekit/http_plugin.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.8/diagralhomekit/main.py` & `diagralhomekit-0.9.9/diagralhomekit/nut.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,141 +1,119 @@
 # ##############################################################################
 #  Copyright (c) Matthieu Gallet <github@19pouces.net> 2023.                   #
-#  This file main.py is part of DiagralHomekit.                                #
+#  This file nut.py is part of DiagralHomekit.                                 #
 #  Please check the LICENSE file for sharing or distribution permissions.      #
 # ##############################################################################
-"""All the main functions."""
-import argparse
+"""UPS sensor fetching data from the local NUT client."""
 import logging
-import os
-import pathlib
-import signal
-import socket
-import sys
-import urllib.parse
-from multiprocessing import Queue
+from configparser import ConfigParser
+from typing import List
 
-import sentry_sdk
-from logging_loki import LokiQueueHandler, emitter
+from nut2 import PyNUTClient, PyNUTError
 
 # noinspection PyPackageRequirements
-from pyhap.accessory import Bridge
+from pyhap.accessory import Accessory
 
 # noinspection PyPackageRequirements
-from pyhap.accessory_driver import AccessoryDriver
+from pyhap.const import CATEGORY_SENSOR
 
-from diagralhomekit.config import HomekitConfig
-from diagralhomekit.diagral import DiagralHomekitPlugin
+from diagralhomekit.plugin import HomekitPlugin
 
-logger = logging.getLogger("diagralhomekit")
+logger = logging.getLogger(__name__)
 
 
-def main():
-    """parse arguments and run the daemons."""
-    parser = argparse.ArgumentParser()
-    default_port = int(os.environ.get("DIAGRAL_PORT", "51826"))
-    default_config_dir = os.environ.get("DIAGRAL_CONFIG", "/etc/diagralhomekit")
-    default_sentry_dsn = os.environ.get("DIAGRAL_SENTRY_DSN")
-    default_loki_url = os.environ.get("DIAGRAL_LOKI_URL")
-    verbosity = int(os.environ.get("DIAGRAL_VERBOSITY", 0))
-    parser.add_argument(
-        "--create-config",
-        help="--create-config 'email:password' display a sample configuration file",
-        default=None,
-    )
-    parser.add_argument("-p", "--port", type=int, default=default_port)
-    parser.add_argument(
-        "-C",
-        "--config-dir",
-        default=pathlib.Path(default_config_dir),
-        type=pathlib.Path,
-    )
-    parser.add_argument("--sentry-dsn", default=default_sentry_dsn)
-    parser.add_argument("--loki-url", default=default_loki_url)
-    parser.add_argument("-v", "--verbosity", default=verbosity, type=int)
-    args = parser.parse_args()
-    config_dir = args.config_dir
-    if args.create_config:
-        login, sep, password = args.create_config.partition(":")
-        if sep != ":":
-            print("Usage: --create-config=login:password")
-            return
-        content = DiagralHomekitPlugin.show_basic_config(login, password)
-        print(f"cat << EOF > {config_dir}/config.ini")
-        print(content)
-        print("EOF")
-        return
-
-    handler = logging.StreamHandler(sys.stdout)
-    if args.verbosity == 0:
-        logger.setLevel(logging.WARNING)
-    elif args.verbosity == 1:
-        logger.setLevel(logging.INFO)
-    else:
-        logger.setLevel(logging.DEBUG)
-    logger.addHandler(handler)
-    listen_port = args.port
-
-    if args.loki_url:
+class UPSSensor(Accessory):
+    """UPS sensor., compatible with the NUT server."""
+
+    category = CATEGORY_SENSOR
+
+    def __init__(self, driver, ups_name, ups_verbose_name, ups_data):
+        """init function."""
+        serial = ups_data["ups.serial"]
+        aid = hash(f"{serial}")
+        super().__init__(driver, ups_verbose_name, aid=aid)
+        info_service = self.get_service("AccessoryInformation")
+        for char_name, value in (
+            ("Identify", False),
+            ("Manufacturer", ups_data["ups.mfr"]),
+            ("Model", ups_data["ups.model"]),
+            ("Name", ups_verbose_name),
+            ("SerialNumber", serial),
+            ("FirmwareRevision", str(ups_data["ups.firmware"])),
+        ):
+            characteristic = info_service.get_characteristic(char_name)
+            characteristic.set_value(value)
+        self.ups_name = ups_name
+        service = self.add_preload_service("BatteryService")
+        self.battery_level = service.get_characteristic("BatteryLevel")
+        self.charging_state = service.get_characteristic("ChargingState")
+        self.status_low_battery = service.get_characteristic("StatusLowBattery")
+
+    def extra_log_data(self, **kwargs):
+        """Extra data for logging events."""
+        return {"tags": {"identifier": self.ups_name, "type": "ups", **kwargs}}
+
+    @Accessory.run_at_interval(60)
+    def run(self):
+        """Regularly fetch data."""
         try:
-            hostname = socket.gethostname()
-        except socket.gaierror:
-            hostname = "localhost"
-        emitter.LokiEmitter.level_tag = "level"
-        parsed_url = urllib.parse.urlparse(args.loki_url)
-        url = f"{parsed_url.scheme}://{parsed_url.hostname}"
-        if parsed_url.port:
-            url += f":{parsed_url.port}"
-        url += parsed_url.path
-        if parsed_url.query:
-            url += f"?{parsed_url.query}"
-        handler = LokiQueueHandler(
-            Queue(-1),
-            url=url,
-            tags={
-                "application": "diagralhomekit",
-                "log_source": "diagralhomekit",
-                "hostname": hostname,
-            },
-            auth=(parsed_url.username or "", parsed_url.password or ""),
-            version="1",
+            client = PyNUTClient()
+            data = client.list_vars(self.ups_name)
+        except Exception as e:
+            logger.exception(e, extra=self.extra_log_data())
+            data = {
+                "battery.charge": "100",
+                "battery.charge.low": "20",
+                "ups.status": "OL",
+            }
+
+        battery_level = int(data["battery.charge"])
+        battery_threshold = int(data["battery.charge.low"])
+        is_low = 1 if battery_level <= battery_threshold else 0
+
+        self.battery_level.set_value(battery_level)
+        self.status_low_battery.set_value(is_low)
+        self.charging_state.set_value(1 if data["ups.status"] == "OL" else 0)
+
+
+class UPSMonitoringPlugin(HomekitPlugin):
+    """Plugin for local UPS services, on Linux hosts."""
+
+    config_prefix = "ups"
+
+    def __init__(self, config):
+        """init function."""
+        super().__init__(config)
+        self.ups_names: List[str] = []
+        self.sensors: List[UPSSensor] = []
+
+    def load_config(self, parser: ConfigParser, section):
+        """Load a configuration section."""
+        logger.debug(f"loading {section}")
+        config_errors = []
+        ups_name = parser.get(section, "name", fallback=None)
+        if ups_name is None:
+            msg = f"Invalid option name in section {section}."
+            config_errors.append(msg)
+            logger.fatal(msg)
+        self.ups_names.append(ups_name)
+        logger.info(
+            f"Configuration for monitoring {ups_name} added.",
+            extra={"tags": {"type": "internet"}},
         )
-        logger.addHandler(handler)
-        logger.debug("Loki configured.")
+        return config_errors
+
+    def load_accessories(self, bridge):
+        """Add accessories to the Homekit bridge."""
+        try:
+            client = PyNUTClient()
+        except PyNUTError as e:
+            logger.exception(e)
+            return
+        available_upses = client.list_ups()
 
-    if args.sentry_dsn:
-        sentry_sdk.init(args.sentry_dsn)
-        logger.debug("Sentry DSN configured.")
-
-    run_daemons(
-        config_dir,
-        listen_port,
-        verbosity=args.verbosity,
-    )
-
-
-def run_daemons(config_dir, listen_port, verbosity: int = 1):
-    """launch all processes: Homekit and Diagral checker."""
-    persist_file = config_dir / "persist.json"
-    config_file = config_dir / "config.ini"
-    logger.info(f"configuration file: {config_file}")
-    logger.info(f"persistence file: {persist_file}")
-    logger.info(f"listen port: {listen_port}")
-
-    driver = AccessoryDriver(
-        port=listen_port,
-        persist_file=persist_file,
-    )
-    bridge = Bridge(driver, "Diagral e-One")
-    config = HomekitConfig()
-    config.verbosity = verbosity
-    try:
-        config.load_config(config_file)
-        config.load_accessories(bridge)
-        driver.add_accessory(accessory=bridge)
-        signal.signal(signal.SIGTERM, driver.signal_handler)
-        config.run_all()
-        driver.start()
-    except Exception as e:
-        logger.exception(e)
-        raise e
-    config.stop_all()
+        for ups_name in self.ups_names:
+            ups_verbose_name = available_upses.get(ups_name)
+            ups_data = client.list_vars(ups_name)
+            sensor = UPSSensor(bridge.driver, ups_name, ups_verbose_name, ups_data)
+            self.sensors.append(sensor)
+            bridge.add_accessory(sensor)
```

### Comparing `diagralhomekit-0.9.8/diagralhomekit/meteofrance.py` & `diagralhomekit-0.9.9/diagralhomekit/meteofrance.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.8/diagralhomekit/plex.py` & `diagralhomekit-0.9.9/diagralhomekit/plex.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.8/diagralhomekit/plugin.py` & `diagralhomekit-0.9.9/diagralhomekit/plugin.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.8/diagralhomekit/utils.py` & `diagralhomekit-0.9.9/diagralhomekit/utils.py`

 * *Files identical despite different names*

### Comparing `diagralhomekit-0.9.8/pyproject.toml` & `diagralhomekit-0.9.9/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -4,25 +4,24 @@
 
 [tool.poetry]
 authors = ["d9pouces <github@19pouces.net>"]
 description = "Apple HomeKit integration for Diagral alarm systems"
 license = "CeCILL-B"
 name = "diagralhomekit"
 readme = "README.md"
-version = "0.9.8"
+version = "0.9.9"
 
 [tool.poetry.dependencies]
 HAP-python = "^4.6.0"
 base36 = "^0.1.1"
 meteofrance-api = "^1.2.0"
 nut2 = "^2.1.1"
 pyqrcode = "^1.2.1"
 python = "^3.9"
-python-logging-loki = "^0.3.1"
 requests = "^2.28.2"
-sentry-sdk = "^1.18.0"
+systemlogger = "^0.1.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.3.0"
 
 [tool.poetry.scripts]
 diagral-homekit = "diagralhomekit.main:main"
```

### Comparing `diagralhomekit-0.9.8/setup.py` & `diagralhomekit-0.9.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 
 install_requires = \
 ['HAP-python>=4.6.0,<5.0.0',
  'base36>=0.1.1,<0.2.0',
  'meteofrance-api>=1.2.0,<2.0.0',
  'nut2>=2.1.1,<3.0.0',
  'pyqrcode>=1.2.1,<2.0.0',
- 'python-logging-loki>=0.3.1,<0.4.0',
  'requests>=2.28.2,<3.0.0',
- 'sentry-sdk>=1.18.0,<2.0.0']
+ 'systemlogger>=0.1.0,<0.2.0']
 
 entry_points = \
 {'console_scripts': ['diagral-homekit = diagralhomekit.main:main']}
 
 setup_kwargs = {
     'name': 'diagralhomekit',
-    'version': '0.9.8',
+    'version': '0.9.9',
     'description': 'Apple HomeKit integration for Diagral alarm systems',
     'long_description': "DiagralHomekit\n==============\n\n[![PyPI version](https://badge.fury.io/py/diagralhomekit.svg)](https://badge.fury.io/py/diagralhomekit)\n\nAllow to control your Diagral alarm systems through Apple Homekit.\n\n\nFirst, you need to create a configuration file `~/.diagralhomekit/config.ini` with connection details for all Diagral systems.\n\n```ini\n[diagral:Home]\nname=[an explicit name for this system]\nlogin=[email address of the Diagral account]\npassword=[password for the Diagral account]\nimap_login=[IMAP login for the email address receiving alarm alerts]\nimap_password=[IMAP password]\nimap_hostname=[IMAP server]\nimap_port=[IMAP port]\nimap_use_tls=[true/1/on if you use SSL for the IMAP connection]\nmaster_code=[a Diagral master code, able to arm or disarm the alarm]\nsystem_id=[system id — see below]\ntransmitter_id=[transmitter id — see below]\ncentral_id=[central id — see below]\n\n```\n`system_id`, `transmitter_id` and `central_id` can be retrieved with the following command, that prepares a configuration file:\n\n```bash\npython3 -m diagralhomekit --config-dir ~/.diagralhomekit --create-config 'diagral@account.com:password'\n```\n\nThen you can run the script:\n\n```bash\npython3 -m diagralhomekit --port 6666 --config-dir ~/.diagralhomekit -v 2\n```\nOn the first launch, a QR code is displayed and can be scanned in Homekit, like any Homekit-compatible device.\n\n\nYou can send logs to [Loki](https://grafana.com/oss/loki/) with `--loki-url=https://username:password@my.loki.server/loki/api/v1/push`.\nYou can also send alerts to [Sentry](https://sentry.io/) with `--sentry-dsn=my_sentry_dsn`.\n\nEverything can be configured by environment variables instead of arguments:\n\n```bash\nDIAGRAL_PORT=6666\nDIAGRAL_CONFIG=/etc/diagralhomekit\nDIAGRAL_SENTRY_DSN=https://sentry_dsn@sentry.io/42\nDIAGRAL_LOKI_URL=https://username:password@my.loki.server/loki/api/v1/push\nDIAGRAL_VERBOSITY=1\n```\n\n\n**As many sensitive data must be stored in this configuration file, so you should create a dedicated email address and Diagral account.**\n\n\nPlex sensor\n-----------\n\nA presence can be detected when a specified Plex player is playing something:\n```ini\n[plex:appletv_web]\nserver_token=[authentication token]\nserver_url=[url of your Plex server]\nplayer_name=[Displayed name for the player]\nplayer_device=None,\nplayer_product=[Product name of the targeted player]\nplayer_title=[Title of the targeted player]\nplayer_address=[IP address of the targeted player]\n```\nOnly one of the last four properties is required to match with the targeted player.\nTo get actual property values, you can use `curl`:\n\n```bash\ncurl -H Accept:application/json -H X-Plex-Token:[authentication token] [url of your Plex server]/status/sessions\n```\n\nHTTP monitoring\n---------------\n\nYou can monitor some websites, as air purifier sensors (no Homekit sensor is available for HTTP monitoring…):\n```ini\n[internet:website]\nurl=[url to check]\nname=[Displayed name]\n```\n\nWeather monitoring\n------------------\n\nYou can monitor weather, and emulate a presence when it will rain in the next 10 minutes:\n\n```ini\n[meteofrance:paris]\nname=Paris\nlatitude=48.866667\nlongitude=2.333333\ncountry=FR\nregion=Île-de-France\n```\n\nUPS monitoring\n--------------\n\nUPS can also be monitoring, as soon as NUT is locally installed (standard UPS monitoring server on Linux.\n```\n[ups:home]\nname=eaton650\n```\n",
     'author': 'd9pouces',
     'author_email': 'github@19pouces.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `diagralhomekit-0.9.8/PKG-INFO` & `diagralhomekit-0.9.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: diagralhomekit
-Version: 0.9.8
+Version: 0.9.9
 Summary: Apple HomeKit integration for Diagral alarm systems
 License: CECILL-B
 Author: d9pouces
 Author-email: github@19pouces.net
 Requires-Python: >=3.9,<4.0
 Classifier: License :: CeCILL-B Free Software License Agreement (CECILL-B)
 Classifier: Programming Language :: Python :: 3
@@ -12,17 +12,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: HAP-python (>=4.6.0,<5.0.0)
 Requires-Dist: base36 (>=0.1.1,<0.2.0)
 Requires-Dist: meteofrance-api (>=1.2.0,<2.0.0)
 Requires-Dist: nut2 (>=2.1.1,<3.0.0)
 Requires-Dist: pyqrcode (>=1.2.1,<2.0.0)
-Requires-Dist: python-logging-loki (>=0.3.1,<0.4.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
-Requires-Dist: sentry-sdk (>=1.18.0,<2.0.0)
+Requires-Dist: systemlogger (>=0.1.0,<0.2.0)
 Description-Content-Type: text/markdown
 
 DiagralHomekit
 ==============
 
 [![PyPI version](https://badge.fury.io/py/diagralhomekit.svg)](https://badge.fury.io/py/diagralhomekit)
```

