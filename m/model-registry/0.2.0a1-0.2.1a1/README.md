# Comparing `tmp/model_registry-0.2.0a1.tar.gz` & `tmp/model_registry-0.2.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_registry-0.2.0a1.tar", max compression
+gzip compressed data, was "model_registry-0.2.1a1.tar", max compression
```

## Comparing `model_registry-0.2.0a1.tar` & `model_registry-0.2.1a1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3938 2024-05-03 07:28:51.288530 model_registry-0.2.0a1/README.md
--rw-r--r--   0        0        0     2249 2024-05-03 07:28:51.288530 model_registry-0.2.0a1/pyproject.toml
--rw-r--r--   0        0        0      142 2024-05-03 07:28:51.288530 model_registry-0.2.0a1/src/model_registry/__init__.py
--rw-r--r--   0        0        0     9350 2024-05-03 07:28:51.288530 model_registry-0.2.0a1/src/model_registry/_client.py
--rw-r--r--   0        0        0     3540 2024-05-03 07:28:51.288530 model_registry-0.2.0a1/src/model_registry/_utils.py
--rw-r--r--   0        0        0    12220 2024-05-03 07:28:51.288530 model_registry-0.2.0a1/src/model_registry/core.py
--rw-r--r--   0        0        0      624 2024-05-03 07:28:51.288530 model_registry-0.2.0a1/src/model_registry/exceptions.py
--rw-r--r--   0        0        0      178 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/store/__init__.py
--rw-r--r--   0        0        0      347 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/store/base.py
--rw-r--r--   0        0        0    11616 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/store/wrapper.py
--rw-r--r--   0        0        0      503 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/types/__init__.py
--rw-r--r--   0        0        0     4386 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/types/artifacts.py
--rw-r--r--   0        0        0     5831 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/types/base.py
--rw-r--r--   0        0        0     4302 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/types/contexts.py
--rw-r--r--   0        0        0     1266 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/types/options.py
--rw-r--r--   0        0        0     2405 2024-05-03 07:28:51.292530 model_registry-0.2.0a1/src/model_registry/utils.py
--rw-r--r--   0        0        0     4749 1970-01-01 00:00:00.000000 model_registry-0.2.0a1/PKG-INFO
+-rw-r--r--   0        0        0     4083 2024-06-01 18:50:04.009593 model_registry-0.2.1a1/README.md
+-rw-r--r--   0        0        0     2286 2024-06-01 18:50:04.013593 model_registry-0.2.1a1/pyproject.toml
+-rw-r--r--   0        0        0      142 2024-06-01 18:50:04.013593 model_registry-0.2.1a1/src/model_registry/__init__.py
+-rw-r--r--   0        0        0    10480 2024-06-01 18:50:04.013593 model_registry-0.2.1a1/src/model_registry/_client.py
+-rw-r--r--   0        0        0     3540 2024-06-01 18:50:04.013593 model_registry-0.2.1a1/src/model_registry/_utils.py
+-rw-r--r--   0        0        0    13181 2024-06-01 18:50:04.013593 model_registry-0.2.1a1/src/model_registry/core.py
+-rw-r--r--   0        0        0      624 2024-06-01 18:50:04.013593 model_registry-0.2.1a1/src/model_registry/exceptions.py
+-rw-r--r--   0        0        0      178 2024-06-01 18:50:04.013593 model_registry-0.2.1a1/src/model_registry/store/__init__.py
+-rw-r--r--   0        0        0      347 2024-06-01 18:50:04.013593 model_registry-0.2.1a1/src/model_registry/store/base.py
+-rw-r--r--   0        0        0    12262 2024-06-01 18:50:04.013593 model_registry-0.2.1a1/src/model_registry/store/wrapper.py
+-rw-r--r--   0        0        0      503 2024-06-01 18:50:04.013593 model_registry-0.2.1a1/src/model_registry/types/__init__.py
+-rw-r--r--   0        0        0     4386 2024-06-01 18:50:04.013593 model_registry-0.2.1a1/src/model_registry/types/artifacts.py
+-rw-r--r--   0        0        0     5831 2024-06-01 18:50:04.013593 model_registry-0.2.1a1/src/model_registry/types/base.py
+-rw-r--r--   0        0        0     4671 2024-06-01 18:50:04.013593 model_registry-0.2.1a1/src/model_registry/types/contexts.py
+-rw-r--r--   0        0        0     1266 2024-06-01 18:50:04.013593 model_registry-0.2.1a1/src/model_registry/types/options.py
+-rw-r--r--   0        0        0     5532 2024-06-01 18:50:04.013593 model_registry-0.2.1a1/src/model_registry/utils.py
+-rw-r--r--   0        0        0     4894 1970-01-01 00:00:00.000000 model_registry-0.2.1a1/PKG-INFO
```

### Comparing `model_registry-0.2.0a1/README.md` & `model_registry-0.2.1a1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 This library provides a high level interface for interacting with a model registry server.
 
 ## Basic usage
 
 ```py
 from model_registry import ModelRegistry
 
-registry = ModelRegistry(server_address="server-address", port=9090, author="author")
+registry = ModelRegistry("server-address", author="Ada Lovelace")  # Defaults to a secure connection via port 443
+
+# registry = ModelRegistry("server-address", 1234, author="Ada Lovelace", is_secure=False)  # To use MR without TLS
 
 model = registry.register_model(
     "my-model",  # model name
     "https://storage-place.my-company.com",  # model URI
     version="2.0.0",
     description="lorem ipsum",
     model_format_name="onnx",
```

