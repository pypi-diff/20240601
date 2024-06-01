# Comparing `tmp/vaul-0.1.24.tar.gz` & `tmp/vaul-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vaul-0.1.24.tar", last modified: Sat Jun  1 17:57:54 2024, max compression
+gzip compressed data, was "vaul-0.1.25.tar", last modified: Sat Jun  1 18:25:25 2024, max compression
```

## Comparing `vaul-0.1.24.tar` & `vaul-0.1.25.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-06-01 17:57:54.318092 vaul-0.1.24/
--rw-r--r--   0 sporter    (501) staff       (20)    34599 2024-05-29 00:30:50.000000 vaul-0.1.24/LICENSE.txt
--rw-r--r--   0 sporter    (501) staff       (20)       33 2024-05-29 00:36:56.000000 vaul-0.1.24/MANIFEST.in
--rw-r--r--   0 sporter    (501) staff       (20)     3860 2024-06-01 17:57:54.318021 vaul-0.1.24/PKG-INFO
--rw-r--r--   0 sporter    (501) staff       (20)     3567 2024-05-29 13:35:57.000000 vaul-0.1.24/README.md
--rw-r--r--   0 sporter    (501) staff       (20)       79 2024-06-01 17:57:54.318299 vaul-0.1.24/setup.cfg
--rw-r--r--   0 sporter    (501) staff       (20)      525 2024-06-01 17:57:51.000000 vaul-0.1.24/setup.py
-drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-06-01 17:57:54.317205 vaul-0.1.24/vaul/
--rw-r--r--   0 sporter    (501) staff       (20)     5260 2024-06-01 17:57:00.000000 vaul-0.1.24/vaul/__init__.py
--rw-r--r--   0 sporter    (501) staff       (20)     1301 2024-05-30 23:29:53.000000 vaul-0.1.24/vaul/ctx.py
--rw-r--r--   0 sporter    (501) staff       (20)      228 2024-05-28 17:31:12.000000 vaul-0.1.24/vaul/enums.py
--rw-r--r--   0 sporter    (501) staff       (20)      485 2024-06-01 16:06:37.000000 vaul-0.1.24/vaul/errors.py
--rw-r--r--   0 sporter    (501) staff       (20)     6014 2024-06-01 17:49:25.000000 vaul-0.1.24/vaul/helpers.py
--rw-r--r--   0 sporter    (501) staff       (20)      899 2024-05-30 23:30:46.000000 vaul-0.1.24/vaul/logging.py
--rw-r--r--   0 sporter    (501) staff       (20)     6053 2024-06-01 16:21:20.000000 vaul-0.1.24/vaul/models.py
--rw-r--r--   0 sporter    (501) staff       (20)     1135 2024-05-30 23:33:15.000000 vaul-0.1.24/vaul/request.py
-drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-06-01 17:57:54.317809 vaul-0.1.24/vaul.egg-info/
--rw-r--r--   0 sporter    (501) staff       (20)     3860 2024-06-01 17:57:54.000000 vaul-0.1.24/vaul.egg-info/PKG-INFO
--rw-r--r--   0 sporter    (501) staff       (20)      312 2024-06-01 17:57:54.000000 vaul-0.1.24/vaul.egg-info/SOURCES.txt
--rw-r--r--   0 sporter    (501) staff       (20)        1 2024-06-01 17:57:54.000000 vaul-0.1.24/vaul.egg-info/dependency_links.txt
--rw-r--r--   0 sporter    (501) staff       (20)       16 2024-06-01 17:57:54.000000 vaul-0.1.24/vaul.egg-info/requires.txt
--rw-r--r--   0 sporter    (501) staff       (20)        5 2024-06-01 17:57:54.000000 vaul-0.1.24/vaul.egg-info/top_level.txt
+drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-06-01 18:25:25.494991 vaul-0.1.25/
+-rw-r--r--   0 sporter    (501) staff       (20)    34599 2024-05-29 00:30:50.000000 vaul-0.1.25/LICENSE.txt
+-rw-r--r--   0 sporter    (501) staff       (20)       33 2024-05-29 00:36:56.000000 vaul-0.1.25/MANIFEST.in
+-rw-r--r--   0 sporter    (501) staff       (20)     3860 2024-06-01 18:25:25.494919 vaul-0.1.25/PKG-INFO
+-rw-r--r--   0 sporter    (501) staff       (20)     3567 2024-05-29 13:35:57.000000 vaul-0.1.25/README.md
+-rw-r--r--   0 sporter    (501) staff       (20)       79 2024-06-01 18:25:25.495216 vaul-0.1.25/setup.cfg
+-rw-r--r--   0 sporter    (501) staff       (20)      525 2024-06-01 18:25:23.000000 vaul-0.1.25/setup.py
+drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-06-01 18:25:25.494097 vaul-0.1.25/vaul/
+-rw-r--r--   0 sporter    (501) staff       (20)     5765 2024-06-01 18:23:17.000000 vaul-0.1.25/vaul/__init__.py
+-rw-r--r--   0 sporter    (501) staff       (20)     1301 2024-05-30 23:29:53.000000 vaul-0.1.25/vaul/ctx.py
+-rw-r--r--   0 sporter    (501) staff       (20)      228 2024-05-28 17:31:12.000000 vaul-0.1.25/vaul/enums.py
+-rw-r--r--   0 sporter    (501) staff       (20)      485 2024-06-01 16:06:37.000000 vaul-0.1.25/vaul/errors.py
+-rw-r--r--   0 sporter    (501) staff       (20)     6014 2024-06-01 17:49:25.000000 vaul-0.1.25/vaul/helpers.py
+-rw-r--r--   0 sporter    (501) staff       (20)      979 2024-06-01 18:20:17.000000 vaul-0.1.25/vaul/logging.py
+-rw-r--r--   0 sporter    (501) staff       (20)     6053 2024-06-01 16:21:20.000000 vaul-0.1.25/vaul/models.py
+-rw-r--r--   0 sporter    (501) staff       (20)     1135 2024-05-30 23:33:15.000000 vaul-0.1.25/vaul/request.py
+drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-06-01 18:25:25.494693 vaul-0.1.25/vaul.egg-info/
+-rw-r--r--   0 sporter    (501) staff       (20)     3860 2024-06-01 18:25:25.000000 vaul-0.1.25/vaul.egg-info/PKG-INFO
+-rw-r--r--   0 sporter    (501) staff       (20)      312 2024-06-01 18:25:25.000000 vaul-0.1.25/vaul.egg-info/SOURCES.txt
+-rw-r--r--   0 sporter    (501) staff       (20)        1 2024-06-01 18:25:25.000000 vaul-0.1.25/vaul.egg-info/dependency_links.txt
+-rw-r--r--   0 sporter    (501) staff       (20)       16 2024-06-01 18:25:25.000000 vaul-0.1.25/vaul.egg-info/requires.txt
+-rw-r--r--   0 sporter    (501) staff       (20)        5 2024-06-01 18:25:25.000000 vaul-0.1.25/vaul.egg-info/top_level.txt
```

### Comparing `vaul-0.1.24/LICENSE.txt` & `vaul-0.1.25/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vaul-0.1.24/PKG-INFO` & `vaul-0.1.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaul
-Version: 0.1.24
+Version: 0.1.25
 Summary: A nano-framework for deploying Python functions as APIs on AWS Lambda using Function URLs.
 Author: Spencer Porter
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pydantic==2.6.4
```

### Comparing `vaul-0.1.24/README.md` & `vaul-0.1.25/README.md`

 * *Files identical despite different names*

### Comparing `vaul-0.1.24/setup.py` & `vaul-0.1.25/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="vaul",
-    version="0.1.24",
+    version="0.1.25",
     description="A nano-framework for deploying Python functions as APIs on AWS Lambda using Function URLs.",
     author="Spencer Porter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         'pydantic==2.6.4',
     ],
