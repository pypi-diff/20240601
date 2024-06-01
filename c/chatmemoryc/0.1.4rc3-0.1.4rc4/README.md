# Comparing `tmp/chatmemoryc-0.1.4rc3.tar.gz` & `tmp/chatmemoryc-0.1.4rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatmemoryc-0.1.4rc3.tar", last modified: Sat Jun  1 08:19:16 2024, max compression
+gzip compressed data, was "chatmemoryc-0.1.4rc4.tar", last modified: Sat Jun  1 08:43:22 2024, max compression
```

## Comparing `chatmemoryc-0.1.4rc3.tar` & `chatmemoryc-0.1.4rc4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 08:19:16.111918 chatmemoryc-0.1.4rc3/
--rw-rw-rw-   0        0        0    11324 2024-04-15 03:15:05.000000 chatmemoryc-0.1.4rc3/LICENSE.txt
--rw-rw-rw-   0        0        0     8021 2024-06-01 08:19:16.098522 chatmemoryc-0.1.4rc3/PKG-INFO
--rw-rw-rw-   0        0        0     7392 2024-04-15 03:59:14.000000 chatmemoryc-0.1.4rc3/README.md
-drwxrwxrwx   0        0        0        0 2024-06-01 08:19:16.082884 chatmemoryc-0.1.4rc3/chatmemoryc/
--rw-rw-rw-   0        0        0        0 2024-01-24 23:42:20.000000 chatmemoryc-0.1.4rc3/chatmemoryc/__init__.py
--rw-rw-rw-   0        0        0     1346 2024-06-01 07:41:39.000000 chatmemoryc-0.1.4rc3/chatmemoryc/__main__.py
--rw-rw-rw-   0        0        0    15289 2024-06-01 00:49:29.000000 chatmemoryc-0.1.4rc3/chatmemoryc/chatmemoryc.py
--rw-rw-rw-   0        0        0     3279 2024-03-19 10:01:43.000000 chatmemoryc-0.1.4rc3/chatmemoryc/client.py
--rw-rw-rw-   0        0        0    12330 2024-06-01 00:48:06.000000 chatmemoryc-0.1.4rc3/chatmemoryc/server.py
-drwxrwxrwx   0        0        0        0 2024-06-01 08:19:16.098522 chatmemoryc-0.1.4rc3/chatmemoryc.egg-info/
--rw-rw-rw-   0        0        0     8021 2024-06-01 08:19:15.000000 chatmemoryc-0.1.4rc3/chatmemoryc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      323 2024-06-01 08:19:16.000000 chatmemoryc-0.1.4rc3/chatmemoryc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 08:19:15.000000 chatmemoryc-0.1.4rc3/chatmemoryc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-06-01 08:19:15.000000 chatmemoryc-0.1.4rc3/chatmemoryc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-06-01 08:19:15.000000 chatmemoryc-0.1.4rc3/chatmemoryc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-06-01 08:19:16.111918 chatmemoryc-0.1.4rc3/setup.cfg
--rw-rw-rw-   0        0        0      753 2024-06-01 08:12:40.000000 chatmemoryc-0.1.4rc3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 08:43:22.733609 chatmemoryc-0.1.4rc4/
+-rw-rw-rw-   0        0        0    11324 2024-04-15 03:15:05.000000 chatmemoryc-0.1.4rc4/LICENSE.txt
+-rw-rw-rw-   0        0        0     8021 2024-06-01 08:43:22.733609 chatmemoryc-0.1.4rc4/PKG-INFO
+-rw-rw-rw-   0        0        0     7392 2024-04-15 03:59:14.000000 chatmemoryc-0.1.4rc4/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 08:43:22.698315 chatmemoryc-0.1.4rc4/chatmemoryc/
+-rw-rw-rw-   0        0        0        0 2024-01-24 23:42:20.000000 chatmemoryc-0.1.4rc4/chatmemoryc/__init__.py
+-rw-rw-rw-   0        0        0     1347 2024-06-01 08:37:01.000000 chatmemoryc-0.1.4rc4/chatmemoryc/__main__.py
+-rw-rw-rw-   0        0        0    15289 2024-06-01 00:49:29.000000 chatmemoryc-0.1.4rc4/chatmemoryc/chatmemoryc.py
+-rw-rw-rw-   0        0        0     3279 2024-03-19 10:01:43.000000 chatmemoryc-0.1.4rc4/chatmemoryc/client.py
+-rw-rw-rw-   0        0        0    12330 2024-06-01 00:48:06.000000 chatmemoryc-0.1.4rc4/chatmemoryc/server.py
+drwxrwxrwx   0        0        0        0 2024-06-01 08:43:22.733609 chatmemoryc-0.1.4rc4/chatmemoryc.egg-info/
+-rw-rw-rw-   0        0        0     8021 2024-06-01 08:43:22.000000 chatmemoryc-0.1.4rc4/chatmemoryc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      323 2024-06-01 08:43:22.000000 chatmemoryc-0.1.4rc4/chatmemoryc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 08:43:22.000000 chatmemoryc-0.1.4rc4/chatmemoryc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-06-01 08:43:22.000000 chatmemoryc-0.1.4rc4/chatmemoryc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-06-01 08:43:22.000000 chatmemoryc-0.1.4rc4/chatmemoryc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 08:43:22.733609 chatmemoryc-0.1.4rc4/setup.cfg
+-rw-rw-rw-   0        0        0      753 2024-06-01 08:40:24.000000 chatmemoryc-0.1.4rc4/setup.py
```

### Comparing `chatmemoryc-0.1.4rc3/LICENSE.txt` & `chatmemoryc-0.1.4rc4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `chatmemoryc-0.1.4rc3/PKG-INFO` & `chatmemoryc-0.1.4rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatmemoryc
-Version: 0.1.4rc3
+Version: 0.1.4rc4
 Summary: Long-term and medium-term memories between you and chatbot
 Home-page: https://github.com/f6844710/chatmemoryc
 Author: pino
 Author-email: f6844710@nifty.com
 Maintainer: pino
 Maintainer-email: f6844710@nifty.com
 License: Apache v2
```

