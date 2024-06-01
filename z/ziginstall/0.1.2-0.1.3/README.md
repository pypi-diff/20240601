# Comparing `tmp/ziginstall-0.1.2.tar.gz` & `tmp/ziginstall-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ziginstall-0.1.2.tar", max compression
+gzip compressed data, was "ziginstall-0.1.3.tar", max compression
```

## Comparing `ziginstall-0.1.2.tar` & `ziginstall-0.1.3.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0     1071 2024-06-01 07:33:57.107898 ziginstall-0.1.2/LICENSE
--rw-r--r--   0        0        0      641 2024-06-01 07:33:57.107898 ziginstall-0.1.2/README.md
--rw-r--r--   0        0        0      497 2024-06-01 07:33:57.107898 ziginstall-0.1.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/__init__.py
--rw-r--r--   0        0        0      432 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/_locations.py
--rw-r--r--   0        0        0     1321 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/_logging.py
--rw-r--r--   0        0        0      602 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/cli.py
--rw-r--r--   0        0        0        0 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/install/__init__.py
--rw-r--r--   0        0        0     2113 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/install/_core.py
--rw-r--r--   0        0        0     3847 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/install/_install_steps.py
--rw-r--r--   0        0        0      482 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/install/_verification.py
--rw-r--r--   0        0        0     2267 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/install/cli.py
--rw-r--r--   0        0        0        0 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/version_management/__init__.py
--rw-r--r--   0        0        0     1048 2024-06-01 07:33:57.107898 ziginstall-0.1.2/ziginstall/version_management/core.py
--rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 ziginstall-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-06-01 08:11:51.450441 ziginstall-0.1.3/LICENSE
+-rw-r--r--   0        0        0      641 2024-06-01 08:11:51.450441 ziginstall-0.1.3/README.md
+-rw-r--r--   0        0        0      514 2024-06-01 08:11:51.450441 ziginstall-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-01 08:11:51.450441 ziginstall-0.1.3/ziginstall/__init__.py
+-rw-r--r--   0        0        0      432 2024-06-01 08:11:51.450441 ziginstall-0.1.3/ziginstall/_locations.py
+-rw-r--r--   0        0        0     1321 2024-06-01 08:11:51.450441 ziginstall-0.1.3/ziginstall/_logging.py
+-rw-r--r--   0        0        0      763 2024-06-01 08:11:51.450441 ziginstall-0.1.3/ziginstall/cli.py
+-rw-r--r--   0        0        0        0 2024-06-01 08:11:51.450441 ziginstall-0.1.3/ziginstall/install/__init__.py
+-rw-r--r--   0        0        0     2113 2024-06-01 08:11:51.450441 ziginstall-0.1.3/ziginstall/install/_core.py
+-rw-r--r--   0        0        0     3846 2024-06-01 08:11:51.450441 ziginstall-0.1.3/ziginstall/install/_install_steps.py
+-rw-r--r--   0        0        0      482 2024-06-01 08:11:51.450441 ziginstall-0.1.3/ziginstall/install/_verification.py
+-rw-r--r--   0        0        0     2267 2024-06-01 08:11:51.450441 ziginstall-0.1.3/ziginstall/install/cli.py
+-rw-r--r--   0        0        0        0 2024-06-01 08:11:51.450441 ziginstall-0.1.3/ziginstall/version_management/__init__.py
+-rw-r--r--   0        0        0     2179 2024-06-01 08:11:51.450441 ziginstall-0.1.3/ziginstall/version_management/cli.py
+-rw-r--r--   0        0        0      275 2024-06-01 08:11:51.450441 ziginstall-0.1.3/ziginstall/version_management/core.py
+-rw-r--r--   0        0        0     1180 1970-01-01 00:00:00.000000 ziginstall-0.1.3/PKG-INFO
```

### Comparing `ziginstall-0.1.2/LICENSE` & `ziginstall-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ziginstall-0.1.2/README.md` & `ziginstall-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ziginstall-0.1.2/ziginstall/_logging.py` & `ziginstall-0.1.3/ziginstall/_logging.py`

 * *Files identical despite different names*

### Comparing `ziginstall-0.1.2/ziginstall/cli.py` & `ziginstall-0.1.3/ziginstall/cli.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import click
 
 from ziginstall._logging import init_logging, log
 from ziginstall.install.cli import install
+from ziginstall.version_management.cli import list, use, uninstall
 
 
 @click.group(name="ziginstall")
 @click.option("--debug",
               help="Whether to show debug and info log messages.",
               is_flag=True
               )
@@ -18,7 +19,10 @@
     """
     ctx.obj = { "DEBUG": debug }
     init_logging(debug)
     log.debug(f"Debug mode : {debug}")
 
 
 zig_install.add_command(install)
+zig_install.add_command(list)
+zig_install.add_command(use)
+zig_install.add_command(uninstall)
```

### Comparing `ziginstall-0.1.2/ziginstall/install/_core.py` & `ziginstall-0.1.3/ziginstall/install/_core.py`

 * *Files identical despite different names*

### Comparing `ziginstall-0.1.2/ziginstall/install/_install_steps.py` & `ziginstall-0.1.3/ziginstall/install/_install_steps.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,12 +95,12 @@
         log.debug(f"Creating {used_file_path}")
         with open(used_file_path, "w") as f:
             f.write(components.version)
             try:
                 os.remove(os.path.join(install_directories_path, "zig"))
             except FileNotFoundError:
                 pass
-            shutil.copy(os.path.join(install_directories_path, components.version, "zig"), bin_directory_path)
+            os.symlink(os.path.join(install_directories_path, components.version, "zig"), bin_directory_path)
 
     __do_cleanup()
 
     return True
```

### Comparing `ziginstall-0.1.2/ziginstall/install/cli.py` & `ziginstall-0.1.3/ziginstall/install/cli.py`

 * *Files identical despite different names*

### Comparing `ziginstall-0.1.2/PKG-INFO` & `ziginstall-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: ziginstall
-Version: 0.1.2
+Version: 0.1.3
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
 Requires-Dist: requests (>=2.32.3,<3.0.0)
+Requires-Dist: rich (>=13.7.1,<14.0.0)
 Description-Content-Type: text/markdown
 
 # Zig Install
 
 [![PyPI](https://github.com/charlotdupont/ZigInstall/actions/workflows/python-publish.yml/badge.svg)](https://github.com/charlotdupont/ZigInstall/actions/workflows/python-publish.yml)
 
 Personal project to install Zig.
```

