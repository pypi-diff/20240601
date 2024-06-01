# Comparing `tmp/coherence_client-1.1.0.tar.gz` & `tmp/coherence_client-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coherence_client-1.1.0.tar", max compression
+gzip compressed data, was "coherence_client-1.1.1.tar", max compression
```

## Comparing `coherence_client-1.1.0.tar` & `coherence_client-1.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1839 2024-04-30 22:39:15.460961 coherence_client-1.1.0/LICENSE.txt
--rw-r--r--   0        0        0     4794 2024-04-30 22:39:15.460961 coherence_client-1.1.0/README.md
--rw-r--r--   0        0        0     2053 2024-04-30 22:39:15.460961 coherence_client-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1090 2024-04-30 22:39:15.460961 coherence_client-1.1.0/src/coherence/__init__.py
--rw-r--r--   0        0        0    33785 2024-04-30 22:39:15.460961 coherence_client-1.1.0/src/coherence/aggregator.py
--rw-r--r--   0        0        0    71570 2024-04-30 22:39:15.460961 coherence_client-1.1.0/src/coherence/client.py
--rw-r--r--   0        0        0     1468 2024-04-30 22:39:15.460961 coherence_client-1.1.0/src/coherence/comparator.py
--rw-r--r--   0        0        0    31490 2024-04-30 22:39:15.460961 coherence_client-1.1.0/src/coherence/event.py
--rw-r--r--   0        0        0    13494 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/extractor.py
--rw-r--r--   0        0        0    36730 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/filter.py
--rw-r--r--   0        0        0    11698 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/messages_pb2.py
--rw-r--r--   0        0        0      159 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/messages_pb2_grpc.py
--rw-r--r--   0        0        0    33984 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/processor.py
--rw-r--r--   0        0        0    10395 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/serialization.py
--rw-r--r--   0        0        0     4040 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/services_pb2.py
--rw-r--r--   0        0        0    45397 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/services_pb2_grpc.py
--rw-r--r--   0        0        0    12807 2024-04-30 22:39:15.464961 coherence_client-1.1.0/src/coherence/util.py
--rw-r--r--   0        0        0     5993 1970-01-01 00:00:00.000000 coherence_client-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1839 2024-06-01 00:09:43.034612 coherence_client-1.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     4794 2024-06-01 00:09:43.034612 coherence_client-1.1.1/README.md
+-rw-r--r--   0        0        0     2060 2024-06-01 00:09:43.038612 coherence_client-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1089 2024-06-01 00:09:43.038612 coherence_client-1.1.1/src/coherence/__init__.py
+-rw-r--r--   0        0        0    33785 2024-06-01 00:09:43.038612 coherence_client-1.1.1/src/coherence/aggregator.py
+-rw-r--r--   0        0        0    71570 2024-06-01 00:09:43.038612 coherence_client-1.1.1/src/coherence/client.py
+-rw-r--r--   0        0        0     1468 2024-06-01 00:09:43.038612 coherence_client-1.1.1/src/coherence/comparator.py
+-rw-r--r--   0        0        0    31490 2024-06-01 00:09:43.038612 coherence_client-1.1.1/src/coherence/event.py
+-rw-r--r--   0        0        0    13494 2024-06-01 00:09:43.038612 coherence_client-1.1.1/src/coherence/extractor.py
+-rw-r--r--   0        0        0    36730 2024-06-01 00:09:43.038612 coherence_client-1.1.1/src/coherence/filter.py
+-rw-r--r--   0        0        0    11698 2024-06-01 00:09:43.038612 coherence_client-1.1.1/src/coherence/messages_pb2.py
+-rw-r--r--   0        0        0      159 2024-06-01 00:09:43.038612 coherence_client-1.1.1/src/coherence/messages_pb2_grpc.py
+-rw-r--r--   0        0        0    33984 2024-06-01 00:09:43.038612 coherence_client-1.1.1/src/coherence/processor.py
+-rw-r--r--   0        0        0    10395 2024-06-01 00:09:43.038612 coherence_client-1.1.1/src/coherence/serialization.py
+-rw-r--r--   0        0        0     4040 2024-06-01 00:09:43.038612 coherence_client-1.1.1/src/coherence/services_pb2.py
+-rw-r--r--   0        0        0    45397 2024-06-01 00:09:43.038612 coherence_client-1.1.1/src/coherence/services_pb2_grpc.py
+-rw-r--r--   0        0        0    12807 2024-06-01 00:09:43.038612 coherence_client-1.1.1/src/coherence/util.py
+-rw-r--r--   0        0        0     5993 1970-01-01 00:00:00.000000 coherence_client-1.1.1/PKG-INFO
```

### Comparing `coherence_client-1.1.0/LICENSE.txt` & `coherence_client-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coherence_client-1.1.0/README.md` & `coherence_client-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `coherence_client-1.1.0/pyproject.toml` & `coherence_client-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) 2022, 2024, Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at
 # https://oss.oracle.com/licenses/upl.
 [tool.poetry]
 name = "coherence-client"
-version = "1.1.0"
+version = "1.1.1"
 description = """The Coherence Python Client allows Python applications to act as cache clients to a \
 Coherence Cluster using Google's gRPC framework as the network transport."""
 packages = [
     { include = "coherence", from = "./src"},
 ]
 readme = "README.md"
 authors = ["Oracle <dhiru.pandey@oracle.com>"]
@@ -19,19 +19,19 @@
     "Operating System :: OS Independent",
     "Development Status :: 5 - Production/Stable",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 protobuf = ">=4.23,<4.26"
-grpcio = ">=1.54,<1.63"
+grpcio = ">=1.54,<1.65"
 grpcio-tools = ">=1.54,<1.63"
 jsonpickle = "~3.0"
 pymitter = ">=0.4,<0.6"
-typing-extensions = "~4.11"
+typing-extensions = ">=4.11,<4.13"
 
 [tool.poetry.dev-dependencies]
 pytest = "~8.2"
 pytest-asyncio = "~0.23"
 pytest-cov = "~5.0"
 pytest-unordered = "~0.6"
 pre-commit = "~3.5"
```

