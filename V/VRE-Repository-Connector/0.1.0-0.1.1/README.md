# Comparing `tmp/vre_repository_connector-0.1.0.tar.gz` & `tmp/vre_repository_connector-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vre_repository_connector-0.1.0.tar", max compression
+gzip compressed data, was "vre_repository_connector-0.1.1.tar", max compression
```

## Comparing `vre_repository_connector-0.1.0.tar` & `vre_repository_connector-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.0/LICENSE
--rw-r--r--   0        0        0     1314 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.0/README.md
--rw-r--r--   0        0        0      669 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      183 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.0/vre_repository_connector/__init__.py
--rw-r--r--   0        0        0      203 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.0/vre_repository_connector/api/__init__.py
--rw-r--r--   0        0        0     5437 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.0/vre_repository_connector/api/auto.py
--rw-r--r--   0        0        0     2052 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.0/vre_repository_connector/api/base.py
--rw-r--r--   0        0        0     8669 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.0/vre_repository_connector/api/dbrepo.py
--rw-r--r--   0        0        0     5697 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.0/vre_repository_connector/api/inveniordm.py
--rw-r--r--   0        0        0      182 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.0/vre_repository_connector/utils.py
--rw-r--r--   0        0        0     1962 1970-01-01 00:00:00.000000 vre_repository_connector-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1372 2024-05-31 19:01:04.479402 vre_repository_connector-0.1.1/README.md
+-rw-r--r--   0        0        0      745 2024-05-31 19:01:04.479402 vre_repository_connector-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      183 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.1/vre_repository_connector/__init__.py
+-rw-r--r--   0        0        0      203 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.1/vre_repository_connector/api/__init__.py
+-rw-r--r--   0        0        0     5437 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.1/vre_repository_connector/api/auto.py
+-rw-r--r--   0        0        0     2154 2024-05-31 19:01:04.479402 vre_repository_connector-0.1.1/vre_repository_connector/api/base.py
+-rw-r--r--   0        0        0     9302 2024-05-31 19:01:04.479402 vre_repository_connector-0.1.1/vre_repository_connector/api/dbrepo.py
+-rw-r--r--   0        0        0     6366 2024-05-31 19:01:04.479402 vre_repository_connector-0.1.1/vre_repository_connector/api/inveniordm.py
+-rw-r--r--   0        0        0      182 2024-05-31 13:15:46.462204 vre_repository_connector-0.1.1/vre_repository_connector/utils.py
+-rw-r--r--   0        0        0     2180 1970-01-01 00:00:00.000000 vre_repository_connector-0.1.1/PKG-INFO
```

### Comparing `vre_repository_connector-0.1.0/LICENSE` & `vre_repository_connector-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vre_repository_connector-0.1.0/README.md` & `vre_repository_connector-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -18,7 +18,12 @@
 
 ## Supported repository types
 
 Since the VRE/Repository Connector is currently in a proof of concept stage, support for repository types is very limited.
 It includes:
 * [InvenioRDM](https://inveniordm.docs.cern.ch/)
 * [DBRepo](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/)
+
+
+## Changes
+
+See the [changelog](./CHANGES.md) document.
```

### Comparing `vre_repository_connector-0.1.0/pyproject.toml` & `vre_repository_connector-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "VRE-Repository-Connector"
-version = "0.1.0"
+version = "0.1.1"
 description = "Library for connecting the virtual research environment of TU Wien with its research data repositories"
 authors = ["Maximilian Moser <maximilian.moser@tuwien.ac.at>", "Sotirios Tsepelakis <sotirios.tsepelakis@tuwien.ac.at>", "Martin Weise <martin.weise@tuwien.ac.at>"]
 license = "MIT"
 readme = "README.md"
+repository = "https://gitlab.tuwien.ac.at/fairdata/vre-repository-connector"
 
 [tool.poetry.dependencies]
 python = ">=3.11"
 inveniordm-py = "^0.1.0"
 pandas = "^2"
 dbrepo = "^1.4.4rc1"
 
-
 [tool.poetry.group.dev.dependencies]
 ipython = "^8.24.0"
 
 [tool.isort]
 profile = "black"
 
 [build-system]
```

### Comparing `vre_repository_connector-0.1.0/vre_repository_connector/api/auto.py` & `vre_repository_connector-0.1.1/vre_repository_connector/api/auto.py`

 * *Files identical despite different names*

### Comparing `vre_repository_connector-0.1.0/vre_repository_connector/api/base.py` & `vre_repository_connector-0.1.1/vre_repository_connector/api/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,21 +26,23 @@
     @abc.abstractmethod
     def clear_auth(self):
         """Clear the credentials."""
 
     @abc.abstractmethod
     def upload(
         self, file_path: str, container_id: Optional[str | int], name: Optional[str]
-    ) -> Optional[int | str]:
+    ) -> Tuple[Optional[int | str], Optional[int | str]]:
         """Upload the local file under ``file_path`` to the repository.
 
         If the ``container_id`` is specified, then the file will be uploaded to this
         container.
         Otherwise, a new container will be created.
 
+        A tuple with the container ID and file name/ID will be returned.
+
         :param file_path:    The local path of the file to upload.
         :param container_id: The ID of the container to which to add the uploaded file.
         :param name:         Override for the name of the file after upload.
         """
 
     @abc.abstractmethod
     def download(self, container_id: str | int, name: str | int) -> Optional[str]:
