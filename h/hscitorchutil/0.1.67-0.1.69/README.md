# Comparing `tmp/hscitorchutil-0.1.67.tar.gz` & `tmp/hscitorchutil-0.1.69.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hscitorchutil-0.1.67.tar", max compression
+gzip compressed data, was "hscitorchutil-0.1.69.tar", max compression
```

## Comparing `hscitorchutil-0.1.67.tar` & `hscitorchutil-0.1.69.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        0 2023-10-26 13:56:57.077205 hscitorchutil-0.1.67/README.md
--rw-r--r--   0        0        0     2961 2024-01-19 12:53:41.148969 hscitorchutil-0.1.67/hscitorchutil/callbacks.py
--rw-r--r--   0        0        0     9141 2024-05-28 21:20:36.543633 hscitorchutil-0.1.67/hscitorchutil/dataset.py
--rw-r--r--   0        0        0    13146 2024-05-28 21:10:07.909175 hscitorchutil-0.1.67/hscitorchutil/fsspec.py
--rw-r--r--   0        0        0      847 2023-12-11 20:57:21.481430 hscitorchutil-0.1.67/hscitorchutil/processlocal.py
--rw-r--r--   0        0        0     8676 2024-04-18 13:19:14.770983 hscitorchutil-0.1.67/hscitorchutil/sqlite.py
--rw-r--r--   0        0        0      908 2024-05-28 21:20:43.478204 hscitorchutil-0.1.67/pyproject.toml
--rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 hscitorchutil-0.1.67/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-10-26 13:56:57.077205 hscitorchutil-0.1.69/README.md
+-rw-r--r--   0        0        0     2980 2024-06-01 14:43:53.714159 hscitorchutil-0.1.69/hscitorchutil/callbacks.py
+-rw-r--r--   0        0        0    13729 2024-06-01 14:51:32.919026 hscitorchutil-0.1.69/hscitorchutil/dataset.py
+-rw-r--r--   0        0        0    13146 2024-05-28 21:10:07.909175 hscitorchutil-0.1.69/hscitorchutil/fsspec.py
+-rw-r--r--   0        0        0      847 2023-12-11 20:57:21.481430 hscitorchutil-0.1.69/hscitorchutil/processlocal.py
+-rw-r--r--   0        0        0     7891 2024-06-01 14:40:16.874796 hscitorchutil-0.1.69/hscitorchutil/sqlite.py
+-rw-r--r--   0        0        0      908 2024-06-01 14:41:47.049982 hscitorchutil-0.1.69/pyproject.toml
+-rw-r--r--   0        0        0      924 1970-01-01 00:00:00.000000 hscitorchutil-0.1.69/PKG-INFO
```

### Comparing `hscitorchutil-0.1.67/hscitorchutil/callbacks.py` & `hscitorchutil-0.1.69/hscitorchutil/callbacks.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os
 from typing import Callable, Generic, Literal, Optional, Sequence, TypeVar
 from lightning import LightningModule, Trainer
 import lightning.pytorch as pl
 from lightning.pytorch.callbacks import Callback, BasePredictionWriter
 import torch
 
