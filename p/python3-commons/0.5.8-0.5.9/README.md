# Comparing `tmp/python3_commons-0.5.8.tar.gz` & `tmp/python3_commons-0.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python3_commons-0.5.8.tar", last modified: Sat Jun  1 08:05:18 2024, max compression
+gzip compressed data, was "python3_commons-0.5.9.tar", last modified: Sat Jun  1 09:53:56 2024, max compression
```

## Comparing `python3_commons-0.5.8.tar` & `python3_commons-0.5.9.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.261991 python3_commons-0.5.8/
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 08:05:06.000000 python3_commons-0.5.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.253991 python3_commons-0.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.257991 python3_commons-0.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-06-01 08:05:06.000000 python3_commons-0.5.8/.github/workflows/python-publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 08:05:06.000000 python3_commons-0.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-01 08:05:06.000000 python3_commons-0.5.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-01 08:05:06.000000 python3_commons-0.5.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-06-01 08:05:06.000000 python3_commons-0.5.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-06-01 08:05:18.261991 python3_commons-0.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-01 08:05:06.000000 python3_commons-0.5.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 08:05:06.000000 python3_commons-0.5.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.257991 python3_commons-0.5.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-06-01 08:05:06.000000 python3_commons-0.5.8/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.257991 python3_commons-0.5.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 08:05:06.000000 python3_commons-0.5.8/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 08:05:06.000000 python3_commons-0.5.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-01 08:05:06.000000 python3_commons-0.5.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-06-01 08:05:06.000000 python3_commons-0.5.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-06-01 08:05:06.000000 python3_commons-0.5.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-01 08:05:06.000000 python3_commons-0.5.8/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-01 08:05:06.000000 python3_commons-0.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-06-01 08:05:06.000000 python3_commons-0.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 08:05:06.000000 python3_commons-0.5.8/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-01 08:05:06.000000 python3_commons-0.5.8/requirements_test.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-06-01 08:05:18.261991 python3_commons-0.5.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-06-01 08:05:06.000000 python3_commons-0.5.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.253991 python3_commons-0.5.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.257991 python3_commons-0.5.8/src/python3_commons/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3805 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/db.py
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/fs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.261991 python3_commons-0.5.8/src/python3_commons/logging/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/logging/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/logging/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/object_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.261991 python3_commons-0.5.8/src/python3_commons/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/serializers/msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-06-01 08:05:06.000000 python3_commons-0.5.8/src/python3_commons/serializers/msgspec.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.261991 python3_commons-0.5.8/src/python3_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-06-01 08:05:18.000000 python3_commons-0.5.8/src/python3_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-06-01 08:05:18.000000 python3_commons-0.5.8/src/python3_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 08:05:18.000000 python3_commons-0.5.8/src/python3_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 08:05:18.000000 python3_commons-0.5.8/src/python3_commons.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-06-01 08:05:18.000000 python3_commons-0.5.8/src/python3_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 08:05:18.000000 python3_commons-0.5.8/src/python3_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 08:05:18.261991 python3_commons-0.5.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-06-01 08:05:06.000000 python3_commons-0.5.8/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-06-01 08:05:06.000000 python3_commons-0.5.8/tests/test_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-06-01 08:05:06.000000 python3_commons-0.5.8/tests/test_msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:53:56.201016 python3_commons-0.5.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 09:53:50.000000 python3_commons-0.5.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:53:56.193016 python3_commons-0.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:53:56.197016 python3_commons-0.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-06-01 09:53:50.000000 python3_commons-0.5.9/.github/workflows/python-publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-06-01 09:53:50.000000 python3_commons-0.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-01 09:53:50.000000 python3_commons-0.5.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-06-01 09:53:50.000000 python3_commons-0.5.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    34575 2024-06-01 09:53:50.000000 python3_commons-0.5.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-06-01 09:53:56.201016 python3_commons-0.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-06-01 09:53:50.000000 python3_commons-0.5.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-06-01 09:53:50.000000 python3_commons-0.5.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:53:56.197016 python3_commons-0.5.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-06-01 09:53:50.000000 python3_commons-0.5.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:53:56.197016 python3_commons-0.5.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-06-01 09:53:50.000000 python3_commons-0.5.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-06-01 09:53:50.000000 python3_commons-0.5.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-01 09:53:50.000000 python3_commons-0.5.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9373 2024-06-01 09:53:50.000000 python3_commons-0.5.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2253 2024-06-01 09:53:50.000000 python3_commons-0.5.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-06-01 09:53:50.000000 python3_commons-0.5.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-06-01 09:53:50.000000 python3_commons-0.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-06-01 09:53:50.000000 python3_commons-0.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-06-01 09:53:50.000000 python3_commons-0.5.9/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-06-01 09:53:50.000000 python3_commons-0.5.9/requirements_test.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-06-01 09:53:56.205016 python3_commons-0.5.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-06-01 09:53:50.000000 python3_commons-0.5.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:53:56.193016 python3_commons-0.5.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:53:56.201016 python3_commons-0.5.9/src/python3_commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-06-01 09:53:50.000000 python3_commons-0.5.9/src/python3_commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5177 2024-06-01 09:53:50.000000 python3_commons-0.5.9/src/python3_commons/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-06-01 09:53:50.000000 python3_commons-0.5.9/src/python3_commons/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-06-01 09:53:50.000000 python3_commons-0.5.9/src/python3_commons/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-06-01 09:53:50.000000 python3_commons-0.5.9/src/python3_commons/fs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-06-01 09:53:50.000000 python3_commons-0.5.9/src/python3_commons/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:53:56.201016 python3_commons-0.5.9/src/python3_commons/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 09:53:50.000000 python3_commons-0.5.9/src/python3_commons/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      175 2024-06-01 09:53:50.000000 python3_commons-0.5.9/src/python3_commons/logging/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-06-01 09:53:50.000000 python3_commons-0.5.9/src/python3_commons/logging/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-06-01 09:53:50.000000 python3_commons-0.5.9/src/python3_commons/object_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:53:56.201016 python3_commons-0.5.9/src/python3_commons/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 09:53:50.000000 python3_commons-0.5.9/src/python3_commons/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-06-01 09:53:50.000000 python3_commons-0.5.9/src/python3_commons/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-06-01 09:53:50.000000 python3_commons-0.5.9/src/python3_commons/serializers/msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-06-01 09:53:50.000000 python3_commons-0.5.9/src/python3_commons/serializers/msgspec.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:53:56.201016 python3_commons-0.5.9/src/python3_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-06-01 09:53:56.000000 python3_commons-0.5.9/src/python3_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1146 2024-06-01 09:53:56.000000 python3_commons-0.5.9/src/python3_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 09:53:56.000000 python3_commons-0.5.9/src/python3_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 09:53:56.000000 python3_commons-0.5.9/src/python3_commons.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-06-01 09:53:56.000000 python3_commons-0.5.9/src/python3_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 09:53:56.000000 python3_commons-0.5.9/src/python3_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 09:53:56.201016 python3_commons-0.5.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-06-01 09:53:50.000000 python3_commons-0.5.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-06-01 09:53:50.000000 python3_commons-0.5.9/tests/test_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-06-01 09:53:50.000000 python3_commons-0.5.9/tests/test_msgspec.py
```

### Comparing `python3_commons-0.5.8/.coveragerc` & `python3_commons-0.5.9/.coveragerc`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/.github/workflows/python-publish.yaml` & `python3_commons-0.5.9/.github/workflows/python-publish.yaml`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/.gitignore` & `python3_commons-0.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/LICENSE` & `python3_commons-0.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/PKG-INFO` & `python3_commons-0.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.5.8
+Version: 0.5.9
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3_commons-0.5.8/docs/Makefile` & `python3_commons-0.5.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/docs/conf.py` & `python3_commons-0.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/docs/index.rst` & `python3_commons-0.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/setup.cfg` & `python3_commons-0.5.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = python3-commons
-version = 0.5.8
+version = 0.5.9
 description = Re-usable Python3 code
 author = Oleg Korsak
 author_email = kamikaze.is.waiting.you@gmail.com
 license = gpl-3
 long_description = file: README.rst
 long_description_content_type = text/x-rst; charset=UTF-8
 url = https://github.com/kamikaze/python3-commons
