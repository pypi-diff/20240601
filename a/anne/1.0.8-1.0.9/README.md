# Comparing `tmp/anne-1.0.8.tar.gz` & `tmp/anne-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anne-1.0.8.tar", last modified: Fri May 31 00:59:09 2024, max compression
+gzip compressed data, was "anne-1.0.9.tar", last modified: Sat Jun  1 08:25:30 2024, max compression
```

## Comparing `anne-1.0.8.tar` & `anne-1.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 00:59:09.863311 anne-1.0.8/
--rw-rw-rw-   0        0        0     1090 2024-05-28 14:49:46.000000 anne-1.0.8/LICENSE
--rw-rw-rw-   0        0        0     1731 2024-05-31 00:59:09.863311 anne-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       45 2024-05-28 15:27:28.000000 anne-1.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 00:59:09.857332 anne-1.0.8/app/
-drwxrwxrwx   0        0        0        0 2024-05-31 00:59:09.859325 anne-1.0.8/app/anne/
--rw-rw-rw-   0        0        0       64 2024-05-31 00:19:07.000000 anne-1.0.8/app/anne/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 00:59:09.861318 anne-1.0.8/app/anne/browser/
--rw-rw-rw-   0        0        0    18825 2024-05-31 00:58:51.000000 anne-1.0.8/app/anne/browser/AnneBrowser.py
--rw-rw-rw-   0        0        0       38 2024-05-31 00:17:53.000000 anne-1.0.8/app/anne/browser/__init__.py
--rw-rw-rw-   0        0        0      692 2024-05-28 16:07:51.000000 anne-1.0.8/app/anne/browser/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 00:59:09.862315 anne-1.0.8/app/anne/proxy/
--rw-rw-rw-   0        0        0      883 2024-05-31 00:59:04.000000 anne-1.0.8/app/anne/proxy/AnneProxy.py
--rw-rw-rw-   0        0        0       32 2024-05-31 00:19:01.000000 anne-1.0.8/app/anne/proxy/__init__.py
--rw-rw-rw-   0        0        0       16 2024-05-31 00:09:11.000000 anne-1.0.8/app/anne/proxy/utils.py
-drwxrwxrwx   0        0        0        0 2024-05-31 00:59:09.860321 anne-1.0.8/app/anne.egg-info/
--rw-rw-rw-   0        0        0     1731 2024-05-31 00:59:09.000000 anne-1.0.8/app/anne.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2024-05-31 00:59:09.000000 anne-1.0.8/app/anne.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 00:59:09.000000 anne-1.0.8/app/anne.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-05-31 00:59:09.000000 anne-1.0.8/app/anne.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-31 00:59:09.000000 anne-1.0.8/app/anne.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 00:59:09.863311 anne-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      859 2024-05-31 00:59:09.000000 anne-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 08:25:30.244944 anne-1.0.9/
+-rw-rw-rw-   0        0        0     1090 2024-05-28 14:49:46.000000 anne-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0     1731 2024-06-01 08:25:30.244944 anne-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       45 2024-05-28 15:27:28.000000 anne-1.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 08:25:30.240958 anne-1.0.9/app/
+drwxrwxrwx   0        0        0        0 2024-06-01 08:25:30.241954 anne-1.0.9/app/anne/
+-rw-rw-rw-   0        0        0       64 2024-05-31 00:19:07.000000 anne-1.0.9/app/anne/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 08:25:30.243947 anne-1.0.9/app/anne/browser/
+-rw-rw-rw-   0        0        0    18825 2024-05-31 00:58:51.000000 anne-1.0.9/app/anne/browser/AnneBrowser.py
+-rw-rw-rw-   0        0        0       38 2024-05-31 00:17:53.000000 anne-1.0.9/app/anne/browser/__init__.py
+-rw-rw-rw-   0        0        0      692 2024-05-28 16:07:51.000000 anne-1.0.9/app/anne/browser/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 08:25:30.243947 anne-1.0.9/app/anne/proxy/
+-rw-rw-rw-   0        0        0     1441 2024-06-01 08:25:02.000000 anne-1.0.9/app/anne/proxy/AnneProxy.py
+-rw-rw-rw-   0        0        0       32 2024-05-31 00:19:01.000000 anne-1.0.9/app/anne/proxy/__init__.py
+-rw-rw-rw-   0        0        0        2 2024-06-01 08:18:38.000000 anne-1.0.9/app/anne/proxy/utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 08:25:30.242951 anne-1.0.9/app/anne.egg-info/
+-rw-rw-rw-   0        0        0     1731 2024-06-01 08:25:30.000000 anne-1.0.9/app/anne.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2024-06-01 08:25:30.000000 anne-1.0.9/app/anne.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 08:25:30.000000 anne-1.0.9/app/anne.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-06-01 08:25:30.000000 anne-1.0.9/app/anne.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-06-01 08:25:30.000000 anne-1.0.9/app/anne.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 08:25:30.244944 anne-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      859 2024-06-01 08:25:29.000000 anne-1.0.9/setup.py
```

### Comparing `anne-1.0.8/LICENSE` & `anne-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `anne-1.0.8/PKG-INFO` & `anne-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anne
-Version: 1.0.8
+Version: 1.0.9
 Summary: Lib for lazy dev
 Home-page: https://github.com/mrship666/anne-lib
 Author: AnneHouman
 Author-email: annehouman01@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `anne-1.0.8/app/anne/browser/AnneBrowser.py` & `anne-1.0.9/app/anne/browser/AnneBrowser.py`

 * *Files identical despite different names*

### Comparing `anne-1.0.8/app/anne/browser/utils.py` & `anne-1.0.9/app/anne/browser/utils.py`

 * *Files identical despite different names*

### Comparing `anne-1.0.8/app/anne/proxy/AnneProxy.py` & `anne-1.0.9/app/anne/proxy/AnneProxy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,48 @@
-
-import requests, time, re
-from .utils import *
-
-
+import requests, time, re, os, zipfile
 
 
 class AnneProxy:
     def __init__(self, debug=False):
         self.debug = debug
