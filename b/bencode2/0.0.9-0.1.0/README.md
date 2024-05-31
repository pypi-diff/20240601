# Comparing `tmp/bencode2-0.0.9.tar.gz` & `tmp/bencode2-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bencode2-0.0.9.tar", last modified: Sun Apr 14 14:26:11 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `bencode2-0.0.9.tar` & `bencode2-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,9 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:26:11.301989 bencode2-0.0.9/
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-14 14:26:06.000000 bencode2-0.0.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-14 14:26:06.000000 bencode2-0.0.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-14 14:26:11.301989 bencode2-0.0.9/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:26:11.297989 bencode2-0.0.9/bencode2/
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-14 14:26:06.000000 bencode2-0.0.9/bencode2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   487607 2024-04-14 14:26:10.000000 bencode2-0.0.9/bencode2/_decoder.c
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-04-14 14:26:06.000000 bencode2-0.0.9/bencode2/_decoder.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   375778 2024-04-14 14:26:10.000000 bencode2-0.0.9/bencode2/_encoder.c
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-04-14 14:26:06.000000 bencode2-0.0.9/bencode2/_encoder.pyx
--rw-r--r--   0 runner    (1001) docker     (127)   190928 2024-04-14 14:26:10.000000 bencode2-0.0.9/bencode2/_exceptions.c
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-14 14:26:06.000000 bencode2-0.0.9/bencode2/_exceptions.pyx
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-14 14:26:06.000000 bencode2-0.0.9/bencode2/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:26:11.301989 bencode2-0.0.9/bencode2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-14 14:26:11.000000 bencode2-0.0.9/bencode2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-14 14:26:11.000000 bencode2-0.0.9/bencode2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-14 14:26:11.000000 bencode2-0.0.9/bencode2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-14 14:26:11.000000 bencode2-0.0.9/bencode2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-14 14:26:06.000000 bencode2-0.0.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-14 14:26:11.301989 bencode2-0.0.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-14 14:26:06.000000 bencode2-0.0.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-14 14:26:11.301989 bencode2-0.0.9/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-14 14:26:06.000000 bencode2-0.0.9/tests/test_decode.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-14 14:26:06.000000 bencode2-0.0.9/tests/test_encode.py
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-14 14:26:06.000000 bencode2-0.0.9/tests/test_torrent.py
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 bencode2-0.1.0/bencode2/__init__.py
+-rw-r--r--   0        0        0     5362 2020-02-02 00:00:00.000000 bencode2-0.1.0/bencode2/_decoder.py
+-rw-r--r--   0        0        0     4787 2020-02-02 00:00:00.000000 bencode2-0.1.0/bencode2/_encoder.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 bencode2-0.1.0/bencode2/py.typed
+-rw-r--r--   0        0        0     4812 2020-02-02 00:00:00.000000 bencode2-0.1.0/.gitignore
+-rw-r--r--   0        0        0     1085 2020-02-02 00:00:00.000000 bencode2-0.1.0/LICENSE
+-rw-r--r--   0        0        0     2150 2020-02-02 00:00:00.000000 bencode2-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 bencode2-0.1.0/readme.md
+-rw-r--r--   0        0        0     2210 2020-02-02 00:00:00.000000 bencode2-0.1.0/PKG-INFO
```

### Comparing `bencode2-0.0.9/LICENSE` & `bencode2-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bencode2-0.0.9/bencode2/__init__.py` & `bencode2-0.1.0/bencode2/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,25 @@
-# cython: language_level=3
-
 from typing import Any
 
+from ._decoder import BencodeDecodeError
 from ._decoder import Decoder as _Decoder
+from ._encoder import BencodeEncodeError
 from ._encoder import encode as _encode
-from ._exceptions import BencodeDecodeError, BencodeEncodeError
 
 __all__ = (
     "BencodeDecodeError",
     "BencodeEncodeError",
     "bencode",
     "bdecode",
 )
 
 
-def bencode(value: Any) -> bytes:
+def bencode(value: Any, /) -> bytes:
     """Encode value into the bencode format."""
     return _encode(value)
 
 
-def bdecode(value: bytes, *, str_key: bool = False) -> Any:
+def bdecode(value: bytes, /, *, str_key: bool = False) -> Any:
     """Decode bencode formatted bytes to python value."""
-    return _Decoder(str_key).decode(value)
+    if not isinstance(value, bytes):
+        raise TypeError("only support decoding bytes")
+    return _Decoder(value, str_key).decode()
```

