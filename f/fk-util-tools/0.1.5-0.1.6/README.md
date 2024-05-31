# Comparing `tmp/fk_util_tools-0.1.5.tar.gz` & `tmp/fk_util_tools-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fk_util_tools-0.1.5.tar", last modified: Thu May 30 23:47:40 2024, max compression
+gzip compressed data, was "fk_util_tools-0.1.6.tar", last modified: Fri May 31 00:37:08 2024, max compression
```

## Comparing `fk_util_tools-0.1.5.tar` & `fk_util_tools-0.1.6.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/fk_util_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-30 23:47:40.000000 fk_util_tools-0.1.5/fk_util_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-30 23:47:40.000000 fk_util_tools-0.1.5/fk_util_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-30 23:47:40.000000 fk_util_tools-0.1.5/fk_util_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-05-30 23:47:40.000000 fk_util_tools-0.1.5/fk_util_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-30 23:47:40.000000 fk_util_tools-0.1.5/fk_util_tools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.474040 fk_util_tools-0.1.5/fk_utils/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.474040 fk_util_tools-0.1.5/fk_utils/envs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/envs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.474040 fk_util_tools-0.1.5/fk_utils/envs/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/envs/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/envs/aws/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/envs/aws/secrets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.474040 fk_util_tools-0.1.5/fk_utils/middlewares/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/middlewares/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.474040 fk_util_tools-0.1.5/fk_utils/middlewares/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/middlewares/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/middlewares/django/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.474040 fk_util_tools-0.1.5/fk_utils/middlewares/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/middlewares/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/middlewares/fastapi/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.474040 fk_util_tools-0.1.5/fk_utils/middlewares/flask/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/middlewares/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/middlewares/flask/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.474040 fk_util_tools-0.1.5/fk_utils/traces/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/fk_utils/traces/datadog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/datadog/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/django/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/django/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/django/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/fastapi/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/fastapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/fastapi/trace.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/flask/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/flask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-30 23:47:36.000000 fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/flask/trace.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-05-30 23:47:40.478041 fk_util_tools-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1179 2024-05-30 23:47:38.000000 fk_util_tools-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:08.724522 fk_util_tools-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-31 00:37:08.724522 fk_util_tools-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:08.724522 fk_util_tools-0.1.6/fk_util_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-31 00:37:08.000000 fk_util_tools-0.1.6/fk_util_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-31 00:37:08.000000 fk_util_tools-0.1.6/fk_util_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 00:37:08.000000 fk_util_tools-0.1.6/fk_util_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-31 00:37:08.000000 fk_util_tools-0.1.6/fk_util_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-31 00:37:08.000000 fk_util_tools-0.1.6/fk_util_tools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:08.720522 fk_util_tools-0.1.6/fk_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:08.720522 fk_util_tools-0.1.6/fk_utils/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/envs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:08.720522 fk_util_tools-0.1.6/fk_utils/envs/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/envs/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/envs/aws/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/envs/aws/secrets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:08.720522 fk_util_tools-0.1.6/fk_utils/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/middlewares/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:08.720522 fk_util_tools-0.1.6/fk_utils/middlewares/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/middlewares/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/middlewares/django/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:08.720522 fk_util_tools-0.1.6/fk_utils/middlewares/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/middlewares/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/middlewares/fastapi/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:08.720522 fk_util_tools-0.1.6/fk_utils/middlewares/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/middlewares/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/middlewares/flask/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:08.720522 fk_util_tools-0.1.6/fk_utils/traces/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/traces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:08.724522 fk_util_tools-0.1.6/fk_utils/traces/datadog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/traces/datadog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/traces/datadog/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:08.724522 fk_util_tools-0.1.6/fk_utils/traces/opentelemetry/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/traces/opentelemetry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:08.724522 fk_util_tools-0.1.6/fk_utils/traces/opentelemetry/django/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/traces/opentelemetry/django/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2098 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/traces/opentelemetry/django/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:08.724522 fk_util_tools-0.1.6/fk_utils/traces/opentelemetry/fastapi/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/traces/opentelemetry/fastapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1823 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/traces/opentelemetry/fastapi/trace.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:08.724522 fk_util_tools-0.1.6/fk_utils/traces/opentelemetry/flask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/traces/opentelemetry/flask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-31 00:37:04.000000 fk_util_tools-0.1.6/fk_utils/traces/opentelemetry/flask/trace.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      556 2024-05-31 00:37:08.724522 fk_util_tools-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-05-31 00:37:06.000000 fk_util_tools-0.1.6/setup.py
```

### Comparing `fk_util_tools-0.1.5/LICENSE` & `fk_util_tools-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.5/fk_util_tools.egg-info/SOURCES.txt` & `fk_util_tools-0.1.6/fk_util_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 fk_utils/middlewares/django/handler.py
 fk_utils/middlewares/fastapi/__init__.py
 fk_utils/middlewares/fastapi/handler.py
 fk_utils/middlewares/flask/__init__.py
 fk_utils/middlewares/flask/handler.py
 fk_utils/traces/__init__.py
 fk_utils/traces/datadog/__init__.py
