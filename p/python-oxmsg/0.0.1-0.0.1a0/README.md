# Comparing `tmp/python_oxmsg-0.0.1.tar.gz` & `tmp/python_oxmsg-0.0.1a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_oxmsg-0.0.1.tar", last modified: Sat Jun  1 20:53:33 2024, max compression
+gzip compressed data, was "python_oxmsg-0.0.1a0.tar", last modified: Thu May 30 05:20:51 2024, max compression
```

## Comparing `python_oxmsg-0.0.1.tar` & `python_oxmsg-0.0.1a0.tar`

### file list

```diff
@@ -1,36 +1,28 @@
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-06-01 20:53:33.314586 python_oxmsg-0.0.1/
--rw-r--r--   0 scanny     (501) staff       (20)     1104 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/LICENSE.txt
--rw-r--r--   0 scanny     (501) staff       (20)     4959 2024-06-01 20:53:33.314402 python_oxmsg-0.0.1/PKG-INFO
--rw-r--r--   0 scanny     (501) staff       (20)     3599 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/README.md
--rw-r--r--   0 scanny     (501) staff       (20)     3622 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/pyproject.toml
--rw-r--r--   0 scanny     (501) staff       (20)       38 2024-06-01 20:53:33.314643 python_oxmsg-0.0.1/setup.cfg
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-06-01 20:53:33.308754 python_oxmsg-0.0.1/src/
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-06-01 20:53:33.310901 python_oxmsg-0.0.1/src/oxmsg/
--rw-r--r--   0 scanny     (501) staff       (20)      106 2024-06-01 20:50:05.000000 python_oxmsg-0.0.1/src/oxmsg/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     2674 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/src/oxmsg/attachment.py
--rw-r--r--   0 scanny     (501) staff       (20)     6369 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/src/oxmsg/cli.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-06-01 20:53:33.311917 python_oxmsg-0.0.1/src/oxmsg/domain/
--rw-r--r--   0 scanny     (501) staff       (20)        0 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/src/oxmsg/domain/__init__.py
--rw-r--r--   0 scanny     (501) staff       (20)     7034 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/src/oxmsg/domain/constants.py
--rw-r--r--   0 scanny     (501) staff       (20)    10000 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/src/oxmsg/domain/encodings.py
--rw-r--r--   0 scanny     (501) staff       (20)     5398 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/src/oxmsg/domain/model.py
--rw-r--r--   0 scanny     (501) staff       (20)    28548 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/src/oxmsg/domain/reference.py
--rw-r--r--   0 scanny     (501) staff       (20)     6925 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/src/oxmsg/message.py
--rw-r--r--   0 scanny     (501) staff       (20)    15804 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/src/oxmsg/properties.py
--rw-r--r--   0 scanny     (501) staff       (20)        0 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/src/oxmsg/py.typed
--rw-r--r--   0 scanny     (501) staff       (20)     1474 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/src/oxmsg/recipient.py
--rw-r--r--   0 scanny     (501) staff       (20)     4341 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/src/oxmsg/storage.py
--rw-r--r--   0 scanny     (501) staff       (20)     5609 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/src/oxmsg/util.py
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-06-01 20:53:33.314113 python_oxmsg-0.0.1/src/python_oxmsg.egg-info/
--rw-r--r--   0 scanny     (501) staff       (20)     4959 2024-06-01 20:53:33.000000 python_oxmsg-0.0.1/src/python_oxmsg.egg-info/PKG-INFO
--rw-r--r--   0 scanny     (501) staff       (20)      730 2024-06-01 20:53:33.000000 python_oxmsg-0.0.1/src/python_oxmsg.egg-info/SOURCES.txt
--rw-r--r--   0 scanny     (501) staff       (20)        1 2024-06-01 20:53:33.000000 python_oxmsg-0.0.1/src/python_oxmsg.egg-info/dependency_links.txt
--rw-r--r--   0 scanny     (501) staff       (20)       42 2024-06-01 20:53:33.000000 python_oxmsg-0.0.1/src/python_oxmsg.egg-info/entry_points.txt
--rw-r--r--   0 scanny     (501) staff       (20)       39 2024-06-01 20:53:33.000000 python_oxmsg-0.0.1/src/python_oxmsg.egg-info/requires.txt
--rw-r--r--   0 scanny     (501) staff       (20)        6 2024-06-01 20:53:33.000000 python_oxmsg-0.0.1/src/python_oxmsg.egg-info/top_level.txt
-drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-06-01 20:53:33.313621 python_oxmsg-0.0.1/tests/
--rw-r--r--   0 scanny     (501) staff       (20)     2008 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/tests/test_attachment.py
--rw-r--r--   0 scanny     (501) staff       (20)     5350 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/tests/test_message.py
--rw-r--r--   0 scanny     (501) staff       (20)     8813 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/tests/test_properties.py
--rw-r--r--   0 scanny     (501) staff       (20)     1186 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/tests/test_recipient.py
--rw-r--r--   0 scanny     (501) staff       (20)     4476 2024-06-01 20:31:06.000000 python_oxmsg-0.0.1/tests/test_storage.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-30 05:20:51.935888 python_oxmsg-0.0.1a0/
+-rw-r--r--   0 scanny     (501) staff       (20)     1104 2024-05-26 03:34:49.000000 python_oxmsg-0.0.1a0/LICENSE.txt
+-rw-r--r--   0 scanny     (501) staff       (20)     2614 2024-05-30 05:20:51.935711 python_oxmsg-0.0.1a0/PKG-INFO
+-rw-r--r--   0 scanny     (501) staff       (20)     1273 2024-05-26 00:38:16.000000 python_oxmsg-0.0.1a0/README.md
+-rw-r--r--   0 scanny     (501) staff       (20)     3508 2024-05-28 07:47:23.000000 python_oxmsg-0.0.1a0/pyproject.toml
+-rw-r--r--   0 scanny     (501) staff       (20)       38 2024-05-30 05:20:51.935930 python_oxmsg-0.0.1a0/setup.cfg
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-30 05:20:51.931892 python_oxmsg-0.0.1a0/src/
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-30 05:20:51.933520 python_oxmsg-0.0.1a0/src/oxmsg/
+-rw-r--r--   0 scanny     (501) staff       (20)      108 2024-05-28 22:00:52.000000 python_oxmsg-0.0.1a0/src/oxmsg/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     3132 2024-05-30 00:37:58.000000 python_oxmsg-0.0.1a0/src/oxmsg/attachment.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-30 05:20:51.934321 python_oxmsg-0.0.1a0/src/oxmsg/domain/
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2024-05-28 07:47:23.000000 python_oxmsg-0.0.1a0/src/oxmsg/domain/__init__.py
+-rw-r--r--   0 scanny     (501) staff       (20)     7011 2024-05-30 02:13:00.000000 python_oxmsg-0.0.1a0/src/oxmsg/domain/constants.py
+-rw-r--r--   0 scanny     (501) staff       (20)     9960 2024-05-28 07:47:23.000000 python_oxmsg-0.0.1a0/src/oxmsg/domain/encodings.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5253 2024-05-30 00:41:10.000000 python_oxmsg-0.0.1a0/src/oxmsg/domain/model.py
+-rw-r--r--   0 scanny     (501) staff       (20)    28548 2024-05-30 02:13:41.000000 python_oxmsg-0.0.1a0/src/oxmsg/domain/reference.py
+-rw-r--r--   0 scanny     (501) staff       (20)     8147 2024-05-30 02:40:58.000000 python_oxmsg-0.0.1a0/src/oxmsg/message.py
+-rw-r--r--   0 scanny     (501) staff       (20)    15857 2024-05-29 07:34:56.000000 python_oxmsg-0.0.1a0/src/oxmsg/properties.py
+-rw-r--r--   0 scanny     (501) staff       (20)        0 2024-05-29 05:03:00.000000 python_oxmsg-0.0.1a0/src/oxmsg/py.typed
+-rw-r--r--   0 scanny     (501) staff       (20)     1933 2024-05-30 02:35:29.000000 python_oxmsg-0.0.1a0/src/oxmsg/recipient.py
+-rw-r--r--   0 scanny     (501) staff       (20)     4341 2024-05-30 00:35:27.000000 python_oxmsg-0.0.1a0/src/oxmsg/storage.py
+-rw-r--r--   0 scanny     (501) staff       (20)     5569 2024-05-28 07:47:23.000000 python_oxmsg-0.0.1a0/src/oxmsg/util.py
+drwxr-xr-x   0 scanny     (501) staff       (20)        0 2024-05-30 05:20:51.935504 python_oxmsg-0.0.1a0/src/python_oxmsg.egg-info/
+-rw-r--r--   0 scanny     (501) staff       (20)     2614 2024-05-30 05:20:51.000000 python_oxmsg-0.0.1a0/src/python_oxmsg.egg-info/PKG-INFO
+-rw-r--r--   0 scanny     (501) staff       (20)      552 2024-05-30 05:20:51.000000 python_oxmsg-0.0.1a0/src/python_oxmsg.egg-info/SOURCES.txt
+-rw-r--r--   0 scanny     (501) staff       (20)        1 2024-05-30 05:20:51.000000 python_oxmsg-0.0.1a0/src/python_oxmsg.egg-info/dependency_links.txt
+-rw-r--r--   0 scanny     (501) staff       (20)       33 2024-05-30 05:20:51.000000 python_oxmsg-0.0.1a0/src/python_oxmsg.egg-info/requires.txt
+-rw-r--r--   0 scanny     (501) staff       (20)        6 2024-05-30 05:20:51.000000 python_oxmsg-0.0.1a0/src/python_oxmsg.egg-info/top_level.txt
```

### Comparing `python_oxmsg-0.0.1/LICENSE.txt` & `python_oxmsg-0.0.1a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `python_oxmsg-0.0.1/pyproject.toml` & `python_oxmsg-0.0.1a0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -19,43 +19,34 @@
     "Programming Language :: Python :: 3.12",
     "Topic :: Communications :: Email",
     "Topic :: File Formats",
     "Topic :: Office/Business :: Office Suites",
     "Topic :: Software Development :: Libraries",
 ]
 dependencies = [
-    "click",
     "olefile",
     "typing_extensions>=4.9.0",
 ]
 description = "Extract attachments from Outlook .msg files."
 dynamic = ["version"]
 keywords = ["ms-oxmsg", "outlook", "email"]
 license = { text = "MIT" }
 readme = "README.md"
 requires-python = ">=3.9"
 
-[project.scripts]
-oxmsg = "oxmsg.cli:oxmsg"
-
 [project.urls]
 Changelog = "https://github.com/scanny/python-oxmsg/blob/master/CHANGELOG.md"
 Documentation = "https://scanny.github.io/python-oxmsg/"
 Homepage = "https://github.com/scanny/python-oxmsg"
 Repository = "https://github.com/scanny/python-oxmsg"
 
 [tool.black]
 line-length = 100
 target-version = ["py39", "py310", "py311", "py312"]
 
-[tool.coverage.run]
-omit = [
-    "*/domain/model.py"
-]
-
 [tool.pyright]
 include = ["src/oxmsg", "tests"]
 pythonPlatform = "All"
 pythonVersion = "3.9"
 reportImportCycles = true
 reportUnnecessaryCast = true
 reportUnnecessaryTypeIgnoreComment = true
```