```

### Comparing `vre_repository_connector-0.1.0/vre_repository_connector/api/dbrepo.py` & `vre_repository_connector-0.1.1/vre_repository_connector/api/dbrepo.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 import re
 import urllib.parse
 from collections import Counter
 from typing import List, Optional, Tuple
 
 import requests
 from dbrepo.api.dto import (
+    CreateDatabase,
     CreateTable,
     CreateTableColumn,
     CreateTableConstraints,
     DatatypeAnalysis,
 )
 from dbrepo.RestClient import RestClient
 from pandas import concat
@@ -97,14 +98,25 @@
 
             logging.basicConfig(level=logging.WARNING)
             self.client = RestClient(endpoint=endpoint)
 
         else:
             raise ValueError(f"Invalid DBRepo URL: {url}")
 
+    def _create_database(self, name, container_id, is_public):
+        """Create the database."""
+        cdb = CreateDatabase(name=name, container_id=container_id, is_public=is_public)
+        response = requests.post(
+            url=f"{self.client.endpoint}/api/database",
+            json=json.loads(cdb.model_dump_json()),
+            auth=(self.client.username, self.client.password),
+        )
+
+        return response.json()["id"]
+
     def _create_table(
         self, database_id: int, table_name: str, columns: List[CreateTableColumn]
     ) -> int:
         """Create the described table in the given database.
 
         Custom implementation of ``self.client.create_table()``.
         """
@@ -185,36 +197,39 @@
         return (int(db_id) if db_id else None, int(tbl_id) if tbl_id else None)
 
     def upload(
         self,
         file_path: str,
         database_id: Optional[int] = None,
         table_name: Optional[str] = None,
-    ) -> Optional[int]:
+    ) -> Tuple[Optional[int], Optional[int]]:
         """Uploads a table to the specified database.
 
-        Returns the ID of the created table.
+        If no database is specified, a new one will be created.
+        Returns the IDs of the database and the created table.
         """
         sep = self._guess_separator_character(file_path)
         analysis = self.client.analyse_datatypes(file_path, separator=sep, upload=True)
         filename = os.path.basename(file_path)
 
         if database_id is None:
             # TODO find better logic than this
             container_id = min([c.id for c in self.client.get_containers()])
-            self.client.create_database(filename, container_id=container_id)
+            database_id = self._create_database(
+                filename, container_id=container_id, is_public=True
+            )
 
         table_id = self._create_table(
             database_id, table_name or filename, columns_from_analysis(analysis)
         )
 
         for line_data in self._file_to_data_dicts(file_path, separator=sep):
             self._create_table_data(database_id, table_id, line_data)
 
-        return table_id
+        return (database_id, table_id)
 
     def download(self, database_id: str, table: str | int) -> Optional[str]:
         """Downloads specified table from the database.
 
         Returns the path to the downloaded file.
         """
```

### Comparing `vre_repository_connector-0.1.0/vre_repository_connector/api/inveniordm.py` & `vre_repository_connector-0.1.1/vre_repository_connector/api/inveniordm.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 #
 # Copyright (C) 2024 TU Wien.
 #
 
+import os.path
 import pathlib
 import re
 import tempfile
 import urllib.parse
 from typing import Optional, Tuple
 
 from inveniordm_py.client import InvenioAPI as InvenioRESTClient
@@ -24,20 +25,23 @@
 class InvenioRDM(BaseWrapper):
     """Utility class for connecting to an InvenioRDM instance."""
 
     def __init__(self, url: str, api_token: str = None):
         """InvenioRDM constructor."""
         if match := url_regex.match(url):
             scheme, host = match.group(2) or "https", match.group(3)
