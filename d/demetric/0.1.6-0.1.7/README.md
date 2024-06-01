# Comparing `tmp/demetric-0.1.6.tar.gz` & `tmp/demetric-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "demetric-0.1.6.tar", last modified: Fri May 31 15:02:33 2024, max compression
+gzip compressed data, was "demetric-0.1.7.tar", last modified: Sat Jun  1 17:55:56 2024, max compression
```

## Comparing `demetric-0.1.6.tar` & `demetric-0.1.7.tar`

### file list

```diff
@@ -1,22 +1,17 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 15:02:33.085136 demetric-0.1.6/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      825 2024-05-31 15:02:33.085136 demetric-0.1.6/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      457 2024-05-31 15:02:22.000000 demetric-0.1.6/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      580 2024-05-31 15:02:30.000000 demetric-0.1.6/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-31 15:02:33.085136 demetric-0.1.6/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 15:02:33.085136 demetric-0.1.6/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 15:02:33.085136 demetric-0.1.6/src/demetric/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      175 2024-05-30 20:04:30.000000 demetric-0.1.6/src/demetric/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      139 2024-05-30 20:35:13.000000 demetric-0.1.6/src/demetric/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      294 2024-05-30 20:34:56.000000 demetric-0.1.6/src/demetric/comparing.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 15:02:33.085136 demetric-0.1.6/src/demetric/plot/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       95 2024-05-30 20:07:20.000000 demetric-0.1.6/src/demetric/plot/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       90 2024-05-30 20:47:49.000000 demetric-0.1.6/src/demetric/plot/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      480 2024-05-30 20:13:48.000000 demetric-0.1.6/src/demetric/plot/_plot.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     3395 2024-05-31 10:29:33.000000 demetric-0.1.6/src/demetric/run.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      446 2024-05-30 20:35:08.000000 demetric-0.1.6/src/demetric/runs.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 15:02:33.085136 demetric-0.1.6/src/demetric.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      825 2024-05-31 15:02:33.000000 demetric-0.1.6/src/demetric.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      409 2024-05-31 15:02:33.000000 demetric-0.1.6/src/demetric.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-31 15:02:33.000000 demetric-0.1.6/src/demetric.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-05-31 15:02:33.000000 demetric-0.1.6/src/demetric.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-05-31 15:02:33.000000 demetric-0.1.6/src/demetric.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-01 17:55:56.252522 demetric-0.1.7/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1175 2024-06-01 17:55:56.252522 demetric-0.1.7/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      807 2024-06-01 17:55:48.000000 demetric-0.1.7/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      580 2024-06-01 17:55:53.000000 demetric-0.1.7/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-06-01 17:55:56.252522 demetric-0.1.7/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-01 17:55:56.252522 demetric-0.1.7/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-01 17:55:56.252522 demetric-0.1.7/src/demetric/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      175 2024-05-30 20:04:30.000000 demetric-0.1.7/src/demetric/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      127 2024-06-01 17:26:52.000000 demetric-0.1.7/src/demetric/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1029 2024-06-01 17:46:12.000000 demetric-0.1.7/src/demetric/agg.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1902 2024-06-01 17:39:07.000000 demetric-0.1.7/src/demetric/run.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-01 17:55:56.252522 demetric-0.1.7/src/demetric.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1175 2024-06-01 17:55:56.000000 demetric-0.1.7/src/demetric.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      294 2024-06-01 17:55:56.000000 demetric-0.1.7/src/demetric.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-06-01 17:55:56.000000 demetric-0.1.7/src/demetric.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       30 2024-06-01 17:55:56.000000 demetric-0.1.7/src/demetric.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        9 2024-06-01 17:55:56.000000 demetric-0.1.7/src/demetric.egg-info/top_level.txt
```

### Comparing `demetric-0.1.6/pyproject.toml` & `demetric-0.1.7/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "demetric"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple and composable metric tracking and logging for ML"
 dependencies = [
   "pandas", "lazy-loader", "matplotlib"
 ]
```

### Comparing `demetric-0.1.6/src/demetric/run.py` & `demetric-0.1.7/src/demetric/run.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,121 +1,71 @@
-from typing import Sequence, Container, Mapping, NamedTuple, Any, overload
+from dataclasses import dataclass
 import os
-from shutil import rmtree
-import json
-from . import plot
-
-class Entry(NamedTuple):
-  step: int
-  value: float
+from glob import glob
 
+@dataclass
 class Run:
 
