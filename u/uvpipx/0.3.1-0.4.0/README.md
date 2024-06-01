# Comparing `tmp/uvpipx-0.3.1.tar.gz` & `tmp/uvpipx-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uvpipx-0.3.1.tar", max compression
+gzip compressed data, was "uvpipx-0.4.0.tar", max compression
```

## Comparing `uvpipx-0.3.1.tar` & `uvpipx-0.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    35143 2024-05-20 20:45:02.783271 uvpipx-0.3.1/LICENSE
--rw-r--r--   0        0        0     1216 2024-05-28 17:59:36.032234 uvpipx-0.3.1/README.md
--rw-r--r--   0        0        0     1570 2024-05-28 20:28:58.881593 uvpipx-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3721 2024-05-28 20:18:24.941741 uvpipx-0.3.1/uvpipx/UvPipxEnv.py
--rw-r--r--   0        0        0        0 2024-05-28 20:29:31.051597 uvpipx-0.3.1/uvpipx/__init__.py
--rw-r--r--   0        0        0     2020 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/__main__.py
--rw-r--r--   0        0        0     3539 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/cmd_launcher.py
--rw-r--r--   0        0        0     1163 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/config.py
--rw-r--r--   0        0        0        0 2024-05-28 20:29:31.051597 uvpipx-0.3.1/uvpipx/internal_libs/__init__.py
--rw-r--r--   0        0        0     7852 2024-05-27 20:27:55.155655 uvpipx-0.3.1/uvpipx/internal_libs/args.py
--rw-r--r--   0        0        0     3550 2024-05-20 20:45:02.783271 uvpipx-0.3.1/uvpipx/internal_libs/colors.py
--rw-r--r--   0        0        0      979 2024-05-20 20:45:02.783271 uvpipx-0.3.1/uvpipx/internal_libs/http_utils.py
--rw-r--r--   0        0        0     7920 2024-05-26 19:26:28.236343 uvpipx-0.3.1/uvpipx/internal_libs/misc.py
--rw-r--r--   0        0        0     3326 2024-05-20 20:45:02.783271 uvpipx-0.3.1/uvpipx/internal_libs/print.py
--rw-r--r--   0        0        0     1933 2024-05-26 19:26:28.236343 uvpipx-0.3.1/uvpipx/req_spec.py
--rw-r--r--   0        0        0      824 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/uvpipx_all.py
--rw-r--r--   0        0        0     4136 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/uvpipx_args.py
--rw-r--r--   0        0        0     2764 2024-05-20 20:45:02.783271 uvpipx-0.3.1/uvpipx/uvpipx_bins.py
--rw-r--r--   0        0        0     3002 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/uvpipx_infos.py
--rw-r--r--   0        0        0     4151 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/uvpipx_inject.py
--rw-r--r--   0        0        0     4424 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/uvpipx_install.py
--rw-r--r--   0        0        0     1756 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/uvpipx_upgrade.py
--rw-r--r--   0        0        0      499 2024-05-28 20:28:58.881593 uvpipx-0.3.1/uvpipx/version.py
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 uvpipx-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    35143 2024-05-20 20:45:02.783271 uvpipx-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1967 2024-06-01 16:10:58.805271 uvpipx-0.4.0/README.md
+-rw-r--r--   0        0        0     1609 2024-06-01 16:29:17.612982 uvpipx-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     3721 2024-05-28 20:18:24.941741 uvpipx-0.4.0/uvpipx/UvPipxEnv.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:30:26.662961 uvpipx-0.4.0/uvpipx/__init__.py
+-rw-r--r--   0        0        0     2020 2024-06-01 16:29:17.612982 uvpipx-0.4.0/uvpipx/__main__.py
+-rw-r--r--   0        0        0     3539 2024-06-01 16:29:17.612982 uvpipx-0.4.0/uvpipx/cmd_launcher.py
+-rw-r--r--   0        0        0     1163 2024-06-01 16:29:17.612982 uvpipx-0.4.0/uvpipx/config.py
+-rw-r--r--   0        0        0        0 2024-06-01 16:30:26.662961 uvpipx-0.4.0/uvpipx/internal_libs/__init__.py
+-rw-r--r--   0        0        0     7852 2024-05-27 20:27:55.155655 uvpipx-0.4.0/uvpipx/internal_libs/args.py
+-rw-r--r--   0        0        0     3550 2024-05-20 20:45:02.783271 uvpipx-0.4.0/uvpipx/internal_libs/colors.py
+-rw-r--r--   0        0        0      979 2024-05-20 20:45:02.783271 uvpipx-0.4.0/uvpipx/internal_libs/http_utils.py
+-rw-r--r--   0        0        0     7920 2024-05-26 19:26:28.236343 uvpipx-0.4.0/uvpipx/internal_libs/misc.py
+-rw-r--r--   0        0        0     3326 2024-05-20 20:45:02.783271 uvpipx-0.4.0/uvpipx/internal_libs/print.py
+-rw-r--r--   0        0        0     1933 2024-05-26 19:26:28.236343 uvpipx-0.4.0/uvpipx/req_spec.py
+-rw-r--r--   0        0        0      824 2024-06-01 16:29:17.612982 uvpipx-0.4.0/uvpipx/uvpipx_all.py
+-rw-r--r--   0        0        0     4136 2024-06-01 16:29:17.612982 uvpipx-0.4.0/uvpipx/uvpipx_args.py
+-rw-r--r--   0        0        0     2764 2024-05-20 20:45:02.783271 uvpipx-0.4.0/uvpipx/uvpipx_bins.py
+-rw-r--r--   0        0        0     3646 2024-06-01 16:29:17.612982 uvpipx-0.4.0/uvpipx/uvpipx_infos.py
+-rw-r--r--   0        0        0     4151 2024-06-01 16:29:17.612982 uvpipx-0.4.0/uvpipx/uvpipx_inject.py
+-rw-r--r--   0        0        0     4424 2024-06-01 16:29:17.612982 uvpipx-0.4.0/uvpipx/uvpipx_install.py
+-rw-r--r--   0        0        0     2314 2024-06-01 16:29:17.612982 uvpipx-0.4.0/uvpipx/uvpipx_upgrade.py
+-rw-r--r--   0        0        0      499 2024-06-01 16:29:17.612982 uvpipx-0.4.0/uvpipx/version.py
+-rw-r--r--   0        0        0     2749 1970-01-01 00:00:00.000000 uvpipx-0.4.0/PKG-INFO
```

### Comparing `uvpipx-0.3.1/LICENSE` & `uvpipx-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.1/pyproject.toml` & `uvpipx-0.4.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,53 @@
+[build-system]
+build-backend = "poetry.core.masonry.api"
+requires = [
+  "poetry-core",
+]
+
 [tool.poetry]
 name = "uvpipx"
 description = "A small tool like pipx using uv behind the scene. Fast, Small ..."
