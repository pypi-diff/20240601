# Comparing `tmp/vaul-0.1.22.tar.gz` & `tmp/vaul-0.1.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vaul-0.1.22.tar", last modified: Fri May 31 14:32:51 2024, max compression
+gzip compressed data, was "vaul-0.1.23.tar", last modified: Sat Jun  1 16:29:25 2024, max compression
```

## Comparing `vaul-0.1.22.tar` & `vaul-0.1.23.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-05-31 14:32:51.621451 vaul-0.1.22/
--rw-r--r--   0 sporter    (501) staff       (20)    34599 2024-05-29 00:30:50.000000 vaul-0.1.22/LICENSE.txt
--rw-r--r--   0 sporter    (501) staff       (20)       33 2024-05-29 00:36:56.000000 vaul-0.1.22/MANIFEST.in
--rw-r--r--   0 sporter    (501) staff       (20)     3860 2024-05-31 14:32:51.621391 vaul-0.1.22/PKG-INFO
--rw-r--r--   0 sporter    (501) staff       (20)     3567 2024-05-29 13:35:57.000000 vaul-0.1.22/README.md
--rw-r--r--   0 sporter    (501) staff       (20)       79 2024-05-31 14:32:51.621769 vaul-0.1.22/setup.cfg
--rw-r--r--   0 sporter    (501) staff       (20)      525 2024-05-31 14:32:47.000000 vaul-0.1.22/setup.py
-drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-05-31 14:32:51.619895 vaul-0.1.22/vaul/
--rw-r--r--   0 sporter    (501) staff       (20)     5073 2024-05-31 14:32:34.000000 vaul-0.1.22/vaul/__init__.py
--rw-r--r--   0 sporter    (501) staff       (20)     1301 2024-05-30 23:29:53.000000 vaul-0.1.22/vaul/ctx.py
--rw-r--r--   0 sporter    (501) staff       (20)      228 2024-05-28 17:31:12.000000 vaul-0.1.22/vaul/enums.py
--rw-r--r--   0 sporter    (501) staff       (20)     1052 2024-05-30 23:30:22.000000 vaul-0.1.22/vaul/helpers.py
--rw-r--r--   0 sporter    (501) staff       (20)      899 2024-05-30 23:30:46.000000 vaul-0.1.22/vaul/logging.py
--rw-r--r--   0 sporter    (501) staff       (20)     5875 2024-05-31 00:09:42.000000 vaul-0.1.22/vaul/models.py
--rw-r--r--   0 sporter    (501) staff       (20)     1135 2024-05-30 23:33:15.000000 vaul-0.1.22/vaul/request.py
-drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-05-31 14:32:51.620958 vaul-0.1.22/vaul.egg-info/
--rw-r--r--   0 sporter    (501) staff       (20)     3860 2024-05-31 14:32:51.000000 vaul-0.1.22/vaul.egg-info/PKG-INFO
--rw-r--r--   0 sporter    (501) staff       (20)      297 2024-05-31 14:32:51.000000 vaul-0.1.22/vaul.egg-info/SOURCES.txt
--rw-r--r--   0 sporter    (501) staff       (20)        1 2024-05-31 14:32:51.000000 vaul-0.1.22/vaul.egg-info/dependency_links.txt
--rw-r--r--   0 sporter    (501) staff       (20)       16 2024-05-31 14:32:51.000000 vaul-0.1.22/vaul.egg-info/requires.txt
--rw-r--r--   0 sporter    (501) staff       (20)        5 2024-05-31 14:32:51.000000 vaul-0.1.22/vaul.egg-info/top_level.txt
+drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-06-01 16:29:25.268396 vaul-0.1.23/
+-rw-r--r--   0 sporter    (501) staff       (20)    34599 2024-05-29 00:30:50.000000 vaul-0.1.23/LICENSE.txt
+-rw-r--r--   0 sporter    (501) staff       (20)       33 2024-05-29 00:36:56.000000 vaul-0.1.23/MANIFEST.in
+-rw-r--r--   0 sporter    (501) staff       (20)     3860 2024-06-01 16:29:25.268334 vaul-0.1.23/PKG-INFO
+-rw-r--r--   0 sporter    (501) staff       (20)     3567 2024-05-29 13:35:57.000000 vaul-0.1.23/README.md
+-rw-r--r--   0 sporter    (501) staff       (20)       79 2024-06-01 16:29:25.268607 vaul-0.1.23/setup.cfg
+-rw-r--r--   0 sporter    (501) staff       (20)      525 2024-06-01 16:11:08.000000 vaul-0.1.23/setup.py
+drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-06-01 16:29:25.267349 vaul-0.1.23/vaul/
+-rw-r--r--   0 sporter    (501) staff       (20)     5223 2024-06-01 16:11:08.000000 vaul-0.1.23/vaul/__init__.py
+-rw-r--r--   0 sporter    (501) staff       (20)     1301 2024-05-30 23:29:53.000000 vaul-0.1.23/vaul/ctx.py
+-rw-r--r--   0 sporter    (501) staff       (20)      228 2024-05-28 17:31:12.000000 vaul-0.1.23/vaul/enums.py
+-rw-r--r--   0 sporter    (501) staff       (20)      485 2024-06-01 16:06:37.000000 vaul-0.1.23/vaul/errors.py
+-rw-r--r--   0 sporter    (501) staff       (20)     1052 2024-05-30 23:30:22.000000 vaul-0.1.23/vaul/helpers.py
+-rw-r--r--   0 sporter    (501) staff       (20)      899 2024-05-30 23:30:46.000000 vaul-0.1.23/vaul/logging.py
+-rw-r--r--   0 sporter    (501) staff       (20)     6053 2024-06-01 16:21:20.000000 vaul-0.1.23/vaul/models.py
+-rw-r--r--   0 sporter    (501) staff       (20)     1135 2024-05-30 23:33:15.000000 vaul-0.1.23/vaul/request.py
+drwxr-xr-x   0 sporter    (501) staff       (20)        0 2024-06-01 16:29:25.268117 vaul-0.1.23/vaul.egg-info/
+-rw-r--r--   0 sporter    (501) staff       (20)     3860 2024-06-01 16:29:25.000000 vaul-0.1.23/vaul.egg-info/PKG-INFO
+-rw-r--r--   0 sporter    (501) staff       (20)      312 2024-06-01 16:29:25.000000 vaul-0.1.23/vaul.egg-info/SOURCES.txt
+-rw-r--r--   0 sporter    (501) staff       (20)        1 2024-06-01 16:29:25.000000 vaul-0.1.23/vaul.egg-info/dependency_links.txt
+-rw-r--r--   0 sporter    (501) staff       (20)       16 2024-06-01 16:29:25.000000 vaul-0.1.23/vaul.egg-info/requires.txt
+-rw-r--r--   0 sporter    (501) staff       (20)        5 2024-06-01 16:29:25.000000 vaul-0.1.23/vaul.egg-info/top_level.txt
```

### Comparing `vaul-0.1.22/LICENSE.txt` & `vaul-0.1.23/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vaul-0.1.22/PKG-INFO` & `vaul-0.1.23/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaul
-Version: 0.1.22
+Version: 0.1.23
 Summary: A nano-framework for deploying Python functions as APIs on AWS Lambda using Function URLs.
 Author: Spencer Porter
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pydantic==2.6.4
```

### Comparing `vaul-0.1.22/README.md` & `vaul-0.1.23/README.md`

 * *Files identical despite different names*

### Comparing `vaul-0.1.22/setup.py` & `vaul-0.1.23/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="vaul",
-    version="0.1.22",
+    version="0.1.23",
     description="A nano-framework for deploying Python functions as APIs on AWS Lambda using Function URLs.",
     author="Spencer Porter",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[
         'pydantic==2.6.4',
     ],
