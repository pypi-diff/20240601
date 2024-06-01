# Comparing `tmp/stashconnect-0.7.7.tar.gz` & `tmp/stashconnect-0.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stashconnect-0.7.7.tar", last modified: Sat Jun  1 15:08:41 2024, max compression
+gzip compressed data, was "stashconnect-0.7.8.tar", last modified: Sat Jun  1 20:58:14 2024, max compression
```

## Comparing `stashconnect-0.7.7.tar` & `stashconnect-0.7.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 15:08:41.511074 stashconnect-0.7.7/
--rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.7.7/LICENSE
--rw-rw-rw-   0        0        0     2263 2024-06-01 15:08:41.507543 stashconnect-0.7.7/PKG-INFO
--rw-rw-rw-   0        0        0     1230 2024-06-01 14:22:32.000000 stashconnect-0.7.7/README.md
--rw-rw-rw-   0        0        0       42 2024-06-01 15:08:41.511573 stashconnect-0.7.7/setup.cfg
--rw-rw-rw-   0        0        0     1422 2024-06-01 15:05:19.000000 stashconnect-0.7.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:08:41.481307 stashconnect-0.7.7/stashconnect/
--rw-rw-rw-   0        0        0      216 2024-06-01 15:03:31.000000 stashconnect-0.7.7/stashconnect/__init__.py
--rw-rw-rw-   0        0        0    17257 2024-05-10 18:47:16.000000 stashconnect-0.7.7/stashconnect/channels.py
--rw-rw-rw-   0        0        0     9403 2024-06-01 14:58:25.000000 stashconnect-0.7.7/stashconnect/client.py
--rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.7.7/stashconnect/companies.py
--rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.7.7/stashconnect/conversations.py
--rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.7.7/stashconnect/crypto_utils.py
--rw-rw-rw-   0        0        0    12503 2024-06-01 14:56:25.000000 stashconnect-0.7.7/stashconnect/files.py
--rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.7.7/stashconnect/messages.py
--rw-rw-rw-   0        0        0    17343 2024-05-11 08:24:59.000000 stashconnect-0.7.7/stashconnect/models.py
--rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.7.7/stashconnect/settings.py
--rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.7.7/stashconnect/tools.py
--rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.7.7/stashconnect/users.py
-drwxrwxrwx   0        0        0        0 2024-06-01 15:08:41.502778 stashconnect-0.7.7/stashconnect.egg-info/
--rw-rw-rw-   0        0        0     2263 2024-06-01 15:08:41.000000 stashconnect-0.7.7/stashconnect.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      502 2024-06-01 15:08:41.000000 stashconnect-0.7.7/stashconnect.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 15:08:41.000000 stashconnect-0.7.7/stashconnect.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-06-01 15:08:41.000000 stashconnect-0.7.7/stashconnect.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-06-01 15:08:41.000000 stashconnect-0.7.7/stashconnect.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 20:58:14.591062 stashconnect-0.7.8/
+-rw-rw-rw-   0        0        0     1087 2024-04-21 06:28:56.000000 stashconnect-0.7.8/LICENSE
+-rw-rw-rw-   0        0        0     2263 2024-06-01 20:58:14.587032 stashconnect-0.7.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1230 2024-06-01 14:22:32.000000 stashconnect-0.7.8/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 20:58:14.591561 stashconnect-0.7.8/setup.cfg
+-rw-rw-rw-   0        0        0     1422 2024-06-01 15:05:19.000000 stashconnect-0.7.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 20:58:14.562144 stashconnect-0.7.8/stashconnect/
+-rw-rw-rw-   0        0        0      216 2024-06-01 20:55:59.000000 stashconnect-0.7.8/stashconnect/__init__.py
+-rw-rw-rw-   0        0        0    17257 2024-05-10 18:47:16.000000 stashconnect-0.7.8/stashconnect/channels.py
+-rw-rw-rw-   0        0        0     9403 2024-06-01 14:58:25.000000 stashconnect-0.7.8/stashconnect/client.py
+-rw-rw-rw-   0        0        0     3618 2024-05-10 20:37:19.000000 stashconnect-0.7.8/stashconnect/companies.py
+-rw-rw-rw-   0        0        0     4704 2024-05-31 06:25:48.000000 stashconnect-0.7.8/stashconnect/conversations.py
+-rw-rw-rw-   0        0        0     2584 2024-04-25 17:41:41.000000 stashconnect-0.7.8/stashconnect/crypto_utils.py
+-rw-rw-rw-   0        0        0    12585 2024-06-01 20:34:55.000000 stashconnect-0.7.8/stashconnect/files.py
+-rw-rw-rw-   0        0        0     6298 2024-05-30 19:29:31.000000 stashconnect-0.7.8/stashconnect/messages.py
+-rw-rw-rw-   0        0        0    18737 2024-06-01 20:56:20.000000 stashconnect-0.7.8/stashconnect/models.py
+-rw-rw-rw-   0        0        0     1458 2024-05-07 15:16:08.000000 stashconnect-0.7.8/stashconnect/settings.py
+-rw-rw-rw-   0        0        0     1001 2024-05-31 18:50:21.000000 stashconnect-0.7.8/stashconnect/tools.py
+-rw-rw-rw-   0        0        0     2101 2024-05-10 15:03:08.000000 stashconnect-0.7.8/stashconnect/users.py
+drwxrwxrwx   0        0        0        0 2024-06-01 20:58:14.583516 stashconnect-0.7.8/stashconnect.egg-info/
+-rw-rw-rw-   0        0        0     2263 2024-06-01 20:58:14.000000 stashconnect-0.7.8/stashconnect.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2024-06-01 20:58:14.000000 stashconnect-0.7.8/stashconnect.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 20:58:14.000000 stashconnect-0.7.8/stashconnect.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-06-01 20:58:14.000000 stashconnect-0.7.8/stashconnect.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-06-01 20:58:14.000000 stashconnect-0.7.8/stashconnect.egg-info/top_level.txt
```

### Comparing `stashconnect-0.7.7/LICENSE` & `stashconnect-0.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.7/PKG-INFO` & `stashconnect-0.7.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.7.7
+Version: 0.7.8
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
```

### Comparing `stashconnect-0.7.7/README.md` & `stashconnect-0.7.8/README.md`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.7/setup.py` & `stashconnect-0.7.8/setup.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.7/stashconnect/channels.py` & `stashconnect-0.7.8/stashconnect/channels.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.7/stashconnect/client.py` & `stashconnect-0.7.8/stashconnect/client.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.7/stashconnect/companies.py` & `stashconnect-0.7.8/stashconnect/companies.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.7/stashconnect/conversations.py` & `stashconnect-0.7.8/stashconnect/conversations.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.7/stashconnect/crypto_utils.py` & `stashconnect-0.7.8/stashconnect/crypto_utils.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.7/stashconnect/files.py` & `stashconnect-0.7.8/stashconnect/files.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import uuid
 from PIL import Image
 import base64
 import io
 import json
 
 from .crypto_utils import CryptoUtils
-from .models import Channel, Conversation
+from .models import Channel, Conversation, File
 
 
 class FileManager:
     def __init__(self, client):
         self.client = client
 
     def quota(self) -> dict:
@@ -132,15 +132,15 @@
                 "iv": iv.hex(),
             }
 
             response = self.client._post("security/set_file_access_key", data=data)
 
         self.client.files.store_preview_image(file_id, filepath)
 
-        return file
+        return File(self.client, file)
 
     def store_preview_image(self, file_id: str | int, filepath: str):
         try:
             with Image.open(filepath) as image:
                 output_size = 100
 
                 image = image.convert("RGB")
@@ -164,15 +164,15 @@
 
             data = {
                 "file_id": file_id,
                 "content": str("data:image/jpeg;base64," + image_base64),
             }
 
             response = self.client._post("file/storePreviewImage", data=data)
-            return response["file"]
+            return File(self.client, response["file"])
 
         except Exception:
             return {"success": False}
 
     def download(self, id: str | int, directory: str = "") -> str:
         """Downloads a file to a local location
 
@@ -223,15 +223,15 @@
         Args:
             id (str | int): The files id.
 
         Returns:
             File: A file object.
         """
         response = self.client._post("file/info", data={"file_id": id})
-        return response["file"]
+        return File(self.client, response["file"])
 
     def delete(self, ids: str | int | list) -> dict:
         """Deletes specified files
 
         Args:
             ids (str | int | list): The file or files ids
 
@@ -304,15 +304,15 @@
         data = {
             "file_id": id,
             "folder_id": folder_id,
             "type": target_type,
             "type_id": type_id,
         }
         response = self.client._post("file/copy", data=data)
-        return response["file"]
+        return File(self.client, response["file"])
 
     def shares(self, id: str | int) -> dict:
         """Get a files shares
 
         Args:
             id (str | int): The files id.
```

