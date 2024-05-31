# Comparing `tmp/mcap-protobuf-support-0.5.0.tar.gz` & `tmp/mcap_protobuf_support-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcap-protobuf-support-0.5.0.tar", last modified: Tue Apr  2 22:52:55 2024, max compression
+gzip compressed data, was "mcap_protobuf_support-0.5.1.tar", last modified: Fri May 31 23:15:21 2024, max compression
```

## Comparing `mcap-protobuf-support-0.5.0.tar` & `mcap_protobuf_support-0.5.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:52:55.746525 mcap-protobuf-support-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-02 22:52:55.746525 mcap-protobuf-support-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:52:55.746525 mcap-protobuf-support-0.5.0/mcap_protobuf/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/mcap_protobuf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/mcap_protobuf/decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/mcap_protobuf/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/mcap_protobuf/reader.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/mcap_protobuf/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/mcap_protobuf/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:52:55.746525 mcap-protobuf-support-0.5.0/mcap_protobuf_support.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-02 22:52:55.000000 mcap-protobuf-support-0.5.0/mcap_protobuf_support.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-04-02 22:52:55.000000 mcap-protobuf-support-0.5.0/mcap_protobuf_support.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-02 22:52:55.000000 mcap-protobuf-support-0.5.0/mcap_protobuf_support.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-02 22:52:55.000000 mcap-protobuf-support-0.5.0/mcap_protobuf_support.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-02 22:52:55.000000 mcap-protobuf-support-0.5.0/mcap_protobuf_support.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-02 22:52:55.746525 mcap-protobuf-support-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-02 22:52:55.746525 mcap-protobuf-support-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/tests/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/tests/test_decoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-04-02 22:50:26.000000 mcap-protobuf-support-0.5.0/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:15:21.893742 mcap_protobuf_support-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-31 23:15:21.893742 mcap_protobuf_support-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-31 23:12:46.000000 mcap_protobuf_support-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:15:21.889742 mcap_protobuf_support-0.5.1/mcap_protobuf/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-31 23:12:46.000000 mcap_protobuf_support-0.5.1/mcap_protobuf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3499 2024-05-31 23:12:46.000000 mcap_protobuf_support-0.5.1/mcap_protobuf/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:12:46.000000 mcap_protobuf_support-0.5.1/mcap_protobuf/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     5061 2024-05-31 23:12:46.000000 mcap_protobuf_support-0.5.1/mcap_protobuf/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2024-05-31 23:12:46.000000 mcap_protobuf_support-0.5.1/mcap_protobuf/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3419 2024-05-31 23:12:46.000000 mcap_protobuf_support-0.5.1/mcap_protobuf/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:15:21.893742 mcap_protobuf_support-0.5.1/mcap_protobuf_support.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-05-31 23:15:21.000000 mcap_protobuf_support-0.5.1/mcap_protobuf_support.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-31 23:15:21.000000 mcap_protobuf_support-0.5.1/mcap_protobuf_support.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 23:15:21.000000 mcap_protobuf_support-0.5.1/mcap_protobuf_support.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 23:15:21.000000 mcap_protobuf_support-0.5.1/mcap_protobuf_support.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-31 23:15:21.000000 mcap_protobuf_support-0.5.1/mcap_protobuf_support.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-31 23:12:46.000000 mcap_protobuf_support-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-31 23:15:21.893742 mcap_protobuf_support-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 23:15:21.889742 mcap_protobuf_support-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 23:12:46.000000 mcap_protobuf_support-0.5.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-31 23:12:46.000000 mcap_protobuf_support-0.5.1/tests/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-05-31 23:12:46.000000 mcap_protobuf_support-0.5.1/tests/test_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 2024-05-31 23:12:46.000000 mcap_protobuf_support-0.5.1/tests/test_writer.py
```

### Comparing `mcap-protobuf-support-0.5.0/PKG-INFO` & `mcap_protobuf_support-0.5.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcap-protobuf-support
-Version: 0.5.0
+Version: 0.5.1
 Summary: Protobuf support for the Python MCAP library
 Home-page: https://github.com/foxglove/mcap
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mcap-protobuf-support-0.5.0/README.md` & `mcap_protobuf_support-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `mcap-protobuf-support-0.5.0/mcap_protobuf/decoder.py` & `mcap_protobuf_support-0.5.1/mcap_protobuf/decoder.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import warnings
 from collections import Counter
 from typing import Any, Callable, Dict, Optional, Type
 
-from google.protobuf.descriptor_pb2 import FileDescriptorSet
+from google.protobuf.descriptor_pb2 import FileDescriptorProto, FileDescriptorSet
 from google.protobuf.descriptor_pool import DescriptorPool
 from google.protobuf.message_factory import GetMessageClassesForFiles
 
 from mcap.decoder import DecoderFactory as McapDecoderFactory
 from mcap.exceptions import McapError
 from mcap.records import Message, Schema
 from mcap.well_known import MessageEncoding, SchemaEncoding
@@ -42,16 +42,25 @@
             for name, count in Counter(fd.name for fd in fds.file).most_common(1):
                 if count > 1:
                     raise McapError(
                         f"FileDescriptorSet contains {count} file descriptors for {name}"
                     )
 
             pool = DescriptorPool()
-            for fd in fds.file:
+            descriptor_by_name = {fd.name: fd for fd in fds.file}
+
+            def _add(fd: FileDescriptorProto):
+                for dependency in fd.dependency:
+                    if dependency in descriptor_by_name:
+                        _add(descriptor_by_name.pop(dependency))
                 pool.Add(fd)
+
+            while descriptor_by_name:
+                _add(descriptor_by_name.popitem()[1])
+
             messages = GetMessageClassesForFiles([fd.name for fd in fds.file], pool)
 
             for name, klass in messages.items():
                 if name == schema.name:
                     self._types[schema.id] = klass
                     generated = klass
         if generated is None:
```