```

### Comparing `vaul-0.1.22/vaul/__init__.py` & `vaul-0.1.23/vaul/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,58 +1,59 @@
-# vaul/__init__.py
 from __future__ import annotations
 import json
 from pydantic import ValidationError
 from typing import Callable
 
 from .ctx import RequestContextMiddleware, get_request
 from .enums import RequestMethod
 from .models import Action
 from .helpers import remove_keys_recursively
+from .errors import VaulError, InvalidRequestError, InternalServerError
 
 class Vaul:
     instance = None
 
     @staticmethod
     def get_instance():
         if Vaul.instance is None:
             Vaul.instance = Vaul()
         return Vaul.instance
 
-    def __init__(self, debug=False):
+    def __init__(self, debug=False, preserve_output_types=False):
         self.middleware = RequestContextMiddleware(self._handler)
         self.routes = {}
         self.debug = debug
+        self.preserve_output_types = preserve_output_types
 
     def action(self, path: str = '/', method: RequestMethod | str = RequestMethod.POST):
         if isinstance(method, str):
             method = method.upper()
             if method not in RequestMethod.to_list():
                 raise ValueError(f"Invalid method: {method}")
             method = getattr(RequestMethod, method)
 
         def decorator(func: Callable):
-            action = Action(func, path, method)
+            action = Action(func, path, method, self.preserve_output_types)
             self._register_action(action)
             return action
         return decorator
 
     def _register_action(self, action):
         self.routes.setdefault(action.path, {})[action.method] = action
 
     def _handler(self, event):
         request = get_request()
         if request is None:
-            return self._response(500, 'Internal server error', RequestMethod.GET)
+            return self._response(500, {'error': 'Internal server error', 'details': 'Request context is missing'}, RequestMethod.GET)
 
         path, method = request.path, request.method
         route_handler = self._get_route_handler(path, method, event.get('requestContext', {}).get('domainName'))
 
         if not route_handler:
