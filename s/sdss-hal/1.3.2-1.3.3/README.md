# Comparing `tmp/sdss_hal-1.3.2.tar.gz` & `tmp/sdss_hal-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdss_hal-1.3.2.tar", max compression
+gzip compressed data, was "sdss_hal-1.3.3.tar", max compression
```

## Comparing `sdss_hal-1.3.2.tar` & `sdss_hal-1.3.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     1504 2024-05-31 03:34:27.436882 sdss_hal-1.3.2/LICENSE.md
--rw-r--r--   0        0        0      816 2024-05-31 03:34:27.436882 sdss_hal-1.3.2/README.md
--rw-r--r--   0        0        0     2708 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/pyproject.toml
--rw-r--r--   0        0        0      483 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/__init__.py
--rw-r--r--   0        0        0     1761 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/__main__.py
--rw-r--r--   0        0        0      356 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/actor/__init__.py
--rw-r--r--   0        0        0     3024 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/actor/actor.py
--rw-r--r--   0        0        0     3357 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/actor/commands/__init__.py
--rw-r--r--   0        0        0     2014 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/actor/commands/abort_exposures.py
--rw-r--r--   0        0        0     4811 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/actor/commands/auto_pilot.py
--rw-r--r--   0        0        0     1593 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/actor/commands/bypass.py
--rw-r--r--   0        0        0      844 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/actor/commands/calibrations.py
--rw-r--r--   0        0        0     8082 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/actor/commands/expose.py
--rw-r--r--   0        0        0     1669 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/actor/commands/goto.py
--rw-r--r--   0        0        0     3498 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/actor/commands/goto_field.py
--rw-r--r--   0        0        0     2537 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/actor/commands/script.py
--rw-r--r--   0        0        0     1419 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/actor/commands/status.py
--rw-r--r--   0        0        0      687 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/actor/commands/test.py
--rw-r--r--   0        0        0     3362 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/etc/hal.yml
--rw-r--r--   0        0        0     2240 2024-05-31 03:34:27.440882 sdss_hal-1.3.2/src/hal/etc/schema.json
--rw-r--r--   0        0        0      346 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/etc/scripts/apo/cartchange.inp
--rw-r--r--   0        0        0     1161 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/etc/scripts/apo/eveningcals.inp
--rw-r--r--   0        0        0      161 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/etc/scripts/apo/example.inp
--rw-r--r--   0        0        0     1616 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/etc/scripts/apo/morningcals.inp
--rw-r--r--   0        0        0       35 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/etc/scripts/apo/test.inp
--rw-r--r--   0        0        0      346 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/etc/scripts/lco/cartchange.inp
--rw-r--r--   0        0        0     1056 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/etc/scripts/lco/eveningcals.inp
--rw-r--r--   0        0        0     1450 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/etc/scripts/lco/morningcals.inp
--rw-r--r--   0        0        0     1180 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/exceptions.py
--rw-r--r--   0        0        0     3502 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/helpers/__init__.py
--rw-r--r--   0        0        0    10870 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/helpers/apogee.py
--rw-r--r--   0        0        0     7773 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/helpers/boss.py
--rw-r--r--   0        0        0     6514 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/helpers/cherno.py
--rw-r--r--   0        0        0     1769 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/helpers/ffs.py
--rw-r--r--   0        0        0     8276 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/helpers/jaeger.py
--rw-r--r--   0        0        0    10429 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/helpers/lamps.py
--rw-r--r--   0        0        0     4732 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/helpers/overhead.py
--rw-r--r--   0        0        0     4671 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/helpers/scripts.py
--rw-r--r--   0        0        0    13441 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/helpers/tcc.py
--rw-r--r--   0        0        0     1399 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/macros/__init__.py
--rw-r--r--   0        0        0     3844 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/macros/apogee_dome_flat.py
--rw-r--r--   0        0        0    13057 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/macros/auto_pilot.py
--rw-r--r--   0        0        0    21726 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/macros/expose.py
--rw-r--r--   0        0        0    23929 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/macros/goto_field.py
--rw-r--r--   0        0        0    18881 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/macros/macro.py
--rw-r--r--   0        0        0     1263 2024-05-31 03:34:27.444882 sdss_hal-1.3.2/src/hal/macros/test_macro.py
--rw-r--r--   0        0        0     2219 1970-01-01 00:00:00.000000 sdss_hal-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1504 2024-06-01 19:36:02.170813 sdss_hal-1.3.3/LICENSE.md
+-rw-r--r--   0        0        0      816 2024-06-01 19:36:02.170813 sdss_hal-1.3.3/README.md
+-rw-r--r--   0        0        0     2708 2024-06-01 19:36:02.174813 sdss_hal-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0      483 2024-06-01 19:36:02.174813 sdss_hal-1.3.3/src/hal/__init__.py
+-rw-r--r--   0        0        0     1761 2024-06-01 19:36:02.174813 sdss_hal-1.3.3/src/hal/__main__.py
+-rw-r--r--   0        0        0      356 2024-06-01 19:36:02.174813 sdss_hal-1.3.3/src/hal/actor/__init__.py
+-rw-r--r--   0        0        0     3024 2024-06-01 19:36:02.174813 sdss_hal-1.3.3/src/hal/actor/actor.py
+-rw-r--r--   0        0        0     3357 2024-06-01 19:36:02.174813 sdss_hal-1.3.3/src/hal/actor/commands/__init__.py
+-rw-r--r--   0        0        0     2014 2024-06-01 19:36:02.174813 sdss_hal-1.3.3/src/hal/actor/commands/abort_exposures.py
+-rw-r--r--   0        0        0     4811 2024-06-01 19:36:02.174813 sdss_hal-1.3.3/src/hal/actor/commands/auto_pilot.py
+-rw-r--r--   0        0        0     1593 2024-06-01 19:36:02.174813 sdss_hal-1.3.3/src/hal/actor/commands/bypass.py
+-rw-r--r--   0        0        0      844 2024-06-01 19:36:02.174813 sdss_hal-1.3.3/src/hal/actor/commands/calibrations.py
+-rw-r--r--   0        0        0     8082 2024-06-01 19:36:02.174813 sdss_hal-1.3.3/src/hal/actor/commands/expose.py
+-rw-r--r--   0        0        0     1669 2024-06-01 19:36:02.174813 sdss_hal-1.3.3/src/hal/actor/commands/goto.py
+-rw-r--r--   0        0        0     3498 2024-06-01 19:36:02.174813 sdss_hal-1.3.3/src/hal/actor/commands/goto_field.py
+-rw-r--r--   0        0        0     2537 2024-06-01 19:36:02.174813 sdss_hal-1.3.3/src/hal/actor/commands/script.py
+-rw-r--r--   0        0        0     1419 2024-06-01 19:36:02.174813 sdss_hal-1.3.3/src/hal/actor/commands/status.py
+-rw-r--r--   0        0        0      687 2024-06-01 19:36:02.174813 sdss_hal-1.3.3/src/hal/actor/commands/test.py
+-rw-r--r--   0        0        0     3362 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/etc/hal.yml
+-rw-r--r--   0        0        0     2240 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/etc/schema.json
+-rw-r--r--   0        0        0      346 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/etc/scripts/apo/cartchange.inp
+-rw-r--r--   0        0        0     1161 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/etc/scripts/apo/eveningcals.inp
+-rw-r--r--   0        0        0      161 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/etc/scripts/apo/example.inp
+-rw-r--r--   0        0        0     1616 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/etc/scripts/apo/morningcals.inp
+-rw-r--r--   0        0        0       35 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/etc/scripts/apo/test.inp
+-rw-r--r--   0        0        0      346 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/etc/scripts/lco/cartchange.inp
+-rw-r--r--   0        0        0     1056 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/etc/scripts/lco/eveningcals.inp
+-rw-r--r--   0        0        0     1450 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/etc/scripts/lco/morningcals.inp
+-rw-r--r--   0        0        0     1180 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/exceptions.py
+-rw-r--r--   0        0        0     3502 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/helpers/__init__.py
+-rw-r--r--   0        0        0    10936 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/helpers/apogee.py
+-rw-r--r--   0        0        0     7942 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/helpers/boss.py
+-rw-r--r--   0        0        0     6514 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/helpers/cherno.py
+-rw-r--r--   0        0        0     1769 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/helpers/ffs.py
+-rw-r--r--   0        0        0     8276 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/helpers/jaeger.py
+-rw-r--r--   0        0        0    10429 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/helpers/lamps.py
+-rw-r--r--   0        0        0     4732 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/helpers/overhead.py
+-rw-r--r--   0        0        0     4671 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/helpers/scripts.py
+-rw-r--r--   0        0        0    13441 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/helpers/tcc.py
+-rw-r--r--   0        0        0     1399 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/macros/__init__.py
+-rw-r--r--   0        0        0     3844 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/macros/apogee_dome_flat.py
+-rw-r--r--   0        0        0    13331 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/macros/auto_pilot.py
+-rw-r--r--   0        0        0    21726 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/macros/expose.py
+-rw-r--r--   0        0        0    24268 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/macros/goto_field.py
+-rw-r--r--   0        0        0    18881 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/macros/macro.py
+-rw-r--r--   0        0        0     1263 2024-06-01 19:36:02.178813 sdss_hal-1.3.3/src/hal/macros/test_macro.py
+-rw-r--r--   0        0        0     2219 1970-01-01 00:00:00.000000 sdss_hal-1.3.3/PKG-INFO
```

### Comparing `sdss_hal-1.3.2/LICENSE.md` & `sdss_hal-1.3.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/README.md` & `sdss_hal-1.3.3/README.md`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/pyproject.toml` & `sdss_hal-1.3.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sdss-hal"
-version = "1.3.2"
+version = "1.3.3"
 description = "High-level observing tool for SDSS-V (replaces SOP)"
 authors = ["José Sánchez-Gallego <gallegoj@uw.edu>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://github.com/sdss/hal"
 repository = "https://github.com/sdss/hal"
 documentation = "https://sdss-hal.readthedocs.org"
```

