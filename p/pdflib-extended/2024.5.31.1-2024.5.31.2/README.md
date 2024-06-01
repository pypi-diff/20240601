# Comparing `tmp/pdflib_extended-2024.5.31.1.tar.gz` & `tmp/pdflib_extended-2024.5.31.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdflib_extended-2024.5.31.1.tar", max compression
+gzip compressed data, was "pdflib_extended-2024.5.31.2.tar", max compression
```

## Comparing `pdflib_extended-2024.5.31.1.tar` & `pdflib_extended-2024.5.31.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0        0 2024-05-31 20:27:46.822221 pdflib_extended-2024.5.31.1/README.md
--rw-r--r--   0        0        0      887 2024-05-31 20:27:55.562231 pdflib_extended-2024.5.31.1/pyproject.toml
--rw-r--r--   0        0        0       29 2024-05-31 20:27:55.558231 pdflib_extended-2024.5.31.1/src/pdflib_extended/__init__.py
--rw-r--r--   0        0        0        0 2024-05-31 20:27:46.822221 pdflib_extended-2024.5.31.1/src/pdflib_extended/core/__init__.py
--rw-r--r--   0        0        0    15405 2024-05-31 20:27:46.826221 pdflib_extended-2024.5.31.1/src/pdflib_extended/core/binaries/linux/pdflib_py.pyi
--rw-r--r--   0        0        0 12241752 2024-05-31 20:27:46.890221 pdflib_extended-2024.5.31.1/src/pdflib_extended/core/binaries/linux/pdflib_py.so
--rw-r--r--   0        0        0  6616576 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/core/binaries/windows/pdflib_py.pyd
--rw-r--r--   0        0        0    15405 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/core/binaries/windows/pdflib_py.pyi
--rw-r--r--   0        0        0    19863 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/core/pdflib_base.py
--rw-r--r--   0        0        0      302 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/exceptions.py
--rw-r--r--   0        0        0        0 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/__init__.py
--rw-r--r--   0        0        0     3856 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/barcodes.py
--rw-r--r--   0        0        0      360 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/classes.py
--rw-r--r--   0        0        0     5103 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/contexts.py
--rw-r--r--   0        0        0      694 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/shapes.py
--rw-r--r--   0        0        0     1004 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/text.py
--rw-r--r--   0        0        0     2098 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/pdflib.py
--rw-r--r--   0        0        0        0 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/py.typed
--rw-r--r--   0        0        0    22144 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/resources/fonts/LibreBarcode128-Regular.ttf
--rw-r--r--   0        0        0   130832 2024-05-31 20:27:46.926221 pdflib_extended-2024.5.31.1/src/pdflib_extended/resources/fonts/OpenSans-Regular.ttf
--rw-r--r--   0        0        0      483 1970-01-01 00:00:00.000000 pdflib_extended-2024.5.31.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-31 21:03:28.534561 pdflib_extended-2024.5.31.2/README.md
+-rw-r--r--   0        0        0      918 2024-05-31 21:03:37.158562 pdflib_extended-2024.5.31.2/pyproject.toml
+-rw-r--r--   0        0        0       29 2024-05-31 21:03:37.158562 pdflib_extended-2024.5.31.2/src/pdflib_extended/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-31 21:03:28.534561 pdflib_extended-2024.5.31.2/src/pdflib_extended/core/__init__.py
+-rw-r--r--   0        0        0    15405 2024-05-31 21:03:28.534561 pdflib_extended-2024.5.31.2/src/pdflib_extended/core/binaries/linux/pdflib_py.pyi
+-rw-r--r--   0        0        0 12241752 2024-05-31 21:03:28.598561 pdflib_extended-2024.5.31.2/src/pdflib_extended/core/binaries/linux/pdflib_py.so
+-rw-r--r--   0        0        0  6616576 2024-05-31 21:03:28.634561 pdflib_extended-2024.5.31.2/src/pdflib_extended/core/binaries/windows/pdflib_py.pyd
+-rw-r--r--   0        0        0    15405 2024-05-31 21:03:28.634561 pdflib_extended-2024.5.31.2/src/pdflib_extended/core/binaries/windows/pdflib_py.pyi
+-rw-r--r--   0        0        0    19863 2024-05-31 21:03:28.634561 pdflib_extended-2024.5.31.2/src/pdflib_extended/core/pdflib_base.py
+-rw-r--r--   0        0        0      302 2024-05-31 21:03:28.634561 pdflib_extended-2024.5.31.2/src/pdflib_extended/exceptions.py
+-rw-r--r--   0        0        0        0 2024-05-31 21:03:28.634561 pdflib_extended-2024.5.31.2/src/pdflib_extended/extensions/__init__.py
+-rw-r--r--   0        0        0     3856 2024-05-31 21:03:28.634561 pdflib_extended-2024.5.31.2/src/pdflib_extended/extensions/barcodes.py
+-rw-r--r--   0        0        0      360 2024-05-31 21:03:28.634561 pdflib_extended-2024.5.31.2/src/pdflib_extended/extensions/classes.py
+-rw-r--r--   0        0        0     5132 2024-05-31 21:03:28.634561 pdflib_extended-2024.5.31.2/src/pdflib_extended/extensions/contexts.py
+-rw-r--r--   0        0        0      694 2024-05-31 21:03:28.634561 pdflib_extended-2024.5.31.2/src/pdflib_extended/extensions/shapes.py
+-rw-r--r--   0        0        0     1004 2024-05-31 21:03:28.634561 pdflib_extended-2024.5.31.2/src/pdflib_extended/extensions/text.py
+-rw-r--r--   0        0        0     2098 2024-05-31 21:03:28.634561 pdflib_extended-2024.5.31.2/src/pdflib_extended/pdflib.py
+-rw-r--r--   0        0        0        0 2024-05-31 21:03:28.634561 pdflib_extended-2024.5.31.2/src/pdflib_extended/py.typed
+-rw-r--r--   0        0        0    22144 2024-05-31 21:03:28.638561 pdflib_extended-2024.5.31.2/src/pdflib_extended/resources/fonts/LibreBarcode128-Regular.ttf
+-rw-r--r--   0        0        0   130832 2024-05-31 21:03:28.638561 pdflib_extended-2024.5.31.2/src/pdflib_extended/resources/fonts/OpenSans-Regular.ttf
+-rw-r--r--   0        0        0      564 1970-01-01 00:00:00.000000 pdflib_extended-2024.5.31.2/PKG-INFO
```

### Comparing `pdflib_extended-2024.5.31.1/pyproject.toml` & `pdflib_extended-2024.5.31.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [tool.poetry]
 name = "pdflib-extended"
