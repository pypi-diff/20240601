# Comparing `tmp/stashconnect-0.7.6.tar.gz` & `tmp/stashconnect-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stashconnect-0.7.6.tar", last modified: Fri May 31 20:43:26 2024, max compression
+gzip compressed data, was "stashconnect-0.7.7.tar", last modified: Sat Jun  1 15:08:41 2024, max compression
```

## Comparing `stashconnect-0.7.6.tar` & `stashconnect-0.7.7.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 20:43:26.636630 stashconnect-0.7.6/
--rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.7.6/LICENSE
--rw-rw-rw-   0        0        0     1728 2024-05-31 20:43:26.633619 stashconnect-0.7.6/PKG-INFO
--rw-rw-rw-   0        0        0      693 2024-05-31 07:27:08.000000 stashconnect-0.7.6/README.md
--rw-rw-rw-   0        0        0       42 2024-05-31 20:43:26.637129 stashconnect-0.7.6/setup.cfg
--rw-rw-rw-   0        0        0     1380 2024-05-31 20:41:53.000000 stashconnect-0.7.6/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-31 20:43:26.612070 stashconnect-0.7.6/stashconnect/
--rw-rw-rw-   0        0        0      216 2024-05-31 20:41:35.000000 stashconnect-0.7.6/stashconnect/__init__.py
--rw-rw-rw-   0        0        0    17257 2024-05-10 18:47:16.000000 stashconnect-0.7.6/stashconnect/channels.py
--rw-rw-rw-   0        0        0     9246 2024-05-31 20:41:47.000000 stashconnect-0.7.6/stashconnect/client.py
--rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.7.6/stashconnect/companies.py
--rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.7.6/stashconnect/conversations.py
--rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.7.6/stashconnect/crypto_utils.py
--rw-rw-rw-   0        0        0    12358 2024-05-31 20:31:12.000000 stashconnect-0.7.6/stashconnect/files.py
--rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.7.6/stashconnect/messages.py
--rw-rw-rw-   0        0        0    17343 2024-05-11 08:24:59.000000 stashconnect-0.7.6/stashconnect/models.py
--rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.7.6/stashconnect/settings.py
--rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.7.6/stashconnect/tools.py
--rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.7.6/stashconnect/users.py
-drwxrwxrwx   0        0        0        0 2024-05-31 20:43:26.630619 stashconnect-0.7.6/stashconnect.egg-info/
--rw-rw-rw-   0        0        0     1728 2024-05-31 20:43:26.000000 stashconnect-0.7.6/stashconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2024-05-31 20:43:26.000000 stashconnect-0.7.6/stashconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 20:43:26.000000 stashconnect-0.7.6/stashconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-05-31 20:43:26.000000 stashconnect-0.7.6/stashconnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-31 20:43:26.000000 stashconnect-0.7.6/stashconnect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 15:08:41.511074 stashconnect-0.7.7/
+-rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.7.7/LICENSE
+-rw-rw-rw-   0        0        0     2263 2024-06-01 15:08:41.507543 stashconnect-0.7.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1230 2024-06-01 14:22:32.000000 stashconnect-0.7.7/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 15:08:41.511573 stashconnect-0.7.7/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2024-06-01 15:05:19.000000 stashconnect-0.7.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:08:41.481307 stashconnect-0.7.7/stashconnect/
+-rw-rw-rw-   0        0        0      216 2024-06-01 15:03:31.000000 stashconnect-0.7.7/stashconnect/__init__.py
+-rw-rw-rw-   0        0        0    17257 2024-05-10 18:47:16.000000 stashconnect-0.7.7/stashconnect/channels.py
+-rw-rw-rw-   0        0        0     9403 2024-06-01 14:58:25.000000 stashconnect-0.7.7/stashconnect/client.py
+-rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.7.7/stashconnect/companies.py
+-rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.7.7/stashconnect/conversations.py
+-rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.7.7/stashconnect/crypto_utils.py
+-rw-rw-rw-   0        0        0    12503 2024-06-01 14:56:25.000000 stashconnect-0.7.7/stashconnect/files.py
+-rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.7.7/stashconnect/messages.py
+-rw-rw-rw-   0        0        0    17343 2024-05-11 08:24:59.000000 stashconnect-0.7.7/stashconnect/models.py
+-rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.7.7/stashconnect/settings.py
+-rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.7.7/stashconnect/tools.py
+-rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.7.7/stashconnect/users.py
+drwxrwxrwx   0        0        0        0 2024-06-01 15:08:41.502778 stashconnect-0.7.7/stashconnect.egg-info/
+-rw-rw-rw-   0        0        0     2263 2024-06-01 15:08:41.000000 stashconnect-0.7.7/stashconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2024-06-01 15:08:41.000000 stashconnect-0.7.7/stashconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 15:08:41.000000 stashconnect-0.7.7/stashconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-06-01 15:08:41.000000 stashconnect-0.7.7/stashconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-01 15:08:41.000000 stashconnect-0.7.7/stashconnect.egg-info/top_level.txt
```

### Comparing `stashconnect-0.7.6/LICENSE` & `stashconnect-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.6/PKG-INFO` & `stashconnect-0.7.7/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.7.6
+Version: 0.7.7
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
@@ -19,28 +19,53 @@
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: pycryptodome
 Requires-Dist: python-socketio
 Requires-Dist: Pillow
 Requires-Dist: websocket-client
 