+from hscitorchutil.dataset import identity_transformation
+
 
 def _get_save_path(trainer: Trainer) -> str:
     if len(trainer.loggers) > 0 and trainer.loggers[0].save_dir is not None:
         save_dir = trainer.loggers[0].save_dir
         name = trainer.loggers[0].name
         version = trainer.loggers[0].version
         version = version if isinstance(
@@ -34,20 +36,16 @@
         torch.cuda.memory._dump_snapshot(self.save_path)
 
 
 T = TypeVar('T')
 T2 = TypeVar('T2')
 
 
-def identity_transform(x: T) -> T:
-    return x
-
-
 class PredictionWriterCallback(BasePredictionWriter, Generic[T, T2]):
-    def __init__(self, write_interval: Literal["batch", "epoch", "batch_and_epoch"] = "batch", save_path: str | None = None, transform_batch: Callable[[T], T] = identity_transform, transform_outputs: Callable[[T2], T2] = identity_transform) -> None:
+    def __init__(self, write_interval: Literal["batch", "epoch", "batch_and_epoch"] = "batch", save_path: str | None = None, transform_batch: Callable[[T], T] = identity_transformation, transform_outputs: Callable[[T2], T2] = identity_transformation) -> None:
         super().__init__(write_interval=write_interval)
         self.save_path = save_path
         self.transform_batch = transform_batch
         self.transform_outputs = transform_outputs
 
     def setup(self, trainer: pl.Trainer, pl_module: pl.LightningModule, stage: str) -> None:
         super().setup(trainer, pl_module, stage)
```

### Comparing `hscitorchutil-0.1.67/hscitorchutil/fsspec.py` & `hscitorchutil-0.1.69/hscitorchutil/fsspec.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.67/hscitorchutil/processlocal.py` & `hscitorchutil-0.1.69/hscitorchutil/processlocal.py`

 * *Files identical despite different names*

### Comparing `hscitorchutil-0.1.67/hscitorchutil/sqlite.py` & `hscitorchutil-0.1.69/hscitorchutil/sqlite.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 import logging
 import os
 import sqlite3
-from typing import Callable, Generic, Iterable, Iterator, Optional, Tuple, TypeVar, Sequence, TypeVarTuple, cast
+from typing import Callable, Generic, Iterable, Iterator, Literal, Optional, Tuple, TypeVar, Sequence, TypeVarTuple, cast
 from zipfile import ZipFile
 import click
 import fsspec
 import torch.utils.data.dataloader
 from torch.utils.data import Dataset, DataLoader
 import torch
 import lightning.pytorch
 from edzip.sqlite import create_sqlite_directory_from_zip
+from hscitorchutil.dataset import ABaseDataModule, identity_transformation
 from hscitorchutil.fsspec import get_s3fs_credentials, cache_locally_if_remote
 
 Ts = TypeVarTuple("Ts")
 T_co = TypeVar('T_co', covariant=True)
 T2_co = TypeVar('T2_co', covariant=True)
 
 
-def _identity(x: T_co) -> T_co:
-    return x
-
-
 class SQLiteDataset(Dataset[T_co], Generic[*Ts, T_co]):
     def __init__(self, sqlite_filename: str, table_name: str, index_column: str, columns_to_return: str, id_column: str):
         self.sqlite_filename = sqlite_filename
         self.table_name = table_name
         self.index_column = index_column
         self.id_column = id_column
         self.columns_to_return = columns_to_return
@@ -64,99 +61,78 @@
             self.index_column,
             self.columns_to_return,
             self.id_column,
             self._len
         )
 
 
-def _remove_nones_from_batch(batch: Sequence) -> Sequence:
-    """Removes None values from batch. Used to recover from errors."""
-    batch = list(filter(lambda x: x is not None, batch))
-    if batch:
-        try:
-            return torch.utils.data.dataloader.default_collate(batch)
-        except Exception as e:
-            logging.exception("Failed to collate batch, returning empty batch")
-            return ()
-    logging.warn("Batch is empty")
-    return ()
-
-
 class TypedDataLoader(Iterable[T_co], DataLoader[T_co], Generic[T_co]):
     pass
 
 
-class SQLiteDataModule(lightning.pytorch.LightningDataModule, Generic[*Ts, T_co, T2_co]):
+class SQLiteDataModule(ABaseDataModule[T_co, T2_co], Generic[*Ts, T_co, T2_co]):
     def __init__(self,
                  train_sqlite_url: str,
                  val_sqlite_url: str,
                  test_sqlite_url: str,
                  cache_dir: str,
                  table_name: str,
                  index_column: str,
                  columns_to_return: str,
                  id_column: str,
                  storage_options: dict = dict(),
-                 batch_size: int = 64,
-                 num_workers: int = 0,
                  train_transform: Callable[[
-                     Dataset[tuple[*Ts]]], Dataset[T_co]] = _identity,
+                     Dataset[tuple[*Ts]]], Dataset[T_co]] = identity_transformation,
                  test_transform: Callable[[
-                     Dataset[tuple[*Ts]]], Dataset[T_co]] = _identity,
-                 prepare_data_per_node: bool = True,
-                 collate_fn: Optional[Callable[[Sequence[T_co]], T2_co]] = _remove_nones_from_batch):
+                     Dataset[tuple[*Ts]]], Dataset[T_co]] = identity_transformation,
+                 **kwargs):
+        super().__init__(**kwargs)
         self.train_sqlite_url = train_sqlite_url
         self.val_sqlite_url = val_sqlite_url
         self.test_sqlite_url = test_sqlite_url
         self.cache_dir = cache_dir
         self.storage_options = storage_options
-        self.batch_size = batch_size
-        self.num_workers = num_workers
 
         self.table_name = table_name
         self.index_column = index_column
         self.columns_to_return = columns_to_return
         self.id_column = id_column
         self.train_transform = train_transform
         self.test_transform = test_transform