### Comparing `stashconnect-0.7.7/stashconnect/messages.py` & `stashconnect-0.7.8/stashconnect/messages.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.7/stashconnect/models.py` & `stashconnect-0.7.8/stashconnect/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -551,7 +551,56 @@
     def enable_notifications(self) -> dict:
         """Enables notifications for a channel
 
         Returns:
             dict: The success status.
         """
         return self.client.channels.enable_notifications(self.id)
+
+
+class File:
+    def __init__(self, client, data):
+        self.client = client
+        self.id = data["id"]
+
+        try:
+            self.set_attributes(data)
+        except KeyError:
+            data = self.client.files.info(self.id)
+            self.set_attributes(data)
+
+    def set_attributes(self, data):
+        self.name = data["name"]
+
+        self.virtual_folder = data["virtual_folder"]
+        self.folder_type = data["folder_type"]
+        self.type_id = data["type_id"]
+
+        self.size = data["size"]
+        self.size_byte = data["size_byte"]
+        self.size_string = data["size_string"]
+
+        self.width = data["dimensions"]["width"]
+        self.height = data["dimensions"]["height"]
+
+        self.extension = data["ext"]
+        self.mimetype = data["mime"]
+
+        self.base_64 = data["base_64"]
+
+        self.uploaded = data["uploaded"]
+        self.modified = data["modified"]
+
+        self.permission = data["permission"]
+
+        self.owner_id = data["owner_id"]
+        self.owner = User(self.client, data["owner"])
+
+        self.last_download = data["last_download"]
+        self.times_downloaded = data["times_downloaded"]
+
+        self.status = data["status"]
+        self.deleted = data["deleted"]
+        self.encrypted = data["encrypted"]
+
+        self.iv = data["e2e_iv"]
+        self.md5 = data["md5"]
```

### Comparing `stashconnect-0.7.7/stashconnect/settings.py` & `stashconnect-0.7.8/stashconnect/settings.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.7/stashconnect/tools.py` & `stashconnect-0.7.8/stashconnect/tools.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.7/stashconnect/users.py` & `stashconnect-0.7.8/stashconnect/users.py`

 * *Files identical despite different names*

### Comparing `stashconnect-0.7.7/stashconnect.egg-info/PKG-INFO` & `stashconnect-0.7.8/stashconnect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stashconnect
-Version: 0.7.7
+Version: 0.7.8
 Summary: An API wrapper for stashcat and schul.cloud.
 Home-page: https://github.com/BuStudios/StashConnect
 Author: BuStudios
 Author-email: support@bustudios.org
 Project-URL: Bug Tracker, https://github.com/BuStudios/StashConnect/issues
 Project-URL: Documentation, https://github.com/BuStudios/StashConnect/wiki
 Project-URL: Source Code, https://github.com/BuStudios/StashConnect
```

