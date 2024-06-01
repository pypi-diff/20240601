# Comparing `tmp/viessmann_gridbox_connector-1.3.9.tar.gz` & `tmp/viessmann_gridbox_connector-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viessmann_gridbox_connector-1.3.9.tar", last modified: Sat Jun  1 00:15:31 2024, max compression
+gzip compressed data, was "viessmann_gridbox_connector-1.4.0.tar", last modified: Sat Jun  1 01:20:20 2024, max compression
```

## Comparing `viessmann_gridbox_connector-1.3.9.tar` & `viessmann_gridbox_connector-1.4.0.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:15:31.568275 viessmann_gridbox_connector-1.3.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-06-01 00:15:27.000000 viessmann_gridbox_connector-1.3.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-06-01 00:15:31.568275 viessmann_gridbox_connector-1.3.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2558 2024-06-01 00:15:27.000000 viessmann_gridbox_connector-1.3.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:15:31.568275 viessmann_gridbox_connector-1.3.9/gridbox_connector/
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-06-01 00:15:27.000000 viessmann_gridbox_connector-1.3.9/gridbox_connector/GridboxConnector.py
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-06-01 00:15:27.000000 viessmann_gridbox_connector-1.3.9/gridbox_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 00:15:31.568275 viessmann_gridbox_connector-1.3.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-06-01 00:15:27.000000 viessmann_gridbox_connector-1.3.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 00:15:31.568275 viessmann_gridbox_connector-1.3.9/viessmann_gridbox_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-06-01 00:15:31.000000 viessmann_gridbox_connector-1.3.9/viessmann_gridbox_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-06-01 00:15:31.000000 viessmann_gridbox_connector-1.3.9/viessmann_gridbox_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 00:15:31.000000 viessmann_gridbox_connector-1.3.9/viessmann_gridbox_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 00:15:31.000000 viessmann_gridbox_connector-1.3.9/viessmann_gridbox_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 00:15:31.000000 viessmann_gridbox_connector-1.3.9/viessmann_gridbox_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:20:20.064374 viessmann_gridbox_connector-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-06-01 01:20:16.000000 viessmann_gridbox_connector-1.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-06-01 01:20:20.064374 viessmann_gridbox_connector-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2816 2024-06-01 01:20:16.000000 viessmann_gridbox_connector-1.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 01:20:20.064374 viessmann_gridbox_connector-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-06-01 01:20:16.000000 viessmann_gridbox_connector-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:20:20.064374 viessmann_gridbox_connector-1.4.0/viessmann_gridbox_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)     2814 2024-06-01 01:20:16.000000 viessmann_gridbox_connector-1.4.0/viessmann_gridbox_connector/GridboxConnector.py
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-06-01 01:20:16.000000 viessmann_gridbox_connector-1.4.0/viessmann_gridbox_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-06-01 01:20:16.000000 viessmann_gridbox_connector-1.4.0/viessmann_gridbox_connector/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-06-01 01:20:16.000000 viessmann_gridbox_connector-1.4.0/viessmann_gridbox_connector/config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 01:20:20.064374 viessmann_gridbox_connector-1.4.0/viessmann_gridbox_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2024-06-01 01:20:20.000000 viessmann_gridbox_connector-1.4.0/viessmann_gridbox_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-06-01 01:20:20.000000 viessmann_gridbox_connector-1.4.0/viessmann_gridbox_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 01:20:20.000000 viessmann_gridbox_connector-1.4.0/viessmann_gridbox_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-01 01:20:20.000000 viessmann_gridbox_connector-1.4.0/viessmann_gridbox_connector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 01:20:20.000000 viessmann_gridbox_connector-1.4.0/viessmann_gridbox_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-01 01:20:20.000000 viessmann_gridbox_connector-1.4.0/viessmann_gridbox_connector.egg-info/top_level.txt
```

### Comparing `viessmann_gridbox_connector-1.3.9/LICENSE` & `viessmann_gridbox_connector-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `viessmann_gridbox_connector-1.3.9/PKG-INFO` & `viessmann_gridbox_connector-1.4.0/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,36 +1,56 @@
-Metadata-Version: 2.1
-Name: viessmann-gridbox-connector
-Version: 1.3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: requests
-
 # Viessmann Gridbox Connector
+
 ### **<h3 style="text-align: center;">This is not an official Viessmann library</h3>**
 
-a GridboxConnector Lib to fetch your Data from the Cloud.
-It is using the same Rest-API like the Dashboard and the App.
+Harness the power of your photovoltaic system with the GridboxConnector library. This versatile tool taps into the same REST API as the official dashboard and app, providing you with direct access to your data from the cloud.<br>
+
+Whether you're a developer looking to integrate solar data into your own project, or a power user seeking command-line access, GridboxConnector has you covered. With its dual functionality, you can either embed it into your Python project as a library or use it as a standalone command-line interface (CLI) tool.<br>
+
+**Take control of your solar data with GridboxConnector, and unlock the full potential of your photovoltaic system.**<br><br>
 ![Screenshot vom mygridbox](images/screenshot.png)
 
 ## Installation
+
 ```script shell
 pip install viessmann-gridbox-connector
 ```
-Set your email and password in the config.json. 
-Use your Login Data from the App or from https://mygridbox.viessmann.com/login
 
-### Setup the python environment and install all dependencies
+## Usage
+
+You can use the CLI to retrieve live data from the Viessmann Gridbox API or use the GridboxConnector class in your own code. <br>
+Use your Login data from the App or from https://mygridbox.viessmann.com/login
+
+### CLI
 
 ```script shell
