# Comparing `tmp/dbt_loom-0.5.3.tar.gz` & `tmp/dbt_loom-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt_loom-0.5.3.tar", max compression
+gzip compressed data, was "dbt_loom-0.5.4.tar", max compression
```

## Comparing `dbt_loom-0.5.3.tar` & `dbt_loom-0.5.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1211 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/LICENSE
--rw-r--r--   0        0        0     6654 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/README.md
--rw-r--r--   0        0        0     6762 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/dbt_loom/__init__.py
--rw-r--r--   0        0        0     2088 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/dbt_loom/clients/az_blob.py
--rw-r--r--   0        0        0     2632 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/dbt_loom/clients/dbt_cloud.py
--rw-r--r--   0        0        0     1603 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/dbt_loom/clients/gcs.py
--rw-r--r--   0        0        0     1641 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/dbt_loom/clients/s3.py
--rw-r--r--   0        0        0     1161 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/dbt_loom/config.py
--rw-r--r--   0        0        0      396 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/dbt_loom/logging.py
--rw-r--r--   0        0        0     4716 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/dbt_loom/manifests.py
--rw-r--r--   0        0        0     1061 2024-05-11 01:00:32.151226 dbt_loom-0.5.3/pyproject.toml
--rw-r--r--   0        0        0     7506 1970-01-01 00:00:00.000000 dbt_loom-0.5.3/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-06-01 01:55:59.776910 dbt_loom-0.5.4/LICENSE
+-rw-r--r--   0        0        0     6654 2024-06-01 01:55:59.776910 dbt_loom-0.5.4/README.md
+-rw-r--r--   0        0        0     8637 2024-06-01 01:55:59.776910 dbt_loom-0.5.4/dbt_loom/__init__.py
+-rw-r--r--   0        0        0     2088 2024-06-01 01:55:59.776910 dbt_loom-0.5.4/dbt_loom/clients/az_blob.py
+-rw-r--r--   0        0        0     2632 2024-06-01 01:55:59.776910 dbt_loom-0.5.4/dbt_loom/clients/dbt_cloud.py
+-rw-r--r--   0        0        0     1603 2024-06-01 01:55:59.776910 dbt_loom-0.5.4/dbt_loom/clients/gcs.py
+-rw-r--r--   0        0        0     1641 2024-06-01 01:55:59.776910 dbt_loom-0.5.4/dbt_loom/clients/s3.py
+-rw-r--r--   0        0        0     1161 2024-06-01 01:55:59.776910 dbt_loom-0.5.4/dbt_loom/config.py
+-rw-r--r--   0        0        0      396 2024-06-01 01:55:59.776910 dbt_loom-0.5.4/dbt_loom/logging.py
+-rw-r--r--   0        0        0     4748 2024-06-01 01:55:59.776910 dbt_loom-0.5.4/dbt_loom/manifests.py
+-rw-r--r--   0        0        0     1061 2024-06-01 01:55:59.776910 dbt_loom-0.5.4/pyproject.toml
+-rw-r--r--   0        0        0     7506 1970-01-01 00:00:00.000000 dbt_loom-0.5.4/PKG-INFO
```

### Comparing `dbt_loom-0.5.3/LICENSE` & `dbt_loom-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.3/README.md` & `dbt_loom-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.3/dbt_loom/__init__.py` & `dbt_loom-0.5.4/dbt_loom/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from dataclasses import dataclass
 import os
 import re
 from pathlib import Path
-from typing import Callable, Dict, Optional
+from typing import Callable, Dict, Optional, Set
 
 import yaml
 from dbt.contracts.graph.node_args import ModelNodeArgs
-
+from dbt.contracts.graph.nodes import ModelNode
 
 from dbt.plugins.manager import dbt_hook, dbtPlugin
 from dbt.plugins.manifest import PluginNodes
 from dbt.config.project import VarProvider
 
 try:
     from dbt.artifacts.resources.types import NodeType
