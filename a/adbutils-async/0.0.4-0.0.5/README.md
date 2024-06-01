# Comparing `tmp/adbutils_async-0.0.4.tar.gz` & `tmp/adbutils_async-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbutils_async-0.0.4.tar", last modified: Wed Apr  3 09:08:15 2024, max compression
+gzip compressed data, was "adbutils_async-0.0.5.tar", last modified: Sat Jun  1 04:47:04 2024, max compression
```

## Comparing `adbutils_async-0.0.4.tar` & `adbutils_async-0.0.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:08:15.386158 adbutils_async-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:08:15.378158 adbutils_async-0.0.4/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:08:15.378158 adbutils_async-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-03 09:08:15.000000 adbutils_async-0.0.4/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-03 09:08:15.000000 adbutils_async-0.0.4/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17604 2024-04-03 09:08:15.386158 adbutils_async-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:08:15.382158 adbutils_async-0.0.4/adbutils_async/
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/adbutils_async/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/adbutils_async/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9015 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/adbutils_async/_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)    42508 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/adbutils_async/_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/adbutils_async/_proto.py
--rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/adbutils_async/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/adbutils_async/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:08:15.382158 adbutils_async-0.0.4/adbutils_async/binaries/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/adbutils_async/binaries/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/adbutils_async/binaries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/adbutils_async/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    12635 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/adbutils_async/pidcat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:08:15.386158 adbutils_async-0.0.4/adbutils_async.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17604 2024-04-03 09:08:15.000000 adbutils_async-0.0.4/adbutils_async.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-03 09:08:15.000000 adbutils_async-0.0.4/adbutils_async.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:08:15.000000 adbutils_async-0.0.4/adbutils_async.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:08:15.000000 adbutils_async-0.0.4/adbutils_async.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-03 09:08:15.000000 adbutils_async-0.0.4/adbutils_async.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-03 09:08:15.000000 adbutils_async-0.0.4/adbutils_async.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-03 09:08:15.000000 adbutils_async-0.0.4/adbutils_async.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/build_wheel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-03 09:08:15.386158 adbutils_async-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:08:15.382158 adbutils_async-0.0.4/test_real_device/
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/test_real_device/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/test_real_device/test_adb.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/test_real_device/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/test_real_device/test_device.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/test_real_device/test_forward_reverse.py
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/test_real_device/test_import.py
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/test_real_device/test_record.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/test_real_device/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:08:15.382158 adbutils_async-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/tests/adb_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-03 09:08:10.000000 adbutils_async-0.0.4/tests/test_adb_server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:47:04.046463 adbutils_async-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:47:04.038462 adbutils_async-0.0.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:47:04.042462 adbutils_async-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1471 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-06-01 04:47:04.000000 adbutils_async-0.0.5/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-06-01 04:47:03.000000 adbutils_async-0.0.5/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17604 2024-06-01 04:47:04.046463 adbutils_async-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15377 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:47:04.042462 adbutils_async-0.0.5/adbutils_async/
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/adbutils_async/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11467 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/adbutils_async/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9039 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/adbutils_async/_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42508 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/adbutils_async/_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/adbutils_async/_proto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7657 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/adbutils_async/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/adbutils_async/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:47:04.042462 adbutils_async-0.0.5/adbutils_async/binaries/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/adbutils_async/binaries/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/adbutils_async/binaries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/adbutils_async/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12635 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/adbutils_async/pidcat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:47:04.046463 adbutils_async-0.0.5/adbutils_async.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17604 2024-06-01 04:47:04.000000 adbutils_async-0.0.5/adbutils_async.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-06-01 04:47:04.000000 adbutils_async-0.0.5/adbutils_async.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 04:47:04.000000 adbutils_async-0.0.5/adbutils_async.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 04:47:04.000000 adbutils_async-0.0.5/adbutils_async.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-06-01 04:47:04.000000 adbutils_async-0.0.5/adbutils_async.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 04:47:04.000000 adbutils_async-0.0.5/adbutils_async.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-06-01 04:47:04.000000 adbutils_async-0.0.5/adbutils_async.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6050 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/build_wheel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-06-01 04:47:04.046463 adbutils_async-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:47:04.046463 adbutils_async-0.0.5/test_real_device/
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/test_real_device/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/test_real_device/test_adb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/test_real_device/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/test_real_device/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/test_real_device/test_forward_reverse.py
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/test_real_device/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)      276 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/test_real_device/test_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/test_real_device/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 04:47:04.046463 adbutils_async-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3772 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/tests/adb_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1204 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-06-01 04:46:59.000000 adbutils_async-0.0.5/tests/test_adb_server.py
```

### Comparing `adbutils_async-0.0.4/.github/workflows/main.yml` & `adbutils_async-0.0.5/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/.github/workflows/publish-to-pypi.yml` & `adbutils_async-0.0.5/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/LICENSE` & `adbutils_async-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/PKG-INFO` & `adbutils_async-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbutils_async
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python adb async library for adb service.
 Home-page: https://github.com/touxiaoling/adbutils_async
 Author: tomin
 Author-email: tomin <tomin@tomin.com>
 License: MIT License
         
         Copyright (c) 2019 openatx