### Comparing `model_registry-0.2.0a1/pyproject.toml` & `model_registry-0.2.1a1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "model-registry"
-version = "0.2.0a1"
+version = "0.2.1a1"
 description = "Client for Kubeflow Model Registry"
 authors = ["Isabella Basso do Amaral <idoamara@redhat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/kubeflow/model-registry"
 
 [tool.poetry.urls]
@@ -14,28 +14,28 @@
 python = ">= 3.9, < 3.11"
 attrs = "^21.0"
 ml-metadata = "^1.14.0"
 # you might consider using locally the following alternative, when developing on Apple-silicon/ARM-based computers:
 # ml-metadata = { url = "https://github.com/opendatahub-io/ml-metadata/releases/download/v1.14.0%2Bremote.1/ml_metadata-1.14.0+remote.1-py3-none-any.whl" }
 typing-extensions = "^4.8"
 
-huggingface-hub = { version = "^0.20.1", optional = true }
+huggingface-hub = { version = ">=0.20.1,<0.24.0", optional = true }
 
 [tool.poetry.extras]
 hf = ["huggingface-hub"]
 
 [tool.poetry.group.dev.dependencies]
 sphinx = "^7.2.6"
-furo = "^2023.9.10"
+furo = ">=2023.9.10,<2025.0.0"
 myst-parser = { extras = ["linkify"], version = "^2.0.0" }
-pytest = "^7.4.2"
+pytest = ">=7.4.2,<9.0.0"
 coverage = { extras = ["toml"], version = "^7.3.2" }
 pytest-cov = "^4.1.0"
-sphinx-autobuild = "^2021.3.14"
-ruff = "^0.1.6"
+sphinx-autobuild = ">=2021.3.14,<2025.0.0"
+ruff = "^0.4.4"
 mypy = "^1.7.0"
 testcontainers = "^3.7.1"
 
 [tool.coverage.run]
 branch = true
 source = ["model_registry"]
 
@@ -51,14 +51,17 @@
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 119
 
 [tool.ruff]
 target-version = "py39"
+respect-gitignore = true
+
+[tool.ruff.lint]
 select = [
     "F", # pyflakes
     # pycodestyle
     "W", # warnings
     "E", # errors
 
     "C90", # mccabe
@@ -71,24 +74,19 @@
     "I",   # isort
     "PT",  # pytest
     "Q",   # flake8-quotes
     "RET", # flake8-return
     "SIM", # flake8-simplify
     "UP",  # pyupgrade
 ]
-respect-gitignore = true
 ignore = [
     "D105", # missing docstring in magic method
     "E501", # line too long
     "S101", # use of assert detected
 ]
+mccabe.max-complexity = 8
+per-file-ignores = { "tests/**/*.py" = [
+    "D", # missing docstring in public module
+] }
 
 [tool.ruff.lint.pydocstyle]
 convention = "google"
-
-[tool.ruff.per-file-ignores]
-"tests/**/*.py" = [
-    "D", # missing docstring in public module
-]
-
-[tool.ruff.mccabe]
-max-complexity = 8
```

### Comparing `model_registry-0.2.0a1/src/model_registry/_client.py` & `model_registry-0.2.1a1/src/model_registry/_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Standard client for the model registry."""
 
 from __future__ import annotations
 
+import os
+from pathlib import Path
 from typing import get_args
 from warnings import warn
 
 from .core import ModelRegistryAPIClient
 from .exceptions import StoreException
 from .store import ScalarType
 from .types import ModelArtifact, ModelVersion, RegisteredModel
@@ -13,35 +15,63 @@
 
 class ModelRegistry:
     """Model registry client."""
 
     def __init__(
         self,
         server_address: str,
-        port: int,
+        port: int = 443,
+        *,
         author: str,
-        client_key: str | None = None,
-        server_cert: str | None = None,
-        custom_ca: str | None = None,
+        is_secure: bool = True,
+        user_token: bytes | None = None,
+        custom_ca: bytes | None = None,
     ):
         """Constructor.
 
         Args:
             server_address: Server address.
-            port: Server port.
+            port: Server port. Defaults to 443.
+
+        Keyword Args:
             author: Name of the author.
-            client_key: The PEM-encoded private key as a byte string.
-            server_cert: The PEM-encoded certificate as a byte string.
-            custom_ca: The PEM-encoded root certificates as a byte string.
+            is_secure: Whether to use a secure connection. Defaults to True.
+            user_token: The PEM-encoded user token as a byte string. Defaults to content of path on envvar KF_PIPELINES_SA_TOKEN_PATH.
+            custom_ca: The PEM-encoded root certificates as a byte string. Defaults to contents of path on envvar CERT.
         """
-        # TODO: get args from env
+        # TODO: get remaining args from env
         self._author = author
-        self._api = ModelRegistryAPIClient(
-            server_address, port, client_key, server_cert, custom_ca
-        )
+
+        if not user_token:
+            # /var/run/secrets/kubernetes.io/serviceaccount/token
+            sa_token = os.environ.get("KF_PIPELINES_SA_TOKEN_PATH")
+            if sa_token:
+                user_token = Path(sa_token).read_bytes()
+            else:
+                warn("User access token is missing", stacklevel=2)
+
+        if is_secure:
+            root_ca = None
+            if not custom_ca:
+                if ca_path := os.getenv("CERT"):
+                    root_ca = Path(ca_path).read_bytes()
+                    # client might have a default CA setup
+            else:
+                root_ca = custom_ca
+
+            self._api = ModelRegistryAPIClient.secure_connection(
+                server_address, port, user_token, root_ca
+            )
+        elif custom_ca:
+            msg = "Custom CA provided without secure connection"
+            raise StoreException(msg)
+        else:
+            self._api = ModelRegistryAPIClient.insecure_connection(
+                server_address, port, user_token
+            )
 
     def _register_model(self, name: str) -> RegisteredModel:
         if rm := self._api.get_registered_model_by_params(name):
             return rm
 
         rm = RegisteredModel(name)
         self._api.upsert_registered_model(rm)
```

### Comparing `model_registry-0.2.0a1/src/model_registry/_utils.py` & `model_registry-0.2.1a1/src/model_registry/_utils.py`

 * *Files identical despite different names*

### Comparing `model_registry-0.2.0a1/src/model_registry/core.py` & `model_registry-0.2.1a1/src/model_registry/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,63 +1,97 @@
 """Client for the model registry."""
 
 from __future__ import annotations
 
-from ml_metadata.proto import MetadataStoreClientConfig
+from dataclasses import dataclass
+
+import grpc
 
 from .exceptions import StoreException
 from .store import MLMDStore, ProtoType
 from .types import ListOptions, ModelArtifact, ModelVersion, RegisteredModel
 from .types.base import ProtoBase
 from .types.options import MLMDListOptions
+from .utils import header_adder_interceptor
 
 
+@dataclass
 class ModelRegistryAPIClient:
     """Model registry API."""
 
-    def __init__(
-        self,
+    store: MLMDStore
+
+    @classmethod
+    def secure_connection(
+        cls,
+        server_address: str,
+        port: int = 443,
+        user_token: bytes | None = None,
+        custom_ca: bytes | None = None,
+    ) -> ModelRegistryAPIClient:
+        """Constructor.
+
+        Args:
+            server_address: Server address.
+            port: Server port. Defaults to 443.
+            user_token: The PEM-encoded user token as a byte string.
+            custom_ca: The PEM-encoded root certificates as a byte string. Defaults to GRPC_DEFAULT_SSL_ROOTS_FILE_PATH, then system default.
+        """
+        if not user_token:
+            msg = "user token must be provided for secure connection"
+            raise StoreException(msg)
+
+        chan = grpc.secure_channel(
+            f"{server_address}:{port}",
+            grpc.composite_channel_credentials(
+                # custom_ca = None will get the default root certificates
+                grpc.ssl_channel_credentials(custom_ca),
+                grpc.access_token_call_credentials(user_token),
+            ),
+        )
+
+        return cls(MLMDStore.from_channel(chan))
+
+    @classmethod
+    def insecure_connection(
+        cls,
         server_address: str,
         port: int,
-        client_key: str | None = None,
-        server_cert: str | None = None,
-        custom_ca: str | None = None,
-    ):
+        user_token: bytes | None = None,
+    ) -> ModelRegistryAPIClient:
         """Constructor.
 
         Args:
             server_address: Server address.
             port: Server port.
-            client_key: The PEM-encoded private key as a byte string.
-            server_cert: The PEM-encoded certificate as a byte string.
-            custom_ca: The PEM-encoded root certificates as a byte string.
-        """
-        config = MetadataStoreClientConfig()
-        config.host = server_address
-        config.port = port
-        if client_key is not None:
-            config.ssl_config.client_key = client_key
-        if server_cert is not None:
-            config.ssl_config.server_cert = server_cert
-        if custom_ca is not None:
-            config.ssl_config.custom_ca = custom_ca
-        self._store = MLMDStore(config)
+            user_token: The PEM-encoded user token as a byte string.
+        """
+        if user_token:
+            chan = grpc.intercept_channel(
+                grpc.insecure_channel(f"{server_address}:{port}"),
+                # header key has to be lowercase
+                header_adder_interceptor("authorization", f"Bearer {user_token}"),
+            )
+        else:
+            chan = grpc.insecure_channel(f"{server_address}:{port}")
+
+        return cls(MLMDStore.from_channel(chan))
 
     def _map(self, py_obj: ProtoBase) -> ProtoType:
         """Map a Python object to a proto object.
 
         Helper around the `map` method of the Python object.
 
         Args:
             py_obj: Python object.
 
         Returns:
             Proto object.
         """
-        type_id = self._store.get_type_id(
+        type_id = self.store.get_type_id(
             py_obj.get_proto_type(), py_obj.get_proto_type_name()
         )
         return py_obj.map(type_id)
 
     def upsert_registered_model(self, registered_model: RegisteredModel) -> str:
         """Upsert a registered model.
 
@@ -66,17 +100,17 @@
 
         Args:
             registered_model: Registered model.
 
         Returns:
             ID of the registered model.
         """
-        id = self._store.put_context(self._map(registered_model))
+        id = self.store.put_context(self._map(registered_model))
         new_py_rm = RegisteredModel.unmap(
-            self._store.get_context(RegisteredModel.get_proto_type_name(), id)
+            self.store.get_context(RegisteredModel.get_proto_type_name(), id)
         )
         id = str(id)
         registered_model.id = id
         registered_model.create_time_since_epoch = new_py_rm.create_time_since_epoch
         registered_model.last_update_time_since_epoch = (
             new_py_rm.last_update_time_since_epoch
         )
@@ -87,15 +121,15 @@
 
         Args:
             id: Registered model ID.
 
         Returns:
             Registered model.
         """
-        proto_rm = self._store.get_context(
+        proto_rm = self.store.get_context(
             RegisteredModel.get_proto_type_name(), id=int(id)
         )
         if proto_rm is not None:
             return RegisteredModel.unmap(proto_rm)
 
         return None
 
@@ -113,15 +147,15 @@
 
         Raises:
             StoreException: If neither name nor external ID is provided.
         """
         if name is None and external_id is None:
             msg = "Either name or external_id must be provided"
             raise StoreException(msg)
-        proto_rm = self._store.get_context(
+        proto_rm = self.store.get_context(
             RegisteredModel.get_proto_type_name(),
             name=name,
             external_id=external_id,
         )
         if proto_rm is not None:
             return RegisteredModel.unmap(proto_rm)
 
@@ -135,15 +169,15 @@
         Args:
             options: Options for listing registered models.
 
         Returns:
             Registered models.
         """
         mlmd_options = options.as_mlmd_list_options() if options else MLMDListOptions()
-        proto_rms = self._store.get_contexts(
+        proto_rms = self.store.get_contexts(
             RegisteredModel.get_proto_type_name(), mlmd_options
         )
         return [RegisteredModel.unmap(proto_rm) for proto_rm in proto_rms]
 
     def upsert_model_version(
         self, model_version: ModelVersion, registered_model_id: str
     ) -> str:
@@ -157,18 +191,18 @@
             registered_model_id: ID of the registered model this version will be associated to.
 
         Returns:
             ID of the model version.
         """
         # this is not ideal but we need this info for the prefix
         model_version._registered_model_id = registered_model_id
-        id = self._store.put_context(self._map(model_version))
-        self._store.put_context_parent(int(registered_model_id), id)
+        id = self.store.put_context(self._map(model_version))
+        self.store.put_context_parent(int(registered_model_id), id)
         new_py_mv = ModelVersion.unmap(
-            self._store.get_context(ModelVersion.get_proto_type_name(), id)
+            self.store.get_context(ModelVersion.get_proto_type_name(), id)
         )
         id = str(id)
         model_version.id = id
         model_version.create_time_since_epoch = new_py_mv.create_time_since_epoch
         model_version.last_update_time_since_epoch = (
             new_py_mv.last_update_time_since_epoch
         )
@@ -179,15 +213,15 @@
 
         Args:
             model_version_id: Model version ID.
 
         Returns:
             Model version.
         """
-        proto_mv = self._store.get_context(
+        proto_mv = self.store.get_context(
             ModelVersion.get_proto_type_name(), id=int(model_version_id)
         )
         if proto_mv is not None:
             return ModelVersion.unmap(proto_mv)
 
         return None
 
@@ -203,15 +237,15 @@
         Returns:
             Model versions.
         """
         mlmd_options = options.as_mlmd_list_options() if options else MLMDListOptions()
         mlmd_options.filter_query = f"parent_contexts_a.id = {registered_model_id}"
         return [
             ModelVersion.unmap(proto_mv)
-            for proto_mv in self._store.get_contexts(
+            for proto_mv in self.store.get_contexts(
                 ModelVersion.get_proto_type_name(), mlmd_options
             )
         ]
 
     def get_model_version_by_params(
         self,
         registered_model_id: str | None = None,
@@ -230,24 +264,24 @@
         Returns:
             Model version.
 
         Raises:
             StoreException: If neither external ID nor registered model ID and version is provided.
         """
         if external_id is not None:
-            proto_mv = self._store.get_context(
+            proto_mv = self.store.get_context(
                 ModelVersion.get_proto_type_name(), external_id=external_id
             )
         elif registered_model_id is None or version is None:
             msg = (
                 "Either registered_model_id and version or external_id must be provided"
             )
             raise StoreException(msg)
         else:
-            proto_mv = self._store.get_context(
+            proto_mv = self.store.get_context(
                 ModelVersion.get_proto_type_name(),
                 name=f"{registered_model_id}:{version}",
             )
         if proto_mv is not None:
             return ModelVersion.unmap(proto_mv)
 
         return None
@@ -267,25 +301,25 @@
         Returns:
             ID of the model artifact.
 
         Raises:
             StoreException: If the model version already has a model artifact.
         """
         mv_id = int(model_version_id)
-        if self._store.get_attributed_artifact(
+        if self.store.get_attributed_artifact(
             ModelArtifact.get_proto_type_name(), mv_id
         ):
             msg = f"Model version with ID {mv_id} already has a model artifact"
             raise StoreException(msg)
 
         model_artifact._model_version_id = model_version_id
-        id = self._store.put_artifact(self._map(model_artifact))
-        self._store.put_attribution(mv_id, id)
+        id = self.store.put_artifact(self._map(model_artifact))
+        self.store.put_attribution(mv_id, id)
         new_py_ma = ModelArtifact.unmap(
-            self._store.get_artifact(ModelArtifact.get_proto_type_name(), id)
+            self.store.get_artifact(ModelArtifact.get_proto_type_name(), id)
         )
         id = str(id)
         model_artifact.id = id
         model_artifact.create_time_since_epoch = new_py_ma.create_time_since_epoch
         model_artifact.last_update_time_since_epoch = (
             new_py_ma.last_update_time_since_epoch
         )
@@ -296,17 +330,15 @@
 
         Args:
             id: Model artifact ID.
 
         Returns:
             Model artifact.
         """
-        proto_ma = self._store.get_artifact(
-            ModelArtifact.get_proto_type_name(), int(id)
-        )
+        proto_ma = self.store.get_artifact(ModelArtifact.get_proto_type_name(), int(id))
         if proto_ma is not None:
             return ModelArtifact.unmap(proto_ma)
 
         return None
 
     def get_model_artifact_by_params(
         self, model_version_id: str | None = None, external_id: str | None = None
@@ -320,22 +352,22 @@
         Returns:
             Model artifact.
 
         Raises:
             StoreException: If neither external ID nor model version ID is provided.
         """
         if external_id:
-            proto_ma = self._store.get_artifact(
+            proto_ma = self.store.get_artifact(
                 ModelArtifact.get_proto_type_name(), external_id=external_id
             )
         elif not model_version_id:
             msg = "Either model_version_id or external_id must be provided"
             raise StoreException(msg)
         else:
-            proto_ma = self._store.get_attributed_artifact(
+            proto_ma = self.store.get_attributed_artifact(
                 ModelArtifact.get_proto_type_name(), int(model_version_id)
             )
         if proto_ma is not None:
             return ModelArtifact.unmap(proto_ma)
 
         return None
 
@@ -353,11 +385,11 @@
         Returns:
             Model artifacts.
         """
         mlmd_options = options.as_mlmd_list_options() if options else MLMDListOptions()
         if model_version_id is not None:
             mlmd_options.filter_query = f"contexts_a.id = {model_version_id}"
 
-        proto_mas = self._store.get_artifacts(
+        proto_mas = self.store.get_artifacts(
             ModelArtifact.get_proto_type_name(), mlmd_options
         )
         return [ModelArtifact.unmap(proto_ma) for proto_ma in proto_mas]
```

### Comparing `model_registry-0.2.0a1/src/model_registry/exceptions.py` & `model_registry-0.2.1a1/src/model_registry/exceptions.py`

 * *Files identical despite different names*

### Comparing `model_registry-0.2.0a1/src/model_registry/store/wrapper.py` & `model_registry-0.2.1a1/src/model_registry/store/wrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,47 +1,74 @@
 """MLMD storage backend wrapper."""
 
 from __future__ import annotations
 
 from collections.abc import Sequence
+from dataclasses import dataclass
 from typing import ClassVar
 
+from grpc import Channel
 from ml_metadata import errors
 from ml_metadata.metadata_store import ListOptions, MetadataStore
 from ml_metadata.proto import (
     Artifact,
     Attribution,
     Context,
     MetadataStoreClientConfig,
     ParentContext,
 )
+from ml_metadata.proto.metadata_store_service_pb2_grpc import MetadataStoreServiceStub
 
 from model_registry.exceptions import (
     DuplicateException,
     ServerException,
     StoreException,
     TypeNotFoundException,
 )
 
 from .base import ProtoType
 
 
+@dataclass
 class MLMDStore:
     """MLMD storage backend."""
 
+    store: MetadataStore
     # cache for MLMD type IDs
     _type_ids: ClassVar[dict[str, int]] = {}
 
-    def __init__(self, config: MetadataStoreClientConfig):
+    @classmethod
+    def from_config(cls, host: str, port: int):
         """Constructor.
 
         Args:
-            config: MLMD config.
+            host: MLMD store server host.
+            port: MLMD store server port.
         """
-        self._mlmd_store = MetadataStore(config)
+        return cls(
+            MetadataStore(
+                MetadataStoreClientConfig(
+                    host=host,
+                    port=port,
+                )
+            )
+        )
+
+    @classmethod
+    def from_channel(cls, chan: Channel):
+        """Constructor.
+
+        Args:
+            chan: gRPC channel to the MLMD store.
+        """
+        store = MetadataStore(
+            MetadataStoreClientConfig(host="localhost", port=8080),
+        )
+        store._metadata_store_stub = MetadataStoreServiceStub(chan)
+        return cls(store)
 
     def get_type_id(self, pt: type[ProtoType], type_name: str) -> int:
         """Get backend ID for a type.
 
         Args:
             pt: Proto type.
             type_name: Name of the type.
@@ -55,15 +82,15 @@
         """
         if type_name in self._type_ids:
             return self._type_ids[type_name]
 
         pt_name = pt.__name__.lower()
 
         try:
-            _type = getattr(self._mlmd_store, f"get_{pt_name}_type")(type_name)
+            _type = getattr(self.store, f"get_{pt_name}_type")(type_name)
         except errors.NotFoundError as e:
             msg = f"{pt_name} type {type_name} does not exist"
             raise TypeNotFoundException(msg) from e
         except errors.InternalError as e:
             msg = f"Couldn't get {pt_name} type {type_name} from MLMD store"
             raise ServerException(msg) from e
 
@@ -81,15 +108,15 @@
 
         Raises:
             DuplicateException: If an artifact with the same name or external id already exists.
             TypeNotFoundException: If the type doesn't exist.
             StoreException: If the artifact isn't properly formed.
         """
         try:
-            return self._mlmd_store.put_artifacts([artifact])[0]
+            return self.store.put_artifacts([artifact])[0]
         except errors.AlreadyExistsError as e:
             msg = f"Artifact {artifact.name} already exists"
             raise DuplicateException(msg) from e
         except errors.InvalidArgumentError as e:
             msg = "Artifact has invalid properties"
             raise StoreException(msg) from e
         except errors.NotFoundError as e:
@@ -107,15 +134,15 @@
 
         Raises:
             DuplicateException: If a context with the same name or external id already exists.
             TypeNotFoundException: If the type doesn't exist.
             StoreException: If the context isn't propertly formed.
         """
         try:
-            return self._mlmd_store.put_contexts([context])[0]
+            return self.store.put_contexts([context])[0]
         except errors.AlreadyExistsError as e:
             msg = f"Context {context.name} already exists"
             raise DuplicateException(msg) from e
         except errors.InvalidArgumentError as e:
             msg = "Context has invalid properties"
             raise StoreException(msg) from e
         except errors.NotFoundError as e:
@@ -148,20 +175,20 @@
         Returns:
             Context.
 
         Raises:
             StoreException: Invalid arguments.
         """
         if name is not None:
-            return self._mlmd_store.get_context_by_type_and_name(ctx_type_name, name)
+            return self.store.get_context_by_type_and_name(ctx_type_name, name)
 
         if id is not None:
-            contexts = self._mlmd_store.get_contexts_by_id([id])
+            contexts = self.store.get_contexts_by_id([id])
         elif external_id is not None:
-            contexts = self._mlmd_store.get_contexts_by_external_ids([external_id])
+            contexts = self.store.get_contexts_by_external_ids([external_id])
         else:
             msg = "Either id, name or external_id must be provided"
             raise StoreException(msg)
 
         contexts = self._filter_type(ctx_type_name, contexts)
         if contexts:
             return contexts[0]
@@ -182,28 +209,28 @@
             TypeNotFoundException: If the type doesn't exist.
             ServerException: If there was an error getting the type.
             StoreException: Invalid arguments.
         """
         # TODO: should we make options optional?
         # if options is not None:
         try:
-            contexts = self._mlmd_store.get_contexts(options)
+            contexts = self.store.get_contexts(options)
         except errors.InvalidArgumentError as e:
             msg = f"Invalid arguments for get_contexts: {e}"
             raise StoreException(msg) from e
         except errors.InternalError as e:
             msg = "Couldn't get contexts from MLMD store"
             raise ServerException(msg) from e
 
         contexts = self._filter_type(ctx_type_name, contexts)
         # else:
-        #     contexts = self._mlmd_store.get_contexts_by_type(ctx_type_name)
+        #     contexts = self.store.get_contexts_by_type(ctx_type_name)
 
         if not contexts and ctx_type_name not in [
-            t.name for t in self._mlmd_store.get_context_types()
+            t.name for t in self.store.get_context_types()
         ]:
             msg = f"Context type {ctx_type_name} does not exist"
             raise TypeNotFoundException(msg)
 
         return contexts
 
     def put_context_parent(self, parent_id: int, child_id: int):
@@ -214,15 +241,15 @@
             child_id: ID of the child context.
 
         Raises:
             StoreException: If the parent context doesn't exist.
             ServerException: If there was an error putting the parent context.
         """
         try:
-            self._mlmd_store.put_parent_contexts(
+            self.store.put_parent_contexts(
                 [ParentContext(parent_id=parent_id, child_id=child_id)]
             )
         except errors.AlreadyExistsError as e:
             msg = f"Parent context {parent_id} already exists for context {child_id}"
             raise StoreException(msg) from e
         except errors.InternalError as e:
             msg = f"Couldn't put parent context {parent_id} for context {child_id}"
@@ -236,15 +263,15 @@
             artifact_id: ID of the artifact.
 
         Raises:
             StoreException: Invalid argument.
         """
         attribution = Attribution(context_id=context_id, artifact_id=artifact_id)
         try:
-            self._mlmd_store.put_attributions_and_associations([attribution], [])
+            self.store.put_attributions_and_associations([attribution], [])
         except errors.InvalidArgumentError as e:
             if "artifact" in str(e).lower():
                 msg = f"Artifact with ID {artifact_id} does not exist"
                 raise StoreException(msg) from e
 
             if "context" in str(e).lower():
                 msg = f"Context with ID {context_id} does not exist"
@@ -273,20 +300,20 @@
         Returns:
             Artifact.
 
         Raises:
             StoreException: Invalid arguments.
         """
         if name is not None:
-            return self._mlmd_store.get_artifact_by_type_and_name(art_type_name, name)
+            return self.store.get_artifact_by_type_and_name(art_type_name, name)
 
         if id is not None:
-            artifacts = self._mlmd_store.get_artifacts_by_id([id])
+            artifacts = self.store.get_artifacts_by_id([id])
         elif external_id is not None:
-            artifacts = self._mlmd_store.get_artifacts_by_external_ids([external_id])
+            artifacts = self.store.get_artifacts_by_external_ids([external_id])
         else:
             msg = "Either id, name or external_id must be provided"
             raise StoreException(msg)
 
         artifacts = self._filter_type(art_type_name, artifacts)
         if artifacts:
             return artifacts[0]
@@ -300,15 +327,15 @@
             art_type_name: Name of the artifact type.
             ctx_id: ID of the context.
 
         Returns:
             Artifact.
         """
         try:
-            artifacts = self._mlmd_store.get_artifacts_by_context(ctx_id)
+            artifacts = self.store.get_artifacts_by_context(ctx_id)
         except errors.InternalError as e:
             msg = f"Couldn't get artifacts by context {ctx_id}"
             raise ServerException(msg) from e
         artifacts = self._filter_type(art_type_name, artifacts)
         if artifacts:
             return artifacts[0]
 
@@ -326,23 +353,23 @@
 
         Raises:
             TypeNotFoundException: If the type doesn't exist.
             ServerException: If there was an error getting the type.
             StoreException: Invalid arguments.
         """
         try:
-            artifacts = self._mlmd_store.get_artifacts(options)
+            artifacts = self.store.get_artifacts(options)
         except errors.InvalidArgumentError as e:
             msg = f"Invalid arguments for get_artifacts: {e}"
             raise StoreException(msg) from e
         except errors.InternalError as e:
             msg = "Couldn't get artifacts from MLMD store"
             raise ServerException(msg) from e
 
         artifacts = self._filter_type(art_type_name, artifacts)
         if not artifacts and art_type_name not in [
-            t.name for t in self._mlmd_store.get_artifact_types()
+            t.name for t in self.store.get_artifact_types()
         ]:
             msg = f"Artifact type {art_type_name} does not exist"
             raise TypeNotFoundException(msg)
 
         return artifacts
```

### Comparing `model_registry-0.2.0a1/src/model_registry/types/artifacts.py` & `model_registry-0.2.1a1/src/model_registry/types/artifacts.py`

 * *Files identical despite different names*

### Comparing `model_registry-0.2.0a1/src/model_registry/types/base.py` & `model_registry-0.2.1a1/src/model_registry/types/base.py`

 * *Files identical despite different names*

### Comparing `model_registry-0.2.0a1/src/model_registry/types/contexts.py` & `model_registry-0.2.1a1/src/model_registry/types/contexts.py`

 * *Files 8% similar despite different names*

```diff
@@ -125,21 +125,33 @@
 
 @define(slots=False)
 class RegisteredModel(BaseContext):
     """Represents a registered model.
 
     Attributes:
         name: Registered model name.
+        owner: Owner of this Registered Model.
         description: Description of the object.
         external_id: Customizable ID. Has to be unique among instances of the same type.
     """
 
     name: str
+    owner: str = None
+
+    @override
+    def map(self, type_id: int) -> Context:
+        mlmd_obj = super().map(type_id)
+        props = {
+            "owner": self.owner
+        }
+        self._map_props(props, mlmd_obj.properties)
+        return mlmd_obj
 
     @classmethod
     @override
     def unmap(cls, mlmd_obj: Context) -> RegisteredModel:
         py_obj = super().unmap(mlmd_obj)
         assert isinstance(
             py_obj, RegisteredModel
         ), f"Expected RegisteredModel, got {type(py_obj)}"
+        py_obj.owner = mlmd_obj.properties["owner"].string_value
         return py_obj
```

### Comparing `model_registry-0.2.0a1/src/model_registry/types/options.py` & `model_registry-0.2.1a1/src/model_registry/types/options.py`

 * *Files identical despite different names*

### Comparing `model_registry-0.2.0a1/PKG-INFO` & `model_registry-0.2.1a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: model-registry
-Version: 0.2.0a1
+Version: 0.2.1a1
 Summary: Client for Kubeflow Model Registry
 Home-page: https://github.com/kubeflow/model-registry
 License: Apache-2.0
 Author: Isabella Basso do Amaral
 Author-email: idoamara@redhat.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: hf
 Requires-Dist: attrs (>=21.0,<22.0)
-Requires-Dist: huggingface-hub (>=0.20.1,<0.21.0) ; extra == "hf"
+Requires-Dist: huggingface-hub (>=0.20.1,<0.24.0) ; extra == "hf"
 Requires-Dist: ml-metadata (>=1.14.0,<2.0.0)
 Requires-Dist: typing-extensions (>=4.8,<5.0)
 Project-URL: Issues, https://github.com/kubeflow/model-registry/issues
 Description-Content-Type: text/markdown
 
 # Model Registry Python Client
 
@@ -27,15 +27,17 @@
 This library provides a high level interface for interacting with a model registry server.
 
 ## Basic usage
 
 ```py
 from model_registry import ModelRegistry
 
-registry = ModelRegistry(server_address="server-address", port=9090, author="author")
+registry = ModelRegistry("server-address", author="Ada Lovelace")  # Defaults to a secure connection via port 443
+
+# registry = ModelRegistry("server-address", 1234, author="Ada Lovelace", is_secure=False)  # To use MR without TLS
 
 model = registry.register_model(
     "my-model",  # model name
     "https://storage-place.my-company.com",  # model URI
     version="2.0.0",
     description="lorem ipsum",
     model_format_name="onnx",
```

