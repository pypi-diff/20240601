# Comparing `tmp/joppy-0.2.2.tar.gz` & `tmp/joppy-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joppy-0.2.2.tar", last modified: Wed Jan 17 17:49:40 2024, max compression
+gzip compressed data, was "joppy-0.2.3.tar", last modified: Sat Jun  1 14:26:31 2024, max compression
```

## Comparing `joppy-0.2.2.tar` & `joppy-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 17:49:40.427383 joppy-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-01-17 17:49:32.000000 joppy-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-01-17 17:49:40.427383 joppy-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10090 2024-01-17 17:49:32.000000 joppy-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 17:49:40.423383 joppy-0.2.2/joppy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 17:49:32.000000 joppy-0.2.2/joppy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16173 2024-01-17 17:49:32.000000 joppy-0.2.2/joppy/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     8675 2024-01-17 17:49:32.000000 joppy-0.2.2/joppy/data_types.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-17 17:49:32.000000 joppy-0.2.2/joppy/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-01-17 17:49:32.000000 joppy-0.2.2/joppy/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 17:49:40.427383 joppy-0.2.2/joppy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10875 2024-01-17 17:49:40.000000 joppy-0.2.2/joppy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-01-17 17:49:40.000000 joppy-0.2.2/joppy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-17 17:49:40.000000 joppy-0.2.2/joppy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-01-17 17:49:40.000000 joppy-0.2.2/joppy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-01-17 17:49:40.000000 joppy-0.2.2/joppy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-01-17 17:49:40.427383 joppy-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-01-17 17:49:32.000000 joppy-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-17 17:49:40.427383 joppy-0.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)    36071 2024-01-17 17:49:32.000000 joppy-0.2.2/test/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:26:31.978932 joppy-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-06-01 14:26:20.000000 joppy-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-06-01 14:26:31.978932 joppy-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10705 2024-06-01 14:26:20.000000 joppy-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:26:31.974932 joppy-0.2.3/joppy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 14:26:20.000000 joppy-0.2.3/joppy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18401 2024-06-01 14:26:20.000000 joppy-0.2.3/joppy/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9802 2024-06-01 14:26:20.000000 joppy-0.2.3/joppy/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 14:26:20.000000 joppy-0.2.3/joppy/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-06-01 14:26:20.000000 joppy-0.2.3/joppy/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:26:31.978932 joppy-0.2.3/joppy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11541 2024-06-01 14:26:31.000000 joppy-0.2.3/joppy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-06-01 14:26:31.000000 joppy-0.2.3/joppy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 14:26:31.000000 joppy-0.2.3/joppy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-06-01 14:26:31.000000 joppy-0.2.3/joppy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-06-01 14:26:31.000000 joppy-0.2.3/joppy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-06-01 14:26:31.978932 joppy-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-06-01 14:26:20.000000 joppy-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 14:26:31.978932 joppy-0.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    39078 2024-06-01 14:26:20.000000 joppy-0.2.3/test/test_api.py
```

### Comparing `joppy-0.2.2/LICENSE` & `joppy-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `joppy-0.2.2/PKG-INFO` & `joppy-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: joppy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python API for Joplin
 Home-page: https://github.com/marph91/joppy
 Author: Martin Dörfelt
 Author-email: martin.d@andix.de
 License: Mozilla Public License version 2.0
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # joppy
@@ -25,15 +26,15 @@
 Python interface for the [Joplin data API](https://joplinapp.org/api/references/rest_api/).
 
 [![build](https://github.com/marph91/joppy/actions/workflows/build.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/build.yml)
 [![lint](https://github.com/marph91/joppy/actions/workflows/lint.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/lint.yml)
 [![tests](https://github.com/marph91/joppy/actions/workflows/tests.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/marph91/joppy/branch/master/graph/badge.svg?token=97E6IX792A)](https://codecov.io/gh/marph91/joppy)
 
-[![https://img.shields.io/badge/Joplin-2.13.9-blueviolet](https://img.shields.io/badge/Joplin-2.13.9-blueviolet)](https://github.com/laurent22/joplin)
+[![https://img.shields.io/badge/Joplin-2.14.17-blueviolet](https://img.shields.io/badge/Joplin-2.14.17-blueviolet)](https://github.com/laurent22/joplin)
 [![Python version](https://img.shields.io/pypi/pyversions/joppy.svg)](https://pypi.python.org/pypi/joppy/)
 
 ## :computer: Installation
 
 From pypi:
 
 ```bash
