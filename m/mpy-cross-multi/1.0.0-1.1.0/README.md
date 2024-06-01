# Comparing `tmp/mpy_cross_multi-1.0.0.tar.gz` & `tmp/mpy_cross_multi-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpy_cross_multi-1.0.0.tar", max compression
+gzip compressed data, was "mpy_cross_multi-1.1.0.tar", max compression
```

## Comparing `mpy_cross_multi-1.0.0.tar` & `mpy_cross_multi-1.1.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      864 2024-05-04 22:32:08.906814 mpy_cross_multi-1.0.0/README.md
--rw-r--r--   0        0        0      928 2024-05-04 22:32:08.906814 mpy_cross_multi-1.0.0/mpy_cross_multi/__init__.py
--rw-r--r--   0        0        0     1708 2024-05-04 22:32:08.906814 mpy_cross_multi-1.0.0/mpy_cross_multi/__main__.py
--rw-r--r--   0        0        0      604 2024-05-04 22:32:08.906814 mpy_cross_multi-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 mpy_cross_multi-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0      864 2024-06-01 20:12:02.742365 mpy_cross_multi-1.1.0/README.md
+-rw-r--r--   0        0        0      983 2024-06-01 20:12:02.742365 mpy_cross_multi-1.1.0/mpy_cross_multi/__init__.py
+-rw-r--r--   0        0        0     1708 2024-06-01 20:12:02.742365 mpy_cross_multi-1.1.0/mpy_cross_multi/__main__.py
+-rw-r--r--   0        0        0      632 2024-06-01 20:12:02.742365 mpy_cross_multi-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1657 1970-01-01 00:00:00.000000 mpy_cross_multi-1.1.0/PKG-INFO
```

### Comparing `mpy_cross_multi-1.0.0/README.md` & `mpy_cross_multi-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `mpy_cross_multi-1.0.0/mpy_cross_multi/__init__.py` & `mpy_cross_multi-1.1.0/mpy_cross_multi/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,16 +13,19 @@
     Returns:
         str: mpy-cross ABI version
 
     Raises:
         TypeError: If the input is not a valid version string
         NotImplementedError: If the MicroPython version is not supported
     """
+    if mp_ver.match(">=1.24.0"):
+        raise NotImplementedError("MicroPython version must be <1.24.0")
+
     if mp_ver.match(">=1.23.0"):
-        raise NotImplementedError("MicroPython version must be <1.23.0")
+        return "6.3"
 
     if mp_ver.match(">=1.22.0"):
         return "6.2"
 
     if mp_ver.match(">=1.20.0"):
         return "6.1"
```

### Comparing `mpy_cross_multi-1.0.0/mpy_cross_multi/__main__.py` & `mpy_cross_multi-1.1.0/mpy_cross_multi/__main__.py`

 * *Files identical despite different names*

### Comparing `mpy_cross_multi-1.0.0/pyproject.toml` & `mpy_cross_multi-1.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 [tool.poetry]
 name = "mpy-cross-multi"
-version = "1.0.0"
+version = "1.1.0"
 description = "MicroPython cross-compiler targeting multiple runtime versions."
 authors = ["David Lechner <david@pybricks.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.scripts]
 "mpy-cross-multi" = "mpy_cross_multi.__main__:_run"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 mpy-cross-v5 = "^1.0.2"
 mpy-cross-v6 = "^1.0.2"
 "mpy-cross-v6.1" = "^1.0.1"
 "mpy-cross-v6.2" = "^1.0.0"
+"mpy-cross-v6.3" = "^1.0.0"
 semver = "^3.0.2"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.4.3"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `mpy_cross_multi-1.0.0/PKG-INFO` & `mpy_cross_multi-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: mpy-cross-multi
-Version: 1.0.0
+Version: 1.1.0
 Summary: MicroPython cross-compiler targeting multiple runtime versions.
 License: MIT
 Author: David Lechner
 Author-email: david@pybricks.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: mpy-cross-v5 (>=1.0.2,<2.0.0)
 Requires-Dist: mpy-cross-v6 (>=1.0.2,<2.0.0)
 Requires-Dist: mpy-cross-v6.1 (>=1.0.1,<2.0.0)
 Requires-Dist: mpy-cross-v6.2 (>=1.0.0,<2.0.0)
+Requires-Dist: mpy-cross-v6.3 (>=1.0.0,<2.0.0)
 Requires-Dist: semver (>=3.0.2,<4.0.0)
 Description-Content-Type: text/markdown
 
 # Python packaging for multi-target mpy-cross
 
 This repository contains Python packaging to distribute the `mpy-cross` tool
 from [MicroPython](https://github.com/micropython/micropython) via PyPI.
```

