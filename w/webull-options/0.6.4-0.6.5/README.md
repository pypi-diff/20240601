# Comparing `tmp/webull_options-0.6.4.tar.gz` & `tmp/webull_options-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webull_options-0.6.4.tar", last modified: Sat Jun  1 18:46:29 2024, max compression
+gzip compressed data, was "webull_options-0.6.5.tar", last modified: Sat Jun  1 18:49:10 2024, max compression
```

## Comparing `webull_options-0.6.4.tar` & `webull_options-0.6.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 18:46:29.367531 webull_options-0.6.4/
--rw-rw-rw-   0        0        0     7366 2024-06-01 18:46:29.366531 webull_options-0.6.4/PKG-INFO
--rw-rw-rw-   0        0        0       55 2024-01-06 17:03:12.000000 webull_options-0.6.4/README.md
--rw-rw-rw-   0        0        0       42 2024-06-01 18:46:29.367531 webull_options-0.6.4/setup.cfg
--rw-rw-rw-   0        0        0      370 2024-06-01 18:46:17.000000 webull_options-0.6.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 18:46:29.341023 webull_options-0.6.4/webull_options/
--rw-rw-rw-   0        0        0        0 2024-01-06 17:03:12.000000 webull_options-0.6.4/webull_options/__init__.py
--rw-rw-rw-   0        0        0    15129 2024-01-06 17:03:12.000000 webull_options-0.6.4/webull_options/helpers.py
-drwxrwxrwx   0        0        0        0 2024-06-01 18:46:29.358531 webull_options-0.6.4/webull_options/models/
--rw-rw-rw-   0        0        0        0 2024-01-06 17:03:12.000000 webull_options-0.6.4/webull_options/models/__init__.py
--rw-rw-rw-   0        0        0    36853 2024-02-06 07:52:04.000000 webull_options-0.6.4/webull_options/models/db_manager.py
--rw-rw-rw-   0        0        0    23420 2024-04-23 23:48:07.000000 webull_options-0.6.4/webull_options/models/options_data.py
--rw-rw-rw-   0        0        0    47798 2024-06-01 18:46:08.000000 webull_options-0.6.4/webull_options/webull_options.py
--rw-rw-rw-   0        0        0      957 2024-02-06 07:52:33.000000 webull_options-0.6.4/webull_options/webull_trader.py
-drwxrwxrwx   0        0        0        0 2024-06-01 18:46:29.356527 webull_options-0.6.4/webull_options.egg-info/
--rw-rw-rw-   0        0        0     7366 2024-06-01 18:46:29.000000 webull_options-0.6.4/webull_options.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      433 2024-06-01 18:46:29.000000 webull_options-0.6.4/webull_options.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 18:46:29.000000 webull_options-0.6.4/webull_options.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     3865 2024-06-01 18:46:29.000000 webull_options-0.6.4/webull_options.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-06-01 18:46:29.000000 webull_options-0.6.4/webull_options.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-06-01 18:49:10.565854 webull_options-0.6.5/
+-rw-rw-rw-   0        0        0     7366 2024-06-01 18:49:10.564854 webull_options-0.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0       55 2024-01-06 17:03:12.000000 webull_options-0.6.5/README.md
+-rw-rw-rw-   0        0        0       42 2024-06-01 18:49:10.565854 webull_options-0.6.5/setup.cfg
+-rw-rw-rw-   0        0        0      370 2024-06-01 18:48:29.000000 webull_options-0.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:49:10.544855 webull_options-0.6.5/webull_options/
+-rw-rw-rw-   0        0        0        0 2024-01-06 17:03:12.000000 webull_options-0.6.5/webull_options/__init__.py
+-rw-rw-rw-   0        0        0    15129 2024-01-06 17:03:12.000000 webull_options-0.6.5/webull_options/helpers.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:49:10.556854 webull_options-0.6.5/webull_options/models/
+-rw-rw-rw-   0        0        0        0 2024-01-06 17:03:12.000000 webull_options-0.6.5/webull_options/models/__init__.py
+-rw-rw-rw-   0        0        0    36853 2024-02-06 07:52:04.000000 webull_options-0.6.5/webull_options/models/db_manager.py
+-rw-rw-rw-   0        0        0    23420 2024-04-23 23:48:07.000000 webull_options-0.6.5/webull_options/models/options_data.py
+-rw-rw-rw-   0        0        0    47798 2024-06-01 18:46:08.000000 webull_options-0.6.5/webull_options/webull_options.py
+-rw-rw-rw-   0        0        0      957 2024-02-06 07:52:33.000000 webull_options-0.6.5/webull_options/webull_trader.py
+drwxrwxrwx   0        0        0        0 2024-06-01 18:49:10.554855 webull_options-0.6.5/webull_options.egg-info/
+-rw-rw-rw-   0        0        0     7366 2024-06-01 18:49:10.000000 webull_options-0.6.5/webull_options.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2024-06-01 18:49:10.000000 webull_options-0.6.5/webull_options.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 18:49:10.000000 webull_options-0.6.5/webull_options.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     3865 2024-06-01 18:49:10.000000 webull_options-0.6.5/webull_options.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-06-01 18:49:10.000000 webull_options-0.6.5/webull_options.egg-info/top_level.txt
```

### Comparing `webull_options-0.6.4/PKG-INFO` & `webull_options-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webull_options
-Version: 0.6.4
+Version: 0.6.5
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: appdirs==1.4.4
@@ -114,15 +114,15 @@
 Requires-Dist: mypy-extensions==1.0.0
 Requires-Dist: namex==0.0.7
 Requires-Dist: natsort==8.4.0
 Requires-Dist: nh3==0.2.14
 Requires-Dist: numpy==1.26.4
 Requires-Dist: oauthlib==3.2.2
 Requires-Dist: onnxruntime==1.16.1
