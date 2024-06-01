# Comparing `tmp/ziginstall-0.1.1.tar.gz` & `tmp/ziginstall-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziginstall-0.1.1.tar", max compression
+gzip compressed data, was "ziginstall-0.1.2.tar", max compression
```

## Comparing `ziginstall-0.1.1.tar` & `ziginstall-0.1.2.tar`

### file list

```diff
@@ -1,11 +1,15 @@
--rw-r--r--   0        0        0     1071 2024-05-30 10:17:56.721248 ziginstall-0.1.1/LICENSE
--rw-r--r--   0        0        0      782 2024-05-30 10:17:56.721248 ziginstall-0.1.1/README.md
--rw-r--r--   0        0        0      459 2024-05-30 10:17:56.721248 ziginstall-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-30 10:17:56.721248 ziginstall-0.1.1/ziginstall/__init__.py
--rw-r--r--   0        0        0     1321 2024-05-30 10:17:56.721248 ziginstall-0.1.1/ziginstall/_logging.py
--rw-r--r--   0        0        0     3478 2024-05-30 10:17:56.721248 ziginstall-0.1.1/ziginstall/cli.py
--rw-r--r--   0        0        0        0 2024-05-30 10:17:56.721248 ziginstall-0.1.1/ziginstall/tools/__init__.py
--rw-r--r--   0        0        0     4616 2024-05-30 10:17:56.721248 ziginstall-0.1.1/ziginstall/tools/core.py
--rw-r--r--   0        0        0     3441 2024-05-30 10:17:56.721248 ziginstall-0.1.1/ziginstall/tools/install.py
--rw-r--r--   0        0        0     1723 2024-05-30 10:17:56.721248 ziginstall-0.1.1/ziginstall/tools/tracking.py
--rw-r--r--   0        0        0     1321 1970-01-01 00:00:00.000000 ziginstall-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-06-01 07:33:57.107898 ziginstall-0.1.2/LICENSE
+-rw-r--r--   0        0        0      641 2024-06-01 07:33:57.107898 ziginstall-0.1.2/README.md
+-rw-r--r--   0        0        0      497 2024-06-01 07:33:57.107898 ziginstall-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/__init__.py
+-rw-r--r--   0        0        0      432 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/_locations.py
+-rw-r--r--   0        0        0     1321 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/_logging.py
+-rw-r--r--   0        0        0      602 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/cli.py
+-rw-r--r--   0        0        0        0 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/install/__init__.py
+-rw-r--r--   0        0        0     2113 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/install/_core.py
+-rw-r--r--   0        0        0     3847 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/install/_install_steps.py
+-rw-r--r--   0        0        0      482 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/install/_verification.py
+-rw-r--r--   0        0        0     2267 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/install/cli.py
+-rw-r--r--   0        0        0        0 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/version_management/__init__.py
+-rw-r--r--   0        0        0     1048 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/version_management/core.py
+-rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 ziginstall-0.1.2/PKG-INFO
```

### Comparing `ziginstall-0.1.1/LICENSE` & `ziginstall-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ziginstall-0.1.1/ziginstall/_logging.py` & `ziginstall-0.1.2/ziginstall/_logging.py`

 * *Files identical despite different names*

### Comparing `ziginstall-0.1.1/PKG-INFO` & `ziginstall-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,37 @@
 Metadata-Version: 2.1
 Name: ziginstall
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: charlotdupont
 Author-email: charlo.dupont@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: packaging (>=24.0,<25.0)
 Requires-Dist: platformdirs (>=4.2.2,<5.0.0)
-Requires-Dist: pytest (>=8.2.1,<9.0.0)
 Requires-Dist: requests (>=2.32.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Zig Install
-[![PyPI](https://github.com/charlotdupont/ZigInstall/actions/workflows/python-publish.yml/badge.svg?branch=master&event=deployment)](https://github.com/charlotdupont/ZigInstall/actions/workflows/python-publish.yml)
+
+[![PyPI](https://github.com/charlotdupont/ZigInstall/actions/workflows/python-publish.yml/badge.svg)](https://github.com/charlotdupont/ZigInstall/actions/workflows/python-publish.yml)
 
 Personal project to install Zig.
 
 **Should work on all systems, but only tested on Ubuntu 20.04.**
 
 **Note**: This project is not affiliated with the official Zig project.
 
 ## Usage
 
 - run ```ziginstall``` to see available commands.
 - run ```ziginstall install``` to install Zig.
     - You can specify the version to install by running ```ziginstall install -v <version>```.
-    - You can specify the installation directory by running ```ziginstall install -d <directory>```.
-      ull
 
 ## TODO
 
 - Uninstall functionality.
 - Add to path functionality.
```

