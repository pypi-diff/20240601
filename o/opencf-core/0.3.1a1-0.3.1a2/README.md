# Comparing `tmp/opencf_core-0.3.1a1.tar.gz` & `tmp/opencf_core-0.3.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opencf_core-0.3.1a1.tar", max compression
+gzip compressed data, was "opencf_core-0.3.1a2.tar", max compression
```

## Comparing `opencf_core-0.3.1a1.tar` & `opencf_core-0.3.1a2.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     7078 2024-05-08 14:58:19.894394 opencf_core-0.3.1a1/README.md
--rw-r--r--   0        0        0        0 2024-05-08 14:58:19.894394 opencf_core-0.3.1a1/opencf_core/__init__.py
--rw-r--r--   0        0        0    19810 2024-05-28 01:21:54.874612 opencf_core-0.3.1a1/opencf_core/base_converter.py
--rw-r--r--   0        0        0     6372 2024-05-28 01:21:54.842612 opencf_core-0.3.1a1/opencf_core/converter_app.py
--rw-r--r--   0        0        0     1109 2024-05-23 17:46:59.309102 opencf_core-0.3.1a1/opencf_core/exceptions.py
--rw-r--r--   0        0        0    21502 2024-05-28 01:21:54.874612 opencf_core-0.3.1a1/opencf_core/filetypes.py
--rw-r--r--   0        0        0     5891 2024-05-08 14:58:19.894394 opencf_core-0.3.1a1/opencf_core/io_handler.py
--rw-r--r--   0        0        0     3566 2024-05-23 09:27:20.464956 opencf_core-0.3.1a1/opencf_core/logging_config.py
--rw-r--r--   0        0        0     2030 2024-05-23 10:30:58.320136 opencf_core-0.3.1a1/opencf_core/mimes.py
--rw-r--r--   0        0        0      543 2024-05-23 17:46:59.309102 opencf_core-0.3.1a1/opencf_core/utils.py
--rw-r--r--   0        0        0     1128 2024-05-28 01:22:20.078967 opencf_core-0.3.1a1/pyproject.toml
--rw-r--r--   0        0        0     8314 1970-01-01 00:00:00.000000 opencf_core-0.3.1a1/PKG-INFO
+-rw-r--r--   0        0        0     7078 2024-05-28 01:37:09.732547 opencf_core-0.3.1a2/README.md
+-rw-r--r--   0        0        0        0 2024-05-08 14:58:19.894394 opencf_core-0.3.1a2/opencf_core/__init__.py
+-rw-r--r--   0        0        0    19795 2024-05-28 02:16:09.827136 opencf_core-0.3.1a2/opencf_core/base_converter.py
+-rw-r--r--   0        0        0     6372 2024-05-28 01:37:09.732547 opencf_core-0.3.1a2/opencf_core/converter_app.py
+-rw-r--r--   0        0        0     2052 2024-05-28 03:09:31.863769 opencf_core-0.3.1a2/opencf_core/enum.py
+-rw-r--r--   0        0        0     1552 2024-05-28 03:09:31.863769 opencf_core-0.3.1a2/opencf_core/exceptions.py
+-rw-r--r--   0        0        0    19916 2024-05-28 03:09:31.863769 opencf_core-0.3.1a2/opencf_core/filetypes.py
+-rw-r--r--   0        0        0     5891 2024-05-08 14:58:19.894394 opencf_core-0.3.1a2/opencf_core/io_handler.py
+-rw-r--r--   0        0        0     3566 2024-05-23 09:27:20.464956 opencf_core-0.3.1a2/opencf_core/logging_config.py
+-rw-r--r--   0        0        0     2030 2024-05-23 10:30:58.320136 opencf_core-0.3.1a2/opencf_core/mimes.py
+-rw-r--r--   0        0        0      543 2024-05-23 17:46:59.309102 opencf_core-0.3.1a2/opencf_core/utils.py
+-rw-r--r--   0        0        0     1128 2024-05-28 03:11:09.804887 opencf_core-0.3.1a2/pyproject.toml
+-rw-r--r--   0        0        0     8314 1970-01-01 00:00:00.000000 opencf_core-0.3.1a2/PKG-INFO
```

### Comparing `opencf_core-0.3.1a1/README.md` & `opencf_core-0.3.1a2/README.md`

 * *Files identical despite different names*

### Comparing `opencf_core-0.3.1a1/opencf_core/base_converter.py` & `opencf_core-0.3.1a2/opencf_core/base_converter.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 Base Converter Module
 
 This module serves as a foundation for creating file conversion utilities. It facilitates the development
 of file converters through abstract base classes, managing file types, and handling input and output files
 efficiently. The module is designed to be extendible, supporting various file formats and conversion strategies.
 
 Classes:
