# Comparing `tmp/plugin_jm_server-0.1.8.tar.gz` & `tmp/plugin_jm_server-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plugin_jm_server-0.1.8.tar", last modified: Sun Jan 14 08:49:05 2024, max compression
+gzip compressed data, was "plugin_jm_server-0.1.9.tar", last modified: Sun Jan 14 09:28:03 2024, max compression
```

## Comparing `plugin_jm_server-0.1.8.tar` & `plugin_jm_server-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 08:49:05.528127 plugin_jm_server-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-01-14 08:49:05.524127 plugin_jm_server-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-01-14 08:48:57.000000 plugin_jm_server-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-14 08:49:05.528127 plugin_jm_server-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-01-14 08:48:57.000000 plugin_jm_server-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 08:49:05.524127 plugin_jm_server-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 08:49:05.524127 plugin_jm_server-0.1.8/src/plugin_jm_server/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-14 08:48:57.000000 plugin_jm_server-0.1.8/src/plugin_jm_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9643 2024-01-14 08:48:57.000000 plugin_jm_server-0.1.8/src/plugin_jm_server/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-01-14 08:48:57.000000 plugin_jm_server-0.1.8/src/plugin_jm_server/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     3138 2024-01-14 08:48:57.000000 plugin_jm_server-0.1.8/src/plugin_jm_server/files.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 08:49:05.524127 plugin_jm_server-0.1.8/src/plugin_jm_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-01-14 08:49:05.000000 plugin_jm_server-0.1.8/src/plugin_jm_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-01-14 08:49:05.000000 plugin_jm_server-0.1.8/src/plugin_jm_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 08:49:05.000000 plugin_jm_server-0.1.8/src/plugin_jm_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-14 08:49:05.000000 plugin_jm_server-0.1.8/src/plugin_jm_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-14 08:49:05.000000 plugin_jm_server-0.1.8/src/plugin_jm_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 09:28:03.927359 plugin_jm_server-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-01-14 09:28:03.927359 plugin_jm_server-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-01-14 09:27:55.000000 plugin_jm_server-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-14 09:28:03.927359 plugin_jm_server-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 2024-01-14 09:27:55.000000 plugin_jm_server-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 09:28:03.923359 plugin_jm_server-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 09:28:03.923359 plugin_jm_server-0.1.9/src/plugin_jm_server/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-01-14 09:27:55.000000 plugin_jm_server-0.1.9/src/plugin_jm_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9681 2024-01-14 09:27:55.000000 plugin_jm_server-0.1.9/src/plugin_jm_server/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-01-14 09:27:55.000000 plugin_jm_server-0.1.9/src/plugin_jm_server/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3130 2024-01-14 09:27:55.000000 plugin_jm_server-0.1.9/src/plugin_jm_server/files.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-14 09:28:03.927359 plugin_jm_server-0.1.9/src/plugin_jm_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-01-14 09:28:03.000000 plugin_jm_server-0.1.9/src/plugin_jm_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-01-14 09:28:03.000000 plugin_jm_server-0.1.9/src/plugin_jm_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-14 09:28:03.000000 plugin_jm_server-0.1.9/src/plugin_jm_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-01-14 09:28:03.000000 plugin_jm_server-0.1.9/src/plugin_jm_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-01-14 09:28:03.000000 plugin_jm_server-0.1.9/src/plugin_jm_server.egg-info/top_level.txt
```

### Comparing `plugin_jm_server-0.1.8/PKG-INFO` & `plugin_jm_server-0.1.9/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugin_jm_server
-Version: 0.1.8
+Version: 0.1.9
 Summary: plugin_jm_server, a plugin for jmcomic that can be used to view comics in a web browser.
 Home-page: https://github.com/hect0x7/plugin-jm-server
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -19,10 +19,58 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: jmcomic
 Requires-Dist: flask
 Requires-Dist: psutil
 
