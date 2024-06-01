# Comparing `tmp/lines_dataset-0.1.8.tar.gz` & `tmp/lines_dataset-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lines_dataset-0.1.8.tar", last modified: Fri May 31 11:52:23 2024, max compression
+gzip compressed data, was "lines_dataset-0.2.0.tar", last modified: Sat Jun  1 13:22:38 2024, max compression
```

## Comparing `lines_dataset-0.1.8.tar` & `lines_dataset-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 11:52:23.435701 lines_dataset-0.1.8/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      455 2024-05-31 11:52:23.435701 lines_dataset-0.1.8/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       91 2024-05-30 21:28:08.000000 lines_dataset-0.1.8/README.md
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      588 2024-05-31 11:52:19.000000 lines_dataset-0.1.8/pyproject.toml
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-05-31 11:52:23.435701 lines_dataset-0.1.8/setup.cfg
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 11:52:23.415701 lines_dataset-0.1.8/src/
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 11:52:23.425701 lines_dataset-0.1.8/src/lines_dataset/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      196 2024-05-30 21:28:45.000000 lines_dataset-0.1.8/src/lines_dataset/__init__.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-05-30 21:30:44.000000 lines_dataset-0.1.8/src/lines_dataset/__init__.pyi
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      318 2024-05-31 11:33:08.000000 lines_dataset-0.1.8/src/lines_dataset/compression.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1693 2024-05-31 11:51:52.000000 lines_dataset-0.1.8/src/lines_dataset/dataset.py
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      254 2024-05-31 11:36:52.000000 lines_dataset-0.1.8/src/lines_dataset/meta.py
-drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-05-31 11:52:23.425701 lines_dataset-0.1.8/src/lines_dataset.egg-info/
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      455 2024-05-31 11:52:23.000000 lines_dataset-0.1.8/src/lines_dataset.egg-info/PKG-INFO
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)      377 2024-05-31 11:52:23.000000 lines_dataset-0.1.8/src/lines_dataset.egg-info/SOURCES.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-05-31 11:52:23.000000 lines_dataset-0.1.8/src/lines_dataset.egg-info/dependency_links.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       20 2024-05-31 11:52:23.000000 lines_dataset-0.1.8/src/lines_dataset.egg-info/requires.txt
--rw-r--r--   0 m4rs      (1000) m4rs      (1000)       14 2024-05-31 11:52:23.000000 lines_dataset-0.1.8/src/lines_dataset.egg-info/top_level.txt
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-01 13:22:38.970638 lines_dataset-0.2.0/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1606 2024-06-01 13:22:38.970638 lines_dataset-0.2.0/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1242 2024-06-01 13:08:31.000000 lines_dataset-0.2.0/README.md
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      588 2024-06-01 13:22:29.000000 lines_dataset-0.2.0/pyproject.toml
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       38 2024-06-01 13:22:38.970638 lines_dataset-0.2.0/setup.cfg
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-01 13:22:38.960638 lines_dataset-0.2.0/src/
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-01 13:22:38.960638 lines_dataset-0.2.0/src/lines_dataset/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      218 2024-06-01 12:32:30.000000 lines_dataset-0.2.0/src/lines_dataset/__init__.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      118 2024-05-30 21:30:44.000000 lines_dataset-0.2.0/src/lines_dataset/__init__.pyi
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      318 2024-05-31 11:33:08.000000 lines_dataset-0.2.0/src/lines_dataset/compression.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1926 2024-06-01 13:10:44.000000 lines_dataset-0.2.0/src/lines_dataset/dataset.py
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      277 2024-06-01 12:58:18.000000 lines_dataset-0.2.0/src/lines_dataset/meta.py
+drwxr-xr-x   0 m4rs      (1000) m4rs      (1000)        0 2024-06-01 13:22:38.970638 lines_dataset-0.2.0/src/lines_dataset.egg-info/
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)     1606 2024-06-01 13:22:38.000000 lines_dataset-0.2.0/src/lines_dataset.egg-info/PKG-INFO
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)      377 2024-06-01 13:22:38.000000 lines_dataset-0.2.0/src/lines_dataset.egg-info/SOURCES.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)        1 2024-06-01 13:22:38.000000 lines_dataset-0.2.0/src/lines_dataset.egg-info/dependency_links.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       20 2024-06-01 13:22:38.000000 lines_dataset-0.2.0/src/lines_dataset.egg-info/requires.txt
+-rw-r--r--   0 m4rs      (1000) m4rs      (1000)       14 2024-06-01 13:22:38.000000 lines_dataset-0.2.0/src/lines_dataset.egg-info/top_level.txt
```

### Comparing `lines_dataset-0.1.8/pyproject.toml` & `lines_dataset-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lines-dataset"
-version = "0.1.8"
+version = "0.2.0"
 authors = [
   {name="Marcel Claramunt", email="marcel@moveread.com"}
 ]
 description = "Simple tools for storing inputs + labels datasets as one sample per line"
 dependencies = [
   "pydantic", "haskellian"
 ]