-version = "0.3.1" # to bump
-authors = ["Pytgaen <32298455+pytgaen@users.noreply.github.com>"]
+version = "0.4.0" # to bump
+authors = [
+  "Pytgaen <32298455+pytgaen@users.noreply.github.com>",
+]
 readme = "README.md"
 license = "GPL"
 
 homepage = "https://gitlab.com/pytgaen-group/uvpipx"
 repository = "https://gitlab.com/pytgaen-group/uvpipx"
 # documentation = "https://gitlab.com/pytgaen-group/uvpipx" # gitlab page 
 
-include = ["uvpipx"]
+include = [
+  "uvpipx",
+]
 
 [tool.poetry.dependencies]
-python = "^3.8" # not 3.7 because we use pytest
+python = "^3.8"         # not 3.7 because we use pytest
 uv = ">=0.1.45, <1.0.0"
 
-
 [tool.poetry.group.dev.dependencies]
-pytest = "^8.2.0"
+pytest = "^8.2.1"
 # infer-types = "^1.0.0"
 
 # mkdocs
 mkdocs = { version = "1.6.0" }
 mkdocs-material-extensions = { version = "1.3.1" }
-mkdocs-material = { version = "9.5.21" }
+mkdocs-material = { version = "9.5.25" }
 mkdocs-mermaid2-plugin = { version = "1.1.1" }
 # mkdocs-build-plantuml-plugin = { version = "~1.8.0" }
 mkdocs-minify-plugin = { version = "0.8.0" }
 pymdown-extensions = { version = "10.8.1" }
 # mkdocs-kroki-plugin = { version = "0.7.1" }