### Comparing `python_oxmsg-0.0.1/src/oxmsg/attachment.py` & `python_oxmsg-0.0.1a0/src/oxmsg/attachment.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,13 @@
-"""Provides access to the properties of an attachment in an Outlook MSG file.
-
-These properies include the attached file's original file-name, its last-modified date, size, and
-content-type (MIME-type).
-
-```python
->>> from oxmsg import Message
-
->>> msg = Message.load("message.msg")
->>> msg.attachment_count
-1
->>> attachment = msg.attachments[0]
->>> attachment.file_name
-'financial-forecast.xlsx'
->>> with open(attachment.file_name, "wb") as f:
-...     f.write()
-```
-"""
+"""The interface object for an attachment in an Outlook MSG file."""
 
 from __future__ import annotations
 
 import datetime as dt
+from typing import Iterator
 
 from oxmsg.domain import constants as c
 from oxmsg.domain import model as m
 from oxmsg.properties import Properties
 from oxmsg.util import lazyproperty
 
 
@@ -31,42 +15,64 @@
     """A file attached to an Outlook email message."""
 
     def __init__(self, storage: m.StorageT):
         self._storage = storage
 
     @lazyproperty
     def attached_by_value(self) -> bool:
-        """True when the `PidTagAttachDataBinary` property contains the attachment data.
+        """The PidTagAttachDataBinary property contains the attachment data.
 
         This is as opposed to "by-reference" where only a path or URL is stored.
         """
         attach_method = self.properties.int_prop_value(c.PID_ATTACH_METHOD)
         assert attach_method is not None
         return bool(attach_method & m.AF_BY_VALUE)
 
+    def dump_properties(self) -> str:
+        """Report of message properies suitable for writing to the console."""
+
+        def iter_lines() -> Iterator[str]:
+            yield ""
+            yield "---------------------"
+            yield "Attachment Properties"
+            yield "---------------------"
+            yield ""
+            yield "distinguished-properties"
+            yield "------------------------"
+            yield f"filename:          {self.filename}"
+            yield f"MIME-type:         {self.mime_type}"
+            yield f"size:              {self.size:,}"
+            yield f"attached-by-value: {self.attached_by_value}"
+            yield f"last-modified:     {self.last_modified}"
+            yield ""
+            yield "other properties"
+            yield self.properties.dump()
+
+        return "\n".join(iter_lines())
+
     @lazyproperty
     def file_bytes(self) -> bytes | None:
         """The attachment binary, suitable for saving to a file when detaching."""
         return self.properties.binary_prop_value(c.PID_ATTACH_DATA_BINARY)
 
     @lazyproperty
-    def file_name(self) -> str | None:
+    def filename(self) -> str | None:
         """The full name of this file as it was originally attached.
 
         Like "FY24-quarterly-projections.xlsx". Does not include a path.
         """
         return self.properties.str_prop_value(c.PID_ATTACH_LONG_FILENAME)
 
     @lazyproperty
     def last_modified(self) -> dt.datetime | None:
         """Timezone-aware UTC datetime when this attachment was last modified.
 
         `None` if this property is not present on the attachment.
         """
-        return self.properties.date_prop_value(c.PID_LAST_MODIFICATION_TIME)
+        self.properties.date_prop_value(c.PID_LAST_MODIFICATION_TIME)
 
     @lazyproperty
     def mime_type(self) -> str | None:
         """ISO 8601 str representation of time this attachment was last modified."""
         return self.properties.str_prop_value(c.PID_ATTACH_MIME_TAG) or "application/octet-stream"
 
     @lazyproperty
```

### Comparing `python_oxmsg-0.0.1/src/oxmsg/domain/constants.py` & `python_oxmsg-0.0.1a0/src/oxmsg/domain/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,14 @@
 PID_ATTACH_RENDERING = 0x3709
 PID_ATTACH_RENDERING_POSITION = 0x370B
 PID_ATTACH_SIZE = 0x0E20
 PID_AUTHORIZING_USERS = 0x0003
 PID_AUTO_FORWARDED = 0x0005
 PID_AUTO_FORWARD_COMMENT = 0x0004
 PID_BODY = 0x1000
-PID_BODY_HTML = 0x1013
 PID_CHANGE_KEY = 0x65E2
 PID_CLIENT_SUBMIT_TIME = 0x0039
 PID_CONTENT_CONFIDENTIALITY_ALGORITHM_ID = 0x0006
 PID_CONTENT_CORRELATOR = 0x0007
 PID_CONTENT_IDENTIFIER = 0x0008
 PID_CONTENT_LENGTH = 0x0009
 PID_CONTENT_RETURN_REQUESTED = 0x000A
```

### Comparing `python_oxmsg-0.0.1/src/oxmsg/domain/encodings.py` & `python_oxmsg-0.0.1a0/src/oxmsg/domain/encodings.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,20 +20,20 @@
       codepage.
     - Raises `UnsupportedEncodingError` when `codepage` is recognized but Python has no builtin
       codec for that encoding.
     """
     encoding = _CODE_PAGE_ENCODINGS.get(codepage)
 
     if encoding is None:
