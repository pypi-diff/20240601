# Comparing `tmp/vre_repository_connector-0.1.1.tar.gz` & `tmp/vre_repository_connector-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vre_repository_connector-0.1.1.tar", max compression
+gzip compressed data, was "vre_repository_connector-0.2.0.tar", max compression
```

## Comparing `vre_repository_connector-0.1.1.tar` & `vre_repository_connector-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.1/LICENSE
--rw-r--r--   0        0        0     1372 2024-05-31 19:01:04.479402 vre_repository_connector-0.1.1/README.md
--rw-r--r--   0        0        0      745 2024-05-31 19:01:04.479402 vre_repository_connector-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      183 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.1/vre_repository_connector/__init__.py
--rw-r--r--   0        0        0      203 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.1/vre_repository_connector/api/__init__.py
--rw-r--r--   0        0        0     5437 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.1/vre_repository_connector/api/auto.py
--rw-r--r--   0        0        0     2154 2024-05-31 19:01:04.479402 vre_repository_connector-0.1.1/vre_repository_connector/api/base.py
--rw-r--r--   0        0        0     9302 2024-05-31 19:01:04.479402 vre_repository_connector-0.1.1/vre_repository_connector/api/dbrepo.py
--rw-r--r--   0        0        0     6366 2024-05-31 19:01:04.479402 vre_repository_connector-0.1.1/vre_repository_connector/api/inveniordm.py
--rw-r--r--   0        0        0      182 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.1/vre_repository_connector/utils.py
--rw-r--r--   0        0        0     2180 1970-01-01 00:00:00.000000 vre_repository_connector-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-31 13:15:46.462204 vre_repository_connector-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1314 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.0/README.md
+-rw-r--r--   0        0        0      745 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      266 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.0/vre_repository_connector/__init__.py
+-rw-r--r--   0        0        0      164 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.0/vre_repository_connector/api/__init__.py
+-rw-r--r--   0        0        0     2928 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.0/vre_repository_connector/api/base.py
+-rw-r--r--   0        0        0    10211 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.0/vre_repository_connector/api/dbrepo.py
+-rw-r--r--   0        0        0     6886 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.0/vre_repository_connector/api/inveniordm.py
+-rw-r--r--   0        0        0     4879 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.0/vre_repository_connector/auto.py
+-rw-r--r--   0        0        0      182 2024-05-31 13:15:46.462204 vre_repository_connector-0.2.0/vre_repository_connector/utils.py
+-rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 vre_repository_connector-0.2.0/PKG-INFO
```

### Comparing `vre_repository_connector-0.1.1/LICENSE` & `vre_repository_connector-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vre_repository_connector-0.1.1/README.md` & `vre_repository_connector-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,12 +18,7 @@
 
 ## Supported repository types
 
 Since the VRE/Repository Connector is currently in a proof of concept stage, support for repository types is very limited.
 It includes:
 * [InvenioRDM](https://inveniordm.docs.cern.ch/)
 * [DBRepo](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/)
-
-
-## Changes
-
-See the [changelog](./CHANGES.md) document.
```

### Comparing `vre_repository_connector-0.1.1/pyproject.toml` & `vre_repository_connector-0.2.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "VRE-Repository-Connector"
-version = "0.1.1"
+version = "0.2.0"
 description = "Library for connecting the virtual research environment of TU Wien with its research data repositories"
 authors = ["Maximilian Moser <maximilian.moser@tuwien.ac.at>", "Sotirios Tsepelakis <sotirios.tsepelakis@tuwien.ac.at>", "Martin Weise <martin.weise@tuwien.ac.at>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.tuwien.ac.at/fairdata/vre-repository-connector"
 
 [tool.poetry.dependencies]
```

### Comparing `vre_repository_connector-0.1.1/vre_repository_connector/api/base.py` & `vre_repository_connector-0.2.0/vre_repository_connector/api/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,28 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2024 TU Wien.
 #
 
 import abc
-from typing import Optional, Tuple
+from typing import Dict, Iterable, Optional, Tuple
 
 
 class BaseWrapper(abc.ABC):
     """The common denominator of operations that need to be supported."""
 
     @abc.abstractmethod
+    def ask_credentials(cls) -> Dict[str, str]:
+        """Ask the user interactively for credentials.
+
+        The returned dictionary can be used as keyword arguments for ``authenticate``.
+        """
+        return {}
+
+    @abc.abstractmethod
     def authenticate(self, token_or_username, password=None):
         """Set the credentials for future API calls.
 
         Provides the API wrapper with a set of credentials to be used for future
         API calls.
         This method accepts two different shapes of credentials: Either just an API
         token, or a pair of username + password.
@@ -39,21 +47,37 @@
 
         A tuple with the container ID and file name/ID will be returned.
 
         :param file_path:    The local path of the file to upload.
         :param container_id: The ID of the container to which to add the uploaded file.
         :param name:         Override for the name of the file after upload.
         """
+        return None
 
     @abc.abstractmethod
     def download(self, container_id: str | int, name: str | int) -> Optional[str]:
         """Download the file with the specified name from the referenced container.
 
         :param container_id: The ID of the container from which to download the file.
         :param name:         The name of the file to download.
         """
+        return None
+
+    @abc.abstractmethod
+    def list_files(self, container_id: str | int) -> Iterable[str]:
+        """List all the file names attached to the container.
+
+        :param container_id: The container to list the files for.
+        """
+        return []
 
+    @abc.abstractmethod
     def url_to_parts(self, url: str) -> Tuple[Optional[str | int], Optional[str | int]]:
         """Parse the container and file from the URL.
 
         :param url: The URL from which to parse the container ID and file name.
         """
+        return (None, None)
+
+    def authenticate_interactive(self):
+        """Shorthand for ``ask_credentials()`` into ``authenticate()``."""
+        self.authenticate(**self.ask_credentials())
```

### Comparing `vre_repository_connector-0.1.1/vre_repository_connector/api/dbrepo.py` & `vre_repository_connector-0.2.0/vre_repository_connector/api/dbrepo.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2024 TU Wien.
 #
 
 import csv
+import getpass
 import json
 import logging
 import os
 import re
 import urllib.parse
 from collections import Counter
-from typing import List, Optional, Tuple
+from typing import Iterable, List, Optional, Tuple
 
 import requests
 from dbrepo.api.dto import (
     CreateDatabase,
     CreateTable,
     CreateTableColumn,
     CreateTableConstraints,
@@ -154,14 +155,21 @@
         response = requests.post(
             url=f"{self.client.endpoint}/api/database/{database_id}/table/{table_id}/data",  # noqa
             json={"data": row},
             auth=(self.client.username, self.client.password),
         )
         assert 200 <= response.status_code < 300
 
+    def ask_credentials(self):
+        """Ask the user interactively for credentials."""
+        print(f"(DBRepo) Enter your credentials for '{self.client.endpoint}'")
+        username = input("Username: ")
+        password = getpass.getpass("Password: ")
+        return {"auth_str": username, "password": password}
+
     def authenticate(self, auth_str, password=None):
         """Authenticate the client with a username and password.
 
         If only one positional argument is supplied, it is expected to be a string
         with the shape "username:password".
 
         Alternatively, the username can be supplied as the first positional argument
@@ -178,14 +186,20 @@
         self.client.username = username
         self.client.password = password
 
     def clear_auth(self):
         """Clear the DBRepo client's credentials."""
         self.client.username, self.client.password = None, None
 
+    def list_files(self, database_id: int) -> Iterable[str]:
+        """List all tables by name for the container."""
+        url = f"{self.client.endpoint}/api/database/{database_id}/table"
+        response = requests.get(url, auth=(self.client.username, self.client.password))
+        return [tbl["name"] for tbl in response.json()]
+
     def url_to_parts(self, url: str) -> Tuple[Optional[int], Optional[int]]:
         """Get the database ID and table ID from the URL."""
         db_id, tbl_id = None, None
 
         try:
             path = urllib.parse.urlparse(url).path
             match = db_tbl_regex.match(path)
@@ -232,19 +246,24 @@
 
         Returns the path to the downloaded file.
         """
 
         # get the required infos about the table in question
         table_id, table_name = table, table
         if isinstance(table, str):
+            url = f"{self.client.endpoint}/api/database/{database_id}/table"
+            response = requests.get(
+                url, auth=(self.client.username, self.client.password)
+            )
             matching_tables = [
-                t for t in self.client.get_tables(database_id) if t.name == table_id
+                tbl["id"] for tbl in response.json() if tbl["name"] == table_id
             ]
+
             if matching_tables:
-                table = matching_tables[0]
+                table = self.client.get_table(database_id, matching_tables[0])
                 table_id = table.id
             else:
                 return None
         else:
             table = self.client.get_table(database_id, table)
             table_name = table.name
```

### Comparing `vre_repository_connector-0.1.1/vre_repository_connector/api/inveniordm.py` & `vre_repository_connector-0.2.0/vre_repository_connector/api/inveniordm.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2024 TU Wien.
 #
 
+import getpass
 import os.path
 import pathlib
 import re
 import tempfile
 import urllib.parse
-from typing import Optional, Tuple
+from typing import Iterable, Optional, Tuple
 
 from inveniordm_py.client import InvenioAPI as InvenioRESTClient
 from inveniordm_py.files.metadata import FilesListMetadata, OutgoingStream
 from inveniordm_py.records.metadata import DraftMetadata
 from inveniordm_py.records.resources import Draft
 
 from ..utils import doi_regex, url_regex
@@ -31,32 +32,44 @@
             scheme, host = match.group(2) or "https", match.group(3)
             url = f"{scheme}://{host}"
             parts = urllib.parse.urlparse(url)
 
             # Ensure the path in the URL starts with "/api",
             # as the InvenioAPI client can only fetch JSON
             if not parts.path.endswith("/api") and "/api/" not in parts.path:
-                parts = parts._replace(path=(parts.path.lstrip("/api") + "/api"))
+                parts = parts._replace(path="/api")
 
             self.url = urllib.parse.urlunparse(parts)
             self.client = InvenioRESTClient(base_url=self.url, access_token=api_token)
 
         else:
             raise ValueError(f"Invalid InvenioRDM URL: {url}")
 
+    def ask_credentials(self):
+        """Ask the user interactively for credentials."""
+        print(f"(InvenioRDM) Enter your API token for '{self.url}'")
+        token = getpass.getpass("API Token: ")
+        return {"api_token": token}
+
     def authenticate(self, api_token, token=None):
         """Authenticate with an API token."""
-        self.client._access_token = api_token
+        self.client._access_token = api_token or token
         self.client.session.headers["Authorization"] = f"Bearer {api_token}"
 
     def clear_auth(self):
         """Clear the API token."""
         self.client._access_token = None
         self.client.session.headers.pop("Authorization", None)
 
+    def list_files(self, recid: str) -> Iterable[str]:
+        """List all files for the record."""
+        url = f"{self.client._base_url}/records/{recid}/files"
+        response = self.client.session.get(url)
+        return [f["key"] for f in response.json()["entries"]]
+
     def url_to_parts(self, url: str) -> Tuple[Optional[str], Optional[str]]:
         """Get the recid and filename from the URL."""
         recid, filename = None, None
 
         try:
             path = urllib.parse.urlparse(url).path
             match = recid_file_re.match(path)
```

### Comparing `vre_repository_connector-0.1.1/PKG-INFO` & `vre_repository_connector-0.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VRE-Repository-Connector
-Version: 0.1.1
+Version: 0.2.0
 Summary: Library for connecting the virtual research environment of TU Wien with its research data repositories
 Home-page: https://gitlab.tuwien.ac.at/fairdata/vre-repository-connector
 License: MIT
 Author: Maximilian Moser
 Author-email: maximilian.moser@tuwien.ac.at
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -38,12 +38,7 @@
 ## Supported repository types
 
 Since the VRE/Repository Connector is currently in a proof of concept stage, support for repository types is very limited.
 It includes:
 * [InvenioRDM](https://inveniordm.docs.cern.ch/)
 * [DBRepo](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/)
 
-
-## Changes
-
-See the [changelog](./CHANGES.md) document.
-
```

