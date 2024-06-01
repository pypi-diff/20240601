# Comparing `tmp/redbacktechpy-2024.5.0b4.tar.gz` & `tmp/redbacktechpy-2024.5.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbacktechpy-2024.5.0b4.tar", last modified: Sat Jun  1 00:40:44 2024, max compression
+gzip compressed data, was "redbacktechpy-2024.5.1b1.tar", last modified: Sat Jun  1 19:30:08 2024, max compression
```

## Comparing `redbacktechpy-2024.5.0b4.tar` & `redbacktechpy-2024.5.1b1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:40:44.642201 redbacktechpy-2024.5.0b4/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 00:40:40.000000 redbacktechpy-2024.5.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 00:40:44.642201 redbacktechpy-2024.5.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-01 00:40:40.000000 redbacktechpy-2024.5.0b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 00:40:44.642201 redbacktechpy-2024.5.0b4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:40:44.638201 redbacktechpy-2024.5.0b4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:40:44.638201 redbacktechpy-2024.5.0b4/src/redbacktechpy/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 00:40:40.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-01 00:40:40.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-01 00:40:40.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-01 00:40:40.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    54403 2024-06-01 00:40:40.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy/redbacktech_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-01 00:40:40.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy/str_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:40:44.642201 redbacktechpy-2024.5.0b4/src/redbacktechpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 00:40:44.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-01 00:40:44.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:40:44.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 00:40:44.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 00:40:44.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:30:08.044645 redbacktechpy-2024.5.1b1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 19:30:03.000000 redbacktechpy-2024.5.1b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 19:30:08.044645 redbacktechpy-2024.5.1b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-01 19:30:03.000000 redbacktechpy-2024.5.1b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 19:30:08.044645 redbacktechpy-2024.5.1b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:30:08.040645 redbacktechpy-2024.5.1b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:30:08.044645 redbacktechpy-2024.5.1b1/src/redbacktechpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 19:30:03.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-01 19:30:03.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-01 19:30:03.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-01 19:30:03.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50853 2024-06-01 19:30:03.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy/redbacktech_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-01 19:30:03.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy/str_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:30:08.044645 redbacktechpy-2024.5.1b1/src/redbacktechpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 19:30:08.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-01 19:30:08.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 19:30:08.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 19:30:08.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 19:30:08.000000 redbacktechpy-2024.5.1b1/src/redbacktechpy.egg-info/top_level.txt
```

### Comparing `redbacktechpy-2024.5.0b4/LICENSE` & `redbacktechpy-2024.5.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.0b4/PKG-INFO` & `redbacktechpy-2024.5.1b1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.0b4
+Version: 2024.5.1b1
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `redbacktechpy-2024.5.0b4/pyproject.toml` & `redbacktechpy-2024.5.1b1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "redbacktechpy"
-version = "2024.05.0b4"
+version = "2024.05.1b1"
 authors = [
   { name="Chris Abberley", email="unlisted@gmail.com" },
 ]
 description = "Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
```

### Comparing `redbacktechpy-2024.5.0b4/src/redbacktechpy/__init__.py` & `redbacktechpy-2024.5.1b1/src/redbacktechpy/__init__.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.0b4/src/redbacktechpy/constants.py` & `redbacktechpy-2024.5.1b1/src/redbacktechpy/constants.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.0b4/src/redbacktechpy/model.py` & `redbacktechpy-2024.5.1b1/src/redbacktechpy/model.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.0b4/src/redbacktechpy/redbacktech_client.py` & `redbacktechpy-2024.5.1b1/src/redbacktechpy/redbacktech_client.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,32 +3,32 @@
 from aiohttp import ClientResponse, ClientSession
 from typing import Any
 import asyncio
 from datetime import datetime, timedelta, timezone
 from bs4 import BeautifulSoup
 import logging
 