-        raise m.UnrecognizedCodePageError(  # pragma: no cover
+        raise m.UnrecognizedCodePageError(
             "the code-page specified in this message is not a known Microsoft character encoding"
         )
 
     if encoding == "":
-        raise m.UnsupportedEncodingError(  # pragma: no cover
+        raise m.UnsupportedEncodingError(
             "the character-encoding used in this message is not supported by Python"
         )
 
     return encoding
 
 
 _CODE_PAGE_ENCODINGS = {
```

### Comparing `python_oxmsg-0.0.1/src/oxmsg/domain/model.py` & `python_oxmsg-0.0.1a0/src/oxmsg/domain/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,49 +45,45 @@
         """The bytes of the stream for variable-length property identified by `pid`."""
         ...
 
 
 class PropertyT(Protocol):
     """The interface required of a property object, regardless of its type."""
 
-    @property
+    @lazyproperty
     def name(self) -> str:
         """The Microsft name for this property, like "PidTagMessageClass"."""
         ...
 
-    @property
+    @lazyproperty
     def pid(self) -> int:
         """The property-id (PID) for this property, like 0x3701 for attachment bytes."""
         ...
 
-    @property
+    @lazyproperty
     def ptyp(self) -> int:
         """The property-type (PTYP) for this property, like 0x0102 for PtypBinary."""
         ...
 
-    @property
+    @lazyproperty
     def ptyp_name(self) -> str:
         """The Microsft name for the type of this property, like "PtypString"."""
         ...
 
     @lazyproperty
     def value(self) -> bool | bytes | dt.datetime | float | int | str | uuid.UUID:
         """The value of this property, its type depending on the property."""
         ...
 
 
 class StorageT(Protocol):
     """Interface for a storage object."""
 
     def iter_attachment_storages(self) -> Iterator[StorageT]:
-        """Generate each storage object specific to an attachment to this message."""
-        ...
-
-    def iter_recipient_storages(self) -> Iterator[StorageT]:
-        """Generate each storage object specific to a recipient of this message."""
+        """Generate storage object specific to each attachment in this message."""
         ...
 
     @lazyproperty
     def name(self) -> str:
         """The last segment of the storage path.
 
         This is the empty string for the root storage. Other storages are named is clearly specified
```

### Comparing `python_oxmsg-0.0.1/src/oxmsg/domain/reference.py` & `python_oxmsg-0.0.1a0/src/oxmsg/domain/reference.py`

 * *Files identical despite different names*

### Comparing `python_oxmsg-0.0.1/src/oxmsg/message.py` & `python_oxmsg-0.0.1a0/src/oxmsg/message.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,25 @@
-"""The `Message` object is the primary interface object in `python-oxmsg`.
-
-This object is returned by the `Message.load()` classmethod:
-
-```python
->>> from oxmsg import Message
-
->>> msg = Message.load("message.msg")
->>> msg.subject
-'Agenda for the Acme meeting'
-```
-"""
+"""The main interface object for an Outlook MSG file."""
 
 from __future__ import annotations
 
 import datetime as dt
 import email.message
 import email.parser
+import json
 import os
 import struct
 from typing import IO, Iterator
 
 from olefile import OleFileIO, isOleFile
 
 from oxmsg.attachment import Attachment
 from oxmsg.domain import constants as c
 from oxmsg.domain import model as m
+from oxmsg.domain.encodings import encoding_from_codepage
 from oxmsg.properties import Properties
 from oxmsg.recipient import Recipient
 from oxmsg.storage import Storage
 from oxmsg.util import lazyproperty
 
 
 class Message:
@@ -54,65 +45,98 @@
         with OleFileIO(msg_file) as ole:
             root_storage = Storage.from_ole(ole)
 
         self = cls(root_storage)
         self._validate()
         return self
 
-    @property
+    @lazyproperty
     def attachment_count(self) -> int:
         """Number of attachments on this message."""
         return self._header_prop_values[3]
 
-    @property
+    @lazyproperty
     def attachments(self) -> tuple[Attachment, ...]:
         """Attachment object for each attachment in this message."""
         return tuple(self._iter_attachments())
 
-    @property
+    @lazyproperty
     def body(self) -> str | None:
-        """The plain-text body of this message; `None` if not present."""
+        """True if this message includes a non-empty HTML body property."""
         return self.properties.str_prop_value(c.PID_BODY)
 
-    @property
+    def dump_properties(self) -> str:
+        """A summary of this MS-OXMSG object's top-level properties."""
+        string_props_are_unicode = (
+            self.properties._string_props_are_unicode  # pyright: ignore[reportPrivateUsage]
+        )
+        str_prop_encoding = (
+            self.properties._str_prop_encoding  # pyright: ignore[reportPrivateUsage]
+        )
+
+        internet_code_page = self.properties.int_prop_value(0x3FDE)
+        internet_encoding = (
+            None if internet_code_page is None else encoding_from_codepage(internet_code_page)
+        )
+
+        def iter_lines() -> Iterator[str]:
+            yield "header-properties"
+            yield "-----------------"
+            yield f"next_recipient_id: {self._header_prop_values[0]}"
+            yield f"next_attachment_id: {self._header_prop_values[1]}"
+            yield f"recipient_count: {self._header_prop_values[2]}"
+            yield f"attachment_count: {self._header_prop_values[3]}"
+            yield ""
+            yield "distinguished-properties"
+            yield "------------------------"
+            yield f"string_props_are_unicode: {string_props_are_unicode}"
+            if not string_props_are_unicode:
+                yield f"string_props_encoding:    {str_prop_encoding}"
+            yield f"internet_code_page:       {internet_encoding}"
+            yield f"subject:                  {repr(self.subject)}"
+            yield f"message_headers: {json.dumps(self.message_headers, indent=4, sort_keys=True)}"
+            yield ""
+            yield "other properties"
+            yield self.properties.dump()
+
+        return "\n".join(iter_lines())
+
+    @lazyproperty
     def html_body(self) -> str | None:
-        """The HTML body of this message if present, `None` otherwise."""
-        # -- body HTML most commonly (these days) is bytes encoded with internet-codepage --
-        if html_bytes := self.properties.binary_prop_value(c.PID_HTML):
-            return html_bytes.decode(self.properties.body_encoding)
-        # -- however older emails may encode the HTML as Unicode or an 8-bit string --
-        if html_str := self.properties.str_prop_value(c.PID_BODY_HTML):
-            return html_str
-        return None
+        """The HTML body of this message if it has it, `None` otherwise."""
+        html_bytes = self.properties.binary_prop_value(c.PID_HTML)
+        if html_bytes is None:
+            return None
+        return html_bytes.decode(self.properties.body_encoding)
 
-    @property
+    @lazyproperty
     def message_headers(self) -> dict[str, str]:
         """From, To, Content-Type, etc. headers for this message as {name: value} mapping."""
         return dict(self._message_headers)
 
-    @property
+    @lazyproperty
     def message_class(self) -> str:
         """Outlook Message Class identifier like "IPM.Note" for this message."""
-        return self.properties.str_prop_value(c.PID_MESSAGE_CLASS) or ""
+        return self.properties.str_prop_value(c.PID_MESSAGE_CLASS) or "Unknown"
 
-    @property
+    @lazyproperty
     def properties(self) -> Properties:
         """Provides access to the properties of this OXMSG object."""
-        return self._properties
+        return Properties(self._storage, properties_header_offset=m.MSG_HDR_OFFSET)
 
-    @property
+    @lazyproperty
     def recipients(self) -> tuple[Recipient, ...]:
         """`Recipient` object for each recipient of this message."""
         return tuple(self._iter_recipients())
 
-    @property
+    @lazyproperty
     def sender(self) -> str | None:
         """Name and email address of the message sender.
 
-        Like '"John Doe" <john@bigisp.com>'.
+        Like '"Steve Canny" <stcanny@oxmsg.io>'.
 
         None if it is not recorded in the message. This may occur when the message is a draft or
         system-generated or perhaps in other cases.
 
         Note that the value of the From: message header is returned when present (usually I expect)
         and may contain multiple addresses separated by commas.
         """
@@ -124,23 +148,23 @@
         raw_name = (props.str_prop_value(c.PID_SENDER_NAME) or "").strip()
         name = f'"{raw_name}" ' if raw_name else ""
         email = props.str_prop_value(c.PID_SENDER_EMAIL_ADDRESS) or props.str_prop_value(
             c.PID_SENDER_SMTP_ADDRESS
         )
         return f"{name}<{email}>" if email else props.str_prop_value(c.PID_SENT_REPRESENTING_NAME)
 
-    @property
+    @lazyproperty
     def sent_date(self) -> dt.datetime | None:
         """When this message was submitted by the sender.
 
         This value will be `None` if the message has not been sent and possibly in other cases.
         """
         return self.properties.date_prop_value(c.PID_CLIENT_SUBMIT_TIME)
 
-    @property
+    @lazyproperty
     def subject(self) -> str:
         """Subject line of this message."""
         return self.properties.str_prop_value(c.PID_SUBJECT) or ""
 
     @lazyproperty
     def _header_prop_values(self) -> tuple[int, int, int, int]:
         """The property values in the MSG-root properties header.
@@ -173,16 +197,12 @@
 
         This provides case-insensitive access along with some other convenient behaviors not
         available from a `dict`.
         """
         headers = self.properties.str_prop_value(c.PID_TRANSPORT_MESSAGE_HEADERS) or ""
         return email.parser.HeaderParser().parsestr(headers)
 
-    @lazyproperty
-    def _properties(self) -> Properties:
-        return Properties(self._storage, properties_header_offset=m.MSG_HDR_OFFSET)
-
     def _validate(self) -> None:
         """Raise if this message is invalid for one of a variety of possible reasons."""
         # -- for now, we only process email messages --
         # if not self.message_class.startswith("IPM.Note"):
         #     raise ValueError(f"{self.message_class} files not supported")
```

### Comparing `python_oxmsg-0.0.1/src/oxmsg/properties.py` & `python_oxmsg-0.0.1a0/src/oxmsg/properties.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,16 @@
-"""Provides access to all properties of a top-level object (message, recipient, attachment).
-
-This object is accessed using the `.properties` property of a top-level object. The properties for
-each top-level object are segregated into its own properties object.
-
-Many property-ids (PIDs) and property-types (PTYPs) are available as constants in
-`oxml.domain.contants`.
-
-```python
->>> from oxmsg import Message
->>> from oxmsg.domain import constants as c
-
->>> msg = Message.load("message.msg")
->>> properties = msg.properties
->>> properties.str_prop_value(c.PID_MESSAGE_CLASS).value
-'IPM.Note'
-```
-"""
+"""Provides `Properties` object that encapsulates property retrieval from OXMSG format."""
 
 from __future__ import annotations
 
 import datetime as dt
 import itertools
 import struct
 import types
 import uuid
-from collections import defaultdict
 from typing import Final, Iterator, cast
 
 from oxmsg.domain import constants as c
 from oxmsg.domain import encodings
 from oxmsg.domain import model as m
 from oxmsg.domain import reference as ref
 from oxmsg.util import lazyproperty
@@ -47,15 +29,15 @@
         return iter(self._property_sequence)
 
     def binary_prop_value(self, pid: int) -> bytes | None:
         """Retrieve bytes of PtypBinary property identified by `pid`.
 
         Returns `None` if property is not present in this collection.
         """
-        property = self._get_property(pid, c.PTYP_BINARY)
+        property = self._properties_mapping.get(pid)
 
         if property is None:
             return None
 
         return cast(BinaryProperty, property).value
 
     @lazyproperty
@@ -83,76 +65,82 @@
         property = self._properties_mapping.get(pid)
 
         if property is None:
             return None
 
         return cast(TimeProperty, property).value
 
+    def dump(self) -> str:
+        """A summary of these properties suitable for printing to the console."""
+
+        def iter_lines() -> Iterator[str]:
+            head_rule = f"{'-'*53}+{'-'*23}+{'-'*70}"
+            yield head_rule
+            yield "property-id" + " " * 42 + "| type" + " " * 18 + "| value"
+            yield head_rule
+
+            for p in self:
+                value = p.value
+                if p.ptyp in (c.PTYP_STRING, c.PTYP_STRING8):
+                    value = cast(str, self.str_prop_value(p.pid))
+                    value = repr(value)[:64] + "..." if len(value) > 64 else repr(value)
+                elif p.ptyp == c.PTYP_BINARY and p.pid == c.PID_HTML:
+                    assert isinstance(value, bytes)
+                    value = value[:64]
+                elif isinstance(value, bytes):
+                    value = f"{len(value):,} bytes"
+                elif p.ptyp == c.PTYP_INTEGER_32:
+                    assert isinstance(value, int)
+                    b0 = value & 0xFF
+                    b1 = (value & 0xFF00) >> 8
+                    b2 = (value & 0xFF0000) >> 16
+                    b3 = (value & 0xFF000000) >> 24
+                    value = f"{b3:02X} {b2:02X} {b1:02X} {b0:02X}"
+
+                yield f"0x{p.pid:04X} - {p.name:<43} | {p.ptyp_name:<21} | {value}"
+
+        return "\n".join(iter_lines())
+
     def int_prop_value(self, pid: int) -> int | None:
         """Retrieve int value of PtypInteger32 property identified by `pid`.
 
         Returns `None` if no `pid` property is present in this collection.
         """
         property = self._properties_mapping.get(pid)
 
         if property is None:
             return None
 
         return cast(Int32Property, property).value
 
     def str_prop_value(self, pid: int) -> str | None:
-        """Retrieve str value of PtypString or PtypString8 property identified by `pid`.
+        """Retrieve str value of PtypString property identified by `pid`.
 
         Returns the empty str if property is not present in this collection.
         """
-        property = self._get_property(pid, (c.PTYP_STRING, c.PTYP_STRING8))
+        property = self._properties_mapping.get(pid)
 
         if property is None:
             return None
 
         return cast(StringProperty, property).value
 
-    @lazyproperty
-    def string_props_are_unicode(self) -> bool:  # pragma: no cover
-        """True indicates PtypString properties in this message are encoded "utf-16-le"."""
-        store_support_mask = self.int_prop_value(c.PID_STORE_SUPPORT_MASK)
-
-        if store_support_mask is None:
-            return False
-
-        return bool(store_support_mask & m.STORE_UNICODE_OK)
-
     def _cherry_pick_int_prop(self, pid: int) -> Int32Property | None:
         """Get an Int32 property without triggering broader property load.
 
         Used to solve chicken-and-egg problem of determining encoding required by string
         properties before atomically loading all properties.
         """
         PID = struct.Struct("<2xH")
         for segment in self._prop_segment_sequence:
             pid_ = PID.unpack(segment[:4])[0]
             if pid_ == pid:
                 return Int32Property(segment)
         return None
 
-    def _get_property(self, pid: int, ptyps: int | tuple[int, ...]) -> m.PropertyT | None:
-        """Retrieve the first property with `pid` and one of `ptyps`.
-
-        The general expectation is that at most one property with `pid` and one of `ptyps` will be
-        present in the collection. In the unusual case there could be more than one this method
-        may need to be called once for each possible type to get them all or in a particular order
-        of preference.
-        """
-        acceptable_ptyps = (ptyps,) if isinstance(ptyps, int) else ptyps
-        candidate_props = self._properties_by_pid[pid]
-        for p in candidate_props:
-            if p.ptyp in acceptable_ptyps:
-                return p
-        return None
-
     @lazyproperty
     def _str_prop_encoding(self) -> str:
         """The encoding used for non-body properties of PtypString8.
 
         Must be cherry-picked because it is required before constructing the properties collection.
 
         Note when PtypString properties are unconditionally encoded with UTF-16LE.
@@ -163,63 +151,66 @@
         if message_codepage is not None:
             return encodings.encoding_from_codepage(message_codepage.value)
 
         # - Case 2: not specified one way or another, default to "iso-8859-15" (Latin 9) --
         return "iso-8859-15"
 
     @lazyproperty
+    def _message_codepage(self) -> int | None:
+        """16-byte segments comprising property blocks from the attachment properties stream."""
+        message_codepage = self.int_prop_value(c.PID_MESSAGE_CODEPAGE)
+        return message_codepage if message_codepage else None
+
+    @lazyproperty
     def _prop_segment_sequence(self) -> tuple[bytes, ...]:
         """16-byte segments comprising property blocks from the attachment properties stream."""
         return tuple(
             segment
             for segment in _batched_bytes(
                 self._storage.properties_stream_bytes[self._properties_header_offset :], 16
             )
             # -- drop any trailing short segment, happens sometimes --
             if len(segment) == 16
         )
 
     @lazyproperty
-    def _properties_by_pid(self) -> defaultdict[int, list[m.PropertyT]]:
-        """Properties in this collection grouped by property-id (PID).
-
-        Not sure if this solves an actual problem in practice, but it's at least
-        theoretically possible that the same PID could appear twice in a property collection
-        with different PTYPs.
-        """
-        properties_by_pid: defaultdict[int, list[m.PropertyT]] = defaultdict(list)
-        for p in self._property_sequence:
-            properties_by_pid[p.pid].append(p)
-        return properties_by_pid
-
-    @lazyproperty
     def _properties_mapping(self) -> types.MappingProxyType[int, m.PropertyT]:
         """The property objects in this collection keyed by pid."""
         return types.MappingProxyType({p.pid: p for p in self._property_sequence})
 
     @lazyproperty
     def _property_sequence(self) -> tuple[m.PropertyT, ...]:
         """Property object for each property in this collection.
 
         Properties are in property-id (PID) order.
         """
         PID = struct.Struct("<2xH")
         segments = sorted(self._prop_segment_sequence, key=lambda x: PID.unpack(x[:4])[0])
         return tuple(
-            BaseProperty.factory(
+            _BaseProperty.factory(
                 segment=segment,
                 storage=self._storage,
                 str_prop_encoding=self._str_prop_encoding,
                 body_encoding=self.body_encoding,
             )
             for segment in segments
         )
 
+    @lazyproperty
+    def _string_props_are_unicode(self) -> bool:
+        """True indicates PtypString properties in this message are encoded "utf-16-le"."""
+        store_support_mask = self.int_prop_value(c.PID_STORE_SUPPORT_MASK)
+
+        if store_support_mask is None:
+            return False
+
+        return bool(store_support_mask & m.STORE_UNICODE_OK)
+
 
-class BaseProperty:
+class _BaseProperty:
     """Base class for properties, providing common behaviors."""
 
     PID: Final[struct.Struct] = struct.Struct("<2xH")
     PTYP: Final[struct.Struct] = struct.Struct("<H")
 
     def __init__(self, segment: bytes):
         self._segment = segment
@@ -264,80 +255,87 @@
             return TimeProperty(segment)
 
         # -- default to Int32 --
         print(f"{len(segment)=}")
         print(f"{repr(segment)=}")
         return Int32Property(segment)
 
-    @property
+        # prop_type_desc = m.property_type_descriptors.get(ptyp)
+        # prop_type_name = prop_type_desc.ms_name if prop_type_desc else f"ptyp:{ptyp:04X}"
+        # pid = cls.PID.unpack(segment[:4])[0]
+        # raise NotImplementedError(
+        #     f"no property sub-type available for property {pid:04X}, type {prop_type_name}"
+        # )
+
+    @lazyproperty
     def name(self) -> str:
         """The Microsft name for this property, like "PidTagMessageClass"."""
         prop_desc = ref.property_descriptors.get(self.pid)
         return prop_desc.ms_name if prop_desc is not None else "not recorded in model"
 
-    @property
+    @lazyproperty
     def pid(self) -> int:
         """The property-id (PID) for this property, like 0x3701 for attachment bytes."""
         return self.PID.unpack(self._segment[:4])[0]
 
-    @property
+    @lazyproperty
     def ptyp(self) -> int:
         """The property-type (PTYP) for this property, like 0x0102 for PtypBinary."""
         return self.PTYP.unpack(self._segment[:2])[0]
 
-    @property
+    @lazyproperty
     def ptyp_name(self) -> str:
         """The Microsft name for the type of this property, like "PtypString"."""
         prop_type_desc = ref.property_type_descriptors.get(self.ptyp)
         return (
             prop_type_desc.ms_name if prop_type_desc else f"{self.ptyp:04X} not recorded in model"
         )
 
     @lazyproperty
     def _payload(self) -> bytes:
         """The latter 8 bytes of the property segment, where the property value is stored."""
         return self._segment[8:]
 
 
-class BinaryProperty(BaseProperty):
+class BinaryProperty(_BaseProperty):
     """Property for PtypBinary OLE properties."""
 
     def __init__(self, segment: bytes, storage: m.PropStorageT):
         super().__init__(segment)
         self._storage = storage
 
     @lazyproperty
     def value(self) -> bytes:
         """The bytes of this binary property."""
         return self._storage.property_stream_bytes(self.pid, self.ptyp)
 
 
-class BooleanProperty(BaseProperty):
+class BooleanProperty(_BaseProperty):
     """Property for PtypBoolean OLE properties."""
 
-    SIGNED_CHAR: Final[struct.Struct] = struct.Struct("<b")
+    BOOL: Final[struct.Struct] = struct.Struct("?")
 
     @lazyproperty
     def value(self) -> bool:
-        """The boolean value of this property."""
-        return self.SIGNED_CHAR.unpack(self._payload[:1])[0] != 0
+        """The integer value of this property."""
+        return self.BOOL.unpack(self._payload[:1])[0]
 
 
-class Float64Property(BaseProperty):
+class Float64Property(_BaseProperty):
     """Property for PtypFloating64 OLE properties."""
 
     FLOAT64: Final[struct.Struct] = struct.Struct("<d")
 
     @lazyproperty
     def value(self) -> float:
         """The 64-bit floating-point value of this property."""
         return self.FLOAT64.unpack(self._payload)[0]
 
 
-class GuidProperty(BaseProperty):
+class GuidProperty(_BaseProperty):
     """Property for PtypGuid OLE properties."""
 
     GUID: Final[struct.Struct] = struct.Struct("<IHH8s")
 
     def __init__(self, segment: bytes, storage: m.PropStorageT):
         super().__init__(segment)
         self._storage = storage
@@ -354,50 +352,50 @@
         '9d947746-9662-40a8-a526-abd4faec9737'.
         """
         # -- In the OXMSG format, a GUID (aka. UUID) is stored as four distinct fields, each in
         # -- little-endian form. Luckily Python's uuid built-in can parse this directly.
         return uuid.UUID(bytes_le=self._storage.property_stream_bytes(self.pid, self.ptyp)[:16])
 
 
-class Int16Property(BaseProperty):
+class Int16Property(_BaseProperty):
     """Property for PtypInteger16 OLE properties."""
 
     INT16: Final[struct.Struct] = struct.Struct("<H")
 
     @lazyproperty
     def value(self) -> int:
         """The integer value of this property."""
         return self.INT16.unpack(self._payload[:2])[0]
 
 
-class Int32Property(BaseProperty):
+class Int32Property(_BaseProperty):
     """Property for PtypInteger32 OLE properties."""
 
     INT32: Final[struct.Struct] = struct.Struct("<I")
 
     @lazyproperty
     def value(self) -> int:
         """The integer value of this property."""
         return self.INT32.unpack(self._payload[:4])[0]
 
 
-class StringProperty(BaseProperty):
+class StringProperty(_BaseProperty):
     """Property for PtypString OLE properties."""
 
     def __init__(self, segment: bytes, storage: m.PropStorageT):
         super().__init__(segment)
         self._storage = storage
 
     @lazyproperty
     def value(self) -> str:
         """The decoded str from this string property."""
         return self._storage.property_stream_bytes(self.pid, self.ptyp).decode("utf-16-le")
 
 
-class String8Property(BaseProperty):
+class String8Property(_BaseProperty):
     """Property for PtypString8 (8-bit characters, not Unicode) OLE properties."""
 
     def __init__(
         self, segment: bytes, storage: m.PropStorageT, str_prop_encoding: str, body_encoding: str
     ):
         super().__init__(segment)
         self._storage = storage
@@ -411,15 +409,15 @@
         The caller is responsible for determining the encoding and applying it to get a str value.
         """
         return self._storage.property_stream_bytes(self.pid, self.ptyp).decode(
             self._body_encoding if self.pid == c.PID_BODY else self._str_prop_encoding
         )
 
 
-class TimeProperty(BaseProperty):
+class TimeProperty(_BaseProperty):
     """Property for PtypTime OLE properties."""
 
     TIME: Final[struct.Struct] = struct.Struct("<Q")
 
     @lazyproperty
     def value(self) -> dt.datetime:
         """The value of this property as a timezone-aware `datetime`."""
@@ -430,12 +428,12 @@
 
 
 def _batched_bytes(block: bytes, n: int) -> Iterator[bytes]:
     """Batch bytes from `block` into segments of `n` bytes each.
 
     Last batch is shorter than `n` when `block` is not evenly divisible by `n`.
     """
-    if n < 1:  # pragma: no cover
+    if n < 1:
         raise ValueError("n must be at least one")
     iter_bytes = iter(block)
     while batch := bytes(itertools.islice(iter_bytes, n)):
         yield batch
```

### Comparing `python_oxmsg-0.0.1/src/oxmsg/storage.py` & `python_oxmsg-0.0.1a0/src/oxmsg/storage.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -61,20 +61,14 @@
 
     def iter_attachment_storages(self) -> Iterator[Storage]:
         """Generate storage object specific to each attachment in this message."""
         for s in self.storages:
             if s.name.startswith("__attach_version1.0_#"):
                 yield s
 
-    def iter_recipient_storages(self) -> Iterator[Storage]:
-        """Generate storage object specific to each recipent in this message."""
-        for s in self.storages:
-            if s.name.startswith("__recip_version1.0_#"):
-                yield s
-
     @lazyproperty
     def name(self) -> str:
         """The "directory-name" of this storage, with no path-prefix."""
         return self.path.split("/")[-1]
 
     @lazyproperty
     def properties_stream_bytes(self) -> bytes:
@@ -85,14 +79,20 @@
     def property_stream_bytes(self, pid: int, ptyp: int) -> bytes:
         """Read variable-length property bytes from the stream it's stored in."""
         # -- This method should not be called unless there is an entry for this property in the
         # -- properties stream. If the property exists but its stream does not, that's an
         # -- exception, not an expected occurence.
         return self._streams_by_name[f"__substg1.0_{pid:04X}{ptyp:04X}"].bytes_
 
+    def iter_recipient_storages(self) -> Iterator[Storage]:
+        """Generate storage object specific to each recipent in this message."""
+        for s in self.storages:
+            if s.name.startswith("__recip_version1.0_#"):
+                yield s
+
     @lazyproperty
     def _streams_by_name(self) -> Mapping[str, Stream]:
         """dict semantics on streams of this storage."""
         return {s.name: s for s in self.streams}
 
 
 @dc.dataclass
```

### Comparing `python_oxmsg-0.0.1/src/oxmsg/util.py` & `python_oxmsg-0.0.1a0/src/oxmsg/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,29 +77,29 @@
         the class, e.g. `Obj.fget`.
 
         *type* is the class hosting the decorated getter method (`fget`) on both class
         and instance attribute access.
         """
         # --- when accessed on class, e.g. Obj.fget, just return this descriptor
         # --- instance (patched above to look like fget).
-        if obj is None:  # pragma: no cover
+        if obj is None:
             return self  # type: ignore
 
         # --- when accessed on instance, start by checking instance __dict__ for
         # --- item with key matching the wrapped function's name
         value = obj.__dict__.get(self._name)
         if value is None:
             # --- on first access, the __dict__ item will be absent. Evaluate fget()
             # --- and store that value in the (otherwise unused) host-object
             # --- __dict__ value of same name ('fget' nominally)
             value = self._fget(obj)
             obj.__dict__[self._name] = value
         return cast(_T, value)
 
-    def __set__(self, obj: Any, value: Any) -> None:  # pragma: no cover
+    def __set__(self, obj: Any, value: Any) -> None:
         """Raises unconditionally, to preserve read-only behavior.
 
         This decorator is intended to implement immutable (and idempotent) object
         attributes. For that reason, assignment to this property must be explicitly
         prevented.
 
         If this __set__ method was not present, this descriptor would become a
```

