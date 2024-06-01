# Comparing `tmp/vre_repository_connector-0.2.0.tar.gz` & `tmp/vre_repository_connector-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vre_repository_connector-0.2.0.tar", max compression
+gzip compressed data, was "vre_repository_connector-0.2.1.tar", max compression
```

## Comparing `vre_repository_connector-0.2.0.tar` & `vre_repository_connector-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2024-05-31 13:15:46.462204 vre_repository_connector-0.2.0/LICENSE
--rw-r--r--   0        0        0     1314 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.0/README.md
--rw-r--r--   0        0        0      745 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      266 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.0/vre_repository_connector/__init__.py
--rw-r--r--   0        0        0      164 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.0/vre_repository_connector/api/__init__.py
--rw-r--r--   0        0        0     2928 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.0/vre_repository_connector/api/base.py
--rw-r--r--   0        0        0    10211 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.0/vre_repository_connector/api/dbrepo.py
--rw-r--r--   0        0        0     6886 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.0/vre_repository_connector/api/inveniordm.py
--rw-r--r--   0        0        0     4879 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.0/vre_repository_connector/auto.py
--rw-r--r--   0        0        0      182 2024-05-31 13:15:46.462204 vre_repository_connector-0.2.0/vre_repository_connector/utils.py
--rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 vre_repository_connector-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-31 13:15:46.462204 vre_repository_connector-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1314 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.1/README.md
+-rw-r--r--   0        0        0      745 2024-05-31 23:33:06.703910 vre_repository_connector-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      266 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.1/vre_repository_connector/__init__.py
+-rw-r--r--   0        0        0      164 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.1/vre_repository_connector/api/__init__.py
+-rw-r--r--   0        0        0     2928 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.1/vre_repository_connector/api/base.py
+-rw-r--r--   0        0        0    10211 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.1/vre_repository_connector/api/dbrepo.py
+-rw-r--r--   0        0        0     6886 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.1/vre_repository_connector/api/inveniordm.py
+-rw-r--r--   0        0        0     4885 2024-05-31 23:33:06.703910 vre_repository_connector-0.2.1/vre_repository_connector/auto.py
+-rw-r--r--   0        0        0      182 2024-05-31 13:15:46.462204 vre_repository_connector-0.2.1/vre_repository_connector/utils.py
+-rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 vre_repository_connector-0.2.1/PKG-INFO
```

### Comparing `vre_repository_connector-0.2.0/LICENSE` & `vre_repository_connector-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vre_repository_connector-0.2.0/README.md` & `vre_repository_connector-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `vre_repository_connector-0.2.0/pyproject.toml` & `vre_repository_connector-0.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "VRE-Repository-Connector"
-version = "0.2.0"
+version = "0.2.1"
 description = "Library for connecting the virtual research environment of TU Wien with its research data repositories"
 authors = ["Maximilian Moser <maximilian.moser@tuwien.ac.at>", "Sotirios Tsepelakis <sotirios.tsepelakis@tuwien.ac.at>", "Martin Weise <martin.weise@tuwien.ac.at>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.tuwien.ac.at/fairdata/vre-repository-connector"
 
 [tool.poetry.dependencies]
```

### Comparing `vre_repository_connector-0.2.0/vre_repository_connector/api/base.py` & `vre_repository_connector-0.2.1/vre_repository_connector/api/base.py`

 * *Files identical despite different names*

### Comparing `vre_repository_connector-0.2.0/vre_repository_connector/api/dbrepo.py` & `vre_repository_connector-0.2.1/vre_repository_connector/api/dbrepo.py`

 * *Files identical despite different names*

### Comparing `vre_repository_connector-0.2.0/vre_repository_connector/api/inveniordm.py` & `vre_repository_connector-0.2.1/vre_repository_connector/api/inveniordm.py`

 * *Files identical despite different names*

### Comparing `vre_repository_connector-0.2.0/vre_repository_connector/auto.py` & `vre_repository_connector-0.2.1/vre_repository_connector/auto.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     "researchdata.tuwien.ac.at": InvenioRDM,
     "researchdata.tuwien.at": InvenioRDM,
     "test.researchdata.tuwien.at": InvenioRDM,
     "s168.dl.hpc.tuwien.ac.at": InvenioRDM,
 }
 
 DEFAULT_URLS = {
-    [url for url, r in KNOWN_INSTANCES.items() if r == repo][0]
+    repo: [url for url, r in KNOWN_INSTANCES.items() if r == repo][0]
     for repo in set(KNOWN_INSTANCES.values())
 }
 
 
 def _resolve_service(host: str, full_url: str) -> Optional[BaseWrapper]:
     """Resolve service based on known URLs."""
     # TODO maybe we could utilize re3data here, or deduce the repository type
```

### Comparing `vre_repository_connector-0.2.0/PKG-INFO` & `vre_repository_connector-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VRE-Repository-Connector
-Version: 0.2.0
+Version: 0.2.1
 Summary: Library for connecting the virtual research environment of TU Wien with its research data repositories
 Home-page: https://gitlab.tuwien.ac.at/fairdata/vre-repository-connector
 License: MIT
 Author: Maximilian Moser
 Author-email: maximilian.moser@tuwien.ac.at
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
```