-python -m venv venv
-.\venv\Scripts\activate
-pip install -r requirements.txt
+pip install viessmann-gridbox-connector
+viessmann --username <username> --password <password>
 ```
+
+### in your code
+
+```python
+from viessmann_gridbox_connector import GridboxConnector
+from importlib.resources import path
+import json
+
+with path('viessmann_gridbox_connector', 'config.json') as config_file:
+    with open(config_file, 'r') as file:
+        data = json.load(file)
+        data["login"]["username"] = "username"
+        data["login"]["password"] = "password"
+        connector = GridboxConnector(data)
+        # Retrieve live data
+        live_data = connector.retrieve_live_data()
+        print(live_data)
+```
+
 ### Example Output
+
 ```script json
 {
     "consumption": 496,
     "directConsumption": 413,
     "directConsumptionEV": 0,
     "directConsumptionHeatPump": 0,
     "directConsumptionHeater": 0,
@@ -46,57 +66,24 @@
     "selfConsumptionRate": 1,
     "selfSufficiencyRate": 0.8326612903225806,
     "selfSupply": 413,
     "totalConsumption": 496
 }
 ```
 
-# Usage
-```python
-from gridbox_connector import GridboxConnector
-
-# Initialize the connector with your configuration
-config = {
-  "urls": {
-    "login":"https://gridx.eu.auth0.com/oauth/token",
-    "gateways":"https://api.gridx.de/gateways",
-    "live":"https://api.gridx.de/systems/{}/live"
-  },
-  "login":{
-    "grant_type":"http://auth0.com/oauth/grant-type/password-realm",
-    "username":"email",
-    "password":"password",
-    "audience":"my.gridx",
-    "client_id":"oZpr934Ikn8OZOHTJEcrgXkjio0I0Q7b",
-    "scope":"email openid",
-    "realm":"viessmann-authentication-db"
-  }
-}
-
-connector = GridboxConnector(config)
+## Dependencies
 
-# Retrieve live data
-live_data = connector.retrieve_live_data()
-print(live_data)
+- requests
 
-```
-# Configuration
-You need to provide a configuration dictionary with the following keys:
+## Contributing
 
-urls: Dictionary containing endpoint URLs.
-login: Dictionary containing login credentials.
-
-# Dependencies
-requests
-# Contributing
 If you'd like to contribute to viessmann-gridbox-connector, please follow these steps:
 
 Fork the repository.
 Create a new branch for your feature or bug fix.
 Make your changes and write tests if possible.
 Run tests and ensure they pass.
 Submit a pull request.
 
-
-# License
+## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `viessmann_gridbox_connector-1.3.9/README.md` & `viessmann_gridbox_connector-1.4.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,63 @@
+Metadata-Version: 2.1
+Name: viessmann-gridbox-connector
+Version: 1.4.0
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: requests
+
 # Viessmann Gridbox Connector
+
 ### **<h3 style="text-align: center;">This is not an official Viessmann library</h3>**
 
