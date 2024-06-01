# Comparing `tmp/infisical_api-1.0.0.tar.gz` & `tmp/infisical_api-1.0.1.tar.gz`

## Comparing `infisical_api-1.0.0.tar` & `infisical_api-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 infisical_api-1.0.0/.gitattributes
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 infisical_api-1.0.0/infisical_api.code-workspace
--rw-r--r--   0        0        0     1978 2020-02-02 00:00:00.000000 infisical_api-1.0.0/infisical_api.py
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 infisical_api-1.0.0/.github/delete-merged-branch-config.yml
--rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 infisical_api-1.0.0/.github/workflows/pypi-publish.yml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 infisical_api-1.0.0/.github/workflows/testpypi-publish.yml
--rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 infisical_api-1.0.0/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 infisical_api-1.0.0/LICENSE
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 infisical_api-1.0.0/README.md
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 infisical_api-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 infisical_api-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 infisical_api-1.0.1/.gitattributes
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 infisical_api-1.0.1/infisical_api.code-workspace
+-rw-r--r--   0        0        0     2362 2020-02-02 00:00:00.000000 infisical_api-1.0.1/infisical_api.py
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 infisical_api-1.0.1/.github/delete-merged-branch-config.yml
+-rw-r--r--   0        0        0      939 2020-02-02 00:00:00.000000 infisical_api-1.0.1/.github/workflows/pypi-publish.yml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 infisical_api-1.0.1/.github/workflows/testpypi-publish.yml
+-rw-r--r--   0        0        0     3982 2020-02-02 00:00:00.000000 infisical_api-1.0.1/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 infisical_api-1.0.1/LICENSE
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 infisical_api-1.0.1/README.md
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 infisical_api-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1047 2020-02-02 00:00:00.000000 infisical_api-1.0.1/PKG-INFO
```

### Comparing `infisical_api-1.0.0/infisical_api.py` & `infisical_api-1.0.1/infisical_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,28 +6,37 @@
 
 class infisical_api:  # pylint: disable=invalid-name
     """Infisical API Functions"""
 
     def __init__(
         self,
         service_token: str,
-        infisical_url: str = "https://infisical.com",
+        infisical_url: str = "https://app.infisical.com",
+        workspace_id: str = "dynamic",
     ):
         self.service_token = service_token
         self.infisical_url = infisical_url
+        self.workspace_id = workspace_id
 
     def get_secret(
         self, secret_name: str, environment: str = "prod", path: str = "/"
     ) -> dict:  # pylint: disable=no-self-argument
         """Retrieve Secret"""
+        if self.service_token == "":
+            raise PermissionError("Please provide a valid service_token")
+
         try:
+            if self.workspace_id == "dynamic":
+                workspace_id = self.get_workspace_id()
+            else:
+                workspace_id = self.workspace_id
             response = requests.get(
                 url=f"{self.infisical_url}/api/v3/secrets/raw/{secret_name}",
                 params={
-                    "workspaceId": self.get_workspace_id(),
+                    "workspaceId": workspace_id,
                     "environment": environment,
                     "secretPath": path,
                 },
                 headers={
                     "Authorization": f"Bearer {self.service_token}",
                 },
                 timeout=15,
@@ -45,20 +54,22 @@
             response = requests.get(
                 url=f"{self.infisical_url}/api/v2/service-token",
                 headers={
                     "Authorization": f"Bearer {self.service_token}",
                 },
                 timeout=15,
             )
+            print(response)
             data = json.loads(response.text)
             return data["workspace"]
         except requests.exceptions.RequestException:
             print("Failed to get Workspace ID")
 
+
 class convert_to_dot_notation(dict):
     """
     Access dictionary attributes via dot notation
     """
 
     __getattr__ = dict.get
     __setattr__ = dict.__setitem__
-    __delattr__ = dict.__delitem__
+    __delattr__ = dict.__delitem__
```

### Comparing `infisical_api-1.0.0/.github/workflows/pypi-publish.yml` & `infisical_api-1.0.1/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `infisical_api-1.0.0/.github/workflows/testpypi-publish.yml` & `infisical_api-1.0.1/.github/workflows/testpypi-publish.yml`

 * *Files identical despite different names*

### Comparing `infisical_api-1.0.0/.gitignore` & `infisical_api-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `infisical_api-1.0.0/LICENSE` & `infisical_api-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `infisical_api-1.0.0/README.md` & `infisical_api-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `infisical_api-1.0.0/pyproject.toml` & `infisical_api-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "infisical_api"
-version = "1.0.0"
+version = "1.0.1"
 license = "GPL-3.0"
 authors = [
   { name="Justin Kumpe", email="jakumpe@kumpes.com" },
 ]
 description = "Infisical Client using REST API"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `infisical_api-1.0.0/PKG-INFO` & `infisical_api-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: infisical_api
-Version: 1.0.0
+Version: 1.0.1
 Summary: Infisical Client using REST API
 Author-email: Justin Kumpe <jakumpe@kumpes.com>
 License-Expression: GPL-3.0
 License-File: LICENSE
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
```