```

### Comparing `vaul-0.1.24/vaul/__init__.py` & `vaul-0.1.25/vaul/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,44 @@
 from __future__ import annotations
 import json
 from pydantic import ValidationError
 from typing import Callable
 
 from .ctx import RequestContextMiddleware, get_request
 from .enums import RequestMethod
+from .logging import create_logger
 from .models import Action
 from .helpers import remove_keys_recursively
 from .errors import VaulError, InvalidRequestError, InternalServerError
 
 class Vaul:
     instance = None
 
     @staticmethod
     def get_instance():
         if Vaul.instance is None:
             Vaul.instance = Vaul()
         return Vaul.instance
 
-    def __init__(self, name='Vaul', debug=False, preserve_output_types=False):
+    def __init__(self, name='Vaul', log_level='INFO', debug=False, preserve_output_types=False):
         self.middleware = RequestContextMiddleware(self._handler)
         self.name = name
         self.routes = {}
+        self.log_level = self.validate_log_level(log_level)
         self.debug = debug
+        self.logger = create_logger(self)
         self.preserve_output_types = preserve_output_types
 
+    @staticmethod
+    def validate_log_level(log_level: str) -> int:
+        level = getattr(logging, log_level.upper(), None)
+        if not isinstance(level, int):
+            raise ValueError(f"Invalid log level: {log_level} - Must be one of: DEBUG, INFO, WARNING, ERROR, CRITICAL")
+        return level
+
     def action(self, path: str = '/', method: RequestMethod | str = RequestMethod.POST):
         if isinstance(method, str):
             method = method.upper()
             if method not in RequestMethod.to_list():
                 raise ValueError(f"Invalid method: {method}")
             method = getattr(RequestMethod, method)
 