-a GridboxConnector Lib to fetch your Data from the Cloud.
-It is using the same Rest-API like the Dashboard and the App.
+Harness the power of your photovoltaic system with the GridboxConnector library. This versatile tool taps into the same REST API as the official dashboard and app, providing you with direct access to your data from the cloud.<br>
+
+Whether you're a developer looking to integrate solar data into your own project, or a power user seeking command-line access, GridboxConnector has you covered. With its dual functionality, you can either embed it into your Python project as a library or use it as a standalone command-line interface (CLI) tool.<br>
+
+**Take control of your solar data with GridboxConnector, and unlock the full potential of your photovoltaic system.**<br><br>
 ![Screenshot vom mygridbox](images/screenshot.png)
 
 ## Installation
+
 ```script shell
 pip install viessmann-gridbox-connector
 ```
-Set your email and password in the config.json. 
-Use your Login Data from the App or from https://mygridbox.viessmann.com/login
 
-### Setup the python environment and install all dependencies
+## Usage
+
+You can use the CLI to retrieve live data from the Viessmann Gridbox API or use the GridboxConnector class in your own code. <br>
+Use your Login data from the App or from https://mygridbox.viessmann.com/login
+
+### CLI
 
 ```script shell
-python -m venv venv
-.\venv\Scripts\activate
-pip install -r requirements.txt
+pip install viessmann-gridbox-connector
+viessmann --username <username> --password <password>
 ```
+
+### in your code
+
+```python
+from viessmann_gridbox_connector import GridboxConnector
+from importlib.resources import path
+import json
+
+with path('viessmann_gridbox_connector', 'config.json') as config_file:
+    with open(config_file, 'r') as file:
+        data = json.load(file)
+        data["login"]["username"] = "username"
+        data["login"]["password"] = "password"
+        connector = GridboxConnector(data)
+        # Retrieve live data
+        live_data = connector.retrieve_live_data()
+        print(live_data)
+```
+
 ### Example Output
+
 ```script json
 {
     "consumption": 496,
     "directConsumption": 413,
     "directConsumptionEV": 0,
     "directConsumptionHeatPump": 0,
     "directConsumptionHeater": 0,
@@ -39,57 +73,24 @@
     "selfConsumptionRate": 1,
     "selfSufficiencyRate": 0.8326612903225806,
     "selfSupply": 413,
     "totalConsumption": 496
 }
 ```
 
-# Usage
-```python
-from gridbox_connector import GridboxConnector
-
-# Initialize the connector with your configuration
-config = {
-  "urls": {
-    "login":"https://gridx.eu.auth0.com/oauth/token",
-    "gateways":"https://api.gridx.de/gateways",
-    "live":"https://api.gridx.de/systems/{}/live"
-  },
-  "login":{
-    "grant_type":"http://auth0.com/oauth/grant-type/password-realm",
-    "username":"email",
-    "password":"password",
-    "audience":"my.gridx",
-    "client_id":"oZpr934Ikn8OZOHTJEcrgXkjio0I0Q7b",
-    "scope":"email openid",
-    "realm":"viessmann-authentication-db"
-  }
-}
-
-connector = GridboxConnector(config)
+## Dependencies
 
-# Retrieve live data
-live_data = connector.retrieve_live_data()
-print(live_data)
+- requests
 
-```
-# Configuration
-You need to provide a configuration dictionary with the following keys:
+## Contributing
 
-urls: Dictionary containing endpoint URLs.
-login: Dictionary containing login credentials.
-
-# Dependencies
-requests
-# Contributing
 If you'd like to contribute to viessmann-gridbox-connector, please follow these steps:
 
 Fork the repository.
 Create a new branch for your feature or bug fix.
 Make your changes and write tests if possible.
 Run tests and ensure they pass.
 Submit a pull request.
 
-
-# License
+## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
```

### Comparing `viessmann_gridbox_connector-1.3.9/gridbox_connector/GridboxConnector.py` & `viessmann_gridbox_connector-1.4.0/viessmann_gridbox_connector/GridboxConnector.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         self.login_body = config["login"]
         self.gateway_url = config["urls"]["gateways"]
         self.live_url = config["urls"]["live"]
         self.init_auth()
 
     def init_logging(self):
         self.logger = logging.getLogger(__name__)
-        loglevel = os.getenv('LOGLEVEL', 'DEBUG')  # Default to DEBUG if LOGLEVEL is not set
+        loglevel = os.getenv('LOG_LEVEL', 'DEBUG')  # Default to DEBUG if LOGLEVEL is not set
         self.logger.setLevel(logging.getLevelName(loglevel))
         formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(funcName)s - %(message)s')
         console_handler = logging.StreamHandler()
         console_handler.setFormatter(formatter)
         self.logger.addHandler(console_handler)
