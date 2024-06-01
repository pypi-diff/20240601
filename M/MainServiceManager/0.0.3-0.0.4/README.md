# Comparing `tmp/mainservicemanager-0.0.3.tar.gz` & `tmp/mainservicemanager-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainservicemanager-0.0.3.tar", max compression
+gzip compressed data, was "mainservicemanager-0.0.4.tar", max compression
```

## Comparing `mainservicemanager-0.0.3.tar` & `mainservicemanager-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     3851 2024-05-31 14:38:52.000000 mainservicemanager-0.0.3/README.md
--rwxr-xr-x   0        0        0      736 2024-06-01 11:14:09.000000 mainservicemanager-0.0.3/pyproject.toml
--rwxr-xr-x   0        0        0      391 2024-06-01 11:14:03.000000 mainservicemanager-0.0.3/src/MainServiceManager/__init__.py
--rwxr-xr-x   0        0        0     4336 2024-06-01 10:55:15.000000 mainservicemanager-0.0.3/src/MainServiceManager/__main__.py
--rwxr-xr-x   0        0        0     6571 2024-05-31 13:15:12.000000 mainservicemanager-0.0.3/src/MainServiceManager/api.py
--rwxr-xr-x   0        0        0     7214 2024-06-01 08:54:09.000000 mainservicemanager-0.0.3/src/MainServiceManager/server.py
--rwxr-xr-x   0        0        0     6876 2024-06-01 09:36:37.000000 mainservicemanager-0.0.3/src/MainServiceManager/server_utils.py
--rw-r--r--   0        0        0     4756 1970-01-01 00:00:00.000000 mainservicemanager-0.0.3/PKG-INFO
+-rwxr-xr-x   0        0        0     3851 2024-05-31 14:38:52.000000 mainservicemanager-0.0.4/README.md
+-rwxr-xr-x   0        0        0      736 2024-06-01 11:21:01.000000 mainservicemanager-0.0.4/pyproject.toml
+-rwxr-xr-x   0        0        0      391 2024-06-01 11:20:52.000000 mainservicemanager-0.0.4/src/MainServiceManager/__init__.py
+-rwxr-xr-x   0        0        0     4331 2024-06-01 11:17:54.000000 mainservicemanager-0.0.4/src/MainServiceManager/__main__.py
+-rwxr-xr-x   0        0        0     6571 2024-05-31 13:15:12.000000 mainservicemanager-0.0.4/src/MainServiceManager/api.py
+-rwxr-xr-x   0        0        0     7214 2024-06-01 08:54:08.000000 mainservicemanager-0.0.4/src/MainServiceManager/server.py
+-rwxr-xr-x   0        0        0     6876 2024-06-01 09:36:36.000000 mainservicemanager-0.0.4/src/MainServiceManager/server_utils.py
+-rw-r--r--   0        0        0     4756 1970-01-01 00:00:00.000000 mainservicemanager-0.0.4/PKG-INFO
```

### Comparing `mainservicemanager-0.0.3/README.md` & `mainservicemanager-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.3/pyproject.toml` & `mainservicemanager-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MainServiceManager"
-version = "0.0.3"
+version = "0.0.4"
 description = "Пользовательская программа для управления сервисами, аналогично systemd"
 authors = ["MainPlay TG <xbox.roman6666666666@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainServiceManager.py"
 packages = [
 { include = "MainServiceManager", from = "src" },
 ]
```

### Comparing `mainservicemanager-0.0.3/src/MainServiceManager/__main__.py` & `mainservicemanager-0.0.4/src/MainServiceManager/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     action="store_true",
     help="print the version and exit",
     )
   argp.add_argument("-c","--config",
     default=None,
     help='config file. Default "~/.config/MainServiceManager/cfg.json"',
     )
-  argp.add_argument("-h","--host",
+  argp.add_argument("--host",
     default=None,
     help="host on which the server is launched. Default 127.0.0.1",
     )
   argp.add_argument("-p","--port",
     default=None,
     help="port on which the server is launched. Default 8960",
     )
```

### Comparing `mainservicemanager-0.0.3/src/MainServiceManager/api.py` & `mainservicemanager-0.0.4/src/MainServiceManager/api.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.3/src/MainServiceManager/server.py` & `mainservicemanager-0.0.4/src/MainServiceManager/server.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.3/src/MainServiceManager/server_utils.py` & `mainservicemanager-0.0.4/src/MainServiceManager/server_utils.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.3/PKG-INFO` & `mainservicemanager-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MainServiceManager
-Version: 0.0.3
+Version: 0.0.4
 Summary: Пользовательская программа для управления сервисами, аналогично systemd
 Home-page: https://github.com/MainPlay-TG/MainServiceManager.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