### Comparing `sdss_hal-1.3.2/src/hal/__main__.py` & `sdss_hal-1.3.3/src/hal/__main__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/actor/actor.py` & `sdss_hal-1.3.3/src/hal/actor/actor.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/actor/commands/__init__.py` & `sdss_hal-1.3.3/src/hal/actor/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/actor/commands/abort_exposures.py` & `sdss_hal-1.3.3/src/hal/actor/commands/abort_exposures.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/actor/commands/auto_pilot.py` & `sdss_hal-1.3.3/src/hal/actor/commands/auto_pilot.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/actor/commands/bypass.py` & `sdss_hal-1.3.3/src/hal/actor/commands/bypass.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/actor/commands/calibrations.py` & `sdss_hal-1.3.3/src/hal/actor/commands/calibrations.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/actor/commands/expose.py` & `sdss_hal-1.3.3/src/hal/actor/commands/expose.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/actor/commands/goto.py` & `sdss_hal-1.3.3/src/hal/actor/commands/goto.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/actor/commands/goto_field.py` & `sdss_hal-1.3.3/src/hal/actor/commands/goto_field.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/actor/commands/script.py` & `sdss_hal-1.3.3/src/hal/actor/commands/script.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/actor/commands/status.py` & `sdss_hal-1.3.3/src/hal/actor/commands/status.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/actor/commands/test.py` & `sdss_hal-1.3.3/src/hal/actor/commands/test.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/etc/hal.yml` & `sdss_hal-1.3.3/src/hal/etc/hal.yml`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/etc/schema.json` & `sdss_hal-1.3.3/src/hal/etc/schema.json`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/etc/scripts/apo/eveningcals.inp` & `sdss_hal-1.3.3/src/hal/etc/scripts/apo/eveningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/etc/scripts/apo/morningcals.inp` & `sdss_hal-1.3.3/src/hal/etc/scripts/apo/morningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/etc/scripts/lco/eveningcals.inp` & `sdss_hal-1.3.3/src/hal/etc/scripts/lco/eveningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/etc/scripts/lco/morningcals.inp` & `sdss_hal-1.3.3/src/hal/etc/scripts/lco/morningcals.inp`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/exceptions.py` & `sdss_hal-1.3.3/src/hal/exceptions.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/helpers/__init__.py` & `sdss_hal-1.3.3/src/hal/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/helpers/apogee.py` & `sdss_hal-1.3.3/src/hal/helpers/apogee.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,14 +306,15 @@
     async def abort(self, command: HALCommandType):
         """Aborts the ongoing exposure."""
 
         if not self.is_exposing():
             return True
 
         await self._send_command(command, "apogee", "expose stop", time_limit=60)