### Comparing `mcap-protobuf-support-0.5.0/mcap_protobuf/reader.py` & `mcap_protobuf_support-0.5.1/mcap_protobuf/reader.py`

 * *Files identical despite different names*

### Comparing `mcap-protobuf-support-0.5.0/mcap_protobuf/schema.py` & `mcap_protobuf_support-0.5.1/mcap_protobuf/schema.py`

 * *Files identical despite different names*

### Comparing `mcap-protobuf-support-0.5.0/mcap_protobuf/writer.py` & `mcap_protobuf_support-0.5.1/mcap_protobuf/writer.py`

 * *Files identical despite different names*

### Comparing `mcap-protobuf-support-0.5.0/mcap_protobuf_support.egg-info/PKG-INFO` & `mcap_protobuf_support-0.5.1/mcap_protobuf_support.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mcap-protobuf-support
-Version: 0.5.0
+Version: 0.5.1
 Summary: Protobuf support for the Python MCAP library
 Home-page: https://github.com/foxglove/mcap
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mcap-protobuf-support-0.5.0/setup.cfg` & `mcap_protobuf_support-0.5.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `mcap-protobuf-support-0.5.0/tests/generate.py` & `mcap_protobuf_support-0.5.1/tests/generate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,64 @@
 import os
 import sys
 
+from google.protobuf.descriptor_pb2 import FileDescriptorSet
+
+from mcap.writer import Writer as McapWriter
+
 sys.path.append(os.path.dirname(__file__))  # for test_proto imports
 
-from typing import IO, Any  # noqa: #402
+from typing import IO, Any, Set  # noqa: #402
 
 from mcap_protobuf.writer import Writer  # noqa: #402
 from test_proto.complex_message_pb2 import ComplexMessage  # noqa: #402
 from test_proto.intermediate_message_1_pb2 import IntermediateMessage1  # noqa: #402
 from test_proto.intermediate_message_2_pb2 import IntermediateMessage2  # noqa: #402
 from test_proto.simple_message_pb2 import SimpleMessage  # noqa: #402
 
 
+def generate_sample_data_with_disordered_proto_fds(output: IO[Any]):
+    """generates a simple sample MCAP with a protobuf message. This library normally produces
+    file descriptor sets in topological dependency order, but the reader needs to be able to handle
+    schemas with file descriptor sets written in other orders.
+    """
+    file_descriptor_set = FileDescriptorSet()
+    seen_dependencies: Set[str] = set()
+    toplevel = ComplexMessage.DESCRIPTOR.file
+    to_add = {toplevel.name: toplevel}
+    while to_add:
+        fd = to_add.popitem()[1]
+        seen_dependencies.add(fd.name)
+        fd.CopyToProto(file_descriptor_set.file.add())
+        for dep in fd.dependencies:
+            if dep.name not in seen_dependencies:
+                to_add[dep.name] = dep
+
+    writer = McapWriter(output)
+    writer.start()
+    schema_id = writer.register_schema(
+        name=ComplexMessage.DESCRIPTOR.full_name,
+        encoding="protobuf",
+        data=file_descriptor_set.SerializeToString(),
+    )
+    channel_id = writer.register_channel("/complex_msgs", "protobuf", schema_id)
+    writer.add_message(
+        channel_id,
+        0,
+        ComplexMessage(
+            intermediate1=IntermediateMessage1(simple=SimpleMessage(data="a")),
+            intermediate2=IntermediateMessage2(simple=SimpleMessage(data="b")),
+        ).SerializeToString(),
+        0,
+        0,
+    )
+    writer.finish()
+    output.seek(0)
+
+
 def generate_sample_data(output: IO[Any]):
     with Writer(output) as writer:
         for i in range(1, 11):
             simple_message = SimpleMessage(data=f"Hello MCAP protobuf world #{i}!")
             writer.write_message(
                 topic="/simple_message",
                 message=simple_message,
```

### Comparing `mcap-protobuf-support-0.5.0/tests/test_writer.py` & `mcap_protobuf_support-0.5.1/tests/test_writer.py`

 * *Files identical despite different names*

