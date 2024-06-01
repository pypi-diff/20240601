# Comparing `tmp/mainservicemanager-0.0.2.tar.gz` & `tmp/mainservicemanager-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainservicemanager-0.0.2.tar", max compression
+gzip compressed data, was "mainservicemanager-0.0.3.tar", max compression
```

## Comparing `mainservicemanager-0.0.2.tar` & `mainservicemanager-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     3851 2024-05-31 14:38:52.000000 mainservicemanager-0.0.2/README.md
--rwxr-xr-x   0        0        0      691 2024-06-01 06:14:28.000000 mainservicemanager-0.0.2/pyproject.toml
--rwxr-xr-x   0        0        0      376 2024-06-01 06:14:20.000000 mainservicemanager-0.0.2/src/MainServiceManager/__init__.py
--rwxr-xr-x   0        0        0      224 2024-05-31 11:36:30.000000 mainservicemanager-0.0.2/src/MainServiceManager/__main__.py
--rwxr-xr-x   0        0        0     6571 2024-05-31 13:15:12.000000 mainservicemanager-0.0.2/src/MainServiceManager/api.py
--rwxr-xr-x   0        0        0     7205 2024-06-01 06:10:06.000000 mainservicemanager-0.0.2/src/MainServiceManager/server.py
--rwxr-xr-x   0        0        0     6869 2024-06-01 06:06:38.000000 mainservicemanager-0.0.2/src/MainServiceManager/server_utils.py
--rw-r--r--   0        0        0     4756 1970-01-01 00:00:00.000000 mainservicemanager-0.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0     3851 2024-05-31 14:38:52.000000 mainservicemanager-0.0.3/README.md
+-rwxr-xr-x   0        0        0      736 2024-06-01 11:14:09.000000 mainservicemanager-0.0.3/pyproject.toml
+-rwxr-xr-x   0        0        0      391 2024-06-01 11:14:03.000000 mainservicemanager-0.0.3/src/MainServiceManager/__init__.py
+-rwxr-xr-x   0        0        0     4336 2024-06-01 10:55:15.000000 mainservicemanager-0.0.3/src/MainServiceManager/__main__.py
+-rwxr-xr-x   0        0        0     6571 2024-05-31 13:15:12.000000 mainservicemanager-0.0.3/src/MainServiceManager/api.py
+-rwxr-xr-x   0        0        0     7214 2024-06-01 08:54:09.000000 mainservicemanager-0.0.3/src/MainServiceManager/server.py
+-rwxr-xr-x   0        0        0     6876 2024-06-01 09:36:37.000000 mainservicemanager-0.0.3/src/MainServiceManager/server_utils.py
+-rw-r--r--   0        0        0     4756 1970-01-01 00:00:00.000000 mainservicemanager-0.0.3/PKG-INFO
```

### Comparing `mainservicemanager-0.0.2/README.md` & `mainservicemanager-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.2/pyproject.toml` & `mainservicemanager-0.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 [tool.poetry]
 name = "MainServiceManager"
-version = "0.0.2"
+version = "0.0.3"
 description = "Пользовательская программа для управления сервисами, аналогично systemd"
 authors = ["MainPlay TG <xbox.roman6666666666@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainServiceManager.py"
 packages = [
 { include = "MainServiceManager", from = "src" },
 ]
 
 [tool.poetry.scripts]
-MSVC-server = "MainServiceManager.__main__:server_start"
+MSVC-client = "MainServiceManager.__main__:client"
+MSVC-server = "MainServiceManager.__main__:server"
 
 [tool.poetry.dependencies]
 Flask = "^3.0.3"
 MainShortcuts = "^1.6.95"
 python = "^3.8"
 requests = "^2.31.0"
```

### Comparing `mainservicemanager-0.0.2/src/MainServiceManager/api.py` & `mainservicemanager-0.0.3/src/MainServiceManager/api.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.2/src/MainServiceManager/server.py` & `mainservicemanager-0.0.3/src/MainServiceManager/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
   for k,v in list(services.items()):
     if v.closed:
       services.pop(k)
     else:
       v.reload()
       if v.closed:
         services.pop(k)
-  for i in ms.dir.list(cfg["services_dir"],"msvc",dirs=False):
+  for i in ms.dir.list(cfg["services_dir"],["json","msvc"],dirs=False):
     name=os.path.basename(i)
     if not name in services:
       services[name]=service(i)
   r=make_r()
   return r
 @app.route("/svc/info",methods=["GET"])
 def svc_info(internal=False,svc:service=None):
```

### Comparing `mainservicemanager-0.0.2/src/MainServiceManager/server_utils.py` & `mainservicemanager-0.0.3/src/MainServiceManager/server_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -166,15 +166,15 @@
   for i in dont_save:
     d[i]=cfg.data.pop(i)
   cfg.save()
   for i in dont_save:
     cfg[i]=d[i]
   return cfg.path
 def get_args(**kw)->argparse.Namespace:
-  kw["description"]=f"MainServiceManager {__version__}"
+  kw["description"]=f"MainServiceManager {__version__} server"
   kw["epilog"]="Creator: MainPlay_TG\nContact: https://t.me/MainPlay_TG\nMade in Russia"
   kw["formatter_class"]=argparse.RawTextHelpFormatter
   kw["prog"]="MSVC-server"
   argp=argparse.ArgumentParser(**kw)
   argp.add_argument("-v","--version",
     action="store_true",
     help="print the version and exit",
```

### Comparing `mainservicemanager-0.0.2/PKG-INFO` & `mainservicemanager-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MainServiceManager
-Version: 0.0.2
+Version: 0.0.3
 Summary: Пользовательская программа для управления сервисами, аналогично systemd
 Home-page: https://github.com/MainPlay-TG/MainServiceManager.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

