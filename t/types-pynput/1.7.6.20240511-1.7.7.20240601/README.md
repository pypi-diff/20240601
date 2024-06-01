# Comparing `tmp/types-pynput-1.7.6.20240511.tar.gz` & `tmp/types-pynput-1.7.7.20240601.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pynput-1.7.6.20240511.tar", last modified: Sat May 11 02:18:03 2024, max compression
+gzip compressed data, was "types-pynput-1.7.7.20240601.tar", last modified: Sat Jun  1 02:27:25 2024, max compression
```

## Comparing `types-pynput-1.7.6.20240511.tar` & `types-pynput-1.7.7.20240601.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:03.642156 types-pynput-1.7.6.20240511/
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-11 02:18:03.642156 types-pynput-1.7.6.20240511/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:03.638156 types-pynput-1.7.6.20240511/pynput-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/pynput-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/_info.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/_util.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:03.642156 types-pynput-1.7.6.20240511/pynput-stubs/keyboard/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/keyboard/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/keyboard/_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/keyboard/_dummy.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:03.642156 types-pynput-1.7.6.20240511/pynput-stubs/mouse/
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/mouse/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/mouse/_base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-11 02:17:34.000000 types-pynput-1.7.6.20240511/pynput-stubs/mouse/_dummy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/pynput-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-11 02:18:03.642156 types-pynput-1.7.6.20240511/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 02:18:03.642156 types-pynput-1.7.6.20240511/types_pynput.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/types_pynput.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/types_pynput.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/types_pynput.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-11 02:18:03.000000 types-pynput-1.7.6.20240511/types_pynput.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:25.311125 types-pynput-1.7.7.20240601/
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-06-01 02:27:24.000000 types-pynput-1.7.7.20240601/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-06-01 02:27:24.000000 types-pynput-1.7.7.20240601/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-06-01 02:27:25.311125 types-pynput-1.7.7.20240601/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:25.311125 types-pynput-1.7.7.20240601/pynput-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-06-01 02:27:24.000000 types-pynput-1.7.7.20240601/pynput-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-06-01 02:27:05.000000 types-pynput-1.7.7.20240601/pynput-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-06-01 02:27:05.000000 types-pynput-1.7.7.20240601/pynput-stubs/_info.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-06-01 02:27:05.000000 types-pynput-1.7.7.20240601/pynput-stubs/_util.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:25.311125 types-pynput-1.7.7.20240601/pynput-stubs/keyboard/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-06-01 02:27:05.000000 types-pynput-1.7.7.20240601/pynput-stubs/keyboard/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3601 2024-06-01 02:27:05.000000 types-pynput-1.7.7.20240601/pynput-stubs/keyboard/_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-06-01 02:27:05.000000 types-pynput-1.7.7.20240601/pynput-stubs/keyboard/_dummy.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:25.311125 types-pynput-1.7.7.20240601/pynput-stubs/mouse/
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-06-01 02:27:05.000000 types-pynput-1.7.7.20240601/pynput-stubs/mouse/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2024-06-01 02:27:05.000000 types-pynput-1.7.7.20240601/pynput-stubs/mouse/_base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-06-01 02:27:05.000000 types-pynput-1.7.7.20240601/pynput-stubs/mouse/_dummy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:24.000000 types-pynput-1.7.7.20240601/pynput-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 02:27:25.311125 types-pynput-1.7.7.20240601/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-06-01 02:27:24.000000 types-pynput-1.7.7.20240601/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 02:27:25.311125 types-pynput-1.7.7.20240601/types_pynput.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-06-01 02:27:25.000000 types-pynput-1.7.7.20240601/types_pynput.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-06-01 02:27:25.000000 types-pynput-1.7.7.20240601/types_pynput.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 02:27:25.000000 types-pynput-1.7.7.20240601/types_pynput.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-06-01 02:27:25.000000 types-pynput-1.7.7.20240601/types_pynput.egg-info/top_level.txt
```

### Comparing `types-pynput-1.7.6.20240511/CHANGELOG.md` & `types-pynput-1.7.7.20240601/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 1.7.7.20240601 (2024-06-01)
+
+Bump pynput to 1.7.7 (#12069)
+
 ## 1.7.6.20240511 (2024-05-11)
 
 Pin pynput more tightly (#11897)
 
 Fixes  #11896
 
 ## 1.7.5.20240423 (2024-04-23)
```

### Comparing `types-pynput-1.7.6.20240511/PKG-INFO` & `types-pynput-1.7.7.20240601/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pynput
-Version: 1.7.6.20240511
+Version: 1.7.7.20240601
 Summary: Typing stubs for pynput
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pynput.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pynput`.
 
 This version of `types-pynput` aims to provide accurate annotations
-for `pynput==1.7.6`.
+for `pynput==1.7.7`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pynput. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
-with mypy 1.10.0, pyright 1.1.362, and
+This package was generated from typeshed commit `4b6558c12ac43cd40716cd6452fe98a632ae65d7` and was tested
+with mypy 1.10.0, pyright 1.1.365, and
 pytype 2024.4.11.
```

### Comparing `types-pynput-1.7.6.20240511/pynput-stubs/_util.pyi` & `types-pynput-1.7.7.20240601/pynput-stubs/_util.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     def wait(self) -> None: ...
     def run(self) -> None: ...
     @classmethod
     def _emitter(cls, f: Callable[_P, _T]) -> Callable[_P, _T]: ...  # undocumented
     def _mark_ready(self) -> None: ...  # undocumented
     def _run(self) -> None: ...  # undocumented
     def _stop_platform(self) -> None: ...  # undocumented
-    def join(self, *args: Any) -> None: ...
+    def join(self, timeout: float | None = None, *args: Any) -> None: ...
 
 class Events(Generic[_T, _AbstractListener_T]):
     _Listener: type[_AbstractListener_T] | None  # undocumented
 
     class Event:
         def __eq__(self, other: object) -> bool: ...
```

### Comparing `types-pynput-1.7.6.20240511/pynput-stubs/keyboard/__init__.pyi` & `types-pynput-1.7.7.20240601/pynput-stubs/keyboard/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pynput-1.7.6.20240511/pynput-stubs/mouse/__init__.pyi` & `types-pynput-1.7.7.20240601/pynput-stubs/mouse/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-pynput-1.7.6.20240511/pynput-stubs/mouse/_base.pyi` & `types-pynput-1.7.7.20240601/pynput-stubs/mouse/_base.pyi`

 * *Files identical despite different names*

### Comparing `types-pynput-1.7.6.20240511/setup.py` & `types-pynput-1.7.7.20240601/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,27 +11,27 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pynput`.
 
 This version of `types-pynput` aims to provide accurate annotations
-for `pynput==1.7.6`.
+for `pynput==1.7.7`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pynput. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
-with mypy 1.10.0, pyright 1.1.362, and
+This package was generated from typeshed commit `4b6558c12ac43cd40716cd6452fe98a632ae65d7` and was tested
+with mypy 1.10.0, pyright 1.1.365, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="1.7.6.20240511",
+      version="1.7.7.20240601",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pynput.md",
```

### Comparing `types-pynput-1.7.6.20240511/types_pynput.egg-info/PKG-INFO` & `types-pynput-1.7.7.20240601/types_pynput.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-pynput
-Version: 1.7.6.20240511
+Version: 1.7.7.20240601
 Summary: Typing stubs for pynput
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pynput.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,16 +22,16 @@
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `pynput`.
 
 This version of `types-pynput` aims to provide accurate annotations
-for `pynput==1.7.6`.
+for `pynput==1.7.7`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pynput. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `7bfde5b676a19080f4496c618117b748e2a02628` and was tested
-with mypy 1.10.0, pyright 1.1.362, and
+This package was generated from typeshed commit `4b6558c12ac43cd40716cd6452fe98a632ae65d7` and was tested
+with mypy 1.10.0, pyright 1.1.365, and
 pytype 2024.4.11.
```