+        await self.shutter(command, open=False, shutter="apogee")
 
         return True
 
 
 class APOGEEGangHelper:
     """Helper for the APOGEE gang connector."""
```

### Comparing `sdss_hal-1.3.2/src/hal/helpers/boss.py` & `sdss_hal-1.3.3/src/hal/helpers/boss.py`

 * *Files 2% similar despite different names*

```diff
@@ -256,12 +256,18 @@
 
         if not self.is_exposing():
             command.warning("No BOSS exposure to abort.")
             return True
 
         if self.actor.observatory == "LCO":
             await self._send_command(command, "yao", "abort --reset", time_limit=60)
+            await self._send_command(
+                command,
+                "yao",
+                "mech close shutter",
+                time_limit=20,
+            )
         else:
             await self._send_command(command, "boss", "exposure abort", time_limit=60)
             await self._send_command(command, "boss", "clearExposure", time_limit=30)
 
         return True
```

### Comparing `sdss_hal-1.3.2/src/hal/helpers/cherno.py` & `sdss_hal-1.3.3/src/hal/helpers/cherno.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/helpers/ffs.py` & `sdss_hal-1.3.3/src/hal/helpers/ffs.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/helpers/jaeger.py` & `sdss_hal-1.3.3/src/hal/helpers/jaeger.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/helpers/lamps.py` & `sdss_hal-1.3.3/src/hal/helpers/lamps.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/helpers/overhead.py` & `sdss_hal-1.3.3/src/hal/helpers/overhead.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/helpers/scripts.py` & `sdss_hal-1.3.3/src/hal/helpers/scripts.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/helpers/tcc.py` & `sdss_hal-1.3.3/src/hal/helpers/tcc.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/macros/__init__.py` & `sdss_hal-1.3.3/src/hal/macros/__init__.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/macros/apogee_dome_flat.py` & `sdss_hal-1.3.3/src/hal/macros/apogee_dome_flat.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/macros/auto_pilot.py` & `sdss_hal-1.3.3/src/hal/macros/auto_pilot.py`

 * *Files 3% similar despite different names*

```diff
@@ -182,14 +182,20 @@
         c_id = self.helpers.jaeger.configuration.configuration_id
         d_id = self.helpers.jaeger.configuration.design_id
         self._auto_pilot_message(f"Processign configuration {c_id} ({d_id})")
 
     async def goto_field(self):
         """Runs the go-to field procedure."""
 