-            self.url = f"{scheme}://{host}"
+            url = f"{scheme}://{host}"
+            parts = urllib.parse.urlparse(url)
 
-            # Ensure the URL contains "/api" as the InvenioAPI client can only fetch JSON
-            if not self.url.endswith("/api"):
-                self.url += "/api"
+            # Ensure the path in the URL starts with "/api",
+            # as the InvenioAPI client can only fetch JSON
+            if not parts.path.endswith("/api") and "/api/" not in parts.path:
+                parts = parts._replace(path=(parts.path.lstrip("/api") + "/api"))
 
+            self.url = urllib.parse.urlunparse(parts)
             self.client = InvenioRESTClient(base_url=self.url, access_token=api_token)
 
         else:
             raise ValueError(f"Invalid InvenioRDM URL: {url}")
 
     def authenticate(self, api_token, token=None):
         """Authenticate with an API token."""
@@ -101,29 +105,42 @@
             draft.update(data=DraftMetadata(**metadata))
             return True
 
         except Exception as e:
             print(f"Draft update failed: {e}")
             return False
 
-    def upload(self, file_path: str, record_pid: str, file_name: str) -> Optional[str]:
-        """Uploads a file to the specified draft."""
+    def upload(
+        self,
+        file_path: str,
+        record_pid: Optional[str] = None,
+        file_name: Optional[str] = None,
+    ) -> Optional[str]:
+        """Uploads a file to the specified draft.
+
+        If no draft is specified, a new one will be created.
+        Returns the recid of the draft and name of the uploaded file.
+        """
+        file_name = file_name or os.path.basename(file_path)
+        if not record_pid:
+            record_pid = self.create({"metadata": {"title": file_name}})
+
         draft = self._resolve_draft(record_pid)
 
         try:
             draft.get()
             file_meta = FilesListMetadata([{"key": file_name}])
             file = draft.files.create(file_meta)
 
             stream = open(file_path, "rb")
             for f in draft.files:
                 f.set_contents(OutgoingStream(data=stream))
                 f.commit()
 
-            return file.data["entries"][0]["key"]
+            return (record_pid, file.data["entries"][0]["key"])
 
         except Exception as e:
             print(f"File upload failed: {e}")
 
     def remove(self, record_pid: str, file_name: str) -> bool:
         """Removes given file from the specified draft."""
         draft = self._resolve_draft(record_pid)
@@ -134,15 +151,18 @@
             return True
 
         except Exception as e:
             print(f"File removal failed: {e}")
             return False
 
     def download(self, record_pid: str, file_name: str) -> Optional[str]:
-        """Downloads given file from the specified (published) record."""
+        """Downloads given file from the specified (published) record.
+
+        Returns the path to the downloaded file.
+        """
         record = self.client.records(self._normalize_pid(record_pid))
 
         try:
             record.get()
             response = record.files(file_name).download()
 
             with tempfile.NamedTemporaryFile(delete=False) as downloaded_file:
```

### Comparing `vre_repository_connector-0.1.0/PKG-INFO` & `vre_repository_connector-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: VRE-Repository-Connector
-Version: 0.1.0
+Version: 0.1.1
 Summary: Library for connecting the virtual research environment of TU Wien with its research data repositories
+Home-page: https://gitlab.tuwien.ac.at/fairdata/vre-repository-connector
 License: MIT
 Author: Maximilian Moser
 Author-email: maximilian.moser@tuwien.ac.at
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: dbrepo (>=1.4.4rc1,<2.0.0)
 Requires-Dist: inveniordm-py (>=0.1.0,<0.2.0)
 Requires-Dist: pandas (>=2,<3)
+Project-URL: Repository, https://gitlab.tuwien.ac.at/fairdata/vre-repository-connector
 Description-Content-Type: text/markdown
 
 # VRE/Repository Connector
 
 The VRE/Repository Connector aims to simplify the reuse of research data by offering simple interfaces for downloading and uploading data to and from virtual research environments (VREs).
 
 
@@ -36,7 +38,12 @@
 ## Supported repository types
 
 Since the VRE/Repository Connector is currently in a proof of concept stage, support for repository types is very limited.
 It includes:
 * [InvenioRDM](https://inveniordm.docs.cern.ch/)
 * [DBRepo](https://www.ifs.tuwien.ac.at/infrastructures/dbrepo/)
 
+
+## Changes
+
+See the [changelog](./CHANGES.md) document.
+
```