@@ -70,16 +80,15 @@
             body = self.routes[path][method].run(request.json())
             return self._response(200, body, method)
         except ValidationError as e:
             return self._response(400, InvalidRequestError(str(e)).to_dict(), method)
         except VaulError as e:
             return self._response(e.status_code, e.to_dict(), method)
         except Exception as e:
-            if self.debug:
-                print(e)
+            self.logger.error(f"Exception occurred: {e}", exc_info=True)  # Log the exception
             return self._response(500, InternalServerError(str(e)).to_dict(), method)
 
     def _response(self, status_code, body, method, content_type='application/json', is_base64_encoded=False):
         headers = {
             'Content-Type': content_type,
         }
```

### Comparing `vaul-0.1.24/vaul/ctx.py` & `vaul-0.1.25/vaul/ctx.py`

 * *Files identical despite different names*

### Comparing `vaul-0.1.24/vaul/helpers.py` & `vaul-0.1.25/vaul/helpers.py`

 * *Files identical despite different names*

### Comparing `vaul-0.1.24/vaul/logging.py` & `vaul-0.1.25/vaul/logging.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,12 +24,15 @@
 
 
 def create_logger(app) -> logging.Logger:
     logger = logging.getLogger(app.name)
 
     if app.debug and not logger.level:
         logger.setLevel(logging.DEBUG)
+    else:
+        logger.setLevel(app.log_level)
 
     if not has_level_handler(logger):
         logger.addHandler(default_handler)
+        logger.propagate = True
 
-    return logger
+    return logger
```

### Comparing `vaul-0.1.24/vaul/models.py` & `vaul-0.1.25/vaul/models.py`

 * *Files identical despite different names*

### Comparing `vaul-0.1.24/vaul/request.py` & `vaul-0.1.25/vaul/request.py`

 * *Files identical despite different names*

### Comparing `vaul-0.1.24/vaul.egg-info/PKG-INFO` & `vaul-0.1.25/vaul.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaul
-Version: 0.1.24
+Version: 0.1.25
 Summary: A nano-framework for deploying Python functions as APIs on AWS Lambda using Function URLs.
 Author: Spencer Porter
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pydantic==2.6.4
```

