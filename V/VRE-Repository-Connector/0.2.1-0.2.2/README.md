# Comparing `tmp/vre_repository_connector-0.2.1.tar.gz` & `tmp/vre_repository_connector-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vre_repository_connector-0.2.1.tar", max compression
+gzip compressed data, was "vre_repository_connector-0.2.2.tar", max compression
```

## Comparing `vre_repository_connector-0.2.1.tar` & `vre_repository_connector-0.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1064 2024-05-31 13:15:46.462204 vre_repository_connector-0.2.1/LICENSE
--rw-r--r--   0        0        0     1314 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.1/README.md
--rw-r--r--   0        0        0      745 2024-05-31 23:33:06.703910 vre_repository_connector-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      266 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.1/vre_repository_connector/__init__.py
--rw-r--r--   0        0        0      164 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.1/vre_repository_connector/api/__init__.py
--rw-r--r--   0        0        0     2928 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.1/vre_repository_connector/api/base.py
--rw-r--r--   0        0        0    10211 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.1/vre_repository_connector/api/dbrepo.py
--rw-r--r--   0        0        0     6886 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.1/vre_repository_connector/api/inveniordm.py
--rw-r--r--   0        0        0     4885 2024-05-31 23:33:06.703910 vre_repository_connector-0.2.1/vre_repository_connector/auto.py
--rw-r--r--   0        0        0      182 2024-05-31 13:15:46.462204 vre_repository_connector-0.2.1/vre_repository_connector/utils.py
--rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 vre_repository_connector-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-05-31 13:15:46.462204 vre_repository_connector-0.2.2/LICENSE
+-rw-r--r--   0        0        0     1314 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.2/README.md
+-rw-r--r--   0        0        0      745 2024-06-01 17:25:44.417153 vre_repository_connector-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      298 2024-06-01 17:25:44.417153 vre_repository_connector-0.2.2/vre_repository_connector/__init__.py
+-rw-r--r--   0        0        0      164 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.2/vre_repository_connector/api/__init__.py
+-rw-r--r--   0        0        0     2928 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.2/vre_repository_connector/api/base.py
+-rw-r--r--   0        0        0    10211 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.2/vre_repository_connector/api/dbrepo.py
+-rw-r--r--   0        0        0     6886 2024-05-31 23:18:03.497382 vre_repository_connector-0.2.2/vre_repository_connector/api/inveniordm.py
+-rw-r--r--   0        0        0     5517 2024-06-01 17:25:44.417153 vre_repository_connector-0.2.2/vre_repository_connector/auto.py
+-rw-r--r--   0        0        0      182 2024-05-31 13:15:46.462204 vre_repository_connector-0.2.2/vre_repository_connector/utils.py
+-rw-r--r--   0        0        0     2122 1970-01-01 00:00:00.000000 vre_repository_connector-0.2.2/PKG-INFO
```

### Comparing `vre_repository_connector-0.2.1/LICENSE` & `vre_repository_connector-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vre_repository_connector-0.2.1/README.md` & `vre_repository_connector-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `vre_repository_connector-0.2.1/pyproject.toml` & `vre_repository_connector-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "VRE-Repository-Connector"
-version = "0.2.1"
+version = "0.2.2"
 description = "Library for connecting the virtual research environment of TU Wien with its research data repositories"
 authors = ["Maximilian Moser <maximilian.moser@tuwien.ac.at>", "Sotirios Tsepelakis <sotirios.tsepelakis@tuwien.ac.at>", "Martin Weise <martin.weise@tuwien.ac.at>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://gitlab.tuwien.ac.at/fairdata/vre-repository-connector"
 
 [tool.poetry.dependencies]
```

### Comparing `vre_repository_connector-0.2.1/vre_repository_connector/api/base.py` & `vre_repository_connector-0.2.2/vre_repository_connector/api/base.py`

 * *Files identical despite different names*

### Comparing `vre_repository_connector-0.2.1/vre_repository_connector/api/dbrepo.py` & `vre_repository_connector-0.2.2/vre_repository_connector/api/dbrepo.py`

 * *Files identical despite different names*

### Comparing `vre_repository_connector-0.2.1/vre_repository_connector/api/inveniordm.py` & `vre_repository_connector-0.2.2/vre_repository_connector/api/inveniordm.py`

 * *Files identical despite different names*

### Comparing `vre_repository_connector-0.2.1/vre_repository_connector/auto.py` & `vre_repository_connector-0.2.2/vre_repository_connector/auto.py`

 * *Files 7% similar despite different names*

```diff
@@ -107,37 +107,57 @@
     url: str, all: bool = False, interactive: bool = True
 ) -> List[str] | str | None:
     """Download file automatically based on the URL."""
     if (service := suggest_repository(url)) is None:
         return None
 
     # fish out the container & file from the URL
-    cid, fid, fids = *service.url_to_parts(url), []
+    cid, fid, fids = (*service.url_to_parts(url), [])
     if cid is None and fid is None:
         cid, fid = service.url_to_parts(_follow_redirects(url))
 
     # if we couldn't determine a file from the URL...
     if fid is None:
-        if all:
+        avail_files = list(service.list_files(cid))
+        if len(avail_files) == 1:
+            fid = avail_files[0]
+
+        elif all:
             # we either take all of them
-            fids = list(service.list_files(cid))
+            fids = avail_files
+
         elif interactive:
-            # or we ask the user (TODO)
-            pass
+            # or we ask the user
+            selection = 0
+            for idx, file_ in enumerate(avail_files):
+                print(f"{idx+1}) {file_}")
+
+            while not (0 < selection <= len(avail_files)):
+                try:
+                    selection = int(input(f"Select [1-{len(avail_files)}]: "))
+                except ValueError:
+                    selection = 0
+
+            fid = avail_files[selection - 1]
         else:
             # or we give up
             return None
 
     try:
         return _download(service, cid, fid or fids, interactive)
 
     finally:
         service.clear_auth()
 
 
+def download_all(url: str) -> List[str] | str | None:
+    """Download all files from a URL."""
+    return download(url, all=True, interactive=False)
+
+
 def upload(
     file_path: str, url: Optional[str] = None
 ) -> Tuple[Optional[str], Optional[str], Optional[str]]:
     """Upload the file to an auto-selected repository.
 
     Return a triple with the repository's URL, the container ID and the file ID.
     """
```

### Comparing `vre_repository_connector-0.2.1/PKG-INFO` & `vre_repository_connector-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: VRE-Repository-Connector
-Version: 0.2.1
+Version: 0.2.2
 Summary: Library for connecting the virtual research environment of TU Wien with its research data repositories
 Home-page: https://gitlab.tuwien.ac.at/fairdata/vre-repository-connector
 License: MIT
 Author: Maximilian Moser
 Author-email: maximilian.moser@tuwien.ac.at
 Requires-Python: >=3.11
 Classifier: License :: OSI Approved :: MIT License
```