@@ -26,24 +26,26 @@
 
 
 @dataclass
 class LoomModelNodeArgs(ModelNodeArgs):
     """A dbt-loom extension of ModelNodeArgs to preserve resource types across lineages."""
 
     resource_type: NodeType = NodeType.Model
+    group: Optional[str] = None
 
     def __init__(self, **kwargs):
         super().__init__(
             **{
                 key: value
                 for key, value in kwargs.items()
-                if key not in ("resource_type")
+                if key not in ("resource_type", "group")
             }
         )
-        self.resource_type = kwargs["resource_type"]
+        self.resource_type = kwargs.get("resource_type", NodeType.Model)
+        self.group = kwargs.get("group")
 
     @property
     def unique_id(self) -> str:
         unique_id = f"{self.resource_type}.{self.package_name}.{self.name}"
         if self.version:
             unique_id = f"{unique_id}.v{self.version}"
 
@@ -86,28 +88,29 @@
     """Generate a dictionary of ModelNodeArgs based on a dictionary of ModelNodes"""
     return {
         unique_id: LoomModelNodeArgs(
             schema=node.schema_name,
             identifier=node.identifier,
             **(
                 # Small bit of logic to support both pydantic 2 and pydantic 1
-                node.model_dump(exclude={"schema_name", "depends_on", "node_config"})
+                node.model_dump(exclude={"schema_name", "depends_on", "node_config"})  # type: ignore
                 if hasattr(node, "model_dump")
                 else node.dict(exclude={"schema_name", "depends_on", "node_config"})
             ),
         )
         for unique_id, node in selected_nodes.items()
         if node is not None
     }
 
 
+@dataclass
 class LoomRunnableConfig:
     """A shim class to allow is_invalid_*_ref functions to correctly handle access for loom-injected models."""
 
-    restrict_access: bool = True
+    restrict_access: bool = False
     vars: VarProvider = VarProvider(vars={})
 
 
 class dbtLoom(dbtPlugin):
     """
     dbtLoom is a dbt plugin that loads manifest files, parses a DAG from the manifest,
     and injects public nodes from imported manifest.
@@ -120,14 +123,15 @@
         )
 
         configuration_path = Path(
             os.environ.get("DBT_LOOM_CONFIG", "dbt_loom.config.yml")
         )
 
         self._manifest_loader = ManifestLoader()
+        self.manifests: Dict[str, Dict] = {}
 
         self.config: Optional[dbtLoomConfig] = self.read_config(configuration_path)
         self.models: Dict[str, LoomModelNodeArgs] = {}
 
         import dbt.contracts.graph.manifest
 
         fire_event(
@@ -140,26 +144,69 @@
         )
         dbt.contracts.graph.manifest.Manifest.is_invalid_private_ref = (  # type: ignore
             self.dependency_wrapper(
                 dbt.contracts.graph.manifest.Manifest.is_invalid_private_ref
             )
         )
 
+        dbt.parser.manifest.ManifestLoader.check_valid_group_config_node = (  # type: ignore
+            self.group_validation_wrapper(
+                dbt.parser.manifest.ManifestLoader.check_valid_group_config_node  # type: ignore
+            )
+        )
+
+        dbt.contracts.graph.nodes.ModelNode.from_args = (  # type: ignore
+            self.model_node_wrapper(dbt.contracts.graph.nodes.ModelNode.from_args)  # type: ignore
+        )
+
         super().__init__(project_name)
 
+    def model_node_wrapper(self, function) -> Callable:
+        """Wrap the ModelNode.from_args function and inject extra properties from the LoomModelNodeArgs."""
+
+        def outer_function(args: LoomModelNodeArgs) -> ModelNode:
+            model = function(args)
+            model.group = args.group
+            return model
+
+        return outer_function
+
+    def group_validation_wrapper(self, function) -> Callable:
+        """Wrap the check_valid_group_config_node function to inject upstream group names."""
+
+        def outer_function(
+            inner_self, groupable_node, valid_group_names: Set[str]
+        ) -> bool:
+            new_groups: Set[str] = {
+                model.group for model in self.models.values() if model.group is not None
+            }
+
+            return function(
+                inner_self, groupable_node, valid_group_names.union(new_groups)
+            )
+
+        return outer_function
+
     def dependency_wrapper(self, function) -> Callable:
         def outer_function(inner_self, node, target_model, dependencies) -> bool:
             if self.config is not None:
-                for manifest in self.config.manifests:
-                    dependencies[manifest.name] = LoomRunnableConfig()
+                for manifest_name in self.manifests.keys():
+                    dependencies[manifest_name] = LoomRunnableConfig()
 
             return function(inner_self, node, target_model, dependencies)
 
         return outer_function
 
+    def get_groups(self) -> Set[str]:
+        """Get all groups defined in injected models."""
+
+        return {
+            model.group for model in self.models.values() if model.group is not None
+        }
+
     def read_config(self, path: Path) -> Optional[dbtLoomConfig]:
         """Read the dbt-loom configuration file."""
         if not path.exists():
             return None
 
         with open(path) as file:
             config_content = file.read()
@@ -192,14 +239,16 @@
                 f" from `{manifest_reference.type.value}`"
             )
 
             manifest = self._manifest_loader.load(manifest_reference)
             if manifest is None:
                 continue
 
+            self.manifests[manifest_reference.name] = manifest
+
             selected_nodes = identify_node_subgraph(manifest)
             self.models.update(convert_model_nodes_to_model_node_args(selected_nodes))
 
     @dbt_hook
     def get_nodes(self) -> PluginNodes:
         """
         Inject PluginNodes to dbt for injection into dbt's DAG.