+
 - ResolvedInputFile: Manages file paths and types, resolving them as needed.
-- BaseConverter: An abstract base class for creating specific file format converters, enforcing the implementation
-                 of file conversion logic.
+- BaseConverter: An abstract base class for creating specific file format converters, enforcing the implementation of file conversion logic.
 
 Exceptions:
+
 - ValueError: Raised when file paths or types are incompatible or unsupported.
 - AssertionError: Ensured for internal consistency checks, confirming that file types match expected values.
 """
 
 from abc import ABC, abstractmethod
 from enum import Enum
 from pathlib import Path
```

### Comparing `opencf_core-0.3.1a1/opencf_core/converter_app.py` & `opencf_core-0.3.1a2/opencf_core/converter_app.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.3.1a1/opencf_core/exceptions.py` & `opencf_core-0.3.1a2/opencf_core/exceptions.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+"""
+Classes:
+
+- UnsupportedFileTypeError: Custom exception for handling unsupported file types.
+- EmptySuffixError: Specialized exception for cases where a file's suffix does not provide enough information
+                    to determine its type.
+- FileNotFoundError: Raised when a specified file does not exist.
+- MismatchedException: Exception for handling cases where there's a mismatch between expected and actual file attributes.
+"""
+
+
 # Custom Exceptions
 class UnsupportedFileTypeError(Exception):
     """Exception raised for handling cases of unsupported file types."""
 
     def __init__(self, message):
         self.message = message
         super().__init__(self.message)
```

### Comparing `opencf_core-0.3.1a1/opencf_core/filetypes.py` & `opencf_core-0.3.1a2/opencf_core/filetypes.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,33 +3,26 @@
 
 This module provides a comprehensive framework for handling various file types within a file conversion context.
 It defines classes and enumerations for identifying, validating, and working with different file types, based on
 file extensions, MIME types, and optionally, file content. It also includes custom exceptions for handling common
 errors related to file type processing.
 
 Classes:
-- UnsupportedFileTypeError: Custom exception for handling unsupported file types.
-- EmptySuffixError: Specialized exception for cases where a file's suffix does not provide enough information
-                    to determine its type.
-- FileNotFoundError: Raised when a specified file does not exist.
-- MismatchedException: Exception for handling cases where there's a mismatch between expected and actual file attributes.
+
 - FileType: Enum class that encapsulates various file types supported by the system, providing methods for
                 type determination from file attributes.
 
-Functions:
-- test_file_type_parsing(): Demonstrates and validates the parsing functionality for various file types.
-- test_file_type_matching(): Tests the matching and validation capabilities of the FileType class.
-
 Dependencies:
+
 - collections.namedtuple: For defining simple classes for storing MIME type information.
-- enum.Enum: For creating the FileType enumeration.
 - pathlib.Path: For file path manipulations and checks.
 - opencf_core.mimes.guess_mime_type_from_file: Utility function to guess MIME type from a file path.
 
 Usage Examples:
+
 ```python
 from pathlib import Path
 from mymodule import FileType, EmptySuffixError, UnsupportedFileTypeError
 
 # Example: Determine file type from suffix
 try:
     file_type, _ = FileType.from_suffix('.txt')
@@ -53,33 +46,25 @@
 print(f'Is valid: {is_valid}')
 ```
 """
 from __future__ import annotations
 
 from dataclasses import dataclass
 from pathlib import Path
-from typing import TYPE_CHECKING, Dict, Iterable, Tuple, Type, Union
-
-from aenum import extend_enum  # type: ignore
+from typing import Dict, Iterable, Tuple, Type, Union
 
