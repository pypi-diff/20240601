# Comparing `tmp/redbacktechpy-2024.5.0b3.tar.gz` & `tmp/redbacktechpy-2024.5.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbacktechpy-2024.5.0b3.tar", last modified: Fri May 31 22:33:06 2024, max compression
+gzip compressed data, was "redbacktechpy-2024.5.0b4.tar", last modified: Sat Jun  1 00:40:44 2024, max compression
```

## Comparing `redbacktechpy-2024.5.0b3.tar` & `redbacktechpy-2024.5.0b4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:33:06.195505 redbacktechpy-2024.5.0b3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-31 22:33:01.000000 redbacktechpy-2024.5.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-31 22:33:06.195505 redbacktechpy-2024.5.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-31 22:33:01.000000 redbacktechpy-2024.5.0b3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 22:33:06.195505 redbacktechpy-2024.5.0b3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:33:06.191505 redbacktechpy-2024.5.0b3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:33:06.195505 redbacktechpy-2024.5.0b3/src/redbacktechpy/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-05-31 22:33:01.000000 redbacktechpy-2024.5.0b3/src/redbacktechpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2149 2024-05-31 22:33:01.000000 redbacktechpy-2024.5.0b3/src/redbacktechpy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-31 22:33:01.000000 redbacktechpy-2024.5.0b3/src/redbacktechpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-31 22:33:01.000000 redbacktechpy-2024.5.0b3/src/redbacktechpy/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    51345 2024-05-31 22:33:01.000000 redbacktechpy-2024.5.0b3/src/redbacktechpy/redbacktech_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-31 22:33:01.000000 redbacktechpy-2024.5.0b3/src/redbacktechpy/str_enum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 22:33:06.195505 redbacktechpy-2024.5.0b3/src/redbacktechpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-31 22:33:06.000000 redbacktechpy-2024.5.0b3/src/redbacktechpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-31 22:33:06.000000 redbacktechpy-2024.5.0b3/src/redbacktechpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 22:33:06.000000 redbacktechpy-2024.5.0b3/src/redbacktechpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-31 22:33:06.000000 redbacktechpy-2024.5.0b3/src/redbacktechpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-31 22:33:06.000000 redbacktechpy-2024.5.0b3/src/redbacktechpy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:40:44.642201 redbacktechpy-2024.5.0b4/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-06-01 00:40:40.000000 redbacktechpy-2024.5.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 00:40:44.642201 redbacktechpy-2024.5.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-06-01 00:40:40.000000 redbacktechpy-2024.5.0b4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 00:40:44.642201 redbacktechpy-2024.5.0b4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:40:44.638201 redbacktechpy-2024.5.0b4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:40:44.638201 redbacktechpy-2024.5.0b4/src/redbacktechpy/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-06-01 00:40:40.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-06-01 00:40:40.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-06-01 00:40:40.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-06-01 00:40:40.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54403 2024-06-01 00:40:40.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy/redbacktech_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-06-01 00:40:40.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy/str_enum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:40:44.642201 redbacktechpy-2024.5.0b4/src/redbacktechpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-06-01 00:40:44.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-06-01 00:40:44.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:40:44.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-06-01 00:40:44.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 00:40:44.000000 redbacktechpy-2024.5.0b4/src/redbacktechpy.egg-info/top_level.txt
```

### Comparing `redbacktechpy-2024.5.0b3/LICENSE` & `redbacktechpy-2024.5.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.0b3/PKG-INFO` & `redbacktechpy-2024.5.0b4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.0b3
+Version: 2024.5.0b4
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

### Comparing `redbacktechpy-2024.5.0b3/pyproject.toml` & `redbacktechpy-2024.5.0b4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "redbacktechpy"
-version = "2024.05.0b3"
+version = "2024.05.0b4"
 authors = [
   { name="Chris Abberley", email="unlisted@gmail.com" },
 ]
 description = "Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE.txt"}
