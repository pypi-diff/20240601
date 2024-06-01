# Comparing `tmp/event_outbox-0.1.0.tar.gz` & `tmp/event_outbox-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event_outbox-0.1.0.tar", max compression
+gzip compressed data, was "event_outbox-0.1.1.tar", max compression
```

## Comparing `event_outbox-0.1.0.tar` & `event_outbox-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      162 2024-06-01 14:17:48.866043 event_outbox-0.1.0/event_outbox/__init__.py
--rw-r--r--   0        0        0    13354 2024-06-01 14:13:36.273262 event_outbox-0.1.0/event_outbox/eventu.py
--rw-r--r--   0        0        0        0 2024-06-01 14:02:32.595614 event_outbox-0.1.0/event_outbox/py.typed
--rw-r--r--   0        0        0      615 2024-06-01 14:24:29.055351 event_outbox-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 event_outbox-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      165 2024-06-01 14:30:17.044489 event_outbox-0.1.1/event_outbox/__init__.py
+-rw-r--r--   0        0        0        0 2024-06-01 14:02:32.595614 event_outbox-0.1.1/event_outbox/py.typed
+-rw-r--r--   0        0        0    13354 2024-06-01 14:13:36.273262 event_outbox-0.1.1/event_outbox/transport.py
+-rw-r--r--   0        0        0      615 2024-06-01 14:30:29.952530 event_outbox-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      520 1970-01-01 00:00:00.000000 event_outbox-0.1.1/PKG-INFO
```

### Comparing `event_outbox-0.1.0/event_outbox/eventu.py` & `event_outbox-0.1.1/event_outbox/transport.py`

 * *Files identical despite different names*

### Comparing `event_outbox-0.1.0/pyproject.toml` & `event_outbox-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "event-outbox"
-version = "0.1.0"
+version = "0.1.1"
 description = "Transactional outbox and idempotent consumer"
 authors = ["Yuriy Kehter <yuriy.kehter@gmail.com>"]
 packages = [{ include = "event_outbox" }]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 aiokafka = "^0.10.0"
```

### Comparing `event_outbox-0.1.0/PKG-INFO` & `event_outbox-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: event-outbox
-Version: 0.1.0
+Version: 0.1.1
 Summary: Transactional outbox and idempotent consumer
 Author: Yuriy Kehter
 Author-email: yuriy.kehter@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

