# Comparing `tmp/enigma_workflow_14-14.0.8-cp39-cp39-win_amd64.whl.zip` & `tmp/enigma_workflow_14-14.0.9-cp39-cp39-macosx_11_0_arm64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 161212 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   698880 b- defN 24-May-31 07:49 enigma_workflow_14.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2182 b- defN 24-May-31 07:49 enigma_workflow_14-14.0.8.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      260 b- defN 24-May-31 07:49 enigma_workflow_14-14.0.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 24-May-31 07:49 enigma_workflow_14-14.0.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       19 b- defN 24-May-31 07:49 enigma_workflow_14-14.0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      542 b- defN 24-May-31 07:49 enigma_workflow_14-14.0.8.dist-info/RECORD
-6 files, 701983 bytes uncompressed, 160222 bytes compressed:  77.2%
+Zip file size: 175240 bytes, number of entries: 7
+drwxr-xr-x  2.0 unx        0 b- stor 24-Jun-01 00:33 enigma_workflow_14-14.0.9.dist-info/
+-rwxr-xr-x  2.0 unx   813480 b- defN 24-Jun-01 00:33 enigma_workflow_14.cpython-39-darwin.so
+-rw-rw-r--  2.0 unx      550 b- defN 24-Jun-01 00:33 enigma_workflow_14-14.0.9.dist-info/RECORD
+-rw-r--r--  2.0 unx     2182 b- defN 24-Jun-01 00:33 enigma_workflow_14-14.0.9.dist-info/LICENSE
+-rw-r--r--  2.0 unx      108 b- defN 24-Jun-01 00:33 enigma_workflow_14-14.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       19 b- defN 24-Jun-01 00:33 enigma_workflow_14-14.0.9.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      250 b- defN 24-Jun-01 00:33 enigma_workflow_14-14.0.9.dist-info/METADATA
+7 files, 816589 bytes uncompressed, 174098 bytes compressed:  78.7%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
-Filename: enigma_workflow_14.cp39-win_amd64.pyd
+Filename: enigma_workflow_14-14.0.9.dist-info/
 Comment: 
 
-Filename: enigma_workflow_14-14.0.8.dist-info/LICENSE
+Filename: enigma_workflow_14.cpython-39-darwin.so
 Comment: 
 
-Filename: enigma_workflow_14-14.0.8.dist-info/METADATA
+Filename: enigma_workflow_14-14.0.9.dist-info/RECORD
 Comment: 
 
-Filename: enigma_workflow_14-14.0.8.dist-info/WHEEL
+Filename: enigma_workflow_14-14.0.9.dist-info/LICENSE
 Comment: 
 
-Filename: enigma_workflow_14-14.0.8.dist-info/top_level.txt
+Filename: enigma_workflow_14-14.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: enigma_workflow_14-14.0.8.dist-info/RECORD
+Filename: enigma_workflow_14-14.0.9.dist-info/top_level.txt
+Comment: 
+
+Filename: enigma_workflow_14-14.0.9.dist-info/METADATA
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `enigma_workflow_14-14.0.8.dist-info/LICENSE` & `enigma_workflow_14-14.0.9.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `enigma_workflow_14-14.0.8.dist-info/RECORD` & `enigma_workflow_14-14.0.9.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-enigma_workflow_14.cp39-win_amd64.pyd,sha256=PlUhhdDGrayf3gjBbwo1zSdi96ls9XH-Ona_9KDU56Y,698880
-enigma_workflow_14-14.0.8.dist-info/LICENSE,sha256=SBNiCMUPOkN74CrKaGEJk1CNXzPemZ76Qsm106kwI1E,2182
-enigma_workflow_14-14.0.8.dist-info/METADATA,sha256=zb0rFe06l6U4pxTPHbRnHBZAxnwKWpjt3PcaUb9jwA8,260
-enigma_workflow_14-14.0.8.dist-info/WHEEL,sha256=Z6c-bE0pUM47a70GvqO_SvH_XXU0lm62gEAKtoNJ08A,100
-enigma_workflow_14-14.0.8.dist-info/top_level.txt,sha256=cLiZF96feP4ElnLoCeAjzRCrgiOZAGlm2jVcJtpJwmI,19
-enigma_workflow_14-14.0.8.dist-info/RECORD,,
+enigma_workflow_14.cpython-39-darwin.so,sha256=HZ3fNSdoW_mTezY0QvrHyEvkMXeAFf0AO_ckGko_iR0,813480
+enigma_workflow_14-14.0.9.dist-info/RECORD,,
+enigma_workflow_14-14.0.9.dist-info/LICENSE,sha256=SBNiCMUPOkN74CrKaGEJk1CNXzPemZ76Qsm106kwI1E,2182
+enigma_workflow_14-14.0.9.dist-info/WHEEL,sha256=t3aNIuHimB-eyeerOmc50nLML0b4_R6yjydcdcJkGHg,108
+enigma_workflow_14-14.0.9.dist-info/top_level.txt,sha256=cLiZF96feP4ElnLoCeAjzRCrgiOZAGlm2jVcJtpJwmI,19
+enigma_workflow_14-14.0.9.dist-info/METADATA,sha256=IFv26XkYiqsz9x-Lv_LdQSxb-MZgbD2ArYcrjWoIkPc,250
```