+fk_utils/traces/datadog/trace.py
 fk_utils/traces/opentelemetry/__init__.py
 fk_utils/traces/opentelemetry/django/__init__.py
 fk_utils/traces/opentelemetry/django/trace.py
 fk_utils/traces/opentelemetry/fastapi/__init__.py
 fk_utils/traces/opentelemetry/fastapi/trace.py
 fk_utils/traces/opentelemetry/flask/__init__.py
 fk_utils/traces/opentelemetry/flask/trace.py
```

### Comparing `fk_util_tools-0.1.5/fk_utils/config.py` & `fk_util_tools-0.1.6/fk_utils/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,7 +14,11 @@
         self.AWS_REGION_NAME = os.environ.get('AWS_REGION_NAME', 'us-east-1')
         self.SECRET_NAME = os.environ.get('SECRET_NAME', 'api/testing/ms-communicator')
 
         # Opentelemtry
         self.OTLP_HOST = os.environ.get('OTLP_HOST', 'localhost')
         self.OTLP_PORT = os.environ.get('OTLP_PORT', '0000')
         self.OTLP_NAME = os.environ.get('OTLP_NAME', 'ms-localhost')
+
+        # DataDog
+        self.DD_HOST = os.environ.get('DD_HOST', 'localhost')
+        self.DD_PORT = os.environ.get('DD_PORT', '8126')
```

### Comparing `fk_util_tools-0.1.5/fk_utils/envs/aws/parameters.py` & `fk_util_tools-0.1.6/fk_utils/envs/aws/parameters.py`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.5/fk_utils/envs/aws/secrets.py` & `fk_util_tools-0.1.6/fk_utils/envs/aws/secrets.py`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/django/trace.py` & `fk_util_tools-0.1.6/fk_utils/traces/opentelemetry/django/trace.py`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/fastapi/trace.py` & `fk_util_tools-0.1.6/fk_utils/traces/opentelemetry/fastapi/trace.py`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.5/fk_utils/traces/opentelemetry/flask/trace.py` & `fk_util_tools-0.1.6/fk_utils/traces/opentelemetry/flask/trace.py`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.5/setup.cfg` & `fk_util_tools-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `fk_util_tools-0.1.5/setup.py` & `fk_util_tools-0.1.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 
 
-VERSION = '0.1.5'
+VERSION = '0.1.6'
 PACKAGE_NAME = 'fk_util_tools'
 AUTHOR = 'Steven Santacruz Garcia'
 AUTHOR_EMAIL = 'stevengarcia1118@gmail.com'
 URL = 'https://gitlab.com/f3315/team-back-end/cross/packages/package_utils'
 
 LICENSE = 'MIT'
 DESCRIPTION = """Herramientas de utilidad o funciones comunes para los proyectos de FK."""
@@ -19,16 +19,17 @@
     'opentelemetry-instrumentation-fastapi',
     'opentelemetry-instrumentation-flask',
     'opentelemetry-instrumentation-django',
     'opentelemetry-exporter-otlp',
     'opentelemetry-instrumentation-sqlalchemy',
     'opentelemetry-instrumentation-requests',
     'opentelemetry-exporter-jaeger',
-    'opentelemetry-instrumentation-psycopg2'
-
+    'opentelemetry-instrumentation-psycopg2',
+    'psycopg2',
+    'ddtrace'
 ]
 
 setup(
     name=PACKAGE_NAME,
     version=VERSION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type=LONG_DESC_TYPE,
```