```

### Comparing `lines_dataset-0.1.8/src/lines_dataset/dataset.py` & `lines_dataset-0.2.0/src/lines_dataset/dataset.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,55 +6,56 @@
 
 K = TypeVar('K', bound=LiteralString)
 
 @dataclass
 class Dataset(Iterable[Mapping[str, str]]):
 
   base_path: str
-  meta: Meta
+  files: Mapping[str, Meta.File]
 
   @classmethod
   def read(cls, base: str) -> 'Dataset':
     with open(os.path.join(base, 'meta.json')) as f:
       meta = Meta.model_validate_json(f.read())
-    return Dataset(base, meta)
-  
-  @classmethod
-  def create(cls, base: str, meta: Meta, *, overwrite: bool = False) -> 'Dataset':
-    os.makedirs(base, exist_ok=True)
-    mode = 'x' if not overwrite else 'w'
-    with open(os.path.join(base, 'meta.json'), mode) as f:
-      f.write(meta.model_dump_json())
-    return Dataset(base, meta)
-  
-  def keys(self):
-    return list(self.meta.files.keys())
+    return Dataset(base, meta.lines_dataset)
   
   def file(self, key: str) -> Meta.File | None:
-    if key in self.meta.files:
-      file = self.meta.files[key]
+    """Metadata of a given file"""
+    if key in self.files:
+      file = self.files[key]
       return Meta.File(file=os.path.join(self.base_path, file.file), compression=file.compression)
     return None
   
   @I.lift
   def iterate(self, key: str) -> Iterable[str]:
+    """Iterate lines of a single file."""
     file = self.file(key)
     if file:
       if file.compression == 'zstd':
         from .compression import iterate
         yield from iterate(file.file)
       else:
         with open(file.file) as f:
           yield from f
 
   def samples(self, *keys: K) -> Iter[Mapping[K, str]]:
-    keys = keys or list(self.meta.files.keys()) # type: ignore
+    """Iterate all samples of `keys`. If no `keys` are provided, iterates all files."""
+    keys = keys or list(self.files.keys()) # type: ignore
     return D.zip({
       k: self.iterate(k)
       for k in keys
     })
 
   def __iter__(self):
     return iter(self.samples())
 
-  def __len__(self) -> int:
-    return self.meta.samples
+  def len(self, *keys: str) -> int | None:
+    """Returns the minimum length of `keys` (or all files, if not provided). Returns `None` if some length is unspecified, or if some key is not found"""
+    keys = keys or list(self.files.keys()) # type: ignore
+    lens = [self._len(k) for k in keys]
+    if None in lens:
+      return None
+    return min(lens) # type: ignore
+
+  def _len(self, key: str) -> int | None:
+    file = self.file(key)
+    return file and file.num_lines
```