-mkdocstrings = { version = "0.25.1", extras = ["python"] }
-
-mergedeep = { version = "1.3.4"}  # stranges should be managed by mkdocs
-pyyaml-env-tag = { version = "0.1"}  # stranges should be managed by mkdocs
-pathspec = { version = "0.12.1"}  # stranges should be managed by mkdocs
-watchdog = { version = "4.0.0"}  # stranges should be managed by mkdocs
-regex = { version = "^2024.5.10"}  # stranges should be managed by mkdocs
+mkdocstrings = { version = "0.25.1", extras = [
+  "python",
+] }
+
+mergedeep = { version = "1.3.4" }    # stranges should be managed by mkdocs
+pyyaml-env-tag = { version = "0.1" } # stranges should be managed by mkdocs
+pathspec = { version = "0.12.1" }    # stranges should be managed by mkdocs
+watchdog = { version = "4.0.1" }     # stranges should be managed by mkdocs
+regex = { version = "^2024.5.15" }   # stranges should be managed by mkdocs
 
 [tool.poetry.scripts]
 uvpipx = 'uvpipx.__main__:main'
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
```

### Comparing `uvpipx-0.3.1/uvpipx/UvPipxEnv.py` & `uvpipx-0.4.0/uvpipx/UvPipxEnv.py`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.1/uvpipx/__main__.py` & `uvpipx-0.4.0/uvpipx/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from uvpipx.internal_libs.colors import Painter
 from uvpipx.version import show_version
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.1"  # to bump
+__version__ = "0.4.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 import uvpipx.cmd_launcher as cmd_launcher
 
 # import (
```

### Comparing `uvpipx-0.3.1/uvpipx/cmd_launcher.py` & `uvpipx-0.4.0/uvpipx/cmd_launcher.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.1"  # to bump
+__version__ = "0.4.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 import os
 import sys
```

### Comparing `uvpipx-0.3.1/uvpipx/config.py` & `uvpipx-0.4.0/uvpipx/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.1"  # to bump
+__version__ = "0.4.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 import os
 from pathlib import Path
```

### Comparing `uvpipx-0.3.1/uvpipx/internal_libs/args.py` & `uvpipx-0.4.0/uvpipx/internal_libs/args.py`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.1/uvpipx/internal_libs/colors.py` & `uvpipx-0.4.0/uvpipx/internal_libs/colors.py`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.1/uvpipx/internal_libs/http_utils.py` & `uvpipx-0.4.0/uvpipx/internal_libs/http_utils.py`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.1/uvpipx/internal_libs/misc.py` & `uvpipx-0.4.0/uvpipx/internal_libs/misc.py`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.1/uvpipx/internal_libs/print.py` & `uvpipx-0.4.0/uvpipx/internal_libs/print.py`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.1/uvpipx/req_spec.py` & `uvpipx-0.4.0/uvpipx/req_spec.py`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.1/uvpipx/uvpipx_all.py` & `uvpipx-0.4.0/uvpipx/uvpipx_all.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from uvpipx.uvpipx_upgrade import upgrade
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.1"  # to bump
+__version__ = "0.4.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 from uvpipx import config
 from uvpipx.internal_libs.misc import log_info
```

### Comparing `uvpipx-0.3.1/uvpipx/uvpipx_args.py` & `uvpipx-0.4.0/uvpipx/uvpipx_args.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.1"  # to bump
+__version__ = "0.4.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 from uvpipx.internal_libs.args import Arg, ArgParser, ArgParserMode
```

### Comparing `uvpipx-0.3.1/uvpipx/uvpipx_bins.py` & `uvpipx-0.4.0/uvpipx/uvpipx_bins.py`

 * *Files identical despite different names*

### Comparing `uvpipx-0.3.1/uvpipx/uvpipx_infos.py` & `uvpipx-0.4.0/uvpipx/uvpipx_infos.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from uvpipx.version import show_version
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.1"  # to bump
+__version__ = "0.4.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 import json
 import os