```

### Comparing `viessmann_gridbox_connector-1.3.9/viessmann_gridbox_connector.egg-info/PKG-INFO` & `viessmann_gridbox_connector-1.4.0/viessmann_gridbox_connector.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,36 +1,63 @@
 Metadata-Version: 2.1
 Name: viessmann-gridbox-connector
-Version: 1.3.9
+Version: 1.4.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # Viessmann Gridbox Connector
+
 ### **<h3 style="text-align: center;">This is not an official Viessmann library</h3>**
 
-a GridboxConnector Lib to fetch your Data from the Cloud.
-It is using the same Rest-API like the Dashboard and the App.
+Harness the power of your photovoltaic system with the GridboxConnector library. This versatile tool taps into the same REST API as the official dashboard and app, providing you with direct access to your data from the cloud.<br>
+
+Whether you're a developer looking to integrate solar data into your own project, or a power user seeking command-line access, GridboxConnector has you covered. With its dual functionality, you can either embed it into your Python project as a library or use it as a standalone command-line interface (CLI) tool.<br>
+
+**Take control of your solar data with GridboxConnector, and unlock the full potential of your photovoltaic system.**<br><br>
 ![Screenshot vom mygridbox](images/screenshot.png)
 
 ## Installation
+
 ```script shell
 pip install viessmann-gridbox-connector
 ```
-Set your email and password in the config.json. 
-Use your Login Data from the App or from https://mygridbox.viessmann.com/login
 
-### Setup the python environment and install all dependencies
+## Usage
+
+You can use the CLI to retrieve live data from the Viessmann Gridbox API or use the GridboxConnector class in your own code. <br>
+Use your Login data from the App or from https://mygridbox.viessmann.com/login
+
+### CLI
 
 ```script shell
-python -m venv venv
-.\venv\Scripts\activate
-pip install -r requirements.txt
+pip install viessmann-gridbox-connector
+viessmann --username <username> --password <password>
+```
+
+### in your code
+
+```python
+from viessmann_gridbox_connector import GridboxConnector
+from importlib.resources import path
+import json
+
+with path('viessmann_gridbox_connector', 'config.json') as config_file:
+    with open(config_file, 'r') as file:
+        data = json.load(file)
+        data["login"]["username"] = "username"
+        data["login"]["password"] = "password"
+        connector = GridboxConnector(data)
+        # Retrieve live data
+        live_data = connector.retrieve_live_data()
+        print(live_data)
 ```
+
 ### Example Output
+
 ```script json
 {
     "consumption": 496,
     "directConsumption": 413,
     "directConsumptionEV": 0,
     "directConsumptionHeatPump": 0,
     "directConsumptionHeater": 0,
@@ -46,57 +73,24 @@
     "selfConsumptionRate": 1,
     "selfSufficiencyRate": 0.8326612903225806,
     "selfSupply": 413,
     "totalConsumption": 496
 }
 ```
 
-# Usage
-```python
-from gridbox_connector import GridboxConnector
-
-# Initialize the connector with your configuration
-config = {
-  "urls": {
-    "login":"https://gridx.eu.auth0.com/oauth/token",
-    "gateways":"https://api.gridx.de/gateways",
-    "live":"https://api.gridx.de/systems/{}/live"
-  },
-  "login":{
-    "grant_type":"http://auth0.com/oauth/grant-type/password-realm",
-    "username":"email",
-    "password":"password",
-    "audience":"my.gridx",
-    "client_id":"oZpr934Ikn8OZOHTJEcrgXkjio0I0Q7b",
-    "scope":"email openid",
-    "realm":"viessmann-authentication-db"
-  }
-}
-
-connector = GridboxConnector(config)
+## Dependencies
 
-# Retrieve live data
-live_data = connector.retrieve_live_data()
-print(live_data)
+- requests
 
-```
-# Configuration
-You need to provide a configuration dictionary with the following keys:
+## Contributing
 
-urls: Dictionary containing endpoint URLs.
-login: Dictionary containing login credentials.
-
-# Dependencies
-requests
-# Contributing
 If you'd like to contribute to viessmann-gridbox-connector, please follow these steps:
 
 Fork the repository.
 Create a new branch for your feature or bug fix.
 Make your changes and write tests if possible.
 Run tests and ensure they pass.
 Submit a pull request.
 
-
-# License
+## License
 
 This project is licensed under the MIT License - see the LICENSE file for details.
```

