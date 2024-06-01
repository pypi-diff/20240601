# Comparing `tmp/smp-1.0.3.tar.gz` & `tmp/smp-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smp-1.0.3.tar", max compression
+gzip compressed data, was "smp-2.0.0.tar", max compression
```

## Comparing `smp-1.0.3.tar` & `smp-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    11365 2024-05-23 00:03:27.238694 smp-1.0.3/LICENSE
--rw-r--r--   0        0        0     2312 2024-05-23 00:03:27.238694 smp-1.0.3/README.md
--rw-r--r--   0        0        0     1595 2024-05-23 00:03:27.242694 smp-1.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-23 00:03:27.242694 smp-1.0.3/smp/__init__.py
--rw-r--r--   0        0        0     1811 2024-05-23 00:03:27.242694 smp-1.0.3/smp/error.py
--rw-r--r--   0        0        0      471 2024-05-23 00:03:27.242694 smp-1.0.3/smp/exceptions.py
--rw-r--r--   0        0        0     5090 2024-05-23 00:03:27.242694 smp-1.0.3/smp/header.py
--rw-r--r--   0        0        0     6272 2024-05-23 00:03:27.242694 smp-1.0.3/smp/image_management.py
--rw-r--r--   0        0        0     4882 2024-05-23 00:03:27.242694 smp-1.0.3/smp/message.py
--rw-r--r--   0        0        0     7137 2024-05-23 00:03:27.242694 smp-1.0.3/smp/os_management.py
--rw-r--r--   0        0        0     3135 2024-05-23 00:03:27.242694 smp-1.0.3/smp/packet.py
--rw-r--r--   0        0        0        0 2024-05-23 00:03:27.242694 smp-1.0.3/smp/py.typed
--rw-r--r--   0        0        0     1003 2024-05-23 00:03:27.242694 smp-1.0.3/smp/shell_management.py
--rw-r--r--   0        0        0        0 2024-05-23 00:03:27.242694 smp-1.0.3/smp/user/__init__.py
--rw-r--r--   0        0        0     1308 2024-05-23 00:03:27.242694 smp-1.0.3/smp/user/intercreate.py
--rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 smp-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0    11365 2024-06-01 20:58:28.269025 smp-2.0.0/LICENSE
+-rw-r--r--   0        0        0     2312 2024-06-01 20:58:28.269025 smp-2.0.0/README.md
+-rw-r--r--   0        0        0     1595 2024-06-01 20:58:28.269025 smp-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-06-01 20:58:28.269025 smp-2.0.0/smp/__init__.py
+-rw-r--r--   0        0        0     1811 2024-06-01 20:58:28.269025 smp-2.0.0/smp/error.py
+-rw-r--r--   0        0        0      471 2024-06-01 20:58:28.269025 smp-2.0.0/smp/exceptions.py
+-rw-r--r--   0        0        0     5090 2024-06-01 20:58:28.269025 smp-2.0.0/smp/header.py
+-rw-r--r--   0        0        0     6526 2024-06-01 20:58:28.269025 smp-2.0.0/smp/image_management.py
+-rw-r--r--   0        0        0     4882 2024-06-01 20:58:28.269025 smp-2.0.0/smp/message.py
+-rw-r--r--   0        0        0     7137 2024-06-01 20:58:28.269025 smp-2.0.0/smp/os_management.py
+-rw-r--r--   0        0        0     3135 2024-06-01 20:58:28.269025 smp-2.0.0/smp/packet.py
+-rw-r--r--   0        0        0        0 2024-06-01 20:58:28.269025 smp-2.0.0/smp/py.typed
+-rw-r--r--   0        0        0     1003 2024-06-01 20:58:28.273025 smp-2.0.0/smp/shell_management.py
+-rw-r--r--   0        0        0        0 2024-06-01 20:58:28.273025 smp-2.0.0/smp/user/__init__.py
+-rw-r--r--   0        0        0     1308 2024-06-01 20:58:28.273025 smp-2.0.0/smp/user/intercreate.py
+-rw-r--r--   0        0        0     3087 1970-01-01 00:00:00.000000 smp-2.0.0/PKG-INFO
```

### Comparing `smp-1.0.3/LICENSE` & `smp-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smp-1.0.3/README.md` & `smp-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `smp-1.0.3/pyproject.toml` & `smp-2.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `smp-1.0.3/smp/error.py` & `smp-2.0.0/smp/error.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.3/smp/header.py` & `smp-2.0.0/smp/header.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.3/smp/image_management.py` & `smp-2.0.0/smp/image_management.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,28 +71,31 @@
     data: bytes
     image: int | None = None  # 'required' when off == 0
     len: int | None = None  # required when off == 0
     sha: bytes | None = None  # should be sent when off == 0
     upgrade: bool | None = None  # allowed when off == 0
 
 
-class ImageUploadProgressWriteResponse(message.WriteResponse):
+class ImageUploadWriteResponse(message.WriteResponse):
     _GROUP_ID = header.GroupId.IMAGE_MANAGEMENT
     _COMMAND_ID = header.CommandId.ImageManagement.UPLOAD
 
-    rc: int | None = None
     off: int | None = None
+    """The portion of the upload that has been completed, in 8-bit bytes.
 
-
-class ImageUploadFinalWriteResponse(message.WriteResponse):
-    _GROUP_ID = header.GroupId.IMAGE_MANAGEMENT
-    _COMMAND_ID = header.CommandId.ImageManagement.UPLOAD
-
-    off: int | None = None
+    This is the offset of the next byte to be written. If the offset is equal to
+    the length of the image, the upload is complete.
+    """
     match: bool | None = None
+    """Indicates if the uploaded data successfully matches the provided SHA256.
+
+    Only sent in the final packet if CONFIG_IMG_ENABLE_IMAGE_CHECK is enabled.
+    """
+    rc: int | None = None
+    """Unspecified field used by MCUBoot's SMP Server implementation."""
 
 
 class ImageEraseRequest(message.WriteRequest):
     _GROUP_ID = header.GroupId.IMAGE_MANAGEMENT
     _COMMAND_ID = header.CommandId.ImageManagement.ERASE
 
     slot: int | None = None
```

### Comparing `smp-1.0.3/smp/message.py` & `smp-2.0.0/smp/message.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.3/smp/os_management.py` & `smp-2.0.0/smp/os_management.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.3/smp/packet.py` & `smp-2.0.0/smp/packet.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.3/smp/shell_management.py` & `smp-2.0.0/smp/shell_management.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.3/smp/user/intercreate.py` & `smp-2.0.0/smp/user/intercreate.py`

 * *Files identical despite different names*

### Comparing `smp-1.0.3/PKG-INFO` & `smp-2.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smp
-Version: 1.0.3
+Version: 2.0.0
 Summary: Simple Management Protocol (SMP) for remotely managing MCU firmware
 License: Apache-2.0
 Author: J.P. Hutchins
 Author-email: jphutchins@gmail.com
 Requires-Python: >=3.8.1,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