```

### Comparing `dbt_loom-0.5.3/dbt_loom/clients/az_blob.py` & `dbt_loom-0.5.4/dbt_loom/clients/az_blob.py`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.3/dbt_loom/clients/dbt_cloud.py` & `dbt_loom-0.5.4/dbt_loom/clients/dbt_cloud.py`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.3/dbt_loom/clients/gcs.py` & `dbt_loom-0.5.4/dbt_loom/clients/gcs.py`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.3/dbt_loom/clients/s3.py` & `dbt_loom-0.5.4/dbt_loom/clients/s3.py`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.3/dbt_loom/config.py` & `dbt_loom-0.5.4/dbt_loom/config.py`

 * *Files identical despite different names*

### Comparing `dbt_loom-0.5.3/dbt_loom/manifests.py` & `dbt_loom-0.5.4/dbt_loom/manifests.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     schema_name: str = Field(alias="schema")
     database: Optional[str] = None
     relation_name: Optional[str] = None
     version: Optional[str] = None
     latest_version: Optional[str] = None
     deprecation_date: Optional[datetime.datetime] = None
     access: Optional[str] = "protected"
+    group: Optional[str] = None
     generated_at: datetime.datetime = Field(default_factory=datetime.datetime.utcnow)
     depends_on: Optional[DependsOn] = None
     depends_on_nodes: List[str] = Field(default_factory=list)
     enabled: bool = True
 
     @validator("depends_on_nodes", always=True)
     def default_depends_on_nodes(cls, v, values):
```

### Comparing `dbt_loom-0.5.3/pyproject.toml` & `dbt_loom-0.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [tool.poetry]
 name = "dbt-loom"
-version = "0.5.3"
+version = "0.5.4"
 description = "A dbt-core plugin to import public nodes in multi-project deployments."
 authors = ["Nicholas Yager <yager@nicholasyager.com>"]
 readme = "README.md"
 packages = [{ include = "dbt_loom" }]
 
 [tool.commitizen]
-version = "0.5.3"
+version = "0.5.4"
 version_files = ["pyproject.toml:^version"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 dbt-core = ">=1.6.0,<=1.8.0"
 requests = "^2.31.0"
 google-cloud-storage = "^2.13.0"
```

### Comparing `dbt_loom-0.5.3/PKG-INFO` & `dbt_loom-0.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-loom
-Version: 0.5.3
+Version: 0.5.4
 Summary: A dbt-core plugin to import public nodes in multi-project deployments.
 Author: Nicholas Yager
 Author-email: yager@nicholasyager.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