### Comparing `chatmemoryc-0.1.4rc3/README.md` & `chatmemoryc-0.1.4rc4/README.md`

 * *Files identical despite different names*

### Comparing `chatmemoryc-0.1.4rc3/chatmemoryc/__main__.py` & `chatmemoryc-0.1.4rc4/chatmemoryc/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 from argparse import ArgumentParser
 import logging
-from server import ChatMemoryServer
+from .server import ChatMemoryServer
 
 def main():
     logger = logging.getLogger()
     logger.setLevel(logging.INFO)
     log_format = logging.Formatter("%(asctime)s %(levelname)8s %(message)s")
     streamHandler = logging.StreamHandler()
     streamHandler.setFormatter(log_format)
```

### Comparing `chatmemoryc-0.1.4rc3/chatmemoryc/chatmemoryc.py` & `chatmemoryc-0.1.4rc4/chatmemoryc/chatmemoryc.py`

 * *Files identical despite different names*

### Comparing `chatmemoryc-0.1.4rc3/chatmemoryc/client.py` & `chatmemoryc-0.1.4rc4/chatmemoryc/client.py`

 * *Files identical despite different names*

### Comparing `chatmemoryc-0.1.4rc3/chatmemoryc/server.py` & `chatmemoryc-0.1.4rc4/chatmemoryc/server.py`

 * *Files identical despite different names*

### Comparing `chatmemoryc-0.1.4rc3/chatmemoryc.egg-info/PKG-INFO` & `chatmemoryc-0.1.4rc4/chatmemoryc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatmemoryc
-Version: 0.1.4rc3
+Version: 0.1.4rc4
 Summary: Long-term and medium-term memories between you and chatbot
 Home-page: https://github.com/f6844710/chatmemoryc
 Author: pino
 Author-email: f6844710@nifty.com
 Maintainer: pino
 Maintainer-email: f6844710@nifty.com
 License: Apache v2
```

### Comparing `chatmemoryc-0.1.4rc3/setup.py` & `chatmemoryc-0.1.4rc4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name="chatmemoryc",
-    version="0.1.4rc3",
+    version="0.1.4rc4",
     url="https://github.com/f6844710/chatmemoryc",
     author="pino",
     author_email="f6844710@nifty.com",
     maintainer="pino",
     maintainer_email="f6844710@nifty.com",
     description="Long-term and medium-term memories between you and chatbot",
     long_description=open("README.md",'r',encoding='utf-8').read(),
```