-        self.prepare_data_per_node = prepare_data_per_node
-        self.collate_fn = collate_fn
-        self.train_dataset = None
-        self.val_dataset = None
-        self.test_dataset = None
-        super().__init__()
 
     def prepare_data(self):
         # download, IO, etc. Useful with shared filesystems
         # only called on 1 GPU/TPU in distributed
+        super().prepare_data()
 
         # Ensure sqlite databases are downloaded
         cache_locally_if_remote(
             self.train_sqlite_url, storage_options=self.storage_options, cache_dir=self.cache_dir)
         cache_locally_if_remote(
             self.val_sqlite_url, storage_options=self.storage_options, cache_dir=self.cache_dir)
         cache_locally_if_remote(
             self.test_sqlite_url, storage_options=self.storage_options, cache_dir=self.cache_dir)
 
-    def setup(self, stage: Optional[str] = None):
-        if (stage is None or stage == "fit") and self.train_dataset is None:
+    def setup(self, stage: Literal['fit', 'validate', 'test', 'predict']):
+        super().setup(stage)
+        if (stage == "fit") and self.train_dataset is None:
             self.train_dataset = self.train_transform(SQLiteDataset(cache_locally_if_remote(
                 self.train_sqlite_url, storage_options=self.storage_options, cache_dir=self.cache_dir),
                 self.table_name,
                 self.index_column,
                 self.columns_to_return,
                 self.id_column))
-        if (stage is None or stage == "fit" or stage == "validate") and self.val_dataset is None:
+        if (stage == "fit" or stage == "validate") and self.val_dataset is None:
             self.val_dataset = self.test_transform(SQLiteDataset(cache_locally_if_remote(
                 self.val_sqlite_url, storage_options=self.storage_options, cache_dir=self.cache_dir),
                 self.table_name,
                 self.index_column,
                 self.columns_to_return,
                 self.id_column))
-        if (stage is None or stage == "test") and self.test_dataset is None:
+        if (stage == "test") and self.test_dataset is None:
             self.test_dataset = self.test_transform(SQLiteDataset(cache_locally_if_remote(
                 self.test_sqlite_url, storage_options=self.storage_options, cache_dir=self.cache_dir),
                 self.table_name,
                 self.index_column,
                 self.columns_to_return,
                 self.id_column))
 
@@ -172,18 +148,18 @@
         return cast(TypedDataLoader[T2_co], DataLoader(self.val_dataset, batch_size=self.batch_size, num_workers=self.num_workers, persistent_workers=self.num_workers > 0, collate_fn=self.collate_fn, pin_memory=True))
 
     def test_dataloader(self) -> TypedDataLoader[T2_co]:
         if self.test_dataset is None:
             raise ValueError("Test dataset not available")
         return cast(TypedDataLoader[T2_co], DataLoader(self.test_dataset, batch_size=self.batch_size, num_workers=self.num_workers, persistent_workers=self.num_workers > 0, collate_fn=self.collate_fn, pin_memory=True))
 
-    def teardown(self, stage: str):
+    def teardown(self, stage: Literal['fit', 'validate', 'test', 'predict']):
         # clean up state after the trainer stops, delete files...
         # called on every process in DDP
-        pass
+        super().teardown(stage)
 
 
 @click.command()
 @click.option("--key", required=False)
 @click.option("--secret", required=False, help="AWS secret access key or file from which to read credentials")
 @click.option("--endpoint-url", required=False)
 @click.argument("zip-url")
```

### Comparing `hscitorchutil-0.1.67/pyproject.toml` & `hscitorchutil-0.1.69/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hscitorchutil"
-version = "0.1.67"
+version = "0.1.69"
 description = "HSCI research group utilities for pytorch (lightning)"
 authors = ["Eetu Mäkelä <eetu.makela@helsinki.fi>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/hsci-r/hscitorchutil"
 keywords = [
     "pytorch",
```

### Comparing `hscitorchutil-0.1.67/PKG-INFO` & `hscitorchutil-0.1.69/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hscitorchutil
-Version: 0.1.67
+Version: 0.1.69
 Summary: HSCI research group utilities for pytorch (lightning)
 Home-page: https://github.com/hsci-r/hscitorchutil
 License: MIT
 Keywords: pytorch,dataset
 Author: Eetu Mäkelä
 Author-email: eetu.makela@helsinki.fi
 Requires-Python: >=3.10,<3.12
```