+        goto_macro = self.helpers.macros["goto_field"]
+        if goto_macro.running:
+            self._auto_pilot_message("Waiting for goto-field macro to complete", "w")
+            if not await goto_macro.wait_until_complete():
+                raise MacroError("Background goto-field failed. Cancelling auto mode.")
+
         configuration = self.helpers.jaeger.configuration
         if configuration is None:
             raise MacroError("No configuration loaded.")
 
         if configuration.goto_complete:
             self._auto_pilot_message("Goto-field already complete")
             return
@@ -200,17 +206,17 @@
             self._auto_pilot_message("Skipping goto-field")
             return
 
         if self.hartmann and "boss_hartmann" not in stages:
             stages.append("boss_hartmann")
 
         self._auto_pilot_message("Running goto-field")
-        self.helpers.macros["goto_field"].reset(self.command, stages)
+        goto_macro.reset(self.command, stages)
 
-        result = await self.helpers.macros["goto_field"].run()
+        result = await goto_macro.run()
 
         if self.hartmann and "boss_hartmann" in stages:
             self.hartmann = False
 
         if not result:
             raise MacroError("Goto-field failed during auto pilot mode.")
```

### Comparing `sdss_hal-1.3.2/src/hal/macros/expose.py` & `sdss_hal-1.3.3/src/hal/macros/expose.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/macros/goto_field.py` & `sdss_hal-1.3.3/src/hal/macros/goto_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -273,14 +273,16 @@
         )
 
         await self._all_lamps_off(wait=False)
 
     async def acquire(self):
         """Acquires the field."""
 