-# <img src="https://raw.githubusercontent.com/BuStudios/StashConnect/main/assets/icon.png" height="22"> StashConnect
+# StashConnect
+
+StashConnect is an easy-to-use API wrapper for [stashcat](https://stashcat.com/) and [schul.cloud](https://schul.cloud).
+
+![PyPI - Downloads](https://img.shields.io/pypi/dm/stashconnect?labelColor=345165&color=4793c9)
+![PyPI - Version](https://img.shields.io/pypi/v/stashconnect?label=version&labelColor=345165&color=4793c9)
+![PyPI - Status](https://img.shields.io/pypi/status/stashconnect?labelColor=345165&color=44af68)
+
+## Installation
+
+To install StashConnect, use pip in your shell:
 
-An API wrapper for [stashcat](https://stashcat.com/) and [schul.cloud](https://schul.cloud).<br>
 ```bash
-pip install stashconnect
+pip install -U stashconnect
 ```
 
-## Contributors
-- All code made by [BuStudios](https://github.com/bustudios)
-- Create a pull request to contribute code yourself
+## Example Usage
+
+```python
+import stashconnect
+
+client = stashconnect.Client(
+    email="your email", password="you password",
+    encryption_password="you enc password",
+)
+
+client.users.change_status("new status")
+```
+
+## Features to be added
 
-## Version 0.7.5
-#### To be added:
 - [x] fix links
+- [ ] file functions
 - [ ] returnable file object
-- [ ] bot file for easy bot setup
+- [ ] bot method
+
+## Contributors
+
+- All code made by [BuStudios](https://github.com/bustudios)
+- Create a pull request to contribute code yourself
 
 ---
+
 StashConnect is not affiliated with Stashcat GmbH or any of its affiliates.
 
 <img src="https://raw.githubusercontent.com/BuStudios/StashConnect/main/assets/icon-full.png">
```

### Comparing `stashconnect-0.7.6/setup.py` & `stashconnect-0.7.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from setuptools import setup, find_packages
+from stashconnect import __version__
 
-VERSION = "0.7.6"
+VERSION = __version__
 DESCRIPTION = "An API wrapper for stashcat and schul.cloud."
 
 setup(
     name="stashconnect",
     version=VERSION,
     author="BuStudios",
     author_email="support@bustudios.org",
```

### Comparing `stashconnect-0.7.6/stashconnect/channels.py` & `stashconnect-0.7.7/stashconnect/channels.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.6/stashconnect/client.py` & `stashconnect-0.7.7/stashconnect/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,17 +10,18 @@
 from .crypto_utils import CryptoUtils
 from .conversations import ConversationManager
 from .companies import CompanyManager
 from .channels import ChannelManager
 from .files import FileManager
 
 from .tools import Tools
-
 from .models import Message
 
+from . import __version__
+
 headers = {
     "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/123.0.0.0 Safari/537.36",
     "Accept": "application/json, text/plain, */*",
     "Accept-Language": "en",
     "Cache-Control": "no-cache",
     "Accept-Encoding": "gzip, deflate, br",
     "Connection": "keep-alive",
@@ -39,15 +40,23 @@
         .socket_id (str): The ID for the websocket connection.
         .user_id (str): The unique ID of the connected user's account.
         .image_url (str): URL to the user's profile image.
         .first_name (str): User's first name.
         .last_name (str): User's last name.
     """
 
-    def __init__(self, *, email, password, encryption_password=None, device_id=None, app_name=None):
+    def __init__(
+        self,
+        *,
+        email,
+        password,
+        encryption_password=None,
+        device_id=None,
+        app_name=None,
+    ):
 
         self.messages = MessageManager(self)
         self.tools = Tools(self)
         self.settings = Settings(self)
         self.users = UserManager(self)
         self.files = FileManager(self)
         self.conversations = ConversationManager(self)
@@ -55,15 +64,17 @@
         self.channels = ChannelManager(self)
 
         self.email = email
         self.password = password
         self.encryption_password = encryption_password
 
         self.device_id = "stashconnect" if device_id is None else device_id
-        self.app_name = "stashconnect v.0.7.6" if app_name is None else app_name
+        self.app_name = (
+            f"stashconnect v.{__version__}" if app_name is None else app_name
+        )
 
         self._main_url = "https://api.stashcat.com/"
         self._push_url = "https://push.stashcat.com/"
 
         self._headers = headers
         self._session = requests.Session()
         self._session.headers.update(self._headers)
@@ -275,15 +286,17 @@
     def ws_latency(self, target):
         target_type = self.tools.get_type(target)
 
         start_time = time.perf_counter()
         self._end_time = None
         self._ping_target = target
 
-        self.sio.emit("started-typing", (self.device_id, self.client_key, target_type, target))
+        self.sio.emit(
+            "started-typing", (self.device_id, self.client_key, target_type, target)
+        )
 
         time.sleep(2)
 
         if self._end_time is None:
             self._latency_ws = None
             return "[Error]"
         else:
```

### Comparing `stashconnect-0.7.6/stashconnect/companies.py` & `stashconnect-0.7.7/stashconnect/companies.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.6/stashconnect/conversations.py` & `stashconnect-0.7.7/stashconnect/conversations.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.6/stashconnect/crypto_utils.py` & `stashconnect-0.7.7/stashconnect/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.6/stashconnect/files.py` & `stashconnect-0.7.7/stashconnect/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,16 +130,20 @@
                     file_key, self.client.get_conversation_key(target, target_type), iv
                 ).hex(),
                 "iv": iv.hex(),
             }
 
             response = self.client._post("security/set_file_access_key", data=data)
 
+        self.client.files.store_preview_image(file_id, filepath)
+
+        return file
+
+    def store_preview_image(self, file_id: str | int, filepath: str):
         try:
-            # upload a thumbnail image if the file is a image
             with Image.open(filepath) as image:
                 output_size = 100
 
                 image = image.convert("RGB")
                 min_dimension = min(image.width, image.height)
                 scale_factor = output_size / min_dimension
 
@@ -159,20 +163,19 @@
                 image_base64 = base64.b64encode(buffered.getvalue()).decode("utf-8")
 
             data = {
                 "file_id": file_id,
                 "content": str("data:image/jpeg;base64," + image_base64),
             }
 
-            self.client._post("file/storePreviewImage", data=data)
+            response = self.client._post("file/storePreviewImage", data=data)
+            return response["file"]
 
         except Exception:
-            pass
-
-        return file
+            return {"success": False}
 
     def download(self, id: str | int, directory: str = "") -> str:
         """Downloads a file to a local location
 
         Args:
             id (str | int): The files id.
             directory (str, optional): The download dir. Defaults to main.
```

### Comparing `stashconnect-0.7.6/stashconnect/messages.py` & `stashconnect-0.7.7/stashconnect/messages.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.6/stashconnect/models.py` & `stashconnect-0.7.7/stashconnect/models.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.6/stashconnect/settings.py` & `stashconnect-0.7.7/stashconnect/settings.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.6/stashconnect/tools.py` & `stashconnect-0.7.7/stashconnect/tools.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.6/stashconnect/users.py` & `stashconnect-0.7.7/stashconnect/users.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.6/stashconnect.egg-info/PKG-INFO` & `stashconnect-0.7.7/stashconnect.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.7.6
+Version: 0.7.7
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
@@ -19,28 +19,53 @@
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: pycryptodome
 Requires-Dist: python-socketio
 Requires-Dist: Pillow
 Requires-Dist: websocket-client
 
-# <img src="https://raw.githubusercontent.com/BuStudios/StashConnect/main/assets/icon.png" height="22"> StashConnect
+# StashConnect
+
+StashConnect is an easy-to-use API wrapper for [stashcat](https://stashcat.com/) and [schul.cloud](https://schul.cloud).
+
+![PyPI - Downloads](https://img.shields.io/pypi/dm/stashconnect?labelColor=345165&color=4793c9)
+![PyPI - Version](https://img.shields.io/pypi/v/stashconnect?label=version&labelColor=345165&color=4793c9)
+![PyPI - Status](https://img.shields.io/pypi/status/stashconnect?labelColor=345165&color=44af68)
+
+## Installation
+
+To install StashConnect, use pip in your shell:
 
-An API wrapper for [stashcat](https://stashcat.com/) and [schul.cloud](https://schul.cloud).<br>
 ```bash
-pip install stashconnect
+pip install -U stashconnect
 ```
 
-## Contributors
-- All code made by [BuStudios](https://github.com/bustudios)
-- Create a pull request to contribute code yourself
+## Example Usage
+
+```python
+import stashconnect
+
+client = stashconnect.Client(
+    email="your email", password="you password",
+    encryption_password="you enc password",
+)
+
+client.users.change_status("new status")
+```
+
+## Features to be added
 
-## Version 0.7.5
-#### To be added:
 - [x] fix links
+- [ ] file functions
 - [ ] returnable file object
-- [ ] bot file for easy bot setup
+- [ ] bot method
+
+## Contributors
+
+- All code made by [BuStudios](https://github.com/bustudios)
+- Create a pull request to contribute code yourself
 
 ---
+
 StashConnect is not affiliated with Stashcat GmbH or any of its affiliates.
 
 <img src="https://raw.githubusercontent.com/BuStudios/StashConnect/main/assets/icon-full.png">
```