+from opencf_core.enum import Enum, extend_enum_with_methods
 from opencf_core.exceptions import (
     EmptySuffixError,
     MismatchedException,
     UnsupportedFileTypeError,
 )
 
 from .mimes import guess_mime_type_from_file
 
-if TYPE_CHECKING:
-    # this is only processed by MyPy (i.e. not at runtime)
-    from enum import Enum
-else:
-    # this is real runtime code
-    from aenum import Enum
-
 
 @dataclass(eq=False, frozen=True)
 class MimeType:
     """Class representing MIME type information.
 
     Attributes:
         extensions (Tuple[str, ...]): Tuple of file extensions associated with the MIME type.
@@ -92,23 +77,58 @@
     upper_mime_types: Tuple[str, ...] = ()
 
 
 class FileType(Enum):
     """Base enumeration for file types, providing methods for type determination and validation.
 
     Attributes:
-        NOTYPE (MimeType): Represents an undefined file type.
-        TEXT (MimeType): Represents a text file type.
-        UNHANDLED (MimeType): Represents an unhandled file type.
+        NOTYPE (MimeType): Represents an undefined file type (no extensions).
+        TEXT (MimeType): Represents a text file type (.txt).
+        UNHANDLED (MimeType): Represents an unhandled file type (no extensions).
+        CSV (MimeType): Represents a CSV file type (.csv).
+        MARKDOWN (MimeType): Represents a Markdown file type (.md).
+        EXCEL (MimeType): Represents an Excel file type (.xls, .xlsx).
+        MSWORD (MimeType): Represents a Microsoft Word file type (.doc, .docx).
+        JSON (MimeType): Represents a JSON file type (.json).
+        PDF (MimeType): Represents a PDF file type (.pdf).
+        IMAGE (MimeType): Represents an image file type (.jpg, .jpeg, .png).
+        GIF (MimeType): Represents a GIF file type (.gif).
+        VIDEO (MimeType): Represents a video file type (.mp4, .avi).
+        XML (MimeType): Represents a xml file type (.xml).
     """
 
+    # required members
     NOTYPE: MimeType = MimeType()
     TEXT = MimeType(("txt",), ("text/plain",))
     UNHANDLED: MimeType = MimeType()
 
+    # other members
+    CSV = MimeType(("csv",), ("text/csv",), ("text/plain",))
+    MARKDOWN = MimeType(("md",), ("text/markdown",), ("text/plain",))
+
+    EXCEL = MimeType(
+        ("xls", "xlsx"),
+        (
+            "application/vnd.ms-excel",
+            "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
+        ),
+    )
+    MSWORD = MimeType(
+        ("docx", "doc"),
+        (
+            "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
+            "application/msword",
+        ),
+    )
+    JSON = MimeType(("json",), ("application/json",))
+    PDF = MimeType(("pdf",), ("application/pdf",))
+    IMAGE = MimeType(("jpg", "jpeg", "png"), ("image/jpeg", "image/png"))
+    GIF = MimeType(("gif",), ("image/gif",))
+    VIDEO = MimeType(("mp4", "avi"), ("video/mp4", "video/x-msvideo"))
+
     def get_value(self) -> MimeType:
         """Returns the `MimeType` associated with the enumeration member.
 
         Returns:
             MimeType: The MIME type information.
         """
         return self.value  # type:ignore
@@ -342,44 +362,43 @@
             Mimetype: The primary mimetype for the filetype.
                  Returns an empty string if the filetype does not have an associated extension.
         """
         if not self.is_true_filetype():
             return ""
         return self.get_value().mime_types[0]
 
-    def is_valid_suffix(self, suffix: str, raise_err=False):
+    def is_valid_suffix(self, suffix: str, raise_err=False) -> bool:
         """Validates whether a given file extension matches the filetype's expected extensions.
 
         Args:
             suffix (str): The file extension to validate, including the leading period (e.g., ".txt").
             raise_err (bool, optional): If True, raises a MismatchedException for invalid extensions.
                                         Defaults to False.
 
         Returns:
             bool: True if the suffix matches one of the filetype's extensions, False otherwise.
 
         Raises:
             MismatchedException: If the suffix does not match the filetype's extensions and raise_err is True.
         """