```

### Comparing `redbacktechpy-2024.5.0b3/src/redbacktechpy/__init__.py` & `redbacktechpy-2024.5.0b4/src/redbacktechpy/__init__.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.0b3/src/redbacktechpy/constants.py` & `redbacktechpy-2024.5.0b4/src/redbacktechpy/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,17 @@
     API_STATIC = 'Api/v2/EnergyData/{self.siteId}/Static'
     API_STATIC_MULTIPLE_BY_SERIAL = 'Api/v2/Configuration/Multiple/BySerialNumber/Configuration'
     API_CONFIG_BY_SERIAL = 'Api/v2/Configuration/Configuration/BySerialNumber/'
     API_STATIC_BY_SERIAL = 'Api/v2/EnergyData/Static/BySerialNumber/'
     API_ENERGY_DYNAMIC_MULTIPLE_BY_SERIAL = 'Api/v2.21/EnergyData/Multiple/BySerialNumber/Dynamic'
     API_ENERGY_DYNAMIC_BY_SERIAL = 'Api/v2.21/EnergyData/Dynamic/BySerialNumber/'
     API_ENERGY_DYNAMIC_BY_SITE = 'Api/v2.21/EnergyData/{self.siteId}/Dynamic'
+    API_SCHEDULE_CREATE = 'Api/v2/Schedule/Create/By/SerialNumber'  
+    API_SCHEDULE_DELETE = 'Api/v2/Schedule/Delete/By/SerialNumber/'  #{serialNumber}/{scheduleId}
+    API_SCHEDULE_GET = '/Api/v2/Schedule/By/SerialNumber/' #{serialNumber}
     PORTAL_LOGIN = 'Account/Login'
     PORTAL_CONFIGURE = 'productcontrol/Configure?serialNumber='
     PORTAL_INVERTER_SET = 'productcontrol/Index'
     PORTAL_LOGOFF = 'Account/LogOff/'
     PORTAL_DETAILS = 'productcontrol/Details?serialNumber='
```

### Comparing `redbacktechpy-2024.5.0b3/src/redbacktechpy/model.py` & `redbacktechpy-2024.5.0b4/src/redbacktechpy/model.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 class RedbackTechData:
     """Dataclass for all RedbackTech Data."""
 
     user_id: str
     inverters: Optional[dict[int, Any]] = None
     batterys: Optional[dict[int, Any]] = None
     entities: Optional[dict[int, Any]] = None
+    devices: Optional[dict[int, Any]] = None
 
 @dataclass
 class Site:
     """Dataclass for Redback Sites."""
 
     id: str
     data: dict[str, Any]
@@ -48,11 +49,13 @@
     data: dict[str, Any]
     type: str
 
 @dataclass
 class DeviceInfo:
     """Dataclass for Device Info."""
 
-    id: str
-    device_serial_number: str
-    data: dict[str, Any]
-    type: str
+    identifiers: str
+    name: str
+    model: str
+    sw_version: str
+    hw_version: str
+    serial_number: str
```

### Comparing `redbacktechpy-2024.5.0b3/src/redbacktechpy/redbacktech_client.py` & `redbacktechpy-2024.5.0b4/src/redbacktechpy/redbacktech_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 )
 
 from .model import (
     Inverters,
     Batterys,
     RedbackTechData,
     RedbackEntitys,
+    DeviceInfo,
 )
 from .exceptions import (
         AuthError, 
         RedbackTechClientError,
 )
 
 LOGGER = logging.getLogger(__name__)
@@ -47,43 +48,51 @@
         self.token_expiration: datetime | None = None
         self._GAFToken: str | None = None
         self._device_info_refresh_time: datetime | None = None
         self._flatInverters = []
         self._flatBatterys = []
         self._redback_devices = []
         self._redback_entities = []
+        self._redback_device_info = []
     
     async def get_redback_data(self):
         """Get Redback Data."""
         #Check if we need to get a new device list
         await self.create_device_info()
         
         inverter_data: dict[str, Inverters] = {}
         battery_data: dict[str, Batterys] = {}
         entity_data: dict[str, RedbackEntitys] = {}
