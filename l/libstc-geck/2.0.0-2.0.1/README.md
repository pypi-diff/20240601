# Comparing `tmp/libstc_geck-2.0.0.tar.gz` & `tmp/libstc_geck-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libstc_geck-2.0.0.tar", max compression
+gzip compressed data, was "libstc_geck-2.0.1.tar", max compression
```

## Comparing `libstc_geck-2.0.0.tar` & `libstc_geck-2.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     8725 2024-04-15 08:05:18.503358 libstc_geck-2.0.0/README.md
--rw-r--r--   0        0        0        0 2023-12-04 12:28:44.413595 libstc_geck-2.0.0/libstc_geck/__init__.py
--rw-r--r--   0        0        0     9926 2024-05-04 07:26:54.761582 libstc_geck-2.0.0/libstc_geck/advices.py
--rw-r--r--   0        0        0     8977 2024-04-15 08:05:18.804976 libstc_geck-2.0.0/libstc_geck/cli.py
--rw-r--r--   0        0        0    10155 2024-04-15 08:05:18.615270 libstc_geck-2.0.0/libstc_geck/client.py
--rw-r--r--   0        0        0      277 2023-12-04 12:28:44.010382 libstc_geck-2.0.0/libstc_geck/exceptions.py
--rw-r--r--   0        0        0     2043 2023-12-04 12:28:41.860572 libstc_geck-2.0.0/libstc_geck/utils.py
--rw-r--r--   0        0        0      678 2024-05-04 07:34:46.447862 libstc_geck-2.0.0/pyproject.toml
--rw-r--r--   0        0        0    10012 1970-01-01 00:00:00.000000 libstc_geck-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     8731 2024-05-20 04:38:03.705951 libstc_geck-2.0.1/README.md
+-rw-r--r--   0        0        0        0 2023-12-04 12:28:44.413595 libstc_geck-2.0.1/libstc_geck/__init__.py
+-rw-r--r--   0        0        0     6374 2024-05-04 07:48:13.372703 libstc_geck-2.0.1/libstc_geck/advices.py
+-rw-r--r--   0        0        0     8980 2024-05-04 08:03:25.858365 libstc_geck-2.0.1/libstc_geck/cli.py
+-rw-r--r--   0        0        0    10155 2024-04-15 08:05:18.615270 libstc_geck-2.0.1/libstc_geck/client.py
+-rw-r--r--   0        0        0      277 2023-12-04 12:28:44.010382 libstc_geck-2.0.1/libstc_geck/exceptions.py
+-rw-r--r--   0        0        0     2043 2023-12-04 12:28:41.860572 libstc_geck-2.0.1/libstc_geck/utils.py
+-rw-r--r--   0        0        0      681 2024-06-01 19:54:42.029022 libstc_geck-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0    10018 1970-01-01 00:00:00.000000 libstc_geck-2.0.1/PKG-INFO
```

### Comparing `libstc_geck-2.0.0/README.md` & `libstc_geck-2.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 GECK is a Python library and Bash tool to deploy and access STC - the large corpus of scholarly texts.
 GECK includes embedded search engine [Summa](https://github.com/izihawa/summa), helps to feed it with a prepared IPFS-based database of scholarly texts, do search queries over the database and iterate over all documents if you need.
 
 ## Install
 
 Firstly, You should have [installed IPFS](https://libstc.cc/#/help/install-ipfs)
 
-Pre-built wheels of `stc-geck` are available for Python 3.8, 3.9, 3.10 and 3.11
+Pre-built wheels of `libstc-geck` are available for Python 3.8, 3.9, 3.10 and 3.11
 
 ```bash
-pip install stc-geck
+pip install libstc-geck
 ```
 
 ## Usage
 
 **Attention!** STC does not contain every book or publication in the world. We are constantly increasing coverage but there is still a lot to do.
 STC contains metadata for the most of the items, but `links` or `content` fields may be absent.
```

### Comparing `libstc_geck-2.0.0/libstc_geck/cli.py` & `libstc_geck-2.0.1/libstc_geck/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging
 import os.path
 import sys
 from typing import List, Optional
 
 import fire
 import humanfriendly
-from stc_geck.advices import BaseDocumentHolder
+from libstc_geck.advices import BaseDocumentHolder
 from termcolor import colored
 
 from .client import StcGeck
 from .exceptions import IpfsConnectionError
 
 
 def exception_handler(func):
```

### Comparing `libstc_geck-2.0.0/libstc_geck/client.py` & `libstc_geck-2.0.1/libstc_geck/client.py`

 * *Files identical despite different names*

### Comparing `libstc_geck-2.0.0/libstc_geck/utils.py` & `libstc_geck-2.0.1/libstc_geck/utils.py`

 * *Files identical despite different names*

### Comparing `libstc_geck-2.0.0/pyproject.toml` & `libstc_geck-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "libstc-geck"
-version = "2.0.0"
+version = "2.0.1"
 authors = ["Multilingual Loiter"]
 description = "GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3.8",
 ]
 
@@ -23,8 +23,8 @@
 fire = "~0.5.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-geck = "stc_geck.cli:main"
+geck = "libstc_geck.cli:main"
```

### Comparing `libstc_geck-2.0.0/PKG-INFO` & `libstc_geck-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libstc-geck
-Version: 2.0.0
+Version: 2.0.1
 Summary: GECK (Garden Of Eden Creation Kit) is a toolkit for setting up and maintaning STC
 Author: Multilingual Loiter
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
@@ -33,18 +33,18 @@
 GECK is a Python library and Bash tool to deploy and access STC - the large corpus of scholarly texts.
 GECK includes embedded search engine [Summa](https://github.com/izihawa/summa), helps to feed it with a prepared IPFS-based database of scholarly texts, do search queries over the database and iterate over all documents if you need.
 
 ## Install
 
 Firstly, You should have [installed IPFS](https://libstc.cc/#/help/install-ipfs)
 
-Pre-built wheels of `stc-geck` are available for Python 3.8, 3.9, 3.10 and 3.11
+Pre-built wheels of `libstc-geck` are available for Python 3.8, 3.9, 3.10 and 3.11
 
 ```bash
-pip install stc-geck
+pip install libstc-geck
 ```
 
 ## Usage
 
 **Attention!** STC does not contain every book or publication in the world. We are constantly increasing coverage but there is still a lot to do.
 STC contains metadata for the most of the items, but `links` or `content` fields may be absent.
```