-        if not self.is_true_filetype():
-            return False
-        suffix = self.__class__.clean_suffix(suffix)
-        if suffix in self.get_value().extensions:
+        _val, matches = self.from_suffix(suffix, return_matches=True)
+        is_valid = (self == _val) if not self.is_true_filetype() else (self in matches)
+        if is_valid:
             return True
         if raise_err:
             raise MismatchedException(
                 f"filetype ({self.name}) mismatch with suffix ({suffix})",
                 suffix,
                 self.get_one_suffix(),
             )
         return False
 
     def is_valid_path(
         self, file_path: Union[str, Path], read_content=False, raise_err=False
-    ):
+    ) -> bool:
         """Validates the filetype of a given file path. Optionally reads the file's content to verify its type.
 
         Args:
             file_path (Union[str, Path]): The file path to validate.
             read_content (bool, optional): If True, the method also checks the file's content to validate its type.
                                            Defaults to False.
             raise_err (bool, optional): If True, raises exceptions for mismatched or unsupported types.
@@ -392,47 +411,25 @@
             AssertionError: If there is a mismatch between the file type determined from the file's suffix and its content.
             MismatchedException: If the file type determined from the file's suffix or content does not match the filetype.
         """
         _val, matches = self.from_path(
             file_path, read_content=read_content, return_matches=True
         )
         is_valid = (self == _val) if not self.is_true_filetype() else (self in matches)
-        if raise_err and not is_valid:
-            raise MismatchedException(
-                f"suffix/mime-type ({file_path})", _val, self.get_value()
-            )
-        return is_valid
-
-    def is_valid_mimetype(self, file_mimetype: str, raise_err=False):
-        """Validates whether a given MIME type matches the filetype's expected MIME types.
-
-        Args:
-            file_mimetype (str): The MIME type to validate.
-            raise_err (bool, optional): If True, raises a MismatchedException for invalid MIME types.
-                                        Defaults to False.
-
-        Returns:
-            bool: True if the MIME type matches one of the filetype's MIME types, False otherwise.
-
-        Raises:
-            MismatchedException: If the MIME type does not match the filetype's MIME types and raise_err is True.
-        """
-        if not self.is_true_filetype():
-            return False
-        if file_mimetype in self.get_value().mime_types:
+        if is_valid:
             return True
         if raise_err:
             raise MismatchedException(
-                f"filetype ({self.name}) mismatch with mimetype ({file_mimetype})",
-                self.get_one_mimetype(),
-                file_mimetype,
+                f"suffix/mime-type ({file_path})",
+                _val,
+                self.get_value(),
             )
         return False
 
-    def is_valid_mime_type(self, file_path: Path, raise_err=False):
+    def is_valid_mime_type(self, file_path: Path, raise_err=False) -> bool:
         """
         Validates whether the MIME type of the file at the specified path aligns with the filetype's expected MIME types.
 
         This method first determines the filetype based on the file's actual MIME type (determined by reading the file's content)
         and then checks if this determined filetype matches the instance calling this method. Special consideration is given to
         filetype.TEXT, where a broader compatibility check is performed due to the generic nature of text MIME types.
 
@@ -447,41 +444,35 @@
 
         Raises:
             MismatchedException: If raise_err is True and the file's MIME type does not match the expected MIME types
                                 for this filetype instance, including detailed information about the mismatch.
         """
         _val, matches = self.from_mimetype(file_path, return_matches=True)
         is_valid = (self == _val) if not self.is_true_filetype() else (self in matches)
-
-        # many things can be text/plain
-        if (self.TEXT in matches) and "text/plain" in self.get_value().upper_mime_types:
-            is_valid = True
-
-        if raise_err and not is_valid:
+        if is_valid:
+            return True
+        if raise_err:
             raise MismatchedException(
                 f"content-type({file_path})", _val, self.get_value().mime_types
             )
-        return is_valid
+        return False
 
 
 def extract_enum_members(enum_cls: Type) -> Dict[str, MimeType]:
     """Extracts MimeType instances from an enum class.
 
     Args:
         enum_cls (Type): The enum class.
 
     Returns:
         Dict[str, MimeType]: Dictionary of MimeType instances keyed by enum member names.
     """
     extracted_members: Dict[str, MimeType] = {}
     items: Iterable
 