-from .constants import (
+from constants import (
     BaseUrl, 
     Endpoint, 
     Header,
     InverterOperationType,
     TIMEOUT,
     AUTH_ERROR_CODES,
     DEVICEINFOREFRESH,
 )
 
-from .model import (
+from model import (
     Inverters,
     Batterys,
     RedbackTechData,
     RedbackEntitys,
     DeviceInfo,
 )
-from .exceptions import (
+from exceptions import (
         AuthError, 
         RedbackTechClientError,
 )
 
 LOGGER = logging.getLogger(__name__)
 
 class RedbackTechClient:
@@ -618,237 +618,249 @@
             response: dict[str, Any] = await resp.text()
         except Exception as error:
             raise RedbackTechClientError(f'Could not return text {error}') from error
 
         return response
 
     async def _create_device_info_inverter(self, data) -> None:
+        id_temp = data['Data']['Nodes'][0]['StaticData']['Id']
+        id_temp = id_temp[-4:] + 'inv'
+        id_temp = id_temp.lower()
         dataDict = {
-            'identifiers': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter',
+            'identifiers': id_temp, #data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter',
             'name': data['Data']['Nodes'][0]['StaticData']['ModelName'] + ' - inverter',
             'model': data['Data']['Nodes'][0]['StaticData']['ModelName'],
             'sw_version': data['Data']['Nodes'][0]['StaticData']['SoftwareVersion'],
             'hw_version': data['Data']['Nodes'][0]['StaticData']['FirmwareVersion'],
             'serial_number': data['Data']['Nodes'][0]['StaticData']['Id'],
         }
         self._redback_device_info.append(dataDict)
     
     async def _create_device_info_battery(self, data) -> None:
+        id_temp = data['Data']['Nodes'][0]['StaticData']['Id']
+        id_temp = id_temp[-4:] + 'bat'
+        id_temp = id_temp.lower()
         dataDict = {
-            'identifiers': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery',
+            'identifiers': id_temp, #data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery',
             'name': data['Data']['Nodes'][0]['StaticData']['ModelName'] + ' - battery',
             'model': data['Data']['Nodes'][0]['StaticData']['ModelName'],
             'sw_version': data['Data']['Nodes'][0]['StaticData']['SoftwareVersion'],
             'hw_version': data['Data']['Nodes'][0]['StaticData']['FirmwareVersion'],
             'serial_number': data['Data']['Nodes'][0]['StaticData']['Id'],
         }
         self._redback_device_info.append(dataDict)
 
     async def _convert_responses_to_inverter_entities(self, data, data2) -> None:
         """Convert responses to entities."""
         pvId =1
+        id_temp = data['Data']['Nodes'][0]['StaticData']['Id']
+        id_temp = id_temp[-4:] + 'inv'
+        id_temp = id_temp.lower()
         #entity_name
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['ModelName'], 'entity_name': 'model_name', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter', 'type_set': 'sensor.string' }
+        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['ModelName'], 'entity_name': 'model_name', 'device_id': id_temp, 'device_type': 'inverter', 'type_set': 'sensor.string' }
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['Id'], 'entity_name': 'serial_number', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter', 'type_set': 'sensor.string' }
+        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['Id'], 'entity_name': 'serial_number', 'device_id': id_temp, 'device_type': 'inverter', 'type_set': 'sensor.string' }
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['Location']['Latitude'], 'entity_name': 'latitude', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter', 'type_set': 'sensor.string' }
+        dataDict = {'value': data['Data']['StaticData']['Location']['Latitude'], 'entity_name': 'latitude', 'device_id': id_temp, 'device_type': 'inverter', 'type_set': 'sensor.string' }
         self._redback_entities.append(dataDict)
-        dataDict = { 'value': data['Data']['StaticData']['Location']['Latitude'], 'entity_name': 'latitude', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter', 'type_set': 'sensor.string' }
+        dataDict = { 'value': data['Data']['StaticData']['Location']['Latitude'], 'entity_name': 'latitude', 'device_id': id_temp, 'device_type': 'inverter', 'type_set': 'sensor.string' }
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['RemoteAccessConnection']['Type'],'entity_name': 'network_connection', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['RemoteAccessConnection']['Type'],'entity_name': 'network_connection', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['ApprovedCapacityW'],'entity_name': 'approved_capacity', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['ApprovedCapacityW'],'entity_name': 'approved_capacity', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['GenerationHardLimitVA'],'entity_name': 'generation_hard_limit_va', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['GenerationHardLimitVA'],'entity_name': 'generation_hard_limit_va', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['GenerationSoftLimitVA'],'entity_name': 'generation_soft_limit_va', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['GenerationSoftLimitVA'],'entity_name': 'generation_soft_limit_va', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['ExportHardLimitkW'],'entity_name': 'export_hard_limit_kw', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['ExportHardLimitkW'],'entity_name': 'export_hard_limit_kw', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['ExportSoftLimitkW'],'entity_name': 'export_soft_limit_kw', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['ExportSoftLimitkW'],'entity_name': 'export_soft_limit_kw', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['SiteExportLimitkW'],'entity_name': 'site_export_limit_kw', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['SiteExportLimitkW'],'entity_name': 'site_export_limit_kw', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['PanelModel'],'entity_name': 'pv_panel_model', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['PanelModel'],'entity_name': 'pv_panel_model', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['PanelSizekW'],'entity_name': 'pv_panel_size_kw', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['PanelSizekW'],'entity_name': 'pv_panel_size_kw', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['SystemType'],'entity_name': 'system_type', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['SystemType'],'entity_name': 'system_type', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['InverterMaxExportPowerkW'],'entity_name': 'inverter_max_export_power_kw', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['InverterMaxExportPowerkW'],'entity_name': 'inverter_max_export_power_kw', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['InverterMaxImportPowerkW'],'entity_name': 'inverter_max_import_power_kw', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['InverterMaxImportPowerkW'],'entity_name': 'inverter_max_import_power_kw', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['CommissioningDate'],'entity_name': 'commissioning_date', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['CommissioningDate'],'entity_name': 'commissioning_date', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['ModelName'],'entity_name': 'model_name', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['ModelName'],'entity_name': 'model_name', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['NMI'],'entity_name': 'nmi', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['NMI'],'entity_name': 'nmi', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['Id'],'entity_name': 'site_id', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['Id'],'entity_name': 'site_id', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['Type'],'entity_name': 'inverter_site_type', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['StaticData']['Type'],'entity_name': 'inverter_site_type', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['BatteryCount'],'entity_name': 'battery_count', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['BatteryCount'],'entity_name': 'battery_count', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['SoftwareVersion'],'entity_name': 'software_version', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['SoftwareVersion'],'entity_name': 'software_version', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['FirmwareVersion'],'entity_name': 'firmware_version', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['FirmwareVersion'],'entity_name': 'firmware_version', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['Id'],'entity_name': 'inverter_serial_number', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['Id'],'entity_name': 'inverter_serial_number', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['TimestampUtc'],'entity_name': 'timestamp_utc', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data2['Data']['TimestampUtc'],'entity_name': 'timestamp_utc', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['FrequencyInstantaneousHz'],'entity_name': 'frequency_instantaneous', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data2['Data']['FrequencyInstantaneousHz'],'entity_name': 'frequency_instantaneous', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['PvPowerInstantaneouskW'],'entity_name': 'pv_power_instantaneous_kw', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data2['Data']['PvPowerInstantaneouskW'],'entity_name': 'pv_power_instantaneous_kw', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['InverterTemperatureC'],'entity_name': 'inverter_temperature_c', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data2['Data']['InverterTemperatureC'],'entity_name': 'inverter_temperature_c', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['PvAllTimeEnergykWh'],'entity_name': 'pv_all_time_energy_kwh', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data2['Data']['PvAllTimeEnergykWh'],'entity_name': 'pv_all_time_energy_kwh', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['ExportAllTimeEnergykWh'],'entity_name': 'export_all_time_energy_kwh', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data2['Data']['ExportAllTimeEnergykWh'],'entity_name': 'export_all_time_energy_kwh', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['ImportAllTimeEnergykWh'],'entity_name': 'import_all_time_energy_kwh', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data2['Data']['ImportAllTimeEnergykWh'],'entity_name': 'import_all_time_energy_kwh', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['LoadAllTimeEnergykWh'],'entity_name': 'load_all_time_energy_kwh', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data2['Data']['LoadAllTimeEnergykWh'],'entity_name': 'load_all_time_energy_kwh', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['Status'],'entity_name': 'status', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data2['Data']['Status'],'entity_name': 'status', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['Inverters'][0]['PowerMode']['InverterMode'],'entity_name': 'power_mode_inverter_mode', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data2['Data']['Inverters'][0]['PowerMode']['InverterMode'],'entity_name': 'power_mode_inverter_mode', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['Inverters'][0]['PowerMode']['PowerW'],'entity_name': 'power_mode_power_w', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+        dataDict = {'value': data2['Data']['Inverters'][0]['PowerMode']['PowerW'],'entity_name': 'power_mode_power_w', 'device_id': id_temp, 'device_type': 'inverter'}
         self._redback_entities.append(dataDict)
         for pv in data2['Data']['PVs']:
             entity_name_temp = f'pv_{pvId}_current_a'
-            dataDict = {'value': pv['CurrentA'],'entity_name': entity_name_temp, 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+            dataDict = {'value': pv['CurrentA'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
             entity_name_temp = f'pv_{pvId}_voltage_v'
-            dataDict = {'value': pv['VoltageV'],'entity_name': entity_name_temp, 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+            dataDict = {'value': pv['VoltageV'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
             entity_name_temp = f'pv_{pvId}_power_kw'
-            dataDict = {'value': pv['PowerkW'],'entity_name': entity_name_temp, 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+            dataDict = {'value': pv['PowerkW'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
             pvId += 1
         for phase in data2['Data']['Phases']:  
             phaseAlpha=phase['Id']
             entity_name_temp = f'inverter_phase_{phaseAlpha}_active_exported_power_instantaneous_kw'
-            dataDict = {'value': phase['ActiveExportedPowerInstantaneouskW'],'entity_name': entity_name_temp, 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+            dataDict = {'value': phase['ActiveExportedPowerInstantaneouskW'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
             entity_name_temp = f'inverter_phase_{phaseAlpha}_active_imported_power_instantaneous_kw'
-            dataDict = {'value': phase['ActiveImportedPowerInstantaneouskW'],'entity_name': entity_name_temp, 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+            dataDict = {'value': phase['ActiveImportedPowerInstantaneouskW'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
             entity_name_temp = f'inverter_phase_{phaseAlpha}_voltage_instantaneous_v'
-            dataDict = {'value': phase['VoltageInstantaneousV'],'entity_name': entity_name_temp, 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+            dataDict = {'value': phase['VoltageInstantaneousV'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
             entity_name_temp = f'inverter_phase_{phaseAlpha}_current_instantaneous_a'
-            dataDict = {'value': phase['CurrentInstantaneousA'],'entity_name': entity_name_temp, 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+            dataDict = {'value': phase['CurrentInstantaneousA'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
             entity_name_temp = f'inverter_phase_{phaseAlpha}_power_factor_instantaneous_minus_1to1'
-            dataDict = {'value': phase['PowerFactorInstantaneousMinus1to1'],'entity_name': entity_name_temp, 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter'}
+            dataDict = {'value': phase['PowerFactorInstantaneousMinus1to1'],'entity_name': entity_name_temp, 'device_id': id_temp, 'device_type': 'inverter'}
             self._redback_entities.append(dataDict)
 
     async def _convert_responses_to_battery_entities(self, data, data2, soc_data) -> None:
         batteryName = 'Unknown'
         batteryId = 1
         cabinetId = 1
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['Id'],'entity_name': 'serial_number', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        id_temp = data['Data']['Nodes'][0]['StaticData']['Id']
+        id_temp = id_temp[-4:] + 'bat'
+        id_temp = id_temp.lower()
+        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['Id'],'entity_name': 'serial_number', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['ModelName'],'entity_name': 'model', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['ModelName'],'entity_name': 'model', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': soc_data['Data']['MinSoC0to1'],'entity_name': 'min_soc_0_to_1', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': soc_data['Data']['MinSoC0to1'],'entity_name': 'min_soc_0_to_1', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': soc_data['Data']['MinOffgridSoC0to1'],'entity_name': 'min_Offgrid_soc_0_to_1', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': soc_data['Data']['MinOffgridSoC0to1'],'entity_name': 'min_Offgrid_soc_0_to_1', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['Location']['Latitude'],'entity_name': 'latitude', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data['Data']['StaticData']['Location']['Latitude'],'entity_name': 'latitude', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['Location']['Longitude'],'entity_name': 'longitude', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data['Data']['StaticData']['Location']['Longitude'],'entity_name': 'longitude', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['BatteryMaxChargePowerkW'],'entity_name': 'battery_max_charge_power_kw', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['BatteryMaxChargePowerkW'],'entity_name': 'battery_max_charge_power_kw', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['BatteryMaxDischargePowerkW'],'entity_name': 'battery_max_discharge_power_kw', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['BatteryMaxDischargePowerkW'],'entity_name': 'battery_max_discharge_power_kw', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['BatteryCapacitykWh'],'entity_name': 'battery_capacity_kwh', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['BatteryCapacitykWh'],'entity_name': 'battery_capacity_kwh', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['UsableBatteryCapacitykWh'],'entity_name': 'battery_usable_capacity_kwh', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['UsableBatteryCapacitykWh'],'entity_name': 'battery_usable_capacity_kwh', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['SystemType'],'entity_name': 'system_type', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data['Data']['StaticData']['SiteDetails']['SystemType'],'entity_name': 'system_type', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['CommissioningDate'],'entity_name': 'commissioning_date', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data['Data']['StaticData']['CommissioningDate'],'entity_name': 'commissioning_date', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['Id'],'entity_name': 'site_id', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data['Data']['StaticData']['Id'],'entity_name': 'site_id', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['StaticData']['Type'],'entity_name': 'inverter_site_type', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data['Data']['StaticData']['Type'],'entity_name': 'inverter_site_type', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['ModelName'],'entity_name': 'model_name', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['ModelName'],'entity_name': 'model_name', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['BatteryCount'],'entity_name': 'battery_count', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['BatteryCount'],'entity_name': 'battery_count', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['SoftwareVersion'],'entity_name': 'software_version', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['SoftwareVersion'],'entity_name': 'software_version', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['FirmwareVersion'],'entity_name': 'firmware_version', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['FirmwareVersion'],'entity_name': 'firmware_version', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['Id'],'entity_name': 'inverter_serial_number', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['Id'],'entity_name': 'inverter_serial_number', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['TimestampUtc'],'entity_name': 'timestamp_utc', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data2['Data']['TimestampUtc'],'entity_name': 'timestamp_utc', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['BatterySoCInstantaneous0to1'],'entity_name': 'battery_soc_instantaneous_0to1', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data2['Data']['BatterySoCInstantaneous0to1'],'entity_name': 'battery_soc_instantaneous_0to1', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['BatteryPowerNegativeIsChargingkW'],'entity_name': 'battery_power_negative_is_charging_kw', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data2['Data']['BatteryPowerNegativeIsChargingkW'],'entity_name': 'battery_power_negative_is_charging_kw', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['BatteryChargeAllTimeEnergykWh'],'entity_name': 'battery_charge_all_time_energy_kwh', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data2['Data']['BatteryChargeAllTimeEnergykWh'],'entity_name': 'battery_charge_all_time_energy_kwh', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['BatteryDischargeAllTimeEnergykWh'],'entity_name': 'battery_discharge_all_time_energy_kwh', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data2['Data']['BatteryDischargeAllTimeEnergykWh'],'entity_name': 'battery_discharge_all_time_energy_kwh', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['Status'],'entity_name': 'status', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data2['Data']['Status'],'entity_name': 'status', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['Battery']['CurrentNegativeIsChargingA'],'entity_name': 'battery_current_negative_in_charging_a', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data2['Data']['Battery']['CurrentNegativeIsChargingA'],'entity_name': 'battery_current_negative_in_charging_a', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['Battery']['VoltageV'],'entity_name': 'battery_voltage_v', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data2['Data']['Battery']['VoltageV'],'entity_name': 'battery_voltage_v', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['Battery']['VoltageType'],'entity_name': 'battery_voltage_type', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data2['Data']['Battery']['VoltageType'],'entity_name': 'battery_voltage_type', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value': data2['Data']['Battery']['NumberOfModules'],'entity_name': 'battery_no_of_modules', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value': data2['Data']['Battery']['NumberOfModules'],'entity_name': 'battery_no_of_modules', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         
-        dataDict = {'value':(data['Data']['StaticData']['SiteDetails']['BatteryCapacitykWh'] * data2['Data']['BatterySoCInstantaneous0to1'] ),'entity_name': 'battery_currently_stored_kwh', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value':(data['Data']['StaticData']['SiteDetails']['BatteryCapacitykWh'] * data2['Data']['BatterySoCInstantaneous0to1'] ),'entity_name': 'battery_currently_stored_kwh', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
-        dataDict = {'value':  round(data['Data']['StaticData']['SiteDetails']['BatteryCapacitykWh'] * (data2['Data']['BatterySoCInstantaneous0to1']- soc_data['Data']['MinSoC0to1']),2),'entity_name': 'battery_currently_usable_kwh', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+        dataDict = {'value':  round(data['Data']['StaticData']['SiteDetails']['BatteryCapacitykWh'] * (data2['Data']['BatterySoCInstantaneous0to1']- soc_data['Data']['MinSoC0to1']),2),'entity_name': 'battery_currently_usable_kwh', 'device_id': id_temp, 'device_type': 'battery'}
         self._redback_entities.append(dataDict)
         for battery in data['Data']['Nodes'][0]['StaticData']['BatteryModels']:
             if battery != 'Unknown':
                 batteryName = battery
-                dataDict = {'value': batteryName,'entity_name': f'battery_{batteryId}_model', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+                dataDict = {'value': batteryName,'entity_name': f'battery_{batteryId}_model', 'device_id': id_temp, 'device_type': 'battery'}
                 self._redback_entities.append(dataDict)
             else:
-                dataDict = {'value': batteryName,'entity_name': f'battery_{batteryId}_model', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+                dataDict = {'value': batteryName,'entity_name': f'battery_{batteryId}_model', 'device_id': id_temp, 'device_type': 'battery'}
                 self._redback_entities.append(dataDict)
             battery_temp_value = data2['Data']['Battery']['Modules'][batteryId-1]['CurrentNegativeIsChargingA']
             battery_temp_name= f'battery_{batteryId}_current_negative_in_charging_a'
-            dataDict = {'value': battery_temp_value,'entity_name': battery_temp_name, 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+            dataDict = {'value': battery_temp_value,'entity_name': battery_temp_name, 'device_id': id_temp, 'device_type': 'battery'}
             self._redback_entities.append(dataDict)
             battery_temp_value = data2['Data']['Battery']['Modules'][batteryId-1]['VoltageV']
             battery_temp_name= f'battery_{batteryId}_voltage_v'
-            dataDict = {'value': battery_temp_value,'entity_name': battery_temp_name, 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+            dataDict = {'value': battery_temp_value,'entity_name': battery_temp_name, 'device_id': id_temp, 'device_type': 'battery'}
             self._redback_entities.append(dataDict)
             battery_temp_value = data2['Data']['Battery']['Modules'][batteryId-1]['VoltageV']
             battery_temp_name= f'battery_{batteryId}_power_negative_is_charging_kw'
-            dataDict = {'value': battery_temp_value,'entity_name': battery_temp_name, 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+            dataDict = {'value': battery_temp_value,'entity_name': battery_temp_name, 'device_id': id_temp, 'device_type': 'battery'}
             self._redback_entities.append(dataDict)
             battery_temp_value = data2['Data']['Battery']['Modules'][batteryId-1]['PowerNegativeIsChargingkW']
             battery_temp_name= f'battery_{batteryId}_soc_0to1'
-            dataDict = {'value': battery_temp_value,'entity_name': battery_temp_name, 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+            dataDict = {'value': battery_temp_value,'entity_name': battery_temp_name, 'device_id': id_temp, 'device_type': 'battery'}
             self._redback_entities.append(dataDict)
             batteryId += 1
         
         for cabinet in data2['Data']['Battery']['Cabinets']:
             cabinet_temp_name = f'battery_cabinet_{cabinetId}_id'
-            dataDict = {'value': cabinet['TemperatureC'],'entity_name': cabinet_temp_name, 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+            dataDict = {'value': cabinet['TemperatureC'],'entity_name': cabinet_temp_name, 'device_id': id_temp, 'device_type': 'battery'}
             self._redback_entities.append(dataDict)
             cabinet_temp_name = f'battery_cabinet_{cabinetId}_fan_state'
-            dataDict = {'value': cabinet['FanState'],'entity_name': cabinet_temp_name, 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery', 'device_type': 'battery'}
+            dataDict = {'value': cabinet['FanState'],'entity_name': cabinet_temp_name, 'device_id': id_temp, 'device_type': 'battery'}
             self._redback_entities.append(dataDict)
             cabinetId += 1
```

### Comparing `redbacktechpy-2024.5.0b4/src/redbacktechpy/str_enum.py` & `redbacktechpy-2024.5.1b1/src/redbacktechpy/str_enum.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.0b4/src/redbacktechpy.egg-info/PKG-INFO` & `redbacktechpy-2024.5.1b1/src/redbacktechpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.0b4
+Version: 2024.5.1b1
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