+        self._mark_design_as_goto_complete()
+
         if self.helpers.cherno.is_guiding():
             self.command.info("Already guiding.")
             return
 
         await self._guide_preconditions("acquire")
 
         acquisition_config = self.config["acquisition"][self.observatory]
@@ -316,14 +318,16 @@
                 )
             else:
                 raise
 
     async def guide(self):
         """Starts the guide loop."""
 
+        self._mark_design_as_goto_complete()
+
         if self.helpers.cherno.is_guiding():
             self.command.info("Already guiding.")
             return
 
         await self._guide_preconditions("guide")
 
         guide_config = self.config["guide"][self.observatory]
@@ -343,26 +347,34 @@
     async def cleanup(self):
         """Turns off all lamps."""
 
         if self.observatory == "LCO":
             await asyncio.sleep(3)
 
         # If enough stages have run, mark this configuration as goto_complete.
-        if self.helpers.jaeger.configuration is not None and self._is_goto_complete():
-            self.helpers.jaeger.configuration.goto_complete = True
+        self._mark_design_as_goto_complete()
 
         if self._lamps_task is not None and not self._lamps_task.done():
             self._lamps_task.cancel()
 
         await self._all_lamps_off()
 
         # Read any pending BOSS exposure.
         if self.helpers.boss.readout_pending:
             await self.helpers.boss.readout(self.command)
 
+    def _mark_design_as_goto_complete(self):
+        """Marks the design as goto_complete."""
+
+        if self.helpers.jaeger.configuration is not None:
+            if self._is_goto_complete():
+                self.helpers.jaeger.configuration.goto_complete = True
+            else:
+                self.helpers.jaeger.configuration.goto_complete = False
+
     def _get_pointing(self):
         """Returns the configuration pointing."""
 
         configuration_loaded = self.actor.models["jaeger"]["configuration_loaded"]
         ra, dec, pa = configuration_loaded[3:6]
 
         if any([ra is None, dec is None, pa is None]):
```

### Comparing `sdss_hal-1.3.2/src/hal/macros/macro.py` & `sdss_hal-1.3.3/src/hal/macros/macro.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/src/hal/macros/test_macro.py` & `sdss_hal-1.3.3/src/hal/macros/test_macro.py`

 * *Files identical despite different names*

### Comparing `sdss_hal-1.3.2/PKG-INFO` & `sdss_hal-1.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdss-hal
-Version: 1.3.2
+Version: 1.3.3
 Summary: High-level observing tool for SDSS-V (replaces SOP)
 Home-page: https://github.com/sdss/hal
 License: BSD-3-Clause
 Keywords: astronomy,software
 Author: José Sánchez-Gallego
 Author-email: gallegoj@uw.edu
 Requires-Python: >=3.10,<4.0
```

