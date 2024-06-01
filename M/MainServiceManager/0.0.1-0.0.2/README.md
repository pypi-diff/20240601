# Comparing `tmp/mainservicemanager-0.0.1.tar.gz` & `tmp/mainservicemanager-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mainservicemanager-0.0.1.tar", max compression
+gzip compressed data, was "mainservicemanager-0.0.2.tar", max compression
```

## Comparing `mainservicemanager-0.0.1.tar` & `mainservicemanager-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rwxr-xr-x   0        0        0     2362 2024-05-31 12:41:29.000000 mainservicemanager-0.0.1/README.md
--rwxr-xr-x   0        0        0      691 2024-05-31 11:25:14.000000 mainservicemanager-0.0.1/pyproject.toml
--rwxr-xr-x   0        0        0      376 2024-05-31 13:15:11.000000 mainservicemanager-0.0.1/src/MainServiceManager/__init__.py
--rwxr-xr-x   0        0        0      224 2024-05-31 11:36:30.000000 mainservicemanager-0.0.1/src/MainServiceManager/__main__.py
--rwxr-xr-x   0        0        0     6571 2024-05-31 13:15:13.000000 mainservicemanager-0.0.1/src/MainServiceManager/api.py
--rwxr-xr-x   0        0        0     7186 2024-05-31 11:51:16.000000 mainservicemanager-0.0.1/src/MainServiceManager/server.py
--rwxr-xr-x   0        0        0     6465 2024-05-31 12:24:14.000000 mainservicemanager-0.0.1/src/MainServiceManager/server_utils.py
--rw-r--r--   0        0        0     3267 1970-01-01 00:00:00.000000 mainservicemanager-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     3851 2024-05-31 14:38:52.000000 mainservicemanager-0.0.2/README.md
+-rwxr-xr-x   0        0        0      691 2024-06-01 06:14:28.000000 mainservicemanager-0.0.2/pyproject.toml
+-rwxr-xr-x   0        0        0      376 2024-06-01 06:14:20.000000 mainservicemanager-0.0.2/src/MainServiceManager/__init__.py
+-rwxr-xr-x   0        0        0      224 2024-05-31 11:36:30.000000 mainservicemanager-0.0.2/src/MainServiceManager/__main__.py
+-rwxr-xr-x   0        0        0     6571 2024-05-31 13:15:12.000000 mainservicemanager-0.0.2/src/MainServiceManager/api.py
+-rwxr-xr-x   0        0        0     7205 2024-06-01 06:10:06.000000 mainservicemanager-0.0.2/src/MainServiceManager/server.py
+-rwxr-xr-x   0        0        0     6869 2024-06-01 06:06:38.000000 mainservicemanager-0.0.2/src/MainServiceManager/server_utils.py
+-rw-r--r--   0        0        0     4756 1970-01-01 00:00:00.000000 mainservicemanager-0.0.2/PKG-INFO
```

### Comparing `mainservicemanager-0.0.1/README.md` & `mainservicemanager-0.0.2/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,56 @@
+# Описание
+MainServiceManager - менеджер сервисов (аналогично `systemctl` в `Linux`). Каждый пользователь может запустить свой сервер MainServiceManager при условии, что они запущены на разных портах. Программы, у которых есть пароль, могут использовать API для управления всем сервером и всеми сервисами. Сервисы могут использовать API для управления собой (ограниченный доступ).
+# Использование встроенного API
+```python
+from MainServiceManager import Launcher
+# Инициализация API
+launcher=Launcher({"user":"admin","password":"qwerty :)"})
+# Проверить статус сервера
+try:
+  launcher.admin_status()
+  print("Сервер доступен")
+except:
+  print("Сервер недоступен")
+# Остановить сервер
+launcher.admin_stop()
+```
 # Конфиг сервера
-По умолчанию настройки сервера хранятся в файле "~/.config/MainServiceManager/cfg.json"
+По умолчанию настройки сервера хранятся в файле `~/.config/MainServiceManager/cfg.json`
 Если файл не существует, он будет создан
 Настройки по умолчанию:
 ```json
 {
   "host":"127.0.0.1",
   "password":"",
   "port":8960,
   "services_dir":"{папка с конфигом}/services",
 }
 ```
 - `host` - IP адрес, на котором будет запущен сервер
 - `port` - порт, на котором будет запущен сервер
