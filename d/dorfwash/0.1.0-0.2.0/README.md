# Comparing `tmp/dorfwash-0.1.0.tar.gz` & `tmp/dorfwash-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dorfwash-0.1.0.tar", max compression
+gzip compressed data, was "dorfwash-0.2.0.tar", max compression
```

## Comparing `dorfwash-0.1.0.tar` & `dorfwash-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0    42016 2024-05-25 09:26:25.018817 dorfwash-0.1.0/LICENSE
--rw-r--r--   0        0        0      955 2024-05-31 16:18:55.773633 dorfwash-0.1.0/README.md
--rw-r--r--   0        0        0     3429 2024-05-31 14:31:52.969598 dorfwash-0.1.0/dorfwash/__main__.py
--rw-r--r--   0        0        0      779 2024-05-30 13:05:07.398360 dorfwash-0.1.0/dorfwash/config.py
--rw-r--r--   0        0        0      930 2024-05-30 14:02:29.420160 dorfwash-0.1.0/dorfwash/templates/index.html
--rw-r--r--   0        0        0      794 2024-05-30 13:53:45.509758 dorfwash-0.1.0/dorfwash/templates/index_old.html
--rw-r--r--   0        0        0      520 2024-05-31 16:17:49.875751 dorfwash-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1844 1970-01-01 00:00:00.000000 dorfwash-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    42016 2024-05-25 09:26:25.018817 dorfwash-0.2.0/LICENSE
+-rw-r--r--   0        0        0      956 2024-05-31 16:39:19.170786 dorfwash-0.2.0/README.md
+-rw-r--r--   0        0        0     3716 2024-06-01 16:30:57.073422 dorfwash-0.2.0/dorfwash/__main__.py
+-rw-r--r--   0        0        0      875 2024-06-01 16:22:54.408549 dorfwash-0.2.0/dorfwash/config.py
+-rw-r--r--   0        0        0      930 2024-05-30 14:02:29.420160 dorfwash-0.2.0/dorfwash/templates/index.html
+-rw-r--r--   0        0        0      520 2024-06-01 16:20:12.071722 dorfwash-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1845 1970-01-01 00:00:00.000000 dorfwash-0.2.0/PKG-INFO
```

### Comparing `dorfwash-0.1.0/LICENSE` & `dorfwash-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dorfwash-0.1.0/README.md` & `dorfwash-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 You need to mount a valid `config.json` file at
 `/config/config.json` in the container to run it.
 
 Also, in [docker-compose](docker-compose) is an example `docker-compose.yml`.
 This way, you can just run
 ```bash
-docker-compose up
+docker compose up
 ```
 to build, mount the config, and run the server.
 
 
-## Miele IPProfie API
+## Miele IP Profie API
 
 For further information see [washpy](https://pypi.org/project/washpy/)
```

### Comparing `dorfwash-0.1.0/dorfwash/__main__.py` & `dorfwash-0.2.0/dorfwash/__main__.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,18 +82,27 @@
 
 
 def init_machines(config: DorfwashConfig) -> None:
     """
     fills the global machine table
     """
     for device in config.devices:
-        print(f"initializing machine {device.name}")
-        machines[device.name] = DeviceUser(
-            device.url, device.username, device.password, device.verify_https
-        )
+        print(f'initializing machine "{device.name}"')
+        try:
+            machines[device.name] = DeviceUser(
+                device.url,
+                device.username,
+                device.password,
+                verify_https=device.verify_https,
+                https_timeout=config.https_timeout,
+            )
+        except Exception as e:
+            print(f'skipping machine "{device.name}", an error has occoured: {e}')
+
+    print("done initializing")
 
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument(
         "config", type=argparse.FileType("r"), help="path to the json config file"
     )
```

### Comparing `dorfwash-0.1.0/dorfwash/config.py` & `dorfwash-0.2.0/dorfwash/config.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,11 +34,16 @@
 
 
 class DorfwashConfig(BaseModel):
     """
     holds the configuration for the dorfwash application
     """
 
+    https_timeout: float = 3.05
+    """
+    timeout for HTTPS connections, in seconds.
+    """
+
     devices: List[Device]
     """
     list of all device configs
     """
```

### Comparing `dorfwash-0.1.0/dorfwash/templates/index.html` & `dorfwash-0.2.0/dorfwash/templates/index.html`

 * *Files identical despite different names*

### Comparing `dorfwash-0.1.0/pyproject.toml` & `dorfwash-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "dorfwash"
-version = "0.1.0"
+version = "0.2.0"
 description = "A simple webserver, that lets you monitor your Miele washing machines."
 authors = ["Johann Carl Meyer <info@johannc.de>"]
 license = "LGPL-3.0-only"
 readme = "README.md"
 repository = "https://codeberg.org/johann-cm/dorfwash"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-washpy = "^0.4.0"
+washpy = "^0.5.0"
 flask = "^3.0.3"
 flask-caching = "^2.3.0"
 pydantic = "^2.7.1"
 waitress = "^3.0.0"
 
 
 [build-system]
```

### Comparing `dorfwash-0.1.0/PKG-INFO` & `dorfwash-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dorfwash
-Version: 0.1.0
+Version: 0.2.0
 Summary: A simple webserver, that lets you monitor your Miele washing machines.
 Home-page: https://codeberg.org/johann-cm/dorfwash
 License: LGPL-3.0-only
 Author: Johann Carl Meyer
 Author-email: info@johannc.de
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: flask (>=3.0.3,<4.0.0)
 Requires-Dist: flask-caching (>=2.3.0,<3.0.0)
 Requires-Dist: pydantic (>=2.7.1,<3.0.0)
 Requires-Dist: waitress (>=3.0.0,<4.0.0)
-Requires-Dist: washpy (>=0.4.0,<0.5.0)
+Requires-Dist: washpy (>=0.5.0,<0.6.0)
 Project-URL: Repository, https://codeberg.org/johann-cm/dorfwash
 Description-Content-Type: text/markdown
 
 # dorfwash
 
 `dorfwash` lets you monitor your Miele washing machines
 via the Miele Professional IP Profile API.
@@ -51,16 +51,16 @@
 
 You need to mount a valid `config.json` file at
 `/config/config.json` in the container to run it.
 
 Also, in [docker-compose](docker-compose) is an example `docker-compose.yml`.
 This way, you can just run
 ```bash
-docker-compose up
+docker compose up
 ```
 to build, mount the config, and run the server.
 
 
-## Miele IPProfie API
+## Miele IP Profie API
 
 For further information see [washpy](https://pypi.org/project/washpy/)
```

