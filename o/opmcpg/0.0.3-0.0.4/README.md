# Comparing `tmp/opmcpg-0.0.3-cp39-cp39-win_amd64.whl.zip` & `tmp/opmcpg-0.0.4-cp39-cp39-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 137370 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-06 12:04 opmcpg/__init__.py
--rw-rw-rw-  2.0 fat   261632 b- defN 23-Jul-06 12:04 opmcpg/_cpggrid.pyd
--rw-rw-rw-  2.0 fat    34819 b- defN 23-Jul-06 12:04 opmcpg-0.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat    37484 b- defN 23-Jul-06 12:04 opmcpg-0.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Jul-06 12:04 opmcpg-0.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-06 12:04 opmcpg-0.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      533 b- defN 23-Jul-06 12:04 opmcpg-0.0.3.dist-info/RECORD
-7 files, 334575 bytes uncompressed, 136434 bytes compressed:  59.2%
+Zip file size: 136394 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat        0 b- defN 24-May-31 19:43 opmcpg/__init__.py
+-rw-rw-rw-  2.0 fat   252928 b- defN 24-May-31 19:44 opmcpg/_cpggrid.cp39-win_amd64.pyd
+-rw-rw-rw-  2.0 fat    34819 b- defN 24-May-31 19:44 opmcpg-0.0.4.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat    37595 b- defN 24-May-31 19:44 opmcpg-0.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat      100 b- defN 24-May-31 19:44 opmcpg-0.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 24-May-31 19:44 opmcpg-0.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      548 b- defN 24-May-31 19:44 opmcpg-0.0.4.dist-info/RECORD
+7 files, 325997 bytes uncompressed, 135428 bytes compressed:  58.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: opmcpg/__init__.py
 Comment: 
 
-Filename: opmcpg/_cpggrid.pyd
+Filename: opmcpg/_cpggrid.cp39-win_amd64.pyd
 Comment: 
 
-Filename: opmcpg-0.0.3.dist-info/LICENSE
+Filename: opmcpg-0.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: opmcpg-0.0.3.dist-info/METADATA
+Filename: opmcpg-0.0.4.dist-info/METADATA
 Comment: 
 
-Filename: opmcpg-0.0.3.dist-info/WHEEL
+Filename: opmcpg-0.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: opmcpg-0.0.3.dist-info/top_level.txt
+Filename: opmcpg-0.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: opmcpg-0.0.3.dist-info/RECORD
+Filename: opmcpg-0.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `opmcpg-0.0.3.dist-info/LICENSE` & `opmcpg-0.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `opmcpg-0.0.3.dist-info/METADATA` & `opmcpg-0.0.4.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opmcpg
-Version: 0.0.3
+Version: 0.0.4
 Summary: Corner Point Grid processing
 Author-email: Ilshat Saifullin <I.S.Saifullin@tudelft.nl>
 License: GNU GENERAL PUBLIC LICENSE
         Version 3, 29 June 2007
         
         Copyright © 2007 Free Software Foundation, Inc. <https://fsf.org/>
         
@@ -234,10 +234,12 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 
+[![pypi](https://img.shields.io/pypi/v/opmcpg.svg?colorB=blue)](https://pypi.org/project/opmcpg/#description)
+
 The code in folder src\opm was taken from https://opm-project.org/ in particular https://github.com/OPM/opm-grid/tree/master/opm/grid
 and upgraded to C++ using std::vector instead of pointers ans mallocto be able to expose them to python. Added pybind11.
 This wheel contains only dynamic library which could be imported in python
```