@@ -158,17 +159,37 @@
     if re.search("^!", tag.title) is not None:
         api.delete_tag(tag.id)
 ```
 
 </details>
 
 <details>
+<summary>Remove unused tags</summary>
+
+Reference: <https://discourse.joplinapp.org/t/prune-empty-tags-from-web-clipper/36194>
+
+```python name=remove_unused_tags
+from joppy.api import Api
+
+# Create a new Api instance.
+api = Api(token=YOUR_TOKEN)
+
+for tag in api.get_all_tags():
+    notes_for_tag = api.get_all_notes(tag_id=tag.id)
+    if len(notes_for_tag) == 0:
+        print("Deleting tag:", tag.title)
+        api.delete_tag(tag.id)
+```
+
+</details>
+
+<details>
 <summary>Remove spaces from tags</summary>
 
-Inspired by <https://www.reddit.com/r/joplinapp/comments/pozric/batch_remove_spaces_from_all_tags/>.
+Reference: <https://www.reddit.com/r/joplinapp/comments/pozric/batch_remove_spaces_from_all_tags/>
 
 ```python name=remove_spaces_from_tags
 import re
 
 from joppy.api import Api
 
 # Create a new Api instance.
@@ -210,15 +231,15 @@
     matches = re.findall(r"\[.*\]\(:.*\/([A-Za-z0-9]{32})\)", note.body)
     referenced_resources.update(matches)
 
 assert len(referenced_resources) > 0, "sanity check"
 
 for resource in api.get_all_resources():
     if resource.id not in referenced_resources:
-        print("Deleting resource:", resource)
+        print("Deleting resource:", resource.title)
         api.delete_resource(resource.id)
 ```
 
 </details>
 
 For more usage examples, check the example scripts or [tests](test/test_api.py).
 
@@ -248,14 +269,19 @@
 It's possible to configure the test run via some environment variables:
 
 - `SLOW_TESTS`: Set this variable to run the slow tests. Default not set.
 - `API_TOKEN`: Set this variable if there is already a joplin instance running. **Don't use your default joplin profile!** By default, a joplin instance is started inside xvfb. This takes some time, but works for CI.
 
 ## :book: Changelog
 
+### 0.2.3
+
+- Don't use the root logger for logging.
+- Add support for [revisions](https://joplinapp.org/help/api/references/rest_api/#revisions).
+
 ### 0.2.2
 
 - Fix adding non-image ressources (<https://github.com/marph91/joppy/issues/24>).
 - Cast `markup_language` to an appropriate enum type.
 - Add changelog.
 
 ### 0.2.1
```

