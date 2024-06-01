# Comparing `tmp/sdss_lvmnps-1.0.3.tar.gz` & `tmp/sdss_lvmnps-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_lvmnps-1.0.3.tar", max compression
+gzip compressed data, was "sdss_lvmnps-1.1.0.tar", max compression
```

## Comparing `sdss_lvmnps-1.0.3.tar` & `sdss_lvmnps-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1504 2023-11-24 23:52:26.380473 sdss_lvmnps-1.0.3/LICENSE.md
--rw-r--r--   0        0        0     1197 2023-11-24 23:52:26.380473 sdss_lvmnps-1.0.3/README.md
--rw-r--r--   0        0        0     2909 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/pyproject.toml
--rw-r--r--   0        0        0      503 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/__init__.py
--rw-r--r--   0        0        0     1717 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/__main__.py
--rw-r--r--   0        0        0      257 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/actor/__init__.py
--rw-r--r--   0        0        0     2762 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/actor/actor.py
--rw-r--r--   0        0        0      456 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/actor/commands/__init__.py
--rw-r--r--   0        0        0     2967 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/actor/commands/onoff.py
--rw-r--r--   0        0        0      833 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/actor/commands/refresh.py
--rw-r--r--   0        0        0     2612 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/actor/commands/scripts.py
--rw-r--r--   0        0        0     1317 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/actor/commands/status.py
--rw-r--r--   0        0        0     1820 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/actor/schema.json
--rw-r--r--   0        0        0      563 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/exceptions.py
--rw-r--r--   0        0        0      316 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/nps/__init__.py
--rw-r--r--   0        0        0     7042 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/nps/core.py
--rw-r--r--   0        0        0      519 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/nps/implementations/__init__.py
--rw-r--r--   0        0        0     7447 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/nps/implementations/dli.py
--rw-r--r--   0        0        0     3845 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/nps/implementations/netio.py
--rw-r--r--   0        0        0     3233 2023-11-24 23:52:26.392473 sdss_lvmnps-1.0.3/src/lvmnps/tools.py
--rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 sdss_lvmnps-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-06-01 15:45:26.369057 sdss_lvmnps-1.1.0/LICENSE.md
+-rw-r--r--   0        0        0     1197 2024-06-01 15:45:26.369057 sdss_lvmnps-1.1.0/README.md
+-rw-r--r--   0        0        0     2980 2024-06-01 15:45:26.381057 sdss_lvmnps-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      503 2024-06-01 15:45:26.381057 sdss_lvmnps-1.1.0/src/lvmnps/__init__.py
+-rw-r--r--   0        0        0     1717 2024-06-01 15:45:26.381057 sdss_lvmnps-1.1.0/src/lvmnps/__main__.py
+-rw-r--r--   0        0        0      257 2024-06-01 15:45:26.381057 sdss_lvmnps-1.1.0/src/lvmnps/actor/__init__.py
+-rw-r--r--   0        0        0     3936 2024-06-01 15:45:26.381057 sdss_lvmnps-1.1.0/src/lvmnps/actor/actor.py
+-rw-r--r--   0        0        0      456 2024-06-01 15:45:26.385057 sdss_lvmnps-1.1.0/src/lvmnps/actor/commands/__init__.py
+-rw-r--r--   0        0        0     2967 2024-06-01 15:45:26.385057 sdss_lvmnps-1.1.0/src/lvmnps/actor/commands/onoff.py
+-rw-r--r--   0        0        0      833 2024-06-01 15:45:26.385057 sdss_lvmnps-1.1.0/src/lvmnps/actor/commands/refresh.py
+-rw-r--r--   0        0        0     2612 2024-06-01 15:45:26.385057 sdss_lvmnps-1.1.0/src/lvmnps/actor/commands/scripts.py
+-rw-r--r--   0        0        0     1317 2024-06-01 15:45:26.385057 sdss_lvmnps-1.1.0/src/lvmnps/actor/commands/status.py
+-rw-r--r--   0        0        0     1820 2024-06-01 15:45:26.385057 sdss_lvmnps-1.1.0/src/lvmnps/actor/schema.json
+-rw-r--r--   0        0        0      563 2024-06-01 15:45:26.385057 sdss_lvmnps-1.1.0/src/lvmnps/exceptions.py
+-rw-r--r--   0        0        0      316 2024-06-01 15:45:26.385057 sdss_lvmnps-1.1.0/src/lvmnps/nps/__init__.py
+-rw-r--r--   0        0        0     7042 2024-06-01 15:45:26.385057 sdss_lvmnps-1.1.0/src/lvmnps/nps/core.py
+-rw-r--r--   0        0        0      519 2024-06-01 15:45:26.385057 sdss_lvmnps-1.1.0/src/lvmnps/nps/implementations/__init__.py
+-rw-r--r--   0        0        0     7447 2024-06-01 15:45:26.385057 sdss_lvmnps-1.1.0/src/lvmnps/nps/implementations/dli.py
+-rw-r--r--   0        0        0     3845 2024-06-01 15:45:26.385057 sdss_lvmnps-1.1.0/src/lvmnps/nps/implementations/netio.py
+-rw-r--r--   0        0        0     3233 2024-06-01 15:45:26.385057 sdss_lvmnps-1.1.0/src/lvmnps/tools.py
+-rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 sdss_lvmnps-1.1.0/PKG-INFO
```

### Comparing `sdss_lvmnps-1.0.3/LICENSE.md` & `sdss_lvmnps-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmnps-1.0.3/README.md` & `sdss_lvmnps-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmnps-1.0.3/pyproject.toml` & `sdss_lvmnps-1.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-lvmnps"
-version = "1.0.3"
+version = "1.1.0"
 description = "A library and actor to communicate with an SDSS-V LVM network power switch"
 authors = ["Florian Briegel <briegel@mpia.de>", "José Sánchez-Gallego <gallegoj@uw.edu>", "Changgon Kim <changgonkim@khu.ac.kr>", "Mingyeong Yang <mingyeong@khu.ac.kr>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmnps"
 repository = "https://github.com/sdss/lvmnps"
 documentation = "https://lvmnps.readthedocs.org"
@@ -32,14 +32,15 @@
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 sdsstools = "^1.0.0"
 click-default-group = "^1.2.2"
 sdss-clu = "^2.0.0"
 httpx = ">=0.18.1"
 pydantic = "^2.5.2"
+lvmopstools = "^0.2.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = ">=7.11.0"
 ipdb = ">=0.12.3"
 black = ">=21.7b0"
 pytest = ">=5.2.2"
 pytest-asyncio = ">=0.10.0"
@@ -65,29 +66,31 @@
 line-length = 88
 target-version = ['py312']
 fast = true
 
 [tool.ruff]
 line-length = 88
 target-version = 'py312'
+
+[tool.ruff.lint]
 select = ["E", "F", "I"]
-unfixable = ["F841"]
 exclude = ["typings/"]
+unfixable = ["F841"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401", "F403", "E402"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["lvmnps"]
 lines-after-imports = 2
 section-order = ["future", "standard-library", "typing", "third-party", "sdss", "first-party", "local-folder"]
 
-[tool.ruff.isort.sections]
+[tool.ruff.lint.isort.sections]
 typing = ["typing"]
-sdss = ["sdsstools", "clu"]
+sdss = ["sdsstools", "clu", "lvmopstools"]
 
 [tool.pytest.ini_options]
 addopts = "--cov lvmnps --cov-report xml --cov-report html --cov-report term"
 asyncio_mode = "auto"
 
 [tool.coverage.run]
 branch = true
```

### Comparing `sdss_lvmnps-1.0.3/src/lvmnps/__main__.py` & `sdss_lvmnps-1.1.0/src/lvmnps/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmnps-1.0.3/src/lvmnps/actor/actor.py` & `sdss_lvmnps-1.1.0/src/lvmnps/actor/actor.py`

 * *Files 22% similar despite different names*

```diff
@@ -10,34 +10,49 @@
 
 import pathlib
 from os import PathLike
 
 from typing import TYPE_CHECKING
 
 from clu import Command
-from clu.actor import AMQPActor
+from lvmopstools.actor import CheckError, ErrorData, LVMActor, create_error_codes
 from sdsstools.configuration import Configuration
 
 from lvmnps import __version__
 from lvmnps import log as nps_log
 from lvmnps.actor.commands import lvmnps_command_parser
+from lvmnps.exceptions import VerificationError
 from lvmnps.nps.core import NPSClient
 from lvmnps.nps.implementations import VALID_NPS_TYPES
 
 
 if TYPE_CHECKING:
     from sdsstools.logger import SDSSLogger
 
 
 __all__ = ["NPSActor"]
 
 
 AnyPath = str | PathLike[str]
 
 
+CHECK_INTERVAL: float = 30
+
+NPSErrorCodes = create_error_codes(
+    {
+        "VERIFICATION_FAILED": ErrorData(
+            1,
+            critical=True,
+            description="NPS verification failed.",
+        )
+    },
+    name="NPSErrorCodes",
+)
+
+
 def get_nps_from_config(config: Configuration) -> NPSClient:
     """Returns an `.NPSClient` instance from the configuration parameters."""
 
     if "nps" not in config:
         raise ValueError("nps section does not exist in the configuration.")
 
     nps_type = config["nps.type"]
@@ -59,15 +74,15 @@
 
         return NetIOClient(**init_parameters)
 
     else:  # pragma: no cover - This should unreachable.
         raise ValueError(f"Invalid NPS {nps_type}. Valid types are {VALID_NPS_TYPES}.")
 
 
-class NPSActor(AMQPActor):
+class NPSActor(LVMActor):
     """LVM network power switches base actor."""
 
     parser = lvmnps_command_parser
 
     def __init__(
         self,
         *args,
@@ -85,23 +100,50 @@
         super().__init__(*args, log=log, schema=schema, **kwargs)
 
         if not isinstance(self.config, Configuration):
             self.config = Configuration(self.config)
 
         self.nps = get_nps_from_config(self.config)
 
+        self.restart_after = 30
+        self.restart_mode = "exit"
+
     async def start(self, **kwargs):  # pragma: no cover
         """Starts the actor."""
 
         await self.nps.setup()
 
         return await super().start(**kwargs)
 
     async def stop(self):
         "Stops the actor."
 
         await self.nps.stop()
 
         return await super().stop()
 
+    async def _check_internal(self):
+        """Checks the NPS status."""
+
+        try:
+            result = await self.nps.verify()
+            if result is False:
+                raise VerificationError("NPS verification failed.")
+        except Exception as err:
+            self.check_interval = 5  # Speed up checks
+            raise CheckError(str(err), error_code=NPSErrorCodes.VERIFICATION_FAILED)
+
+        self.check_interval = CHECK_INTERVAL
+        return True
+
+    async def _troubleshoot_internal(
+        self,
+        error_code,
+        exception: Exception | None = None,
+    ):
+        """Handles internal troubleshooting."""
+
+        if error_code.value == NPSErrorCodes.VERIFICATION_FAILED:
+            await self.restart(mode="exit")
+
 
 NPSCommand = Command[NPSActor]
```

### Comparing `sdss_lvmnps-1.0.3/src/lvmnps/actor/commands/onoff.py` & `sdss_lvmnps-1.1.0/src/lvmnps/actor/commands/onoff.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmnps-1.0.3/src/lvmnps/actor/commands/refresh.py` & `sdss_lvmnps-1.1.0/src/lvmnps/actor/commands/refresh.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmnps-1.0.3/src/lvmnps/actor/commands/scripts.py` & `sdss_lvmnps-1.1.0/src/lvmnps/actor/commands/scripts.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmnps-1.0.3/src/lvmnps/actor/commands/status.py` & `sdss_lvmnps-1.1.0/src/lvmnps/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmnps-1.0.3/src/lvmnps/actor/schema.json` & `sdss_lvmnps-1.1.0/src/lvmnps/actor/schema.json`

 * *Files identical despite different names*

### Comparing `sdss_lvmnps-1.0.3/src/lvmnps/exceptions.py` & `sdss_lvmnps-1.1.0/src/lvmnps/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmnps-1.0.3/src/lvmnps/nps/core.py` & `sdss_lvmnps-1.1.0/src/lvmnps/nps/core.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmnps-1.0.3/src/lvmnps/nps/implementations/__init__.py` & `sdss_lvmnps-1.1.0/src/lvmnps/nps/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmnps-1.0.3/src/lvmnps/nps/implementations/dli.py` & `sdss_lvmnps-1.1.0/src/lvmnps/nps/implementations/dli.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmnps-1.0.3/src/lvmnps/nps/implementations/netio.py` & `sdss_lvmnps-1.1.0/src/lvmnps/nps/implementations/netio.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmnps-1.0.3/src/lvmnps/tools.py` & `sdss_lvmnps-1.1.0/src/lvmnps/tools.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmnps-1.0.3/PKG-INFO` & `sdss_lvmnps-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-lvmnps
-Version: 1.0.3
+Version: 1.1.0
 Summary: A library and actor to communicate with an SDSS-V LVM network power switch
 Home-page: https://github.com/sdss/lvmnps
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: Florian Briegel
 Author-email: briegel@mpia.de
 Requires-Python: >=3.10,<4.0
@@ -18,14 +18,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
 Requires-Dist: httpx (>=0.18.1)
+Requires-Dist: lvmopstools (>=0.2.0,<0.3.0)
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: sdss-clu (>=2.0.0,<3.0.0)
 Requires-Dist: sdsstools (>=1.0.0,<2.0.0)
 Project-URL: Documentation, https://lvmnps.readthedocs.org
 Project-URL: Repository, https://github.com/sdss/lvmnps
 Description-Content-Type: text/markdown
```

