# Comparing `tmp/nadl-1.5.6.tar.gz` & `tmp/nadl-1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nadl-1.5.6.tar", last modified: Thu May 30 18:15:22 2024, max compression
+gzip compressed data, was "nadl-1.5.7.tar", last modified: Fri May 31 22:42:27 2024, max compression
```

## Comparing `nadl-1.5.6.tar` & `nadl-1.5.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     2302 2024-05-30 18:15:22.024683 nadl-1.5.6/pyproject.toml
--rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.5.6/readme.org
--rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.5.6/src/nadl/.DS_Store
--rw-r--r--   0        0        0     2113 2024-05-30 18:14:45.467011 nadl-1.5.6/src/nadl/__init__.py
--rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.5.6/src/nadl/blocks.py
--rw-r--r--   0        0        0     5812 2024-05-27 05:37:53.227894 nadl-1.5.6/src/nadl/data.py
--rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.5.6/src/nadl/images.py
--rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.5.6/src/nadl/keys.py
--rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.5.6/src/nadl/loops.py
--rw-r--r--   0        0        0     5264 2024-05-30 18:13:31.214975 nadl-1.5.6/src/nadl/metrics.py
--rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.5.6/src/nadl/nets.py
--rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.5.6/src/nadl/preprocessing.py
--rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.5.6/src/nadl/py.typed
--rw-r--r--   0        0        0     3873 2024-05-27 18:49:57.286321 nadl-1.5.6/src/nadl/states.py
--rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.5.6/src/nadl/transformers.py
--rw-r--r--   0        0        0     2814 2024-05-30 17:32:52.960495 nadl-1.5.6/src/nadl/utils.py
--rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 nadl-1.5.6/PKG-INFO
+-rw-r--r--   0        0        0     2302 2024-05-31 22:42:27.327778 nadl-1.5.7/pyproject.toml
+-rw-r--r--   0        0        0      596 2024-04-18 21:07:32.861885 nadl-1.5.7/readme.org
+-rw-r--r--   0        0        0     6148 2024-05-22 06:49:46.036737 nadl-1.5.7/src/nadl/.DS_Store
+-rw-r--r--   0        0        0     2113 2024-05-31 22:41:56.155545 nadl-1.5.7/src/nadl/__init__.py
+-rw-r--r--   0        0        0     8364 2024-04-22 04:28:48.528762 nadl-1.5.7/src/nadl/blocks.py
+-rw-r--r--   0        0        0     5812 2024-05-27 05:37:53.227894 nadl-1.5.7/src/nadl/data.py
+-rw-r--r--   0        0        0     2180 2024-04-26 22:33:55.875764 nadl-1.5.7/src/nadl/images.py
+-rw-r--r--   0        0        0     3564 2024-05-22 05:17:23.233277 nadl-1.5.7/src/nadl/keys.py
+-rw-r--r--   0        0        0     5135 2024-05-21 15:18:23.436274 nadl-1.5.7/src/nadl/loops.py
+-rw-r--r--   0        0        0     5249 2024-05-31 22:39:26.308384 nadl-1.5.7/src/nadl/metrics.py
+-rw-r--r--   0        0        0     3629 2024-04-22 04:28:48.528396 nadl-1.5.7/src/nadl/nets.py
+-rw-r--r--   0        0        0     3401 2024-04-19 20:04:00.936571 nadl-1.5.7/src/nadl/preprocessing.py
+-rw-r--r--   0        0        0        0 2023-12-07 01:36:32.295961 nadl-1.5.7/src/nadl/py.typed
+-rw-r--r--   0        0        0     3869 2024-05-31 22:41:24.111147 nadl-1.5.7/src/nadl/states.py
+-rw-r--r--   0        0        0     1108 2024-04-22 04:28:48.527949 nadl-1.5.7/src/nadl/transformers.py
+-rw-r--r--   0        0        0     2814 2024-05-30 17:32:52.960495 nadl-1.5.7/src/nadl/utils.py
+-rw-r--r--   0        0        0     1403 1970-01-01 00:00:00.000000 nadl-1.5.7/PKG-INFO
```

### Comparing `nadl-1.5.6/pyproject.toml` & `nadl-1.5.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     "equinox>=0.11.4",
     "beartype>=0.18.5",
     "scikit-image>=0.23.2",
     "orbax-checkpoint>=0.5.14",
     "scikit-learn>=1.5.0",
 ]
 requires-python = ">=3.12"
-version = "1.5.6"
+version = "1.5.7"
 
 [project.readme]
 content-type = "text/plain"
 file = "readme.org"
 
 [project.license]
 text = "GPLv3"
```

### Comparing `nadl-1.5.6/readme.org` & `nadl-1.5.7/readme.org`

 * *Files identical despite different names*

### Comparing `nadl-1.5.6/src/nadl/.DS_Store` & `nadl-1.5.7/src/nadl/.DS_Store`

 * *Files identical despite different names*

### Comparing `nadl-1.5.6/src/nadl/__init__.py` & `nadl-1.5.7/src/nadl/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,15 +62,15 @@
   classit,
   filter_concat,
   pformat,
   rle,
   rle_array,
 )
 
