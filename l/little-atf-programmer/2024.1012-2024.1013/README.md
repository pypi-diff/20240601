# Comparing `tmp/little_atf_programmer-2024.1012.tar.gz` & `tmp/little_atf_programmer-2024.1013.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "little_atf_programmer-2024.1012.tar", last modified: Sun May 26 12:22:43 2024, max compression
+gzip compressed data, was "little_atf_programmer-2024.1013.tar", last modified: Sat Jun  1 19:25:14 2024, max compression
```

## Comparing `little_atf_programmer-2024.1012.tar` & `little_atf_programmer-2024.1013.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:43.722056 little_atf_programmer-2024.1012/
--rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    12451 2024-05-26 12:22:43.718056 little_atf_programmer-2024.1012/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-26 12:22:43.722056 little_atf_programmer-2024.1012/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:43.714056 little_atf_programmer-2024.1012/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:43.714056 little_atf_programmer-2024.1012/src/atfu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/check.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:43.714056 little_atf_programmer-2024.1012/src/atfu/converter/
--rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/converter/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     5860 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/converter/fuseconv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/converter/jed2svf.py
--rw-r--r--   0 runner    (1001) docker     (127)    10778 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/converter/jesd3.py
--rw-r--r--   0 runner    (1001) docker     (127)    31144 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/converter/svf2xsvf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/converter/svfeventhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/erase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:43.714056 little_atf_programmer-2024.1012/src/atfu/little_board/
--rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/little_board/jtag_programmer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/program.py
--rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/programmer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:43.718056 little_atf_programmer-2024.1012/src/atfu/standard_vectors/
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/standard_vectors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27936 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/standard_vectors/bc1502.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)    34858 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/standard_vectors/bc1504.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)    51652 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/standard_vectors/bc1508.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)    27916 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/standard_vectors/e1502.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)    34838 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/standard_vectors/e1504.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)    51632 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu/standard_vectors/e1508.xsvf
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-26 12:22:24.000000 little_atf_programmer-2024.1012/src/atfu.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-26 12:22:43.718056 little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12451 2024-05-26 12:22:43.000000 little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-26 12:22:43.000000 little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-26 12:22:43.000000 little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-26 12:22:43.000000 little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-26 12:22:43.000000 little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-26 12:22:43.000000 little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:25:14.446357 little_atf_programmer-2024.1013/
+-rw-r--r--   0 runner    (1001) docker     (127)     4278 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12451 2024-06-01 19:25:14.446357 little_atf_programmer-2024.1013/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6338 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 19:25:14.446357 little_atf_programmer-2024.1013/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:25:14.442357 little_atf_programmer-2024.1013/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:25:14.442357 little_atf_programmer-2024.1013/src/atfu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/check.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:25:14.442357 little_atf_programmer-2024.1013/src/atfu/converter/
+-rw-r--r--   0 runner    (1001) docker     (127)     9005 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/converter/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6520 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/converter/fuseconv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/converter/jed2svf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/converter/jesd3.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31144 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/converter/svf2xsvf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/converter/svfeventhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1846 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/erase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:25:14.442357 little_atf_programmer-2024.1013/src/atfu/little_board/
+-rw-r--r--   0 runner    (1001) docker     (127)     6212 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/little_board/jtag_programmer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1202 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/program.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2348 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/programmer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:25:14.446357 little_atf_programmer-2024.1013/src/atfu/standard_vectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/standard_vectors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27936 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/standard_vectors/bc1502.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)    34858 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/standard_vectors/bc1504.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)    51652 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/standard_vectors/bc1508.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)    27916 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/standard_vectors/e1502.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)    34838 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/standard_vectors/e1504.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)    51632 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu/standard_vectors/e1508.xsvf
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-06-01 19:24:59.000000 little_atf_programmer-2024.1013/src/atfu.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:25:14.446357 little_atf_programmer-2024.1013/src/little_atf_programmer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12451 2024-06-01 19:25:14.000000 little_atf_programmer-2024.1013/src/little_atf_programmer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-06-01 19:25:14.000000 little_atf_programmer-2024.1013/src/little_atf_programmer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 19:25:14.000000 little_atf_programmer-2024.1013/src/little_atf_programmer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-06-01 19:25:14.000000 little_atf_programmer-2024.1013/src/little_atf_programmer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-06-01 19:25:14.000000 little_atf_programmer-2024.1013/src/little_atf_programmer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-06-01 19:25:14.000000 little_atf_programmer-2024.1013/src/little_atf_programmer.egg-info/top_level.txt
```

### Comparing `little_atf_programmer-2024.1012/LICENSE.md` & `little_atf_programmer-2024.1013/LICENSE.md`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/PKG-INFO` & `little_atf_programmer-2024.1013/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: little-atf-programmer
-Version: 2024.1012
+Version: 2024.1013
 Summary: Little ATF150x Programmer Board utility programs
 Author-email: The Really Old-School Company Limited <info@rosco-m68k.com>
 License: Copyright (c) 2024 The Really Old-School Company Limited
         
         Permission is hereby granted, free of charge, to any person obtaining 
         a copy of this software and associated documentation files (the "Software"),
         to deal in the Software without restriction, including without limitation
```