```

### Comparing `adbutils_async-0.0.4/README.md` & `adbutils_async-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/adbutils_async/__init__.py` & `adbutils_async-0.0.5/adbutils_async/__init__.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/adbutils_async/__main__.py` & `adbutils_async-0.0.5/adbutils_async/__main__.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/adbutils_async/_adb.py` & `adbutils_async-0.0.5/adbutils_async/_adb.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         self.timeout = n
 
     async def _safe_connect(self):
         try:
             return await asyncio.open_connection(self.__host, self.__port)
         except ConnectionRefusedError:
             # 20s should enough for adb start
-            await async_run((adb_path(), "start-server"), timeout=20.0)
+            await async_run((adb_path(), "-P", str(self.__port), "start-server"), timeout=20.0)
             return await asyncio.open_connection(self.__host, self.__port)
 
     async def safe_connect(self):
         self.__reader, self.__writer = await self._safe_connect()
         self._finalizer = weakref.finalize(self, self.__writer.close)
 
     @property
```

### Comparing `adbutils_async-0.0.4/adbutils_async/_device.py` & `adbutils_async-0.0.5/adbutils_async/_device.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/adbutils_async/_proto.py` & `adbutils_async-0.0.5/adbutils_async/_proto.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/adbutils_async/_utils.py` & `adbutils_async-0.0.5/adbutils_async/_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/adbutils_async/errors.py` & `adbutils_async-0.0.5/adbutils_async/errors.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/adbutils_async/pidcat.py` & `adbutils_async-0.0.5/adbutils_async/pidcat.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/adbutils_async.egg-info/PKG-INFO` & `adbutils_async-0.0.5/adbutils_async.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbutils_async
-Version: 0.0.4
+Version: 0.0.5
 Summary: Python adb async library for adb service.
 Home-page: https://github.com/touxiaoling/adbutils_async
 Author: tomin
 Author-email: tomin <tomin@tomin.com>
 License: MIT License
         
         Copyright (c) 2019 openatx
```

### Comparing `adbutils_async-0.0.4/adbutils_async.egg-info/SOURCES.txt` & `adbutils_async-0.0.5/adbutils_async.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/build_wheel.py` & `adbutils_async-0.0.5/build_wheel.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/pyproject.toml` & `adbutils_async-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/setup.cfg` & `adbutils_async-0.0.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/test_real_device/conftest.py` & `adbutils_async-0.0.5/test_real_device/conftest.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/test_real_device/test_adb.py` & `adbutils_async-0.0.5/test_real_device/test_adb.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/test_real_device/test_deprecated.py` & `adbutils_async-0.0.5/test_real_device/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/test_real_device/test_device.py` & `adbutils_async-0.0.5/test_real_device/test_device.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/test_real_device/test_forward_reverse.py` & `adbutils_async-0.0.5/test_real_device/test_forward_reverse.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/test_real_device/test_utils.py` & `adbutils_async-0.0.5/test_real_device/test_utils.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/tests/adb_server.py` & `adbutils_async-0.0.5/tests/adb_server.py`

 * *Files identical despite different names*

### Comparing `adbutils_async-0.0.4/tests/conftest.py` & `adbutils_async-0.0.5/tests/conftest.py`

 * *Files identical despite different names*