### Comparing `coherence_client-1.1.0/src/coherence/__init__.py` & `coherence_client-1.1.1/src/coherence/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) 2022, 2024, Oracle and/or its affiliates.
 # Licensed under the Universal Permissive License v 1.0 as shown at
 # https://oss.oracle.com/licenses/upl.
 
 from __future__ import annotations
 
-__version__ = "1.0rc2"
+__version__ = "1.1.1"
 
 import logging
 
 # expose these symbols in top-level namespace
 from .aggregator import Aggregators as Aggregators
 from .client import MapEntry as MapEntry
 from .client import NamedCache as NamedCache
```

### Comparing `coherence_client-1.1.0/src/coherence/aggregator.py` & `coherence_client-1.1.1/src/coherence/aggregator.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.1.0/src/coherence/client.py` & `coherence_client-1.1.1/src/coherence/client.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.1.0/src/coherence/comparator.py` & `coherence_client-1.1.1/src/coherence/comparator.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.1.0/src/coherence/event.py` & `coherence_client-1.1.1/src/coherence/event.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.1.0/src/coherence/extractor.py` & `coherence_client-1.1.1/src/coherence/extractor.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.1.0/src/coherence/filter.py` & `coherence_client-1.1.1/src/coherence/filter.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.1.0/src/coherence/messages_pb2.py` & `coherence_client-1.1.1/src/coherence/messages_pb2.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.1.0/src/coherence/processor.py` & `coherence_client-1.1.1/src/coherence/processor.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.1.0/src/coherence/serialization.py` & `coherence_client-1.1.1/src/coherence/serialization.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.1.0/src/coherence/services_pb2.py` & `coherence_client-1.1.1/src/coherence/services_pb2.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.1.0/src/coherence/services_pb2_grpc.py` & `coherence_client-1.1.1/src/coherence/services_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.1.0/src/coherence/util.py` & `coherence_client-1.1.1/src/coherence/util.py`

 * *Files identical despite different names*

### Comparing `coherence_client-1.1.0/PKG-INFO` & `coherence_client-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: coherence-client
-Version: 1.1.0
+Version: 1.1.1
 Summary: The Coherence Python Client allows Python applications to act as cache clients to a Coherence Cluster using Google's gRPC framework as the network transport.
 Home-page: https://github.com/oracle/coherence-py-client
 Author: Oracle
 Author-email: dhiru.pandey@oracle.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Universal Permissive License (UPL)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: grpcio (>=1.54,<1.63)
+Requires-Dist: grpcio (>=1.54,<1.65)
 Requires-Dist: grpcio-tools (>=1.54,<1.63)
 Requires-Dist: jsonpickle (>=3.0,<3.1)
 Requires-Dist: protobuf (>=4.23,<4.26)
 Requires-Dist: pymitter (>=0.4,<0.6)
-Requires-Dist: typing-extensions (>=4.11,<4.12)
+Requires-Dist: typing-extensions (>=4.11,<4.13)
 Project-URL: Repository, https://github.com/oracle/coherence-py-client
 Description-Content-Type: text/markdown
 
 # Coherence Python Client
 
 ![CI/CD](https://github.com/oracle/coherence-py-client/actions/workflows/validate.yml/badge.svg)
 [![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=oracle_coherence-py-client&metric=alert_status)](https://sonarcloud.io/project/overview?id=oracle_coherence-py-client)
```