-  id: str
-  base_path: str
-  overwrite: bool = False
-
-  def __repr__(self):
-    with open(self.meta_path) as f:
-      meta = json.load(f)
-    return f'Run({self.id}, {meta})'
-
-
-  def __init__(
-    self, id: str, base_path: str, *,
-    meta: Any = None, overwrite: bool = False
-  ):
-    
-    self.id = id
-    self.base_path = base_path
-    self.path = os.path.join(self.base_path, self.id)
-
-    if overwrite:
-      rmtree(self.path, ignore_errors=True)
-
-    os.makedirs(self.path, exist_ok=True)
-    if meta:
-      with open(self.meta_path, 'w') as f:
-        json.dump(meta, f, indent=2)
-
-  def make_path(self, path: str):
-    """Returns a path relative to the run's directory, and creates intermediate folders as needed"""
-    full_path = os.path.join(self.path, path)
-    os.makedirs(os.path.dirname(full_path), exist_ok=True)
-    return full_path
+  path: str
 
   @property
-  def meta_path(self):
-    return os.path.join(self.path, 'meta.json')
+  def id(self):
+    return os.path.basename(os.path.abspath(self.path))
+  
+  def __repr__(self) -> str:
+    return f'Run(id="{self.id}", path="{self.path}")'
 
-  @property
-  def metrics_path(self):
-    return os.path.join(self.path, 'metrics')
+  @classmethod
+  def new(cls, path: str, overwrite: bool = False):
+    exists = os.path.exists(path)
+    if exists and not overwrite:
+      raise FileExistsError(f'Run already exists at {path}. Use overwrite=True to overwrite it, or Run.append to append to it.')
+    elif exists:
+      csvs = glob(os.path.join(path, '*.csv'))
+      for csv in csvs:
+        os.remove(csv)
+        
+    os.makedirs(path, exist_ok=True)
+    return Run(path)
+  
+  @classmethod
+  def append(cls, path: str):
+    if not os.path.exists(path):
+      raise FileNotFoundError(f'Run does not exist at {path}')
+    return Run(path)
 
   def metric_path(self, metric: str):
-    return os.path.join(self.metrics_path, f'{metric}.csv')
+    return os.path.join(self.path, f'{metric}.csv')
 
   def log(self, metric: str, *, value, step: int):
+    """Log a metric `value` at a `step`"""
 
     path = self.metric_path(metric)
-    os.makedirs(os.path.dirname(path), exist_ok=True)
 
     if not os.path.exists(path):
       with open(path, 'w') as f:
         f.write('step,value\n')
     
     with open(path, 'a') as f:
       f.write(f'{step},{value}\n')
 
-
   def read(self, metric: str):
+    """Read `pd.DataFrame` for `metric`"""
     import pandas as pd
-    return pd.read_csv(self.metric_path(metric))
-  
-  @overload
-  def plot(self, metric: str) -> 'plot.Plot':
-    """Plot `metric`"""
-  @overload
-  def plot(self, metric: str, *metrics: str) -> 'plot.Plot':
-    """Plot all `metrics` into a same plot"""
-  @overload
-  def plot(self, *, without_metrics: Container[str]) -> 'plot.Plot':
-    """Plot all metrics except `without_metrics` into a same plot"""
-  @overload
-  def plot(self) -> 'plot.Plot':
-    """Plot all metrics into a same plot"""
-
-  def plot(self, *metrics, without_metrics=None):
-    if len(metrics) == 0:
-      if without_metrics is not None:
-        metrics = { m: self.read(m) for m in self.metrics() if m not in without_metrics }
-        return self._plot_metrics(metrics)
-      else:
-        return self._plot_metrics(self.read_all())
-    elif len(metrics) == 1:
-      return self._plot_metric(metrics[0])
-    else:
-      return self._plot_metrics({ m: self.read(m) for m in metrics })
-
-  def _plot_metric(self, metric: str):
-    df = self.read(metric)
-    p = plot.metric(df)
-    p.ax.set_title(f'{self.id}: {metric} over steps')
-    p.ax.set_xlabel('step')
-    p.ax.set_ylabel(metric)
-    return p
-
-  def _plot_metrics(self, metrics: Mapping):
-    p = plot.metrics(metrics)
-    p.ax.legend()
-    p.ax.set_title(f'{self.id}: Metrics over steps')
-    p.ax.set_xlabel('step')
-    p.ax.set_ylabel('Metrics')
-    return p
+    try:
+      return pd.read_csv(self.metric_path(metric), index_col='step')['value']
+    except FileNotFoundError:
+      ...
 
-  def metrics(self) -> Sequence[str]:
+  def metrics(self) -> list[str]:
     """List all metrics"""
-    return [os.path.splitext(f)[0] for f in os.listdir(self.metrics_path)]
-  
-  def read_all(self):
-    """Read all metrics as `pd.DataFrame` with columns `step` and `value`"""
-    return { metric: self.read(metric) for metric in self.metrics() }
+    return [
+      os.path.splitext(os.path.split(f)[-1])[0]
+      for f in glob(os.path.join(self.path, '*.csv'))
+    ]
+
+def is_run(path: str):
+  return os.path.isdir(path) and glob(os.path.join(path, '*.csv')) != []
+
+def runs(glob_: str) -> list[Run]:
+  """Read all runs in a directory"""
+  return [Run(p) for p in glob(glob_) if is_run(p)]
```

