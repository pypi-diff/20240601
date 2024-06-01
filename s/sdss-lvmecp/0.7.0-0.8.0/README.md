# Comparing `tmp/sdss_lvmecp-0.7.0.tar.gz` & `tmp/sdss_lvmecp-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_lvmecp-0.7.0.tar", max compression
+gzip compressed data, was "sdss_lvmecp-0.8.0.tar", max compression
```

## Comparing `sdss_lvmecp-0.7.0.tar` & `sdss_lvmecp-0.8.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1504 2024-01-19 23:39:39.975666 sdss_lvmecp-0.7.0/LICENSE.md
--rw-r--r--   0        0        0     3293 2024-01-19 23:39:39.975666 sdss_lvmecp-0.7.0/README.md
--rw-r--r--   0        0        0     2833 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      343 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/__init__.py
--rw-r--r--   0        0        0     2600 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/__main__.py
--rw-r--r--   0        0        0      307 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/actor/__init__.py
--rw-r--r--   0        0        0     2191 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/actor/actor.py
--rw-r--r--   0        0        0      774 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/actor/commands/__init__.py
--rw-r--r--   0        0        0     2054 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/actor/commands/dome.py
--rw-r--r--   0        0        0     1358 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/actor/commands/lights.py
--rw-r--r--   0        0        0     1043 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/actor/commands/status.py
--rw-r--r--   0        0        0     4897 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/dome.py
--rw-r--r--   0        0        0     6185 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/etc/lvmecp.yml
--rw-r--r--   0        0        0      666 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/etc/schema.json
--rw-r--r--   0        0        0      567 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/exceptions.py
--rw-r--r--   0        0        0      689 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/hvac.py
--rw-r--r--   0        0        0     3773 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/lights.py
--rw-r--r--   0        0        0     2063 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/maskbits.py
--rw-r--r--   0        0        0    12582 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/modbus.py
--rw-r--r--   0        0        0     3994 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/module.py
--rw-r--r--   0        0        0     2813 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/plc.py
--rw-r--r--   0        0        0     2607 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/safety.py
--rw-r--r--   0        0        0     5106 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/simulator.py
--rw-r--r--   0        0        0     1252 2024-01-19 23:39:39.987666 sdss_lvmecp-0.7.0/python/lvmecp/tools.py
--rw-r--r--   0        0        0     4586 1970-01-01 00:00:00.000000 sdss_lvmecp-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-06-01 15:22:25.598476 sdss_lvmecp-0.8.0/LICENSE.md
+-rw-r--r--   0        0        0     3294 2024-06-01 15:22:25.598476 sdss_lvmecp-0.8.0/README.md
+-rw-r--r--   0        0        0     2889 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      343 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/__init__.py
+-rw-r--r--   0        0        0     2600 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/__main__.py
+-rw-r--r--   0        0        0      307 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/actor/__init__.py
+-rw-r--r--   0        0        0     2514 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/actor/actor.py
+-rw-r--r--   0        0        0      774 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/actor/commands/__init__.py
+-rw-r--r--   0        0        0     2367 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/actor/commands/dome.py
+-rw-r--r--   0        0        0     1358 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/actor/commands/lights.py
+-rw-r--r--   0        0        0     1200 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/actor/commands/status.py
+-rw-r--r--   0        0        0     4775 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/dome.py
+-rw-r--r--   0        0        0     6297 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/etc/lvmecp.yml
+-rw-r--r--   0        0        0      666 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/etc/schema.json
+-rw-r--r--   0        0        0      567 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/exceptions.py
+-rw-r--r--   0        0        0      689 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/hvac.py
+-rw-r--r--   0        0        0     3773 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/lights.py
+-rw-r--r--   0        0        0     2063 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/maskbits.py
+-rw-r--r--   0        0        0    12582 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/modbus.py
+-rw-r--r--   0        0        0     3994 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/module.py
+-rw-r--r--   0        0        0     2813 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/plc.py
+-rw-r--r--   0        0        0     2607 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/safety.py
+-rw-r--r--   0        0        0     5106 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/simulator.py
+-rw-r--r--   0        0        0     1252 2024-06-01 15:22:25.610476 sdss_lvmecp-0.8.0/python/lvmecp/tools.py
+-rw-r--r--   0        0        0     4631 1970-01-01 00:00:00.000000 sdss_lvmecp-0.8.0/PKG-INFO
```

### Comparing `sdss_lvmecp-0.7.0/LICENSE.md` & `sdss_lvmecp-0.8.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_lvmecp-0.7.0/README.md` & `sdss_lvmecp-0.8.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # lvmecp
 
 ![Versions](https://img.shields.io/badge/python-3.11+-blue)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Test](https://github.com/sdss/lvmecp/actions/workflows/test.yml/badge.svg)](https://github.com/sdss/lvmecp/actions/workflows/test.yml)
 [![Documentation Status](https://readthedocs.org/projects/lvmecp/badge/?version=latest)](https://lvmecp.readthedocs.io/en/latest/?badge=latest)
 [![Docker](https://github.com/sdss/lvmecp/actions/workflows/docker.yml/badge.svg)](https://github.com/sdss/lvmecp/actions/workflows/docker.yml)
-[![codecov](https://codecov.io/gh/sdss/lvmecp/branch/develop/graphs/badge.svg)](https://codecov.io/gh/sdss/lvmecp)
+[![codecov](https://codecov.io/gh/sdss/lvmecp/graph/badge.svg?token=3PJVgsyj1l)](https://codecov.io/gh/sdss/lvmecp)
 
 SDSS-V LVM Enclosure Control Package
 
 ## Features
 
 - CLU Actor based interface
 - Supports [DirectLogic 205 (Micro Modular PLC)](https://www.automationdirect.com/adc/overview/catalog/programmable_controllers/directlogic_series_plcs_(micro_to_small,_brick_-a-_modular)/directlogic_205_(micro_modular_plc))
```

### Comparing `sdss_lvmecp-0.7.0/pyproject.toml` & `sdss_lvmecp-0.8.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-lvmecp"
-version = "0.7.0"
+version = "0.8.0"
 description = "A library and actor to communicate with an SDSS-V LVM Enclosure"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>", "mingyeong yang <mingyeong@khu.ac.kr>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/lvmecp"
 repository = "https://github.com/sdss/lvmecp"
 documentation = "https://sdss-lvmecp.readthedocs.org"
@@ -30,14 +30,15 @@
 [tool.poetry.dependencies]
 python = "^3.11,<4.0"
 sdsstools = "^1.0.0"
 sdss-clu = "^2.1.0"
 click-default-group = "^1.2.2"
 pyserial-asyncio = "^0.6"
 pymodbus = "3.6.2"
+lvmopstools = "^0.2.0"
 
 [tool.poetry.group.dev.dependencies]
 ipython = ">=7.11.0"
 flake8 = ">=3.7.9"
 doc8 = ">=0.8.0"
 isort = ">=4.3.21"
 ipdb = ">=0.12.3"
@@ -67,32 +68,34 @@
 nox = ">=2021.6.12"
 sphinx-autobuild = ">=2021.3.14"
 sphinx-copybutton = ">=0.3.3"
 sphinx-click = ">=3.0.1"
 
 [tool.black]
 line-length = 88
-target-version = ['py311']
+target-version = ['py312']
 fast = true
 
 [tool.ruff]
 line-length = 88
-target-version = 'py311'
+target-version = 'py312'
+
+[tool.ruff.lint]
 select = ["E", "F", "I"]
 unfixable = ["F841"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401", "F403", "E402"]
 
-[tool.ruff.isort]
+[tool.ruff.lint.isort]
 known-first-party = ["lvmecp"]
 lines-after-imports = 2
 section-order = ["future", "standard-library", "typing", "third-party", "sdss", "first-party", "local-folder"]
 
-[tool.ruff.isort.sections]
+[tool.ruff.lint.isort.sections]
 typing = ["typing"]
 sdss = ["sdsstools", "clu"]
 
 [tool.pytest.ini_options]
 addopts = "--cov lvmecp --cov-report xml --cov-report html --cov-report term"
 asyncio_mode = "auto"
```

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/__main__.py` & `sdss_lvmecp-0.8.0/python/lvmecp/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/actor/actor.py` & `sdss_lvmecp-0.8.0/python/lvmecp/actor/actor.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 # @License: BSD 3-clause (http://www.opensource.org/licenses/BSD-3-Clause)
 
 from __future__ import annotations
 
 import asyncio
 import logging
 
-from clu.actor import AMQPActor
+from lvmopstools.actor import ErrorCodesBase, LVMActor
+
 from clu.tools import ActorHandler
 
 from lvmecp import __version__, log
 from lvmecp.actor.commands import parser
 from lvmecp.exceptions import ECPWarning
 from lvmecp.plc import PLC
 
 
 __all__ = ["ECPActor"]
 
 
-class ECPActor(AMQPActor):
+class ECPActor(LVMActor):
     """Enclosure actor."""
 
     parser = parser
 
     def __init__(
         self,
         plc: PLC | None = None,
@@ -78,7 +79,17 @@
         while True:
             try:
                 await self.plc.modbus["hb_set"].set(True)
             except Exception:
                 self.write("w", "Failed to set heartbeat variable.")
             finally:
                 await asyncio.sleep(delay)
+
+    async def _check_internal(self):
+        return await super()._check_internal()
+
+    async def _troubleshoot_internal(
+        self,
+        error_code: ErrorCodesBase,
+        exception: Exception | None = None,
+    ):
+        return await super()._troubleshoot_internal(error_code, exception)
```

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/actor/commands/__init__.py` & `sdss_lvmecp-0.8.0/python/lvmecp/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/actor/commands/dome.py` & `sdss_lvmecp-0.8.0/python/lvmecp/actor/commands/dome.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,30 +40,38 @@
     command.info("Opening dome.")
 
     try:
         await command.actor.plc.dome.open(force=force)
     except DomeError as err:
         return command.fail(err)
 
-    return command.finish(dome_open=True, text="Done is now open.")
+    status = command.actor.plc.dome.status
+    if status and status & DomeStatus.OPEN:
+        return command.finish(text="Dome is now open.")
+    else:
+        return command.fail(text="Dome was left in an unknown state.")
 
 
 @dome.command()
 @click.option("--force", is_flag=True, help="Force dome closing.")
 async def close(command: ECPCommand, force=False):
     """Closes the dome."""
 
     command.info("Closing dome.")
 
     try:
         await command.actor.plc.dome.close(force=force)
     except DomeError as err:
         return command.fail(err)
 
-    return command.finish(dome_open=False, text="Done is now closed.")
+    status = command.actor.plc.dome.status
+    if status and status & DomeStatus.CLOSED:
+        return command.finish(text="Dome is now closed.")
+    else:
+        return command.fail(text="Dome was left in an unknown state.")
 
 
 @dome.command()
 async def status(command: ECPCommand):
     """Returns the status of the dome."""
 
     status = await command.actor.plc.dome.update(use_cache=False)
```

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/actor/commands/lights.py` & `sdss_lvmecp-0.8.0/python/lvmecp/actor/commands/lights.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/actor/commands/status.py` & `sdss_lvmecp-0.8.0/python/lvmecp/actor/commands/status.py`

 * *Files 22% similar despite different names*

```diff
@@ -8,29 +8,33 @@
 
 from __future__ import annotations
 
 import asyncio
 
 from typing import TYPE_CHECKING
 
+import click
+
 from . import parser
 
 
 if TYPE_CHECKING:
     from lvmecp.actor import ECPCommand
     from lvmecp.module import PLCModule
 
 
 @parser.command()
-async def status(command: ECPCommand):
+@click.option("--no-registers", is_flag=True, help="Does not output registers.")
+async def status(command: ECPCommand, no_registers: bool = False):
     """Returns the enclosure status."""
 
     plc = command.actor.plc
 
-    command.info(registers=(await plc.read_all_registers(use_cache=False)))
+    if no_registers is False:
+        command.info(registers=(await plc.read_all_registers(use_cache=False)))
 
     modules: list[PLCModule] = [plc.dome, plc.safety, plc.lights]
     await asyncio.gather(
         *[
             module.update(force_output=True, command=command, use_cache=True)
             for module in modules
         ]
```

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/dome.py` & `sdss_lvmecp-0.8.0/python/lvmecp/dome.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,18 +23,14 @@
 
     flag = DomeStatus
     interval = 15.0
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
-        # Temporary, until we have proximity sensors that tell
-        # us whether we are open or closed.
-        self.dome_is_open: bool | None = None
-
     async def _update_internal(self, use_cache: bool = True):
         dome_registers = await self.plc.modbus.read_group("dome", use_cache=use_cache)
 
         dome_status = SimpleNamespace(**dome_registers)
 
         assert self.flag
         new_status = self.flag(0)
@@ -53,20 +49,20 @@
                 new_status |= self.flag.MOTOR_OPENING
             else:
                 new_status |= self.flag.MOTOR_CLOSING
 
         if dome_status.drive_brake:
             new_status |= self.flag.BRAKE_ENABLED
 
-        if dome_status.overcurrent:
-            new_status |= self.flag.OVERCURRENT
+        # if dome_status.overcurrent:
+        #     new_status |= self.flag.OVERCURRENT
 
-        if self.dome_is_open is True:
+        if dome_status.dome_open is True:
             new_status |= self.flag.OPEN
-        elif self.dome_is_open is False:
+        elif dome_status.dome_closed is True:
             new_status |= self.flag.CLOSED
         else:
             new_status |= self.flag.POSITION_UNKNOWN
 
         if new_status.value == 0:
             new_status = self.flag.__unknown__
 
@@ -117,22 +113,24 @@
         await self.modbus["motor_direction"].set(open)
 
         await asyncio.sleep(0.5)
 
         log.debug("Setting drive_enabled.")
         await self.modbus["drive_enabled"].set(True)
 
-        self.dome_is_open = None
-
         await asyncio.sleep(0.5)
-        while await self.modbus["drive_enabled"].get():
+        while True:
             # Still moving.
             await asyncio.sleep(2)
 
-        self.dome_is_open = open
+            drive_enabled = await self.modbus["drive_enabled"].get()
+            move_done = await self.modbus["dome_open" if open else "dome_closed"].get()
+
+            if not drive_enabled and move_done:
+                break
 
         await self.update(use_cache=False)
 
     async def open(self, force: bool = False):
         """Open the dome."""
 
         await self._move(True, force=force)
@@ -149,14 +147,10 @@
         if status is None or self.flag is None:
             raise RuntimeError("Failed retrieving dome status.")
 
         drive_enabled = bool(status & self.flag.DRIVE_ENABLED)
         if not drive_enabled:
             return
 
-        is_moving = status & self.flag.MOVING
         await self.plc.modbus["drive_enabled"].set(False)
 
-        if is_moving:
-            self.dome_is_open = None
-
         await self.update(use_cache=False)
```

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/etc/lvmecp.yml` & `sdss_lvmecp-0.8.0/python/lvmecp/etc/lvmecp.yml`

 * *Files 2% similar despite different names*

```diff
@@ -68,26 +68,32 @@
       group: dome
     drive_brake:
       address: 102
       group: dome
     ne_limit:
       address: 104
       group: dome
-    nw_limit:
+    se_limit:
       address: 105
       group: dome
-    se_limit:
+    nw_limit:
       address: 106
       group: dome
     sw_limit:
       address: 107
       group: dome
-    overcurrent:
+    dome_closed:
+      address: 108
+      group: dome
+    dome_open:
       address: 109
       group: dome
+    # overcurrent:
+    #   address: 109
+    #   group: dome
     drive_velocity1:
       address: 103
       mode: holding_register
       group: dome
     drive_velocity2:
       address: 104
       mode: holding_register
```

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/etc/schema.json` & `sdss_lvmecp-0.8.0/python/lvmecp/etc/schema.json`

 * *Files identical despite different names*

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/exceptions.py` & `sdss_lvmecp-0.8.0/python/lvmecp/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/hvac.py` & `sdss_lvmecp-0.8.0/python/lvmecp/hvac.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/lights.py` & `sdss_lvmecp-0.8.0/python/lvmecp/lights.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/maskbits.py` & `sdss_lvmecp-0.8.0/python/lvmecp/maskbits.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/modbus.py` & `sdss_lvmecp-0.8.0/python/lvmecp/modbus.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/module.py` & `sdss_lvmecp-0.8.0/python/lvmecp/module.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/plc.py` & `sdss_lvmecp-0.8.0/python/lvmecp/plc.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/safety.py` & `sdss_lvmecp-0.8.0/python/lvmecp/safety.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/simulator.py` & `sdss_lvmecp-0.8.0/python/lvmecp/simulator.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmecp-0.7.0/python/lvmecp/tools.py` & `sdss_lvmecp-0.8.0/python/lvmecp/tools.py`

 * *Files identical despite different names*

### Comparing `sdss_lvmecp-0.7.0/PKG-INFO` & `sdss_lvmecp-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-lvmecp
-Version: 0.7.0
+Version: 0.8.0
 Summary: A library and actor to communicate with an SDSS-V LVM Enclosure
 Home-page: https://github.com/sdss/lvmecp
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.11,<4.0
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: Documentation :: Sphinx
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: click-default-group (>=1.2.2,<2.0.0)
+Requires-Dist: lvmopstools (>=0.2.0,<0.3.0)
 Requires-Dist: pymodbus (==3.6.2)
 Requires-Dist: pyserial-asyncio (>=0.6,<0.7)
 Requires-Dist: sdss-clu (>=2.1.0,<3.0.0)
 Requires-Dist: sdsstools (>=1.0.0,<2.0.0)
 Project-URL: Documentation, https://sdss-lvmecp.readthedocs.org
 Project-URL: Repository, https://github.com/sdss/lvmecp
 Description-Content-Type: text/markdown
@@ -32,15 +33,15 @@
 # lvmecp
 
 ![Versions](https://img.shields.io/badge/python-3.11+-blue)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Test](https://github.com/sdss/lvmecp/actions/workflows/test.yml/badge.svg)](https://github.com/sdss/lvmecp/actions/workflows/test.yml)
 [![Documentation Status](https://readthedocs.org/projects/lvmecp/badge/?version=latest)](https://lvmecp.readthedocs.io/en/latest/?badge=latest)
 [![Docker](https://github.com/sdss/lvmecp/actions/workflows/docker.yml/badge.svg)](https://github.com/sdss/lvmecp/actions/workflows/docker.yml)
-[![codecov](https://codecov.io/gh/sdss/lvmecp/branch/develop/graphs/badge.svg)](https://codecov.io/gh/sdss/lvmecp)
+[![codecov](https://codecov.io/gh/sdss/lvmecp/graph/badge.svg?token=3PJVgsyj1l)](https://codecov.io/gh/sdss/lvmecp)
 
 SDSS-V LVM Enclosure Control Package
 
 ## Features
 
 - CLU Actor based interface
 - Supports [DirectLogic 205 (Micro Modular PLC)](https://www.automationdirect.com/adc/overview/catalog/programmable_controllers/directlogic_series_plcs_(micro_to_small,_brick_-a-_modular)/directlogic_205_(micro_modular_plc))
```