```

### Comparing `python3_commons-0.5.8/src/python3_commons/audit.py` & `python3_commons-0.5.9/src/python3_commons/audit.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,91 @@
 import asyncio
 import io
 import logging
 import tarfile
 from datetime import datetime, timedelta, UTC
 from io import BytesIO
+from typing import Generator
 from uuid import uuid4
 
 from lxml import etree
 from minio import S3Error
 from zeep.plugins import Plugin
 from zeep.wsdl.definitions import AbstractOperation
 
 from python3_commons import object_storage
 from python3_commons.conf import S3Settings, s3_settings
 from python3_commons.object_storage import get_s3_client
 
 logger = logging.getLogger(__name__)
 
 
+class BytesIOStream(io.BytesIO):
+    def __init__(self, generator: Generator[bytes, None, None], *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.generator = generator
+
+    def read(self, size: int = -1):
+        if size == -1:
+            size = 4096
+
+        while self.tell() < size:
+            try:
+                chunk = next(self.generator)
+            except StopIteration:
+                break
+
+            self.write(chunk)
+
+        if chunk := self.read(size):
+            pos = self.tell()
+
+            buf = self.getbuffer()
+            unread_data_size = len(buf) - pos
+
+            if unread_data_size > 0:
+                buf[:unread_data_size] = buf[pos:pos+unread_data_size]
+
+            self.truncate(unread_data_size)
+            self.seek(0)
+
+        return chunk
+
+    def readable(self):
+        return True
+
+
+def generate_archive(bucket_name: str, date_path: str, chunk_size: int = 4096) -> Generator[bytes, None, None]:
+    buffer = io.BytesIO()
+
+    with tarfile.open(fileobj=buffer, mode='w|bz2') as archive:
+        objects = object_storage.get_objects(bucket_name, date_path, recursive=True)
+
+        if objects:
+            logger.info(f'Compacting files in: {date_path}')
+
+            for name, last_modified, content in objects:
+                info = tarfile.TarInfo(name)
+                info.size = len(content)
+                info.mtime = last_modified.timestamp()
+                archive.addfile(info, io.BytesIO(content))
+                buffer.seek(0)
+
+                while True:
+                    chunk = buffer.read(chunk_size)
+
+                    if not chunk:
+                        break
+
+                    yield chunk
+
+                buffer.seek(0)
+                buffer.truncate(0)
+
+
 def write_audit_data_sync(settings: S3Settings, key: str, data: bytes):
     if settings.s3_secret_access_key:
         try:
             client = get_s3_client(settings)
             absolute_path = object_storage.get_absolute_path(f'audit/{key}')
 
             client.put_object(settings.s3_bucket, absolute_path, io.BytesIO(data), len(data))
@@ -43,31 +107,20 @@
     month = now.month
     day = now.day
     bucket_name = s3_settings.s3_bucket
     fo = BytesIO()
     object_names = []
     date_path = object_storage.get_absolute_path(f'{root_path}/{year}/{month:02}/{day:02}')
 
-    with tarfile.open(fileobj=fo, mode='w|bz2') as archive:
-        if objects := object_storage.get_objects(bucket_name, date_path, recursive=True):
-            logger.info(f'Compacting files in: {date_path}')
-
-            for name, last_modified, content in objects:
-                info = tarfile.TarInfo(name)
-                info.size = len(content)
-                info.mtime = last_modified.timestamp()
-                archive.addfile(info, BytesIO(content))
-                object_names.append(name)
-
-    fo.seek(0)
+    generator = generate_archive(bucket_name, date_path, chunk_size=4096)
+    archive_stream = BytesIOStream(generator)
 
     if object_names:
-        archive_path = object_storage.get_absolute_path(
-            f'audit/.archive/{year}_{month:02}_{day:02}.tar.bz2')
-        object_storage.put_object(bucket_name, archive_path, fo, fo.getbuffer().nbytes)
+        archive_path = object_storage.get_absolute_path(f'audit/.archive/{year}_{month:02}_{day:02}.tar.bz2')
+        object_storage.put_object(bucket_name, archive_path, archive_stream, -1, part_size=4096)
 
         if errors := object_storage.remove_objects(bucket_name, object_names=object_names):
             for error in errors:
                 logger.error(f'Failed to delete object in {bucket_name=}: {error}')
     else:
         logger.info('No objects to archive found.')
 
@@ -78,18 +131,16 @@
         self.audit_name = audit_name
 
     def store_audit_in_s3(self, envelope, operation: AbstractOperation, direction: str):
         xml = etree.tostring(envelope, encoding='UTF-8', pretty_print=True)
         now = datetime.now(tz=UTC)
         date_path = now.strftime('%Y/%m/%d')
         timestamp = now.strftime('%H%M%S')
-        coro = write_audit_data(
-            s3_settings,
-            f'{date_path}/{self.audit_name}/{operation.name}/{timestamp}_{str(uuid4())[-12:]}_{direction}.xml', xml
-        )
+        path = f'{date_path}/{self.audit_name}/{operation.name}/{timestamp}_{str(uuid4())[-12:]}_{direction}.xml'
+        coro = write_audit_data(s3_settings, path, xml)
 
         try:
             loop = asyncio.get_running_loop()
         except RuntimeError:
             loop = None
 
         if loop and loop.is_running():
```

### Comparing `python3_commons-0.5.8/src/python3_commons/conf.py` & `python3_commons-0.5.9/src/python3_commons/conf.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/src/python3_commons/db.py` & `python3_commons-0.5.9/src/python3_commons/db.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/src/python3_commons/helpers.py` & `python3_commons-0.5.9/src/python3_commons/helpers.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/src/python3_commons/logging/formatter.py` & `python3_commons-0.5.9/src/python3_commons/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/src/python3_commons/object_storage.py` & `python3_commons-0.5.9/src/python3_commons/object_storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 
     if bucket_root := s3_settings.s3_bucket_root:
         path = f'{bucket_root[:1] if bucket_root.startswith('/') else bucket_root}/{path}'
 
     return path
 
 
-def put_object(bucket_name: str, path: str, data: io.BytesIO, length: int) -> str:
+def put_object(bucket_name: str, path: str, data: io.BytesIO, length: int, part_size: int = 0) -> str:
     s3_client = get_s3_client(s3_settings)
 
     if s3_client:
-        result = s3_client.put_object(bucket_name, path, data, length)
+        result = s3_client.put_object(bucket_name, path, data, length, part_size=part_size)
 
         logger.debug(f'Stored object into object storage: {bucket_name}:{path}')
 
         return result.location
     else:
         logger.warning(f'No S3 client available, skipping object put')
```

### Comparing `python3_commons-0.5.8/src/python3_commons/serializers/json.py` & `python3_commons-0.5.9/src/python3_commons/serializers/json.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/src/python3_commons/serializers/msgpack.py` & `python3_commons-0.5.9/src/python3_commons/serializers/msgpack.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/src/python3_commons/serializers/msgspec.py` & `python3_commons-0.5.9/src/python3_commons/serializers/msgspec.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/src/python3_commons.egg-info/PKG-INFO` & `python3_commons-0.5.9/src/python3_commons.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python3-commons
-Version: 0.5.8
+Version: 0.5.9
 Summary: Re-usable Python3 code
 Home-page: https://github.com/kamikaze/python3-commons
 Author: Oleg Korsak
 Author-email: kamikaze.is.waiting.you@gmail.com
 License: gpl-3
 Project-URL: Documentation, https://github.com/kamikaze/python3-commons/wiki
 Platform: any
```

### Comparing `python3_commons-0.5.8/src/python3_commons.egg-info/SOURCES.txt` & `python3_commons-0.5.9/src/python3_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/tests/conftest.py` & `python3_commons-0.5.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/tests/test_msgpack.py` & `python3_commons-0.5.9/tests/test_msgpack.py`

 * *Files identical despite different names*

### Comparing `python3_commons-0.5.8/tests/test_msgspec.py` & `python3_commons-0.5.9/tests/test_msgspec.py`

 * *Files identical despite different names*