-version = "2024.05.31.1"
-description = ""
+version = "2024.05.31.2"
+description = "Extension of the PDFlib library."
 authors = ["RichardS <richards@eoshost.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.9"
 pylibdmtx = "^0.1.10"
 pillow = "^10.3.0"
 
 [tool.poetry.dev-dependencies]
 black = "^24.4.2"
 setuptools = "^70.0.0"
 pytest = "^8.2.1"
```

### Comparing `pdflib_extended-2024.5.31.1/src/pdflib_extended/core/binaries/linux/pdflib_py.pyi` & `pdflib_extended-2024.5.31.2/src/pdflib_extended/core/binaries/linux/pdflib_py.pyi`

 * *Files identical despite different names*

### Comparing `pdflib_extended-2024.5.31.1/src/pdflib_extended/core/binaries/linux/pdflib_py.so` & `pdflib_extended-2024.5.31.2/src/pdflib_extended/core/binaries/linux/pdflib_py.so`

 * *Files identical despite different names*

### Comparing `pdflib_extended-2024.5.31.1/src/pdflib_extended/core/binaries/windows/pdflib_py.pyi` & `pdflib_extended-2024.5.31.2/src/pdflib_extended/core/binaries/windows/pdflib_py.pyi`

 * *Files identical despite different names*

### Comparing `pdflib_extended-2024.5.31.1/src/pdflib_extended/core/pdflib_base.py` & `pdflib_extended-2024.5.31.2/src/pdflib_extended/core/pdflib_base.py`

 * *Files identical despite different names*

### Comparing `pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/barcodes.py` & `pdflib_extended-2024.5.31.2/src/pdflib_extended/extensions/barcodes.py`

 * *Files identical despite different names*

### Comparing `pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/contexts.py` & `pdflib_extended-2024.5.31.2/src/pdflib_extended/extensions/contexts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from contextlib import AbstractContextManager
 from pathlib import Path
-from typing import Union, Optional, Self, ContextManager
+from typing import Union, Optional, ContextManager
+from typing_extensions import Self
 
 from ..core.pdflib_base import PDFlibBase
 from ..exceptions import (
     InvalidDocumentHandle,
     InvalidPageHandle,
     DocumentWriteException,
     EmptyNewDocumentException,
```

### Comparing `pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/shapes.py` & `pdflib_extended-2024.5.31.2/src/pdflib_extended/extensions/shapes.py`

 * *Files identical despite different names*

### Comparing `pdflib_extended-2024.5.31.1/src/pdflib_extended/extensions/text.py` & `pdflib_extended-2024.5.31.2/src/pdflib_extended/extensions/text.py`

 * *Files identical despite different names*

### Comparing `pdflib_extended-2024.5.31.1/src/pdflib_extended/pdflib.py` & `pdflib_extended-2024.5.31.2/src/pdflib_extended/pdflib.py`

 * *Files identical despite different names*

### Comparing `pdflib_extended-2024.5.31.1/src/pdflib_extended/resources/fonts/LibreBarcode128-Regular.ttf` & `pdflib_extended-2024.5.31.2/src/pdflib_extended/resources/fonts/LibreBarcode128-Regular.ttf`

 * *Files identical despite different names*

### Comparing `pdflib_extended-2024.5.31.1/src/pdflib_extended/resources/fonts/OpenSans-Regular.ttf` & `pdflib_extended-2024.5.31.2/src/pdflib_extended/resources/fonts/OpenSans-Regular.ttf`

 * *Files identical despite different names*