-__version__ = "1.5.6"
+__version__ = "1.5.7"
 
 __all__ = [
   "PG",
   "RESC",
   "SCALER",
   "Accuracy",
   "BaseTrainState",
```

### Comparing `nadl-1.5.6/src/nadl/blocks.py` & `nadl-1.5.7/src/nadl/blocks.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.6/src/nadl/data.py` & `nadl-1.5.7/src/nadl/data.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.6/src/nadl/images.py` & `nadl-1.5.7/src/nadl/images.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.6/src/nadl/keys.py` & `nadl-1.5.7/src/nadl/keys.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.6/src/nadl/loops.py` & `nadl-1.5.7/src/nadl/loops.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.6/src/nadl/metrics.py` & `nadl-1.5.7/src/nadl/metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -88,43 +88,42 @@
     labels,
     preds,
   )
 
 
 def pr_auc_score(labels: Num[Array, " A"], preds: Num[Array, " A"]) -> N:
   """Compute PR."""
-  precision, recall, _ = filter_pure_callback(
-    m.precision_recall_curve,
+
+  def _callback(lbl: Num[Array, " A"], prd: Num[Array, " A"]) -> N:
+    precision, recall, _ = m.precision_recall_curve(lbl, prd)
+    return jnp.asarray(m.auc(recall, precision)).reshape(-1)
+
+  return filter_pure_callback(
+    _callback,
     labels,
     preds,
-    result_shape_dtypes=(
-      jax.ShapeDtypeStruct((preds.shape[0] + 1,), jnp.float32),
-      jax.ShapeDtypeStruct((preds.shape[0] + 1,), jnp.float32),
-      jax.ShapeDtypeStruct((preds.shape[0],), jnp.float32),
-    ),
-  )
-  return jax.pure_callback(
-    m.auc, jax.ShapeDtypeStruct((), jnp.float32), recall, precision
+    result_shape_dtypes=jax.ShapeDtypeStruct((), jnp.float32),
   )
 
 
 class Metric[**P, T](Module):
   """Base Metric."""
 
   name: AbstractVar[str | None]
 
   def __post_init__(self) -> None:
     """Post init."""
     for k, v in self.__dict__.items():
-      if isinstance(v, ArrayLike):
+      if isinstance(v, Array):
         self.__dict__[k] = convert(v)
 
   def __check_init__(self) -> None:  # noqa: PLW3201
     """Check init."""
-    if not tree_equal(*jax.tree.map(lambda x: jnp.shape(x)[0], all_array(self))):
+    arrs = all_array(self)
+    if arrs and (not tree_equal(*jax.tree.map(lambda x: jnp.shape(x)[0], arrs))):
       raise ValueError("All metrics should have the same length in first dim.")
 
   @classmethod
   def merge(cls, *metrics: Self) -> Self:
     """Merge all metrics."""
     _, s2 = partition(metrics, is_array)
     if not tree_equal(*s2):
@@ -136,17 +135,17 @@
     return self.merge(self, value)
 
   def __or__(self, value: Self) -> Self:
     """Or."""
     return combine(self, value)
 
   @classmethod
-  def empty(cls, *args: P.args, **kwds: P.kwargs) -> Self:
+  def empty(cls, *args: P.args, **kwds: P.kwargs) -> Self:  # noqa: ARG003
     """Empty."""
-    raise NotImplementedError
+    return cls(dict.fromkeys(cls.__dataclass_fields__))  # type: ignore
 
   def compute(self) -> T:
     """Compute."""
     raise NotImplementedError
 
   def __getitem__(self, idx: int | slice | Int[ArrayLike, "..."]) -> Self:
     """Get item."""
```

### Comparing `nadl-1.5.6/src/nadl/nets.py` & `nadl-1.5.7/src/nadl/nets.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.6/src/nadl/preprocessing.py` & `nadl-1.5.7/src/nadl/preprocessing.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.6/src/nadl/states.py` & `nadl-1.5.7/src/nadl/states.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,15 @@
   ocp.CheckpointManager, Callable[[int, BaseTrainState, dict[str, float] | None], None]
 ]:
   """Get states manager."""
   match (item_names, item_handlers):
     case (None, None):
       item_names = ("state", "extra_metadata")
       item_handlers = {
-        "state": ocp.StandardCheckpointHandler(),
+        "state": ocp.PyTreeCheckpointHandler(),
         "extra_metadata": ocp.JsonCheckpointHandler(),
       }
     case _ if item_names and item_handlers:
       for i in item_names:
         assert i in item_handlers, f"Item {i} not in item_handlers."
     case _:
       raise ValueError("item_names and item_handlers should be both None or not None.")
@@ -132,13 +132,13 @@
   def save(
     step: int, state: BaseTrainState, metadata: dict[str, float] | None = None
   ) -> None:
     """Save state."""
     mngr.save(
       step,
       args=ocp.args.Composite(
-        state=ocp.args.StandardSave(state),  # type: ignore
+        state=ocp.args.PyTreeSave(state),  # type: ignore
         extra_metadata=ocp.args.JsonSave(metadata or {}),  # type: ignore
       ),
     )
 
   return mngr, save
```

### Comparing `nadl-1.5.6/src/nadl/transformers.py` & `nadl-1.5.7/src/nadl/transformers.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.6/src/nadl/utils.py` & `nadl-1.5.7/src/nadl/utils.py`

 * *Files identical despite different names*

### Comparing `nadl-1.5.6/PKG-INFO` & `nadl-1.5.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nadl
-Version: 1.5.6
+Version: 1.5.7
 Summary: Nasy's Deep Learning Toolkit
 Author-Email: Nasy <nasyxx+python@gmail.com>, Nasy <nasyxx+dl@gmail.com>, Nasy <nasyxx+git@gmail.com>
 License: GPLv3
 Requires-Python: >=3.12
 Requires-Dist: jax>=0.4.28
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: rich>=13.7.1
```