### Comparing `little_atf_programmer-2024.1012/README.md` & `little_atf_programmer-2024.1013/README.md`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/pyproject.toml` & `little_atf_programmer-2024.1013/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "little-atf-programmer"
-version = "2024.1012"
+version = "2024.1013"
 description = "Little ATF150x Programmer Board utility programs"
 readme = "README.md"
 authors = [{ name = "The Really Old-School Company Limited", email = "info@rosco-m68k.com" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -34,15 +34,15 @@
 [project.urls]
 Homepage = "https://github.com/roscopeco/atfprog-tools"
 
 [tool.setuptools.package-data]
 "atfu.standard_vectors" = ["*.xsvf"]
 
 [tool.bumpver]
-current_version = "2024.1012"
+current_version = "2024.1013"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 tag_message = "{new_version}"
 tag_scope = "default"
 commit = true
 tag = true
 push = true
```

### Comparing `little_atf_programmer-2024.1012/src/atfu/check.py` & `little_atf_programmer-2024.1013/src/atfu/check.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/src/atfu/command.py` & `little_atf_programmer-2024.1013/src/atfu/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import atfu.program
 import atfu.erase
 import atfu.check
 import atfu.programmer
 
 BOARDNAME = "Little ATF150x Programmer Board"
 PROGNAME = f"{BOARDNAME} Utility"
-VERSION = "2024.1012"
+VERSION = "2024.1013"
 
 
 def main():
     args = _arg_parser().parse_args()
     args.func(args)
```

### Comparing `little_atf_programmer-2024.1012/src/atfu/converter/device.py` & `little_atf_programmer-2024.1013/src/atfu/converter/device.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/src/atfu/converter/fuseconv.py` & `little_atf_programmer-2024.1013/src/atfu/converter/fuseconv.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,34 @@
 import argparse
+import re
 
 from atfu.converter.jesd3 import JESD3Parser
 from atfu.converter.svfeventhandler import SVFEventHandler
 from atfu.converter.device import ATF15xxInstr
 
 
 def read_jed(file):
-    parser = JESD3Parser(file.read())
+    jed = file.read()
+
+    # TODO
+    #
+    # CUPL will emit weird test vectors (with the max vector QV number *after* the
+    # first V0001, which _seems_ to be off-spec. The jesd3 code can't handle this.
+    #
+    # We don't care about test vectors anyway, but we need to at least be able to
+    # checksum them, so for now we'll just refuse to process a jed that has vectors
+    # in it...
+    #
+    # Leaving the regexes below in case they're useful late (to be able to just
+    # remove the problem vectors **by force**). See also jesd3.py:
+    #
+    # jed = re.sub(r'\r?\nQV[0-9]+\*', '', jed)
+    # jed = re.sub(r'V[0-9+][^\r\n]+\r?\n?\*?', '', jed)
+
+    parser = JESD3Parser(jed)
     parser.parse()
     return parser.fuse, parser.design_spec
 
 
 class ATFSVFEventHandler(SVFEventHandler):
     def ignored(self, *args, **kwargs):
         pass
```

### Comparing `little_atf_programmer-2024.1012/src/atfu/converter/jed2svf.py` & `little_atf_programmer-2024.1013/src/atfu/converter/jed2svf.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/src/atfu/converter/jesd3.py` & `little_atf_programmer-2024.1013/src/atfu/converter/jesd3.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Vendored from glasgow.protocol.jesd3
 
 # Ref: JEDEC JESD3-C
 # Accession: G00029
 
 import re
 from bitarray import bitarray
-
+from atfu.output import global_output
 
 __all__ = ["JESD3Parser", "JESD3ParsingError"]
 
 
 class JESD3ParsingError(Exception):
     pass
 
@@ -43,15 +43,19 @@
         (r"UA", r"([\r\n\x20-\x29\x2B-\x7E]+)"),
         (r"UH", r"([0-9A-F]+)"),
         (r"U", r"([01]+)"),
         (r"J", r"([0-9]+)[ \r\n]+([0-9]+)"),
         (r"G", r"([01])"),
         (r"X", r"([01])"),
         (r"P", r"([ \r\n]*[0-9]+)+"),
-        (r"V", r"([0-9]+)[ \r\n]+([0-9BCDFHTUXZ]+)"),
+        # This next one _can_ handle the QV (and has all vector types) but still won't checksum
+        #
+        # TODO fix this properly (currently we just error out with a "helpful" message)
+        #        (r"V", r"([0-9]+)[ \r\n]+(?:QV\d+\* )?([0-9BCDFHLNPTUXZ]+)"),
+        (r"V", r"([0-9]+)[ \r\n]+([0-9BCDFHLNPTUXZ]+)"),
         (r"S", r"([01]+)"),
         (r"R", r"([0-9A-F]{8})"),
         (r"T", r"([0-9]+)"),
         (r"A", r"([\r\n\x20-\x29\x2B-\x7E]*)([0-9]+)"),
     )
     _stx_spec_re = re.compile(r"\x02(.*?)\*[ \r\n]*", re.A | re.S)
     _stx_quirk_re = re.compile(r"\x02()[ \r\n]*", re.A | re.S)
@@ -101,18 +105,25 @@
 
         elif self._state == "fields":
             match = self._ident_re.match(self.buffer, self.position)
             if match:
                 token = match.group(0)
                 match = self._field_res[token].match(self.buffer, self.position)
                 if not match:
-                    raise JESD3ParsingError(
-                        "field %s has invalid format at line %d, column %d"
-                        % (token, *self.line_column())
-                    )
+                    if token == "V":
+                        global_output().error(
+                            "Failure",
+                            "JEDEC file contains test vectors, which cannot be processed by this tool. Please rebuild without them.",
+                        )
+                        exit(1000)
+                    else:
+                        raise JESD3ParsingError(
+                            "field %s has invalid format at line %d, column %d"
+                            % (token, *self.line_column())
+                        )
                 else:
                     self.checksum += sum(map(ord, match.group(0)))
 
             else:
                 match = self._etx_re.match(self.buffer, self.position)
                 if not match:
                     raise JESD3ParsingError(
```

### Comparing `little_atf_programmer-2024.1012/src/atfu/converter/svf2xsvf.py` & `little_atf_programmer-2024.1013/src/atfu/converter/svf2xsvf.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/src/atfu/converter/svfeventhandler.py` & `little_atf_programmer-2024.1013/src/atfu/converter/svfeventhandler.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/src/atfu/erase.py` & `little_atf_programmer-2024.1013/src/atfu/erase.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/src/atfu/little_board/jtag_programmer.py` & `little_atf_programmer-2024.1013/src/atfu/little_board/jtag_programmer.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/src/atfu/output.py` & `little_atf_programmer-2024.1013/src/atfu/output.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,18 +7,22 @@
     cReset = "\x1b[0m"
 else:
     cbRed = ""
     cbGreen = ""
     cbYellow = ""
     cReset = ""
 
+the_output = None
+
 
 class Output:
     def __init__(self, args):
+        global the_output
         self._verbosity = self._verbosity(args)
+        the_output = self
 
     def verbosity(self):
         return self._verbosity
 
     def output(self, level: int, msg: str):
         if self._verbosity > level:
             print(msg)
@@ -42,7 +46,11 @@
         if args.trace:
             return 100
 
         if args.verbose:
             return 2
 
         return 1
+
+
+def global_output() -> Output:
+    return the_output
```

### Comparing `little_atf_programmer-2024.1012/src/atfu/program.py` & `little_atf_programmer-2024.1013/src/atfu/program.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/src/atfu/programmer.py` & `little_atf_programmer-2024.1013/src/atfu/programmer.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/src/atfu/standard_vectors/__init__.py` & `little_atf_programmer-2024.1013/src/atfu/standard_vectors/__init__.py`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/src/atfu/standard_vectors/bc1502.xsvf` & `little_atf_programmer-2024.1013/src/atfu/standard_vectors/bc1502.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/src/atfu/standard_vectors/bc1504.xsvf` & `little_atf_programmer-2024.1013/src/atfu/standard_vectors/bc1504.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/src/atfu/standard_vectors/bc1508.xsvf` & `little_atf_programmer-2024.1013/src/atfu/standard_vectors/bc1508.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/src/atfu/standard_vectors/e1502.xsvf` & `little_atf_programmer-2024.1013/src/atfu/standard_vectors/e1502.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/src/atfu/standard_vectors/e1504.xsvf` & `little_atf_programmer-2024.1013/src/atfu/standard_vectors/e1504.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/src/atfu/standard_vectors/e1508.xsvf` & `little_atf_programmer-2024.1013/src/atfu/standard_vectors/e1508.xsvf`

 * *Files identical despite different names*

### Comparing `little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/PKG-INFO` & `little_atf_programmer-2024.1013/src/little_atf_programmer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: little-atf-programmer
-Version: 2024.1012
+Version: 2024.1013
 Summary: Little ATF150x Programmer Board utility programs
 Author-email: The Really Old-School Company Limited <info@rosco-m68k.com>
 License: Copyright (c) 2024 The Really Old-School Company Limited
         
         Permission is hereby granted, free of charge, to any person obtaining 
         a copy of this software and associated documentation files (the "Software"),
         to deal in the Software without restriction, including without limitation
```

### Comparing `little_atf_programmer-2024.1012/src/little_atf_programmer.egg-info/SOURCES.txt` & `little_atf_programmer-2024.1013/src/little_atf_programmer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