-- `password` - пароль от аккаунта `admin`
+- `password` - пароль от аккаунта `admin`. Не забудьте его изменить!
 - `services_dir` - папка с файлами сервисов
 # Файлы сервисов
 Если параметр не указан, он равен `null`
 Недопустимые параметры игнорируются, но видны при получении информации о сервисе
 Тип записи:
 - `параметр` (`тип`) - описание
 ## Обязательные параметры
 - `args` (`list`) - список аргументов для запуска
 ## Дополнительные параметры
-- `autostart` (`bool`) - включать сервис автоматически?
-- `data_path` (`str`) - путь к файлу JSON для записи информации о сервисе (в том числе пароль)
+- `autostart` (`bool`) - включать сервис при запуске сервера?
+- `data_path` (`str`) - путь к файлу JSON для записи информации о сервисе (в том числе персональный пароль)
 - `cwd` (`str`) - рабочая папка
 - `env` (`dict`) - переменные среды
 - `clean_env` (`bool`) - отключить наследование ENV от процесса сервера?
 - `restart` (`str`) - условие для автоматического перезапуска
 - | `"always"` - перезапускать при любой остановке процесса
-- | `"on_error"` - перезапускать если процесс закрылся с кодом !=0
+- | `"on_error"` - перезапускать если процесс остановился с кодом ≠0
+- | `"code=N"` - (в будущем) перезапускать если процесс остановился с кодом N
+- | `"code!=N"` - (в будущем) перезапускать если процесс остановился с кодом ≠N
+- | `null` - не перезапускать
 ## Параметры для Linux
 Если параметры недоступны, они игнорируются
-- `user` (`str`) - пользователь, от имени которого запускать процесс
-- `group` (`str`) - группа, в которой запускать процесс
+- `user` (`str`) - пользователь, от имени которого нужно запускать процесс
+- `group` (`str`) - группа, в которой нужно запускать процесс
 - `extra_groups` (`unknown`) - неизвестно, не рекомендуется для использования
```

### Comparing `mainservicemanager-0.0.1/pyproject.toml` & `mainservicemanager-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "MainServiceManager"
-version = "0.0.1"
+version = "0.0.2"
 description = "Пользовательская программа для управления сервисами, аналогично systemd"
 authors = ["MainPlay TG <xbox.roman6666666666@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/MainPlay-TG/MainServiceManager.py"
 packages = [
 { include = "MainServiceManager", from = "src" },
 ]
```

### Comparing `mainservicemanager-0.0.1/src/MainServiceManager/api.py` & `mainservicemanager-0.0.2/src/MainServiceManager/api.py`

 * *Files identical despite different names*

### Comparing `mainservicemanager-0.0.1/src/MainServiceManager/server.py` & `mainservicemanager-0.0.2/src/MainServiceManager/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -269,10 +269,11 @@
   name=svc.name
   svc.close()
   if name in services:
     services.pop(name)
   r=make_r()
   return r
 if __name__=="__main__":
+  check_port(cfg)
   admin_reload(True)
   init()
   app.run(cfg["host"],cfg["port"],False)
```

### Comparing `mainservicemanager-0.0.1/src/MainServiceManager/server_utils.py` & `mainservicemanager-0.0.2/src/MainServiceManager/server_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -215,8 +215,19 @@
     "status":status,
     }
   kw["status"]=code
   kw["content_type"]="application/json"
   kw["response"]=ms.json.encode(d)
   r=Response(**kw)
   # r.headers["Content-Type"]="application/json; charset=utf-8"