-            return self._response(404, f"Path or method not found: {path}, {method}", method)
+            return self._response(404, {'error': f"Path or method not found: {path}, {method}"}, method)
 
         return route_handler(request)
 
     def _get_route_handler(self, path, method, domain_name):
         if path == '/' and method == RequestMethod.GET:
             return lambda _: self._response(200, self.handle_base_path(), method)
         if path == '/openapi.json' and method == RequestMethod.GET:
@@ -64,21 +65,21 @@
         return None
 
     def _run_action(self, request, path, method):
         try:
             body = self.routes[path][method].run(request.json())
             return self._response(200, body, method)
         except ValidationError as e:
-            return self._response(400, {'error': 'Invalid request body', 'details': str(e)}, method)
-        except ValueError as e:
-            return self._response(400, {'error': str(e), 'details': 'Check the path and method or JSON body format.'}, method)
+            return self._response(400, InvalidRequestError(str(e)).to_dict(), method)
+        except VaulError as e:
+            return self._response(e.status_code, e.to_dict(), method)
         except Exception as e:
             if self.debug:
                 print(e)
-            return self._response(500, {'error': str(e), 'details': 'Internal server error'}, method)
+            return self._response(500, InternalServerError(str(e)).to_dict(), method)
 
     def _response(self, status_code, body, method, content_type='application/json', is_base64_encoded=False):
         headers = {
             'Content-Type': content_type,
         }
 
         if method == RequestMethod.OPTIONS:
@@ -99,14 +100,15 @@
         return self.middleware(event)
 
     def _generate_openapi_schema(self, url: str):
         openapi_paths = {}
         for path, methods in self.routes.items():
             for method, action in methods.items():
                 openapi_paths.setdefault(path, {})[method.lower()] = action.openapi_schema[path][method.lower()]
+
         return {
             "openapi": "3.0.0",
             "info": {"title": "Vaul API", "version": "1.0.0", "description": "Vaul Cloud API"},
             "servers": [{"url": url}],
             "paths": openapi_paths,
         }
 
@@ -125,9 +127,8 @@
         }
 
     def handle_openapi_request(self, domain_name):
         return self._generate_openapi_schema(url=f'https://{domain_name}/')
 
     @staticmethod
     def handle_base_path():
-        return {'message': 'Vaul Cloud API Base Path'}
-
+        return {'message': 'Vaul Cloud Action API Base Path'}
```

### Comparing `vaul-0.1.22/vaul/ctx.py` & `vaul-0.1.23/vaul/ctx.py`

 * *Files identical despite different names*

### Comparing `vaul-0.1.22/vaul/helpers.py` & `vaul-0.1.23/vaul/helpers.py`

 * *Files identical despite different names*

### Comparing `vaul-0.1.22/vaul/logging.py` & `vaul-0.1.23/vaul/logging.py`

 * *Files identical despite different names*

### Comparing `vaul-0.1.22/vaul/models.py` & `vaul-0.1.23/vaul/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,19 @@
 
 class BaseAction(BaseModel):
     class Config:
         extra = Extra.allow
 
 
 class Action:
-    def __init__(self, func: Callable, path: str, method: RequestMethod):
+    def __init__(self, func: Callable, path: str, method: RequestMethod, preserve_output_types: bool = False):
         self.func = func
         self.validate_func = validate_arguments(func)
         self.method = method
+        self.preserve_output_types = preserve_output_types
         self.path = self._normalize_path(path, func.__name__)
         self.openapi_schema = self._generate_openapi_schema()
 
     @staticmethod
     def _normalize_path(path: str, func_name: str) -> str:
         return path if path != '/' else f'/{func_name.strip("/").replace("/", "_").replace(" ", "_")}'
 
@@ -102,14 +103,17 @@
         schema["properties"] = relevant_properties
         schema["required"] = required_fields
         schema = remove_keys_recursively(schema, "additionalProperties")
         schema = remove_keys_recursively(schema, "title")
         return schema
 
     def _create_output_schema(self) -> Dict[str, Any]:
+        if not self.preserve_output_types:
+            return {"type": "string"}
+
         return_type = get_type_hints(self.func).get('return', Any)
         if return_type == Any:
             return {"type": "object", "additionalProperties": True}
         if return_type and issubclass(return_type, BaseModel):
             return return_type.schema()
         temp_model = create_model('TempModel', result=(return_type, ...))
         return temp_model.schema()["properties"]["result"]
```

### Comparing `vaul-0.1.22/vaul/request.py` & `vaul-0.1.23/vaul/request.py`

 * *Files identical despite different names*

### Comparing `vaul-0.1.22/vaul.egg-info/PKG-INFO` & `vaul-0.1.23/vaul.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaul
-Version: 0.1.22
+Version: 0.1.23
 Summary: A nano-framework for deploying Python functions as APIs on AWS Lambda using Function URLs.
 Author: Spencer Porter
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: pydantic==2.6.4
```

