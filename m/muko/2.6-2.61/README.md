# Comparing `tmp/muko-2.6-py3-none-any.whl.zip` & `tmp/muko-2.61-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 4058310 bytes, number of entries: 10
+Zip file size: 4058322 bytes, number of entries: 10
 -rw-rw-rw-  2.0 fat       20 b- defN 24-Mar-13 17:30 muko/__init__.py
--rw-rw-rw-  2.0 fat  1021952 b- defN 24-Jun-01 11:04 muko/cmuko.cp38-win_amd64.pyd
+-rw-rw-rw-  2.0 fat  1021952 b- defN 24-Jun-01 11:05 muko/cmuko.cp38-win_amd64.pyd
 -rw-rw-rw-  2.0 fat  1575400 b- defN 24-Jun-01 11:04 muko/cmuko.cpython-38-darwin.so
 -rw-rw-rw-  2.0 fat  5818368 b- defN 24-May-25 13:12 muko/cmuko.so
 -rw-rw-rw-  2.0 fat  2082964 b- defN 24-Feb-08 07:11 muko/font/default.otf
--rw-rw-rw-  2.0 fat     1074 b- defN 24-Jun-01 11:04 muko-2.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1422 b- defN 24-Jun-01 11:04 muko-2.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-01 11:04 muko-2.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        5 b- defN 24-Jun-01 11:04 muko-2.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      765 b- defN 24-Jun-01 11:04 muko-2.6.dist-info/RECORD
-10 files, 10502062 bytes uncompressed, 4057040 bytes compressed:  61.4%
+-rw-rw-rw-  2.0 fat     1074 b- defN 24-Jun-01 11:05 muko-2.61.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1423 b- defN 24-Jun-01 11:05 muko-2.61.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Jun-01 11:05 muko-2.61.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        5 b- defN 24-Jun-01 11:05 muko-2.61.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      770 b- defN 24-Jun-01 11:05 muko-2.61.dist-info/RECORD
+10 files, 10502068 bytes uncompressed, 4057042 bytes compressed:  61.4%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: muko/cmuko.so
 Comment: 
 
 Filename: muko/font/default.otf
 Comment: 
 
-Filename: muko-2.6.dist-info/LICENSE
+Filename: muko-2.61.dist-info/LICENSE
 Comment: 
 
-Filename: muko-2.6.dist-info/METADATA
+Filename: muko-2.61.dist-info/METADATA
 Comment: 
 
-Filename: muko-2.6.dist-info/WHEEL
+Filename: muko-2.61.dist-info/WHEEL
 Comment: 
 
-Filename: muko-2.6.dist-info/top_level.txt
+Filename: muko-2.61.dist-info/top_level.txt
 Comment: 
 
-Filename: muko-2.6.dist-info/RECORD
+Filename: muko-2.61.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `muko-2.6.dist-info/LICENSE` & `muko-2.61.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `muko-2.6.dist-info/METADATA` & `muko-2.61.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: muko
-Version: 2.6
+Version: 2.61
 Summary: 加速实现AIGC、自动办公的中文编程工具
 Home-page: https://www.mikooo.cn
 Author: Milk
 Author-email: 719496375@qq.com
 License: The MIT License
 Platform: win64
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `muko-2.6.dist-info/RECORD` & `muko-2.61.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 muko/__init__.py,sha256=CCRGa1csLmHKI_CslhtoPnqhEJA3mszIsRjACQuz5iE,20
-muko/cmuko.cp38-win_amd64.pyd,sha256=eOG62Nlid670ETmzmW3_vMV-_3pOjTDJDmfPHZ-7fQI,1021952
+muko/cmuko.cp38-win_amd64.pyd,sha256=bQtLDlLcUSIUQD765M69EiBxG9xFZ4yzyOBk9vCVObM,1021952
 muko/cmuko.cpython-38-darwin.so,sha256=DMORP81_SracJQuacJGqXYwpXKCx-k8EFnEzo0s0l2s,1575400
 muko/cmuko.so,sha256=70avgde5s4_WavR3f197DOe5iLWPN__96jaGksqn1W0,5818368
 muko/font/default.otf,sha256=ZMqD7VMsbmTwwTRN4d72gVQLIekvjl5SSCvxs8-O4GA,2082964
-muko-2.6.dist-info/LICENSE,sha256=RwagnXR-4KxFgkvsh5PWaPhlca1CH_BNf-ozi5vp0fw,1074
-muko-2.6.dist-info/METADATA,sha256=AkY6KF_jcmtURpJ54YxwVOf27Fm_QPS-QAD-lFhf6U8,1422
-muko-2.6.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-muko-2.6.dist-info/top_level.txt,sha256=fp2J4q9iyOPhu1UrXQqzVFSagtatDPDXHXAFWfVJk2M,5
-muko-2.6.dist-info/RECORD,,
+muko-2.61.dist-info/LICENSE,sha256=RwagnXR-4KxFgkvsh5PWaPhlca1CH_BNf-ozi5vp0fw,1074
+muko-2.61.dist-info/METADATA,sha256=1rbO4bOePfJITX3yjPpjGdLbzcKT0tJOfuwwFm_4J4I,1423
+muko-2.61.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
+muko-2.61.dist-info/top_level.txt,sha256=fp2J4q9iyOPhu1UrXQqzVFSagtatDPDXHXAFWfVJk2M,5
+muko-2.61.dist-info/RECORD,,
```