### Comparing `joppy-0.2.2/README.md` & `joppy-0.2.3/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Python interface for the [Joplin data API](https://joplinapp.org/api/references/rest_api/).
 
 [![build](https://github.com/marph91/joppy/actions/workflows/build.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/build.yml)
 [![lint](https://github.com/marph91/joppy/actions/workflows/lint.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/lint.yml)
 [![tests](https://github.com/marph91/joppy/actions/workflows/tests.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/marph91/joppy/branch/master/graph/badge.svg?token=97E6IX792A)](https://codecov.io/gh/marph91/joppy)
 
-[![https://img.shields.io/badge/Joplin-2.13.9-blueviolet](https://img.shields.io/badge/Joplin-2.13.9-blueviolet)](https://github.com/laurent22/joplin)
+[![https://img.shields.io/badge/Joplin-2.14.17-blueviolet](https://img.shields.io/badge/Joplin-2.14.17-blueviolet)](https://github.com/laurent22/joplin)
 [![Python version](https://img.shields.io/pypi/pyversions/joppy.svg)](https://pypi.python.org/pypi/joppy/)
 
 ## :computer: Installation
 
 From pypi:
 
 ```bash
@@ -136,17 +136,37 @@
     if re.search("^!", tag.title) is not None:
         api.delete_tag(tag.id)
 ```
 
 </details>
 
 <details>
+<summary>Remove unused tags</summary>
+
+Reference: <https://discourse.joplinapp.org/t/prune-empty-tags-from-web-clipper/36194>
+
+```python name=remove_unused_tags
+from joppy.api import Api
+
+# Create a new Api instance.
+api = Api(token=YOUR_TOKEN)
+
+for tag in api.get_all_tags():
+    notes_for_tag = api.get_all_notes(tag_id=tag.id)
+    if len(notes_for_tag) == 0:
+        print("Deleting tag:", tag.title)
+        api.delete_tag(tag.id)
+```
+
+</details>
+
+<details>
 <summary>Remove spaces from tags</summary>
 
-Inspired by <https://www.reddit.com/r/joplinapp/comments/pozric/batch_remove_spaces_from_all_tags/>.
+Reference: <https://www.reddit.com/r/joplinapp/comments/pozric/batch_remove_spaces_from_all_tags/>
 
 ```python name=remove_spaces_from_tags
 import re
 
 from joppy.api import Api
 
 # Create a new Api instance.
@@ -188,15 +208,15 @@
     matches = re.findall(r"\[.*\]\(:.*\/([A-Za-z0-9]{32})\)", note.body)
     referenced_resources.update(matches)
 
 assert len(referenced_resources) > 0, "sanity check"
 
 for resource in api.get_all_resources():
     if resource.id not in referenced_resources:
-        print("Deleting resource:", resource)
+        print("Deleting resource:", resource.title)
         api.delete_resource(resource.id)
 ```
 
 </details>
 
 For more usage examples, check the example scripts or [tests](test/test_api.py).
 
@@ -226,14 +246,19 @@
 It's possible to configure the test run via some environment variables:
 
 - `SLOW_TESTS`: Set this variable to run the slow tests. Default not set.
 - `API_TOKEN`: Set this variable if there is already a joplin instance running. **Don't use your default joplin profile!** By default, a joplin instance is started inside xvfb. This takes some time, but works for CI.
 
 ## :book: Changelog
 
+### 0.2.3
+
+- Don't use the root logger for logging.
+- Add support for [revisions](https://joplinapp.org/help/api/references/rest_api/#revisions).
+
 ### 0.2.2
 
 - Fix adding non-image ressources (<https://github.com/marph91/joppy/issues/24>).
 - Cast `markup_language` to an appropriate enum type.
 - Add changelog.
 
 ### 0.2.1
```

### Comparing `joppy-0.2.2/joppy/api.py` & `joppy-0.2.3/joppy/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Interface for the joplin data API."""
 
 import copy
 import json
 import logging
+import time
 from typing import (
     Any,
     Callable,
     cast,
     Dict,
     List,
     Optional,
@@ -24,14 +25,16 @@
 SESSION = requests.Session()
 
 
 # Don't spam the log. See: https://stackoverflow.com/a/11029841/7410886.
 logging.getLogger("requests").setLevel(logging.WARNING)
 logging.getLogger("urllib3").setLevel(logging.WARNING)
 
+LOGGER = logging.getLogger("joppy")
+
 
 ##############################################################################
 # Base wrapper that manages the requests to the REST API.
 ##############################################################################
 
 
 class ApiBase:
@@ -45,15 +48,15 @@
         self,
         method: str,
         path: str,
         query: Optional[dt.JoplinKwargs] = None,
         data: Optional[dt.JoplinKwargs] = None,
         files: Optional[Dict[str, Any]] = None,
     ) -> requests.models.Response:
-        logging.debug(
+        LOGGER.debug(
             f"API: {method} request: path={path}, query={query}, data={data}, "
             f"files={files}"
         )
         if data is not None and "id_" in data:
             # "id" is a reserved keyword in python, so don't use it.
             data["id"] = data.pop("id_")
         if query is None:
@@ -63,15 +66,15 @@
 
         try:
             response: requests.models.Response = getattr(SESSION, method)(
                 f"{self.url}{path}?{query_str}",
                 json=data,
                 files=files,
             )
-            logging.debug(f"API: response {response.text}")
+            LOGGER.debug(f"API: response {response.text}")
             response.raise_for_status()
         except requests.exceptions.HTTPError as err:
             err.args = err.args + (response.text,)
             raise
         return response
 
     def delete(self, path: str) -> requests.models.Response:
@@ -240,14 +243,62 @@
         return dt.DataList[dt.ResourceData](**response)
 
     def modify_resource(self, id_: str, **data: dt.JoplinTypes) -> None:
         """Modify a resource."""
         self.put(f"/resources/{id_}", data=data)
 
 
+class Revision(ApiBase):
+    """
+    Revisions are supported since Joplin 2.13.2.
+    See: https://github.com/laurent22/joplin/releases/tag/v2.13.2
+    """
+
+    def add_revision(
+        self, item_id: str, item_type: dt.ItemType, **data: dt.JoplinTypes
+    ) -> str:
+        """Add a revision to an item."""
+        now_unix_seconds = int(time.time())
+        return str(
+            self.post(
+                "/revisions",
+                data={
+                    # There seem to be some undocumented required fields.
+                    "item_id": item_id,
+                    "item_type": item_type.value,
+                    "item_updated_time": now_unix_seconds,
+                    "item_created_time": now_unix_seconds,
+                    **data,
+                },
+            ).json()["id"]
+        )
+
+    def delete_revision(self, id_: str) -> None:
+        """Delete a revision."""
+        self.delete(f"/revisions/{id_}")
+
+    def get_revision(self, id_: str, **query: dt.JoplinTypes) -> dt.RevisionData:
+        """Get the revision with the given ID."""
+        response = dt.RevisionData(**self.get(f"/revisions/{id_}", query=query).json())
+        return response
+
+    def get_revisions(self, **query: dt.JoplinTypes) -> dt.DataList[dt.RevisionData]:
+        """
+        Get revisions, paginated. To get all revisions (unpaginated), use
+        "get_all_revisions()".
+        """
+        response = self.get("/revisions", query=query).json()
+        response["items"] = [dt.RevisionData(**item) for item in response["items"]]
+        return dt.DataList[dt.RevisionData](**response)
+
+    def modify_revision(self, id_: str, **data: dt.JoplinTypes) -> None:
+        """Modify a revision."""
+        self.put(f"/revisions/{id_}", data=data)
+
+
 class Search(ApiBase):
     def search(
         self, **query: dt.JoplinTypes
     ) -> Union[
         dt.DataList[dt.NoteData],
         dt.DataList[dt.NotebookData],
         dt.DataList[dt.ResourceData],
@@ -315,15 +366,15 @@
         return dt.DataList[dt.TagData](**response)
 
     def modify_tag(self, id_: str, **data: dt.JoplinTypes) -> None:
         """Modify a tag."""
         self.put(f"/tags/{id_}", data=data)
 
 
-class Api(Event, Note, Notebook, Ping, Resource, Search, Tag):
+class Api(Event, Note, Notebook, Ping, Resource, Revision, Search, Tag):
     """
     Collects all basic API functions and contains a few more useful methods.
     This should be the only class accessed from the users.
     """
 
     def add_tag_to_note(self, tag_id: str, note_id: str) -> None:
         """Add a tag to a given note."""
@@ -360,14 +411,20 @@
 
     def delete_all_resources(self) -> None:
         """Delete all resources."""
         for resource in self.get_all_resources():
             assert resource.id is not None
             self.delete_resource(resource.id)
 
+    def delete_all_revisions(self) -> None:
+        """Delete all revisions."""
+        for revision in self.get_all_revisions():
+            assert revision.id is not None
+            self.delete_revision(revision.id)
+
     def delete_all_tags(self) -> None:
         """Delete all tags."""
         for tag in self.get_all_tags():
             assert tag.id is not None
             self.delete_tag(tag.id)
 
     @staticmethod
@@ -397,14 +454,18 @@
         """Get all notebooks, unpaginated."""
         return self._unpaginate(self.get_notebooks, **query)
 
     def get_all_resources(self, **query: dt.JoplinTypes) -> List[dt.ResourceData]:
         """Get all resources, unpaginated."""
         return self._unpaginate(self.get_resources, **query)
 
+    def get_all_revisions(self, **query: dt.JoplinTypes) -> List[dt.RevisionData]:
+        """Get all revisions, unpaginated."""
+        return self._unpaginate(self.get_revisions, **query)
+
     def get_all_tags(self, **query: dt.JoplinTypes) -> List[dt.TagData]:
         """Get all tags, unpaginated."""
         return self._unpaginate(self.get_tags, **query)
 
     def search_all(
         self, **query: dt.JoplinTypes
     ) -> List[Union[dt.NoteData, dt.NotebookData, dt.ResourceData, dt.TagData]]:
```

### Comparing `joppy-0.2.2/joppy/data_types.py` & `joppy-0.2.3/joppy/data_types.py`

 * *Files 16% similar despite different names*

```diff
@@ -168,14 +168,16 @@
     encryption_cipher_text: Optional[str] = None
     encryption_applied: Optional[bool] = None
     markup_language: Optional[MarkupLanguage] = None
     is_shared: Optional[bool] = None
     share_id: Optional[str] = None
     conflict_original_id: Optional[str] = None
     master_key_id: Optional[str] = None
+    user_data: Optional[str] = None
+    deleted_time: Optional[datetime] = None
     body_html: Optional[str] = None
     base_url: Optional[str] = None
     image_data_url: Optional[str] = None
     crop_rect: Optional[str] = None
 
 
 @dataclass
@@ -191,14 +193,16 @@
     encryption_cipher_text: Optional[str] = None
     encryption_applied: Optional[bool] = None
     parent_id: Optional[str] = None
     is_shared: Optional[bool] = None
     share_id: Optional[str] = None
     master_key_id: Optional[str] = None
     icon: Optional[str] = None
+    user_data: Optional[str] = None
+    deleted_time: Optional[datetime] = None
 
 
 @dataclass
 class ResourceData(BaseData):
     """https://joplinapp.org/api/references/rest_api/#resources"""
 
     id: Optional[str] = None
@@ -213,34 +217,63 @@
     encryption_cipher_text: Optional[str] = None
     encryption_applied: Optional[bool] = None
     encryption_blob_encrypted: Optional[bool] = None
     size: Optional[int] = None
     is_shared: Optional[bool] = None
     share_id: Optional[str] = None
     master_key_id: Optional[str] = None
+    user_data: Optional[str] = None
+    blob_updated_time: Optional[datetime] = None
+    ocr_text: Optional[str] = None
+    ocr_details: Optional[str] = None
+    ocr_status: Optional[int] = None
+    ocr_error: Optional[str] = None
 
     @staticmethod
     def default_fields() -> Set[str]:
         return {"id", "title"}
 
 
 @dataclass
+class RevisionData(BaseData):
+    """https://joplinapp.org/help/api/references/rest_api/#revisions"""
+
+    id: Optional[str] = None
+    parent_id: Optional[str] = None
+    item_type: Optional[ItemType] = None
+    item_id: Optional[str] = None
+    item_updated_time: Optional[datetime] = None
+    title_diff: Optional[str] = None
+    body_diff: Optional[str] = None
+    metadata_diff: Optional[str] = None
+    encryption_cipher_text: Optional[str] = None
+    encryption_applied: Optional[bool] = None
+    updated_time: Optional[datetime] = None
+    created_time: Optional[datetime] = None
+
+    @staticmethod
+    def default_fields() -> Set[str]:
+        return {"id"}
+
+
+@dataclass
 class TagData(BaseData):
     """https://joplinapp.org/api/references/rest_api/#tags"""
 
     id: Optional[str] = None
     title: Optional[str] = None
     created_time: Optional[datetime] = None
     updated_time: Optional[datetime] = None
     user_created_time: Optional[datetime] = None
     user_updated_time: Optional[datetime] = None
     encryption_cipher_text: Optional[str] = None
     encryption_applied: Optional[bool] = None
     is_shared: Optional[bool] = None
     parent_id: Optional[str] = None
+    user_data: Optional[str] = None
 
 
 @dataclass
 class EventData(BaseData):
     """https://joplinapp.org/api/references/rest_api/#events"""
 
     id: Optional[int] = None
@@ -258,15 +291,17 @@
             self.id = int(self.id)
 
     @staticmethod
     def default_fields() -> Set[str]:
         return {"id", "item_type", "item_id", "type", "created_time"}
 
 
-T = TypeVar("T", EventData, NoteData, NotebookData, ResourceData, TagData, str)
+T = TypeVar(
+    "T", EventData, NoteData, NotebookData, ResourceData, RevisionData, TagData, str
+)
 
 
 @dataclass
 class DataList(Generic[T]):
     has_more: bool
     cursor: Optional[int] = None
     items: List[T] = field(default_factory=list)
```

### Comparing `joppy-0.2.2/joppy.egg-info/PKG-INFO` & `joppy-0.2.3/joppy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: joppy
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python API for Joplin
 Home-page: https://github.com/marph91/joppy
 Author: Martin Dörfelt
 Author-email: martin.d@andix.de
 License: Mozilla Public License version 2.0
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 
 # joppy
@@ -25,15 +26,15 @@
 Python interface for the [Joplin data API](https://joplinapp.org/api/references/rest_api/).
 
 [![build](https://github.com/marph91/joppy/actions/workflows/build.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/build.yml)
 [![lint](https://github.com/marph91/joppy/actions/workflows/lint.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/lint.yml)
 [![tests](https://github.com/marph91/joppy/actions/workflows/tests.yml/badge.svg)](https://github.com/marph91/joppy/actions/workflows/tests.yml)
 [![codecov](https://codecov.io/gh/marph91/joppy/branch/master/graph/badge.svg?token=97E6IX792A)](https://codecov.io/gh/marph91/joppy)
 
-[![https://img.shields.io/badge/Joplin-2.13.9-blueviolet](https://img.shields.io/badge/Joplin-2.13.9-blueviolet)](https://github.com/laurent22/joplin)
+[![https://img.shields.io/badge/Joplin-2.14.17-blueviolet](https://img.shields.io/badge/Joplin-2.14.17-blueviolet)](https://github.com/laurent22/joplin)
 [![Python version](https://img.shields.io/pypi/pyversions/joppy.svg)](https://pypi.python.org/pypi/joppy/)
 
 ## :computer: Installation
 
 From pypi:
 
 ```bash
@@ -158,17 +159,37 @@
     if re.search("^!", tag.title) is not None:
         api.delete_tag(tag.id)
 ```
 
 </details>
 
 <details>
+<summary>Remove unused tags</summary>
+
+Reference: <https://discourse.joplinapp.org/t/prune-empty-tags-from-web-clipper/36194>
+
+```python name=remove_unused_tags
+from joppy.api import Api
+
+# Create a new Api instance.
+api = Api(token=YOUR_TOKEN)
+
+for tag in api.get_all_tags():
+    notes_for_tag = api.get_all_notes(tag_id=tag.id)
+    if len(notes_for_tag) == 0:
+        print("Deleting tag:", tag.title)
+        api.delete_tag(tag.id)
+```
+
+</details>
+
+<details>
 <summary>Remove spaces from tags</summary>
 
-Inspired by <https://www.reddit.com/r/joplinapp/comments/pozric/batch_remove_spaces_from_all_tags/>.
+Reference: <https://www.reddit.com/r/joplinapp/comments/pozric/batch_remove_spaces_from_all_tags/>
 
 ```python name=remove_spaces_from_tags
 import re
 
 from joppy.api import Api
 
 # Create a new Api instance.
@@ -210,15 +231,15 @@
     matches = re.findall(r"\[.*\]\(:.*\/([A-Za-z0-9]{32})\)", note.body)
     referenced_resources.update(matches)
 
 assert len(referenced_resources) > 0, "sanity check"
 
 for resource in api.get_all_resources():
     if resource.id not in referenced_resources:
-        print("Deleting resource:", resource)
+        print("Deleting resource:", resource.title)
         api.delete_resource(resource.id)
 ```
 
 </details>
 
 For more usage examples, check the example scripts or [tests](test/test_api.py).
 
@@ -248,14 +269,19 @@
 It's possible to configure the test run via some environment variables:
 
 - `SLOW_TESTS`: Set this variable to run the slow tests. Default not set.
 - `API_TOKEN`: Set this variable if there is already a joplin instance running. **Don't use your default joplin profile!** By default, a joplin instance is started inside xvfb. This takes some time, but works for CI.
 
 ## :book: Changelog
 
+### 0.2.3
+
+- Don't use the root logger for logging.
+- Add support for [revisions](https://joplinapp.org/help/api/references/rest_api/#revisions).
+
 ### 0.2.2
 
 - Fix adding non-image ressources (<https://github.com/marph91/joppy/issues/24>).
 - Cast `markup_language` to an appropriate enum type.
 - Add changelog.
 
 ### 0.2.1
```

### Comparing `joppy-0.2.2/setup.cfg` & `joppy-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `joppy-0.2.2/setup.py` & `joppy-0.2.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pathlib
 from setuptools import setup
 
 
 setup(
     name="joppy",
-    version="0.2.2",
+    version="0.2.3",
     packages=["joppy"],
     # https://stackoverflow.com/a/70386281/7410886
     package_data={
         "joppy": ["py.typed"],
     },
     description="Python API for Joplin",
     long_description=(pathlib.Path(__file__).parent / "README.md").read_text(),
@@ -23,12 +23,13 @@
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Typing :: Typed",
     ],
     python_requires=">=3.7",
     install_requires=["requests"],
 )
```

### Comparing `joppy-0.2.2/test/test_api.py` & `joppy-0.2.3/test/test_api.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,18 +24,19 @@
 os.makedirs("test_output", exist_ok=True)
 logging.basicConfig(
     filename="test_output/test.log",
     filemode="w",
     format="%(asctime)s [%(levelname)s]: %(message)s",
     level=logging.DEBUG,
 )
+LOGGER = logging.getLogger("joppy")
 
 
 SLOW_TESTS = bool(os.getenv("SLOW_TESTS", ""))
-PROFILE = "test_profile"
+PROFILE = os.path.join(os.getcwd(), "test_profile")
 API_TOKEN = ""  # Don't use the API token from env to avoid data loss.
 APP = None
 
 
 def with_resource(func):
     """Create a dummy resource and return it's filename."""
 
@@ -53,49 +54,51 @@
 def setUpModule():  # pylint: disable=invalid-name
     # TODO: When splitting in multiple files, this needs to be run at start of the
     # testsuite.
     global API_TOKEN, APP
     if not API_TOKEN:
         app_path = "./joplin.AppImage"
         setup_joplin.download_joplin(app_path)
-        APP = setup_joplin.JoplinApp(app_path, profile=PROFILE)
+        APP = setup_joplin.JoplinApp(app_path, PROFILE)
         API_TOKEN = APP.api_token
 
 
 def tearDownModule():  # pylint: disable=invalid-name
     if APP is not None:
         APP.stop()
 
 
 class TestBase(unittest.TestCase):
     def setUp(self):
         super().setUp()
 
-        logging.debug("Test: %s", self.id())
+        LOGGER.debug("Test: %s", self.id())
 
         self.api = Api(token=API_TOKEN)
-        # Note: Notes get deleted automatically.
+        # Notes get deleted automatically.
         self.api.delete_all_notebooks()
         self.api.delete_all_resources()
         self.api.delete_all_tags()
+        # Delete revisions last to cover all previous deletions.
+        self.api.delete_all_revisions()
 
     @staticmethod
     def get_random_id() -> str:
         """Return a random, valid ID."""
         # https://stackoverflow.com/a/2782859/7410886
         return f"{random.randrange(16**32):032x}"
 
     @staticmethod
     def get_random_string(length: int = 8, exclude: str = "") -> str:
         """Return a random string."""
         characters = string.printable
         for character in exclude:
             characters = characters.replace(character, "")
         random_string = "".join(random.choice(characters) for _ in range(length))
-        logging.debug("Test: random string: %s", random_string)
+        LOGGER.debug("Test: random string: %s", random_string)
         return random_string
 
     @staticmethod
     def get_combinations(
         iterable: Iterable[str], max_combinations: int = 100
     ) -> Iterable[Tuple[str, ...]]:
         """Get some combinations of an iterable."""
@@ -277,14 +280,16 @@
             "body_html",
             "base_url",
             "image_data_url",
             "crop_rect",
             # todo timestamps can be None
             "todo_due",
             "todo_completed",
+            # we don't delete notes here
+            "deleted_time",
         }
         property_combinations = self.get_combinations(selected_fields)
         for properties in property_combinations:
             notes = self.api.get_notes(fields=",".join(properties))
             for note in notes.items:
                 self.assertEqual(note.assigned_fields(), set(properties))
 
@@ -359,15 +364,19 @@
             f"{invalid_property}",
             context.exception.response.json()["error"],
         )
 
     def test_get_notebooks_valid_properties(self):
         """Try to get specific properties of a notebook."""
         self.api.add_notebook()
-        property_combinations = self.get_combinations(dt.NotebookData.fields())
+        selected_fields = dt.NotebookData.fields() - {
+            # we don't delete notebooks here
+            "deleted_time",
+        }
+        property_combinations = self.get_combinations(selected_fields)
         for properties in property_combinations:
             notebooks = self.api.get_notebooks(fields=",".join(properties))
             for notebook in notebooks.items:
                 self.assertEqual(notebook.assigned_fields(), set(properties))
 
     def test_move(self):
         """Move a root notebok to another notebook. It's now a subnotebook."""
@@ -521,14 +530,70 @@
         """Check the title of a resource."""
         title = self.get_random_string()
         id_ = self.api.add_resource(filename=filename, title=title)
         resource = self.api.get_resource(id_=id_)
         self.assertEqual(resource.title, title)
 
 
+class Revision(TestBase):
+    def test_add(self):
+        """Add a revision."""
+        self.api.add_notebook()  # notebook for the note
+        note_id = self.api.add_note()  # note that gets a new revision
+        id_ = self.api.add_revision(note_id, dt.ItemType.NOTE)
+
+        revisions = self.api.get_revisions().items
+        self.assertEqual(len(revisions), 1)
+        self.assertEqual(revisions[0].id, id_)
+
+    def test_get_revision(self):
+        """Get a specific revision."""
+        self.api.add_notebook()  # notebook for the note
+        note_id = self.api.add_note()  # note that gets a new revision
+        id_ = self.api.add_revision(note_id, dt.ItemType.NOTE)
+        revision = self.api.get_revision(id_=id_)
+        self.assertEqual(revision.assigned_fields(), revision.default_fields())
+        self.assertEqual(revision.type_, dt.ItemType.REVISION)
+
+    def test_get_revisions(self):
+        """Get all revisions."""
+        self.api.add_notebook()  # notebook for the note
+        note_id = self.api.add_note()  # note that gets a new revision
+        self.api.add_revision(note_id, dt.ItemType.NOTE)
+        revisions = self.api.get_revisions()
+        self.assertEqual(len(revisions.items), 1)
+        self.assertFalse(revisions.has_more)
+        for revision in revisions.items:
+            self.assertEqual(revision.assigned_fields(), revision.default_fields())
+
+    def test_get_all_revisions(self):
+        """Get all revisions, unpaginated."""
+        # Small limit and count to create/remove as less as possible items.
+        count, limit = random.randint(1, 10), random.randint(1, 10)
+        self.api.add_notebook()  # notebook for the note
+        note_id = self.api.add_note()  # note that gets a new revision
+        for _ in range(count):
+            self.api.add_revision(note_id, dt.ItemType.NOTE)
+        self.assertEqual(
+            len(self.api.get_revisions(limit=limit).items), min(limit, count)
+        )
+        self.assertEqual(len(self.api.get_all_revisions(limit=limit)), count)
+
+    def test_get_revisions_valid_properties(self):
+        """Try to get specific properties of a revision."""
+        self.api.add_notebook()  # notebook for the note
+        note_id = self.api.add_note()  # note that gets a new revision
+        self.api.add_revision(note_id, dt.ItemType.NOTE)
+        property_combinations = self.get_combinations(dt.RevisionData.fields())
+        for properties in property_combinations:
+            revisions = self.api.get_revisions(fields=",".join(properties))
+            for revision in revisions.items:
+                self.assertEqual(revision.assigned_fields(), set(properties))
+
+
 # TODO: Add more tests for the search parameter.
 class Search(TestBase):
     def test_empty(self):
         """Search should succeed, even if there is no result item."""
         self.assertEqual(self.api.search(query="*").items, [])
 
     def test_notes(self):
```