+        device_info_data: dict[str, DeviceInfo] = {}
         
         #if self._redback_devices is not None:
         #    for device in self._redback_devices:
         #        if device['device_type'] == 'inverter':
         #            in_instance, in_id = await self._handle_inverter(device)
         #            inverter_data[in_id] = in_instance
-        #            
+                    
         #        if device['device_type'] == 'battery':
         #            bat_instance, bat_id = await self._handle_battery(device)
         #            battery_data[bat_id] = bat_instance
         if self._redback_entities is not None:
             for entity in self._redback_entities:
                 ent_instance, ent_id = await self._handle_entity(entity)
                 entity_data[ent_id] = ent_instance            
         
+        if self._redback_device_info is not None:
+            for device in self._redback_device_info:
+                device_instance, dev_id = await self._handle_device_info(device)
+                device_info_data[dev_id] = device_instance
+        
         return RedbackTechData(
             user_id = self.client_id,
             inverters = inverter_data,
             batterys = battery_data,
-            entities = entity_data
+            entities = entity_data,
+            devices = device_info_data
         )
         
     async def api_login(self) -> None:
         """Login to Redback API and obtain token."""
         login_url = f'{BaseUrl.API}{Endpoint.API_AUTH}'
 
         headers = {
@@ -127,14 +136,33 @@
         """Test Portal connection."""
         self._GAFToken = None
         await self.portal_login()
         if self._GAFToken is not None:
             return True 
         return False
 
+    async def set_inverter_schedule(self, serial_number: str, start_time: str, duration, inverter_mode, power_w) :
+        """Set inverter schedule."""
+        self.serial_number = serial_number
+        self.mode = inverter_mode
+        self.power = power_w
+        self.duration = duration
+        self.start_time = start_time
+        
+        self._check_token()
+        ### convert duration to format
+        days = int(duration/1440)
+        if days < 0:
+            days = 0
+        hours = int(duration/60)
+        minutes = int(duration - (hours * 60))
+        duration_str = f'{days}.{hours:2}:{minutes:2}'
+        
+        return
+
     async def set_inverter_mode(self, serial_number: str, mode: str, power: int, ross_version: str) -> dict[str, Any]:
         """Set inverter mode."""
         self.serial_number = serial_number
         self.mode = mode
         self.power = power
         self.ross_version = ross_version
         
@@ -270,20 +298,22 @@
         
         for serial_number in self._serial_numbers:
             response1 = await self.get_static_by_serial(serial_number)
             response2 = await self.get_dynamic_by_serial(serial_number)
             #self._flatInverters = await self._convert_static_by_serial_to_inverter_list(response1, response2)
             #self._redback_devices.append(self._flatInverters)  ###
             await self._convert_responses_to_inverter_entities(response1, response2)
+            await self._create_device_info_inverter(response1)
             #print(self._flatInverters['serial_number'])
             #response = await self.create_dynamic_info()
             if response1['Data']['Nodes'][0]['StaticData']['BatteryCount'] > 0:
                 soc_data = await self.get_config_by_serial(response1['Data']['Nodes'][0]['StaticData']['Id'])
                 #self._flatBatterys = await self._convert_static_by_serial_to_battery_list(response1, response2, soc_data)
                 await self._convert_responses_to_battery_entities(response1, response2, soc_data)
+                await self._create_device_info_battery(response1)
             #self._redback_devices.append(self._flatBatterys)
         self._device_info_refresh_time = datetime.now() + timedelta(seconds=DEVICEINFOREFRESH)
         return 
     
     async def create_dynamic_info(self) -> None:
 
         self._serial_numbers = await self.get_inverter_list()
@@ -410,14 +440,32 @@
         dataDict['battery_voltage_v'] = data2['Data']['Battery']['VoltageV']
         dataDict['battery_voltage_type'] = data2['Data']['Battery']['VoltageType']
         dataDict['battery_no_of_modules'] = data2['Data']['Battery']['NumberOfModules']
         
         dataDict['battery_currently_stored_kwh'] = (data['Data']['StaticData']['SiteDetails']['BatteryCapacitykWh'] * data2['Data']['BatterySoCInstantaneous0to1'] )
         dataDict['battery_currently_usable_kwh'] = round(data['Data']['StaticData']['SiteDetails']['BatteryCapacitykWh'] * (data2['Data']['BatterySoCInstantaneous0to1']- soc_data['Data']['MinSoC0to1']),2)
         return dataDict
+    
+    
+    async def _handle_device_info(self, device: dict[str, Any]) -> (DeviceInfo, str):
+        """Handle device info data."""
+        
+        #data = {
+        #    'id': device['serial_number'] + device['device_type']
+        #}
+        
+        device_instance = DeviceInfo(
+            identifiers=device['identifiers'],
+            name=device['name'],
+            model=device['model'],
+            sw_version=device['sw_version'],
+            hw_version=device['hw_version'],
+            serial_number=device['serial_number'],
+        )
+        return device_instance, device['identifiers']
         
     async def _handle_inverter(self, device: dict[str, Any]) -> (Inverters, str):
         """Handle inverter data."""
         
         device_type: str = device['device_type'].lower()
 
         data = {
@@ -569,14 +617,36 @@
         try:
             response: dict[str, Any] = await resp.text()
         except Exception as error:
             raise RedbackTechClientError(f'Could not return text {error}') from error
 
         return response
 
+    async def _create_device_info_inverter(self, data) -> None:
+        dataDict = {
+            'identifiers': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter',
+            'name': data['Data']['Nodes'][0]['StaticData']['ModelName'] + ' - inverter',
+            'model': data['Data']['Nodes'][0]['StaticData']['ModelName'],
+            'sw_version': data['Data']['Nodes'][0]['StaticData']['SoftwareVersion'],
+            'hw_version': data['Data']['Nodes'][0]['StaticData']['FirmwareVersion'],
+            'serial_number': data['Data']['Nodes'][0]['StaticData']['Id'],
+        }
+        self._redback_device_info.append(dataDict)
+    
+    async def _create_device_info_battery(self, data) -> None:
+        dataDict = {
+            'identifiers': data['Data']['Nodes'][0]['StaticData']['Id'] + 'battery',
+            'name': data['Data']['Nodes'][0]['StaticData']['ModelName'] + ' - battery',
+            'model': data['Data']['Nodes'][0]['StaticData']['ModelName'],
+            'sw_version': data['Data']['Nodes'][0]['StaticData']['SoftwareVersion'],
+            'hw_version': data['Data']['Nodes'][0]['StaticData']['FirmwareVersion'],
+            'serial_number': data['Data']['Nodes'][0]['StaticData']['Id'],
+        }
+        self._redback_device_info.append(dataDict)
+
     async def _convert_responses_to_inverter_entities(self, data, data2) -> None:
         """Convert responses to entities."""
         pvId =1
         #entity_name
         dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['ModelName'], 'entity_name': 'model_name', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter', 'type_set': 'sensor.string' }
         self._redback_entities.append(dataDict)
         dataDict = {'value': data['Data']['Nodes'][0]['StaticData']['Id'], 'entity_name': 'serial_number', 'device_id': data['Data']['Nodes'][0]['StaticData']['Id'] + 'inverter', 'device_type': 'inverter', 'type_set': 'sensor.string' }
```

### Comparing `redbacktechpy-2024.5.0b3/src/redbacktechpy/str_enum.py` & `redbacktechpy-2024.5.0b4/src/redbacktechpy/str_enum.py`

 * *Files identical despite different names*

### Comparing `redbacktechpy-2024.5.0b3/src/redbacktechpy.egg-info/PKG-INFO` & `redbacktechpy-2024.5.0b4/src/redbacktechpy.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbacktechpy
-Version: 2024.5.0b3
+Version: 2024.5.0b4
 Summary: Python Module to support Home Asssistant integration with Redback Technologies Smart Hybrid Inverter
 Author-email: Chris Abberley <unlisted@gmail.com>
 Project-URL: Homepage, https://github.com/cabberley/redbacktechpy
 Project-URL: Issues, https://github.com/cabberley/redbacktechpy/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
```