-    if issubclass(enum_cls, FileType):
-        enum_cls = enum_cls
-
     if issubclass(enum_cls, Enum):
         items = ((item.name, item.value) for item in enum_cls)
     else:
         assert hasattr(enum_cls, "__filetype_members__")
         filetype_members: Dict[str, MimeType] = enum_cls.__filetype_members__
         assert isinstance(filetype_members, dict)
         items = filetype_members.items()
@@ -497,51 +488,23 @@
 
 def extend_filetype_enum(added_enum: Type[Enum]) -> None:
     """Extends the BaseFileType enumeration with members from another enumeration.
 
     Args:
         added_enum (Type[Enum]): The enum class to extend BaseFileType with.
     """
-    inherited_enum = FileType
 
-    # Add new members from added_enum to inherited_enum
-    for name, member in added_enum.__members__.items():
-        extend_enum(inherited_enum, name, member.value)
-
-    # Copy methods from inherited_enum and added_enum to the new class
-    for method_name, method in {
-        **added_enum.__dict__,
-        **inherited_enum.__dict__,
-    }.items():
-        if callable(method) or isinstance(method, classmethod):
-            setattr(inherited_enum, method_name, method)
+    def is_member_mimetype(member: Enum):
+        return isinstance(member.value, MimeType)
+
+    return extend_enum_with_methods(
+        FileType, added_enum, filter_func=is_member_mimetype
+    )
 
 
 class FileTypeExamples(Enum):
     """Enumeration of supported file types with methods for type determination and validation."""
 
-    CSV = MimeType(("csv",), ("text/csv",), ("text/plain",))
-    MARKDOWN = MimeType(("md",), ("text/markdown",), ("text/plain",))
-
-    EXCEL = MimeType(
-        ("xls", "xlsx"),
-        (
-            "application/vnd.ms-excel",
-            "application/vnd.openxmlformats-officedocument.spreadsheetml.sheet",
-        ),
-    )
-    MSWORD = MimeType(
-        ("docx", "doc"),
-        (
-            "application/vnd.openxmlformats-officedocument.wordprocessingml.document",
-            "application/msword",
-        ),
-    )
-    JSON = MimeType(("json",), ("application/json",))
-    PDF = MimeType(("pdf",), ("application/pdf",))
-    IMAGE = MimeType(("jpg", "jpeg", "png"), ("image/jpeg", "image/png"))
-    GIF = MimeType(("gif",), ("image/gif",))
-    VIDEO = MimeType(("mp4", "avi"), ("video/mp4", "video/x-msvideo"))
     XML = MimeType(("xml",), ("application/xml", "text/xml"))
 
 
 extend_filetype_enum(FileTypeExamples)
```

### Comparing `opencf_core-0.3.1a1/opencf_core/io_handler.py` & `opencf_core-0.3.1a2/opencf_core/io_handler.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.3.1a1/opencf_core/logging_config.py` & `opencf_core-0.3.1a2/opencf_core/logging_config.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.3.1a1/opencf_core/mimes.py` & `opencf_core-0.3.1a2/opencf_core/mimes.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.3.1a1/opencf_core/utils.py` & `opencf_core-0.3.1a2/opencf_core/utils.py`

 * *Files identical despite different names*

### Comparing `opencf_core-0.3.1a1/pyproject.toml` & `opencf_core-0.3.1a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "opencf-core"
 packages = [
     {include = "opencf_core"}
 ]
-version = "0.3.1a1"
+version = "0.3.1a2"
 description = "A robust framework for handling file conversion tasks in Python"
 authors = ["Hermann Agossou <agossouhermann7@gmail.com>"]
 readme = "README.md"
 maintainers = [
     "Hermann Agossou <agossouhermann7@gmail.com>"
 ]
 license = "MIT"
```

### Comparing `opencf_core-0.3.1a1/PKG-INFO` & `opencf_core-0.3.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opencf-core
-Version: 0.3.1a1
+Version: 0.3.1a2
 Summary: A robust framework for handling file conversion tasks in Python
 Home-page: https://github.com/Hermann-web/opencf-core
 License: MIT
 Keywords: file conversion,data processing,file formats
 Author: Hermann Agossou
 Author-email: agossouhermann7@gmail.com
 Maintainer: Hermann Agossou
```