-  return r
+  return r
+def check_port(cfg:ms.cfg):
+  try:
+    if cfg["host"]=="0.0.0.0":
+      host="127.0.0.1"
+    else:
+      host=cfg["host"]
+    port=cfg["port"]
+    requests.request("GET",f"http://{host}:{port}/admin/status")
+    raise OSError("It was not possible to launch the server at {host}:{port}".format(host=cfg["host"],port=cfg["port"]))
+  except requests.exceptions.ConnectionError:
+    return True
```

### Comparing `mainservicemanager-0.0.1/PKG-INFO` & `mainservicemanager-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MainServiceManager
-Version: 0.0.1
+Version: 0.0.2
 Summary: Пользовательская программа для управления сервисами, аналогично systemd
 Home-page: https://github.com/MainPlay-TG/MainServiceManager.py
 Author: MainPlay TG
 Author-email: xbox.roman6666666666@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -14,44 +14,63 @@
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Flask (>=3.0.3,<4.0.0)
 Requires-Dist: MainShortcuts (>=1.6.95,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/MainPlay-TG/MainServiceManager.py
 Description-Content-Type: text/markdown
 
+# Описание
+MainServiceManager - менеджер сервисов (аналогично `systemctl` в `Linux`). Каждый пользователь может запустить свой сервер MainServiceManager при условии, что они запущены на разных портах. Программы, у которых есть пароль, могут использовать API для управления всем сервером и всеми сервисами. Сервисы могут использовать API для управления собой (ограниченный доступ).
+# Использование встроенного API
+```python
+from MainServiceManager import Launcher
+# Инициализация API
+launcher=Launcher({"user":"admin","password":"qwerty :)"})
+# Проверить статус сервера
+try:
+  launcher.admin_status()
+  print("Сервер доступен")
+except:
+  print("Сервер недоступен")
+# Остановить сервер
+launcher.admin_stop()
+```
 # Конфиг сервера
-По умолчанию настройки сервера хранятся в файле "~/.config/MainServiceManager/cfg.json"
+По умолчанию настройки сервера хранятся в файле `~/.config/MainServiceManager/cfg.json`
 Если файл не существует, он будет создан
 Настройки по умолчанию:
 ```json
 {
   "host":"127.0.0.1",
   "password":"",
   "port":8960,
   "services_dir":"{папка с конфигом}/services",
 }
 ```
 - `host` - IP адрес, на котором будет запущен сервер
 - `port` - порт, на котором будет запущен сервер
-- `password` - пароль от аккаунта `admin`
+- `password` - пароль от аккаунта `admin`. Не забудьте его изменить!
 - `services_dir` - папка с файлами сервисов
 # Файлы сервисов
 Если параметр не указан, он равен `null`
 Недопустимые параметры игнорируются, но видны при получении информации о сервисе
 Тип записи:
 - `параметр` (`тип`) - описание
 ## Обязательные параметры
 - `args` (`list`) - список аргументов для запуска
 ## Дополнительные параметры
-- `autostart` (`bool`) - включать сервис автоматически?
-- `data_path` (`str`) - путь к файлу JSON для записи информации о сервисе (в том числе пароль)
+- `autostart` (`bool`) - включать сервис при запуске сервера?
+- `data_path` (`str`) - путь к файлу JSON для записи информации о сервисе (в том числе персональный пароль)
 - `cwd` (`str`) - рабочая папка
 - `env` (`dict`) - переменные среды
 - `clean_env` (`bool`) - отключить наследование ENV от процесса сервера?
 - `restart` (`str`) - условие для автоматического перезапуска
 - | `"always"` - перезапускать при любой остановке процесса
-- | `"on_error"` - перезапускать если процесс закрылся с кодом !=0
+- | `"on_error"` - перезапускать если процесс остановился с кодом ≠0
+- | `"code=N"` - (в будущем) перезапускать если процесс остановился с кодом N
+- | `"code!=N"` - (в будущем) перезапускать если процесс остановился с кодом ≠N
+- | `null` - не перезапускать
 ## Параметры для Linux
 Если параметры недоступны, они игнорируются
-- `user` (`str`) - пользователь, от имени которого запускать процесс
-- `group` (`str`) - группа, в которой запускать процесс
+- `user` (`str`) - пользователь, от имени которого нужно запускать процесс
+- `group` (`str`) - группа, в которой нужно запускать процесс
 - `extra_groups` (`unknown`) - неизвестно, не рекомендуется для использования
```