-Requires-Dist: openai==1.30.1
+Requires-Dist: openai==1.30.5
 Requires-Dist: opentelemetry-api==1.20.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-common==1.20.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc==1.20.0
 Requires-Dist: opentelemetry-proto==1.20.0
 Requires-Dist: opentelemetry-sdk==1.20.0
 Requires-Dist: opentelemetry-semantic-conventions==0.41b0
 Requires-Dist: opt-einsum==3.3.0
```

### Comparing `webull_options-0.6.4/webull_options/helpers.py` & `webull_options-0.6.5/webull_options/helpers.py`

 * *Files identical despite different names*

### Comparing `webull_options-0.6.4/webull_options/models/db_manager.py` & `webull_options-0.6.5/webull_options/models/db_manager.py`

 * *Files identical despite different names*

### Comparing `webull_options-0.6.4/webull_options/models/options_data.py` & `webull_options-0.6.5/webull_options/models/options_data.py`

 * *Files identical despite different names*

### Comparing `webull_options-0.6.4/webull_options/webull_options.py` & `webull_options-0.6.5/webull_options/webull_options.py`

 * *Files identical despite different names*

### Comparing `webull_options-0.6.4/webull_options/webull_trader.py` & `webull_options-0.6.5/webull_options/webull_trader.py`

 * *Files identical despite different names*

### Comparing `webull_options-0.6.4/webull_options.egg-info/PKG-INFO` & `webull_options-0.6.5/webull_options.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webull-options
-Version: 0.6.4
+Version: 0.6.5
 Requires-Dist: absl-py==2.0.0
 Requires-Dist: aiofiles==23.2.1
 Requires-Dist: aiohttp==3.9.3
 Requires-Dist: aiosignal==1.3.1
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==3.7.1
 Requires-Dist: appdirs==1.4.4
@@ -114,15 +114,15 @@
 Requires-Dist: mypy-extensions==1.0.0
 Requires-Dist: namex==0.0.7
 Requires-Dist: natsort==8.4.0
 Requires-Dist: nh3==0.2.14
 Requires-Dist: numpy==1.26.4
 Requires-Dist: oauthlib==3.2.2
 Requires-Dist: onnxruntime==1.16.1
-Requires-Dist: openai==1.30.1
+Requires-Dist: openai==1.30.5
 Requires-Dist: opentelemetry-api==1.20.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-common==1.20.0
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc==1.20.0
 Requires-Dist: opentelemetry-proto==1.20.0
 Requires-Dist: opentelemetry-sdk==1.20.0
 Requires-Dist: opentelemetry-semantic-conventions==0.41b0
 Requires-Dist: opt-einsum==3.3.0
```

### Comparing `webull_options-0.6.4/webull_options.egg-info/requires.txt` & `webull_options-0.6.5/webull_options.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -111,15 +111,15 @@
 mypy-extensions==1.0.0
 namex==0.0.7
 natsort==8.4.0
 nh3==0.2.14
 numpy==1.26.4
 oauthlib==3.2.2
 onnxruntime==1.16.1
-openai==1.30.1
+openai==1.30.5
 opentelemetry-api==1.20.0
 opentelemetry-exporter-otlp-proto-common==1.20.0
 opentelemetry-exporter-otlp-proto-grpc==1.20.0
 opentelemetry-proto==1.20.0
 opentelemetry-sdk==1.20.0
 opentelemetry-semantic-conventions==0.41b0
 opt-einsum==3.3.0
```