@@ -51,38 +51,60 @@
 
 ⚠️  To use without restart the shell, launch 
 export PATH=$PATH:{config.uvpipx_local_bin}
 """)
 
 
 def _info(pck_venv: Path) -> str:
+    def get_version(pck_name, stdout_line):
+        vers = next(
+            (line for line in stdout_line if pck_name in line),
+            None,
+        )
+        if vers is None:
+            vers = f"{pck_name} Unknow version"
+
+        return vers
+
     uvpipx_dict = {}
     with (pck_venv / "uvpipx.json").open() as intfile:
         uvpipx_dict = json.load(
             intfile,
         )
     rc, stdout, stderr = shell_run(f"cd {pck_venv}; uv pip freeze")
-    vers = next(
-        (line for line in stdout.split("\n") if uvpipx_dict["package_name"] in line),
-        None,
-    )
-    if vers is None:
-        vers = "Unknow ?"
+    stdout_line =[line for line in stdout.split("\n")]
+    main_vers = get_version(uvpipx_dict["package_name"], stdout_line)
         # vers = "unable to retreive package information"
 
+    injected_vers=[]
+    for pkg_injected in uvpipx_dict.get("injected_package",[]):
+        injected_vers.append(get_version(pkg_injected, stdout_line))
+    injected_vers = sorted(injected_vers)
+
     bins = "\n".join(
         f"   ✅ {bin_.split('/')[-1]}" for _, bin_ in uvpipx_dict["exposed_bins"]
     )
     if not bins:
         bins = "   ❌ Nothing exposed"
 
-    return f""" 📦 {uvpipx_dict['package_name']} ({vers}) in venv {uvpipx_dict['uvpipx_package_path']}
+    output = f""" 📦 {uvpipx_dict['package_name']} ({main_vers}) in venv {uvpipx_dict['uvpipx_package_path']}"""
+    if injected_vers:
+        output_inject = "\n".join(f"""   📦 {pkg_ver}""" for pkg_ver in injected_vers)
+        output += f"""
+
+ 🎯 Injected packages
+{output_inject}"""
+        
+    output += f"""
 
  🎯 Exposed program
 {bins}\n"""
+    
+    return output
+
 
 
 def info(
     package_name: str,
     *,
     venv_name: Union[None, str] = None,
     get_venv: bool = False,
```

### Comparing `uvpipx-0.3.1/uvpipx/uvpipx_inject.py` & `uvpipx-0.4.0/uvpipx/uvpipx_inject.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 
 from __future__ import annotations
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.1"  # to bump
+__version__ = "0.4.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 import json
 import re
```

### Comparing `uvpipx-0.3.1/uvpipx/uvpipx_install.py` & `uvpipx-0.4.0/uvpipx/uvpipx_install.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 
 from uvpipx.uvpipx_bins import relink_bins
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.1"  # to bump
+__version__ = "0.4.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 import json
 import re
```

### Comparing `uvpipx-0.3.1/uvpipx/uvpipx_upgrade.py` & `uvpipx-0.4.0/uvpipx/uvpipx_upgrade.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 #!/usr/bin/env python3
 
 from __future__ import annotations
+import difflib
 
 from uvpipx.uvpipx_bins import relink_bins
 
 __author__ = "Gaëtan Montury"
 __copyright__ = "Copyright (c) 2024-2024 Gaëtan Montury"
 __license__ = """GNU GENERAL PUBLIC LICENSE refer to file LICENSE in repo"""
-__version__ = "0.3.1"  # to bump
+__version__ = "0.4.0"  # to bump
 __maintainer__ = "Gaëtan Montury"
 __email__ = "#"
 __status__ = "Development"
 
 
 import json
 import re
@@ -41,20 +42,38 @@
     with (pck_venv / "uvpipx.json").open() as outfile:
         uvpipx_dict = json.load(
             outfile,
         )
     expose_bin_names_ = uvpipx_dict["bin_names"]
     package_name_ref_ = uvpipx_dict["package_name_ref"]
 
+    rc, stdout, stderr = shell_run(f"cd {pck_venv}; uv pip freeze")
+    old_vers = sorted(line for line in stdout.split("\n"))
+
     shell_run_elapse(
         f"cd {pck_venv}; uv pip install --upgrade {package_name_ref_}",
         f" 📥 uv pip install {package_name_ref_} in uvpipx venv {venv_name_}",
     )
     log_info(f" 🟢 uvpipx venv {venv_name_} with {package_name} ready")
     shell_run(f"cd {pck_venv}; uv pip freeze > requirements.txt")
+    rc, stdout, stderr = shell_run(f"cd {pck_venv}; uv pip freeze")
+    new_vers = sorted(line for line in stdout.split("\n"))
+
+    diff_vers = [
+        n
+        for n in difflib.ndiff(old_vers, new_vers)
+        if n[:2] in ["+ ", "- "]
+    ]
+
+    if diff_vers:
+        log_info("\n 🏗️  changes")
+        log_info("\n".join(f"   {n}" for n in diff_vers))
+    else:
+        log_info("\n ⭕ no change")
+
     log_info("")
 
     with (pck_venv / "uvpipx.json").open("w") as outfile:
         json.dump(uvpipx_dict, outfile, indent=4, default=str)
 
-    log_info(" 🎯 Re-Exposing program change")
-    relink_bins(package_name, expose_bin_names=expose_bin_names_, venv_name=venv_name)
+    # log_info(" 🎯 Re-Exposing program change")
+    # relink_bins(package_name, expose_bin_names=expose_bin_names_, venv_name=venv_name)
```