-        
-    def format(self, proxy)->tuple:
+
+    def format(self, proxy) -> tuple:
         proxy = str(proxy).strip()
         pattern = re.compile(
-            r'(?:(?P<user>[^:@]+):(?P<pass>[^:@]+)[:@])?'
-            r'(?P<host>[^:@/]+)'
-            r':(?P<port>\d+)'
-            r'(?:[:@](?P<user2>[^:@]+):(?P<pass2>[^:@]+))?'
+            r'(?:(?P<user>[^:@|]+):(?P<pass>[^:@|]+)[:@|])?'
+            r'(?P<host>[^:@|/]+)'
+            r'[:@|](?P<port>\d+)'
+            r'(?:[:@|](?P<user2>[^:@|]+):(?P<pass2>[^:@|]+))?'
+            r'|'
+            r'(?:(?P<user3>[^:@|]+):(?P<pass3>[^:@|]+)@)?'
+            r'(?P<host2>[^:@|/]+)'
+            r'@(?P<port2>\d+)'
+            r'|'
+            r'(?P<host3>[^:@|/]+)@(?P<port3>\d+)'
         )
         match = pattern.match(proxy)
         if match:
-            user = match.group('user') if match.group('user') else match.group('user2')
-            passw = match.group('pass') if match.group('pass') else match.group('pass2')
-            return match.group('host'), match.group('port'), user, passw
+            user = match.group('user') or match.group('user2') or match.group('user3')
+            passw = match.group('pass') or match.group('pass2') or match.group('pass3')
+            host = match.group('host') or match.group('host2') or match.group('host3')
+            port = match.group('port') or match.group('port2') or match.group('port3')
+            return host, port, user, passw
         else:
             return None, None, None, None
 
+    def tmproxy(self,
+                mode='get_proxy',
+                api_key=None,
+                timeout=60):
+
+        if not api_key:
+            print('Please set api key')
+            return False
 
-
-
-
-
-
-
-
-
-
+        pass
```

### Comparing `anne-1.0.8/app/anne.egg-info/PKG-INFO` & `anne-1.0.9/app/anne.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anne
-Version: 1.0.8
+Version: 1.0.9
 Summary: Lib for lazy dev
 Home-page: https://github.com/mrship666/anne-lib
 Author: AnneHouman
 Author-email: annehouman01@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `anne-1.0.8/setup.py` & `anne-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("app/README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="anne",
-    version="1.0.8",
+    version="1.0.9",
     description="Lib for lazy dev",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/mrship666/anne-lib",
     author="AnneHouman",
```

