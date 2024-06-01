# Comparing `tmp/pyarmor.cli.core.windows-6.5.1-cp39-none-any.whl.zip` & `tmp/pyarmor.cli.core.windows-6.5.2-cp39-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 851098 bytes, number of entries: 9
--rw-r--r--  2.0 unx       22 b- defN 24-Apr-19 07:50 pyarmor/cli/core/windows/__init__.py
--rwxr-xr-x  2.0 unx   777742 b- defN 24-Apr-19 07:50 pyarmor/cli/core/windows/x86/pyarmor_runtime.pyd
--rwxr-xr-x  2.0 unx   593920 b- defN 24-Apr-19 07:50 pyarmor/cli/core/windows/x86/pytransform3.pyd
--rwxr-xr-x  2.0 unx   632832 b- defN 24-Apr-19 07:50 pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd
--rwxr-xr-x  2.0 unx   455168 b- defN 24-Apr-19 07:50 pyarmor/cli/core/windows/x86_64/pytransform3.pyd
--rw-r--r--  2.0 unx      808 b- defN 24-Apr-19 07:50 pyarmor.cli.core.windows-6.5.1.dist-info/METADATA
--rw-r--r--  2.0 unx       93 b- defN 24-Apr-19 07:50 pyarmor.cli.core.windows-6.5.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 24-Apr-19 07:50 pyarmor.cli.core.windows-6.5.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      883 b- defN 24-Apr-19 07:50 pyarmor.cli.core.windows-6.5.1.dist-info/RECORD
-9 files, 2461476 bytes uncompressed, 849544 bytes compressed:  65.5%
+Zip file size: 851343 bytes, number of entries: 9
+-rw-r--r--  2.0 unx       22 b- defN 24-May-30 03:02 pyarmor/cli/core/windows/__init__.py
+-rwxr-xr-x  2.0 unx   777742 b- defN 24-May-30 03:02 pyarmor/cli/core/windows/x86/pyarmor_runtime.pyd
+-rwxr-xr-x  2.0 unx   594432 b- defN 24-May-30 03:02 pyarmor/cli/core/windows/x86/pytransform3.pyd
+-rwxr-xr-x  2.0 unx   632832 b- defN 24-May-30 03:02 pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd
+-rwxr-xr-x  2.0 unx   455168 b- defN 24-May-30 03:02 pyarmor/cli/core/windows/x86_64/pytransform3.pyd
+-rw-r--r--  2.0 unx      808 b- defN 24-May-30 03:02 pyarmor.cli.core.windows-6.5.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       93 b- defN 24-May-30 03:02 pyarmor.cli.core.windows-6.5.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 24-May-30 03:02 pyarmor.cli.core.windows-6.5.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      883 b- defN 24-May-30 03:02 pyarmor.cli.core.windows-6.5.2.dist-info/RECORD
+9 files, 2461988 bytes uncompressed, 849789 bytes compressed:  65.5%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd
 Comment: 
 
 Filename: pyarmor/cli/core/windows/x86_64/pytransform3.pyd
 Comment: 
 
-Filename: pyarmor.cli.core.windows-6.5.1.dist-info/METADATA
+Filename: pyarmor.cli.core.windows-6.5.2.dist-info/METADATA
 Comment: 
 
-Filename: pyarmor.cli.core.windows-6.5.1.dist-info/WHEEL
+Filename: pyarmor.cli.core.windows-6.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: pyarmor.cli.core.windows-6.5.1.dist-info/top_level.txt
+Filename: pyarmor.cli.core.windows-6.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pyarmor.cli.core.windows-6.5.1.dist-info/RECORD
+Filename: pyarmor.cli.core.windows-6.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyarmor/cli/core/windows/__init__.py

```diff
@@ -1 +1 @@
-__VERSION__ = '6.5.1'
+__VERSION__ = '6.5.2'
```

## Comparing `pyarmor.cli.core.windows-6.5.1.dist-info/METADATA` & `pyarmor.cli.core.windows-6.5.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyarmor.cli.core.windows
-Version: 6.5.1
+Version: 6.5.2
 Summary: Provide pre-built extension modules `pytransform3` and `pyarmor_runtime` for Pyarmor
 Home-page: https://github.com/dashingsoft/pyarmor
 Author: Jondy Zhao
 Author-email: pyarmor@163.com
 License: Free To Use But Restricted
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `pyarmor.cli.core.windows-6.5.1.dist-info/RECORD` & `pyarmor.cli.core.windows-6.5.2.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-pyarmor/cli/core/windows/__init__.py,sha256=M2yOPgFwbZl3SpSI2ME2BW4rRl7JQ9OzeQSR2orDhUc,22
-pyarmor/cli/core/windows/x86/pyarmor_runtime.pyd,sha256=9M_bB7sCkC_P08anBz14b4rsbE-GKyA6QVFJ9oRzT0g,777742
-pyarmor/cli/core/windows/x86/pytransform3.pyd,sha256=yngEz_ag1fSyknR7l_HfFUBXt8WZS1wxSUBlEjqGuo4,593920
-pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd,sha256=ZzDuT7fvPXor-yz70gCZAJbxogjppwBazF3wK9xVdNE,632832
-pyarmor/cli/core/windows/x86_64/pytransform3.pyd,sha256=0lpxwkcaoqCKtwByBrsWEkBwvhWWOR98Satx-x2zc7Q,455168
-pyarmor.cli.core.windows-6.5.1.dist-info/METADATA,sha256=ZBwY8X4kGYWyRXlBY6n_pYYudOAi7nokOQjn14XnRb0,808
-pyarmor.cli.core.windows-6.5.1.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
-pyarmor.cli.core.windows-6.5.1.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
-pyarmor.cli.core.windows-6.5.1.dist-info/RECORD,,
+pyarmor/cli/core/windows/__init__.py,sha256=gENTOkeGBCl4dD88mlntlFgOi31MUMP-EP2jNQnCgts,22
+pyarmor/cli/core/windows/x86/pyarmor_runtime.pyd,sha256=2REMi2joGq2DMMeFU8cqsjriGPecJRa6_WP8N_euxpk,777742
+pyarmor/cli/core/windows/x86/pytransform3.pyd,sha256=PsbdT3r1XznOePL4H2_MR0QhJ3lQTvOfkpLd8x6ZNUs,594432
+pyarmor/cli/core/windows/x86_64/pyarmor_runtime.pyd,sha256=UpV3F8GaPRdLSc2XdMtr3TULRKx8kZxQyGcPacidMZo,632832
+pyarmor/cli/core/windows/x86_64/pytransform3.pyd,sha256=KcRPCNkuI6PQ9m3hCZqd6Ov_yjz7J7hou9f-cVOQn5o,455168
+pyarmor.cli.core.windows-6.5.2.dist-info/METADATA,sha256=b-RnA488QW09OeG6AWkTxPoI6sCg5TXRZwXoDtz1-Fw,808
+pyarmor.cli.core.windows-6.5.2.dist-info/WHEEL,sha256=QbbyyBnlPXzoGKd-349G69XkCwSd1NFnt4kuAN58gNs,93
+pyarmor.cli.core.windows-6.5.2.dist-info/top_level.txt,sha256=UE1ovZ_90YzwF_lZ3LV7o8HKLe-RgzUaUUvdH5UTUus,8
+pyarmor.cli.core.windows-6.5.2.dist-info/RECORD,,
```