-源项目：https://github.com/AiCorein/Flask-Files-Server
+基于原项目：https://github.com/AiCorein/Flask-Files-Server
+
+为了方便修改，将原项目中的文件复制到本项目中，然后进行修改
+
+# 使用方式
+
+
+
+## 1. pip安装
+
+```shell
+pip install plugin_jm_server
+```
+
+
+
+## 2. 运行代码
+
+* **HTTP版**
+
+```python
+from plugin_jm_server import *
+
+# http
+server = JmServer(
+    'D:/',
+    'password',
+)
+server.run(
+    host='0.0.0.0',
+    port=80,
+)
+```
+
+* **HTTPS版**
+
+```python
+from plugin_jm_server import *
+
+# https
+server = JmServer(
+    'D:/',
+    'password',
+)
+server.run(
+    host='0.0.0.0',
+    port=443,
+    ssl_context='adhoc',
+)
+```
 
-为了方便修改，将源项目中的文件复制到本项目中，然后进行修改
```

### Comparing `plugin_jm_server-0.1.8/setup.py` & `plugin_jm_server-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `plugin_jm_server-0.1.8/src/plugin_jm_server/app.py` & `plugin_jm_server-0.1.9/src/plugin_jm_server/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from urllib.parse import quote
 import os
 import re
 from typing import Optional
 
 import common
 from flask import Flask, abort
 from flask import render_template, send_from_directory
@@ -116,15 +117,15 @@
             return abort(404)
 
         print(f'jm_view: {path}')
         return render_template(self.url_format(self.mobile_check(), "jm_view.html"),
                                data={
                                    'title': common.of_file_name(path),
                                    'images': self.file_manager.get_jm_view_images(path),
-                                   'openFromDir': openFromDir,
+                                   'openFromDir': quote(openFromDir),
                                },
                                randomArg=self.url_random_arg())
 
     def view_file(self):
         """
         获取单个文件
         """
```

### Comparing `plugin_jm_server-0.1.8/src/plugin_jm_server/driver.py` & `plugin_jm_server-0.1.9/src/plugin_jm_server/driver.py`

 * *Files identical despite different names*

### Comparing `plugin_jm_server-0.1.8/src/plugin_jm_server/files.py` & `plugin_jm_server-0.1.9/src/plugin_jm_server/files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from urllib.parse import quote
 import os
 import time
 
 import common
 
 
 class FileManager:
@@ -17,15 +18,14 @@
             return get_winDriver()
         else:
             return ['/']
 
     def get_jm_view_images(self, path):
         images_data = []
 
-        from urllib.parse import quote
         for f in self.files_of_dir_safe(path):
             if not self.is_image_file(f):
                 continue
             f = quote(f)
             images_data.append({
                 "filename": common.of_file_name(f),
                 "data_original": f'/view_file?path={f}',
```

### Comparing `plugin_jm_server-0.1.8/src/plugin_jm_server.egg-info/PKG-INFO` & `plugin_jm_server-0.1.9/src/plugin_jm_server.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plugin_jm_server
-Version: 0.1.8
+Version: 0.1.9
 Summary: plugin_jm_server, a plugin for jmcomic that can be used to view comics in a web browser.
 Home-page: https://github.com/hect0x7/plugin-jm-server
 Author: hect0x7
 Author-email: 93357912+hect0x7@users.noreply.github.com
 Keywords: python,jmcomic,18comic,禁漫天堂,NSFW
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -19,10 +19,58 @@
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Requires-Dist: jmcomic
 Requires-Dist: flask
 Requires-Dist: psutil
 
-源项目：https://github.com/AiCorein/Flask-Files-Server
+基于原项目：https://github.com/AiCorein/Flask-Files-Server
+
+为了方便修改，将原项目中的文件复制到本项目中，然后进行修改
+
+# 使用方式
+
+
+
+## 1. pip安装
+
+```shell
+pip install plugin_jm_server
+```
+
+
+
+## 2. 运行代码
+
+* **HTTP版**
+
+```python
+from plugin_jm_server import *
+
+# http
+server = JmServer(
+    'D:/',
+    'password',
+)
+server.run(
+    host='0.0.0.0',
+    port=80,
+)
+```
+
+* **HTTPS版**
+
+```python
+from plugin_jm_server import *
+
+# https
+server = JmServer(
+    'D:/',
+    'password',
+)
+server.run(
+    host='0.0.0.0',
+    port=443,
+    ssl_context='adhoc',
+)
+```
 
-为了方便修改，将源项目中的文件复制到本项目中，然后进行修改
```

