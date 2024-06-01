# Comparing `tmp/sc3dg-0.0.4.tar.gz` & `tmp/sc3dg-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sc3dg-0.0.4.tar", last modified: Sat Jun  1 10:13:05 2024, max compression
+gzip compressed data, was "sc3dg-0.0.5.tar", last modified: Sat Jun  1 10:19:47 2024, max compression
```

## Comparing `sc3dg-0.0.4.tar` & `sc3dg-0.0.5.tar`

### file list

```diff
@@ -1,39 +1,35 @@
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:13:05.000000 sc3dg-0.0.4/
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 10:13:05.000000 sc3dg-0.0.4/PKG-INFO
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9859 2024-06-01 08:07:24.000000 sc3dg-0.0.4/README.md
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:13:05.000000 sc3dg-0.0.4/sc3dg/
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2023-12-22 13:39:36.000000 sc3dg-0.0.4/sc3dg/__init__.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5510 2024-06-01 10:01:05.000000 sc3dg-0.0.4/sc3dg/main.py
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:13:05.000000 sc3dg-0.0.4/sc3dg/utils/
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2951 2023-12-22 13:39:38.000000 sc3dg-0.0.4/sc3dg/utils/Generate_scNanoHIC_pairs.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1361 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/ReformSAM.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      110 2024-06-01 10:12:53.000000 sc3dg-0.0.4/sc3dg/utils/__init__.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      179 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/_version.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10612 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/analysis.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     8049 2023-12-22 13:39:38.000000 sc3dg-0.0.4/sc3dg/utils/assembly.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)       72 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/correct.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3026 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/download.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3706 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/embedding.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10805 2023-12-22 13:39:38.000000 sc3dg-0.0.4/sc3dg/utils/general.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1282 2023-12-22 13:39:38.000000 sc3dg-0.0.4/sc3dg/utils/help.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    30787 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/hicCorrectMatrix.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3231 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/iterativeCorrection.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9663 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/plot.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7430 2023-12-22 13:44:16.000000 sc3dg-0.0.4/sc3dg/utils/scNano.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1423 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/scNano_barcode.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    14322 2024-01-11 01:46:15.000000 sc3dg-0.0.4/sc3dg/utils/scSPRITE.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    25129 2024-01-04 01:09:13.000000 sc3dg-0.0.4/sc3dg/utils/scaffold.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12463 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/sciHic.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12331 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/sn_m3c.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5268 2023-12-22 13:57:33.000000 sc3dg-0.0.4/sc3dg/utils/tools.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    22875 2023-12-22 13:39:38.000000 sc3dg-0.0.4/sc3dg/utils/utilities.py
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2722 2023-12-22 13:39:37.000000 sc3dg-0.0.4/sc3dg/utils/visualize.py
-drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:13:05.000000 sc3dg-0.0.4/sc3dg.egg-info/
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 10:13:04.000000 sc3dg-0.0.4/sc3dg.egg-info/PKG-INFO
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      804 2024-06-01 10:13:05.000000 sc3dg-0.0.4/sc3dg.egg-info/SOURCES.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)        1 2024-06-01 10:13:04.000000 sc3dg-0.0.4/sc3dg.egg-info/dependency_links.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)       42 2024-06-01 10:13:04.000000 sc3dg-0.0.4/sc3dg.egg-info/entry_points.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)      605 2024-06-01 10:13:04.000000 sc3dg-0.0.4/sc3dg.egg-info/requires.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)        6 2024-06-01 10:13:04.000000 sc3dg-0.0.4/sc3dg.egg-info/top_level.txt
--rw-r--r--   0 Kangwen   (1041) wulab     (1006)       38 2024-06-01 10:13:05.000000 sc3dg-0.0.4/setup.cfg
--rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      435 2021-02-01 02:43:23.000000 sc3dg-0.0.4/setup.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:19:47.000000 sc3dg-0.0.5/
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 10:19:47.000000 sc3dg-0.0.5/PKG-INFO
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9859 2024-06-01 08:07:24.000000 sc3dg-0.0.5/README.md
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:19:47.000000 sc3dg-0.0.5/sc3dg/
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2023-12-22 13:39:36.000000 sc3dg-0.0.5/sc3dg/__init__.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5510 2024-06-01 10:01:05.000000 sc3dg-0.0.5/sc3dg/main.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:19:47.000000 sc3dg-0.0.5/sc3dg/utils/
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2951 2024-06-01 10:18:22.000000 sc3dg-0.0.5/sc3dg/utils/Generate_scNanoHIC_pairs.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1361 2024-06-01 10:18:22.000000 sc3dg-0.0.5/sc3dg/utils/ReformSAM.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      133 2024-06-01 10:19:40.000000 sc3dg-0.0.5/sc3dg/utils/__init__.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10612 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/analysis.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7503 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/assembly.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2555 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/download.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     3706 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/embedding.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    10805 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/general.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1282 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/help.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     9663 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/plot.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    15197 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/scMethyl.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     7287 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/scNano.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     1423 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/scNano_barcode.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    13736 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/scSPRITE.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    25080 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/scaffold.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12463 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/sciHic.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)    12315 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/sn_m3c.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     5223 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/tools.py
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)     2722 2024-06-01 10:18:23.000000 sc3dg-0.0.5/sc3dg/utils/visualize.py
+drwxr-xr-x   0 Kangwen   (1041) wulab     (1006)        0 2024-06-01 10:19:47.000000 sc3dg-0.0.5/sc3dg.egg-info/
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      117 2024-06-01 10:19:46.000000 sc3dg-0.0.5/sc3dg.egg-info/PKG-INFO
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      689 2024-06-01 10:19:46.000000 sc3dg-0.0.5/sc3dg.egg-info/SOURCES.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)        1 2024-06-01 10:19:46.000000 sc3dg-0.0.5/sc3dg.egg-info/dependency_links.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)       42 2024-06-01 10:19:46.000000 sc3dg-0.0.5/sc3dg.egg-info/entry_points.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)      605 2024-06-01 10:19:46.000000 sc3dg-0.0.5/sc3dg.egg-info/requires.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)        6 2024-06-01 10:19:46.000000 sc3dg-0.0.5/sc3dg.egg-info/top_level.txt
+-rw-r--r--   0 Kangwen   (1041) wulab     (1006)       38 2024-06-01 10:19:47.000000 sc3dg-0.0.5/setup.cfg
+-rwxr-xr-x   0 Kangwen   (1041) wulab     (1006)      435 2021-02-01 02:48:55.000000 sc3dg-0.0.5/setup.py
```

### Comparing `sc3dg-0.0.4/README.md` & `sc3dg-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.4/sc3dg/main.py` & `sc3dg-0.0.5/sc3dg/main.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.4/sc3dg/utils/Generate_scNanoHIC_pairs.py` & `sc3dg-0.0.5/sc3dg/utils/Generate_scNanoHIC_pairs.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.4/sc3dg/utils/ReformSAM.py` & `sc3dg-0.0.5/sc3dg/utils/ReformSAM.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.4/sc3dg/utils/analysis.py` & `sc3dg-0.0.5/sc3dg/utils/analysis.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.4/sc3dg/utils/assembly.py` & `sc3dg-0.0.5/sc3dg/utils/assembly.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,50 +3,51 @@
 import numpy as np
 import subprocess
 import time
 import os
 import logging
 from .scaffold import *
 import pandas as pd
-
+from joblib import Parallel, delayed
 def assembly(type_,opt, fastq,log_out):
 
     print('********run %s || %s*********' % (type_, fastq))
     # 移动到工作目录
     os.chdir(opt['output'])
     # print(opt)
     start = time.time()
  
 
     # 创建文件夹tmp,并移动
-    os.makedirs(opt['type'] + '_' + fastq + '_tmp', exist_ok=True)
+    if not os.path.exists(opt['type'] + '_' + fastq + '_tmp'): # scHic_sample_tmp
+        os.makedirs(opt['type'] + '_' + fastq + '_tmp')
     os.chdir(opt['type'] + '_' + fastq + '_tmp')
-    os.makedirs('./Result/mcool_folder', exist_ok=True)
-    os.makedirs('./Result/cool_folder', exist_ok=True)
-    os.makedirs('./Result/SCpair', exist_ok=True)
 
+   
+    
     
     # 创建logging文件
     logging.basicConfig(filename=fastq + '_logging.log', level=logging.DEBUG)
     for k in opt.keys():
 
      
         if (k == 'fastq_dir') or (k == 'fastq_log') or (k == 'run_sample'):
             continue
         else:
             logging.debug('# ' + k + ': ' + str(opt[k]))
         
-    if os.path.exists(opt['output'] + '/' + opt['type'] + '_' + fastq + '_tmp/Result/' + fastq +'.mcool'):
+    if os.path.exists(opt['output'] + '/' + opt['type'] + '_' + fastq + '_tmp/' + fastq +'.bam'):
         log_out.info('The result of ' + fastq + ' has been generated')
-        print('==========generated+++++++')
-        return
+        pass
+        # print('==========generated+++++++')
+        # return
     if os.path.exists(opt['output'] + '/' + opt['type'] + '_' + fastq + '_tmp/Result/SCpair'):
-        for val in os.listdir(opt['output'] + '/' + opt['type'] + '_' + fastq + '_tmp/Result/mcool_folder'):
+        for val in os.listdir(opt['output'] + '/' + opt['type'] + '_' + fastq + '_tmp/Result/SCpair'):
             if val.endswith('.mcool'):
-                print('==========generated+++++++')
+                # print('==========generated+++++++')
                 return
 
     
     
     
 
 
@@ -67,14 +68,16 @@
             return
     
     threads = opt['thread']
 
     
     if not os.path.exists('Result'):
         os.makedirs('Result')
+    
+
 
     # 默认inner和outer barcode和fastq文件放在一个目录下面
     if type_ == 'sciHic':
         opt['inner-barcode'] = os.path.dirname(opt['fastq_dir'][opt['fastq_log'].index(fastq)]) + '/' + fastq + '_inner_barcodes.txt'
         opt['outer-barcode'] = os.path.dirname(opt['fastq_dir'][opt['fastq_log'].index(fastq)]) + '/' + fastq + '_outer_barcodes.txt'
 
 
@@ -174,60 +177,47 @@
     t = pairtools_sort(fastq)
     logging.info('pairtools_sort::: %s '%t)
 
     # pairtools dedup
     t = pairtools_dedup(fastq,str(opt['max_mismatch']))
     logging.info('pairtools_dedup::: %s '%t)
 
-    
+    # 整体的mcool
+    t = cooler_cload_pairs(opt['genomesize'],
+                            str(opt['resolution']),
+                            fastq
+                            ,prefix='dedup'
+                            )
+    logging.info('cooler_cload_pairs::: %s '%t)
+
+    # t = KR_correctMatrix(fastq,str(opt['resolution']) )
+    # logging.info('KR_correctMatrix::: %s '%t)
 
+    t = cooelr_zoomify(fastq,opt['resolution'], opt['zoomify_res'])
+    logging.info('cooelr_zoomify::: %s '%t)
+
+    # print(34534534534)
     if opt['exist_barcode']:
         split_cells(fastq)
         t = time.time()
+        pair_list = []
         for p in os.listdir('./Result/SCpair'):
             if p.endswith('pairs.gz'):
-       
-                cload_correct_zoomify('./Result/SCpair/',
+                pair_list.append(p)
+    
+        Parallel(n_jobs=6)(delayed(cload_correct_zoomify)('./Result/SCpair/',
                                       p,
                                       opt['genomesize'],
                                       str(opt['resolution']),
                                        opt['zoomify_res']
-                                      )
+                            ) for p in pair_list)
         logging.info('sub_cload_correct_zoomify::: %s '% (time.time() - t))
-    else:
-        # 整体的mcool
-        t = cooler_cload_pairs(opt['genomesize'],
-                                str(opt['resolution']),
-                                fastq
-                                ,prefix='dedup'
-                                )
-        logging.info('cooler_cload_pairs::: %s '%t)
-
-        t = KR_correctMatrix(fastq,str(opt['resolution']) )
-        logging.info('KR_correctMatrix::: %s '%t)
-
-        t = cooelr_zoomify(fastq,opt['resolution'], opt['zoomify_res'])
-        logging.info('cooelr_zoomify::: %s '%t)
  
-    os.system('mv ./*.mcool ./Result/mcool_folder/')
-    os.system('mv ./*.cool ./Result/cool_folder/')
-    os.system('mv ./*restrict.pairs.gz ./Result/SCpair/')
-    os.system('mv ./%s.pairs.gz ./Result/SCpair/'%fastq)
-    os.system('mv ./Result/SCpair/*.mcool ./Result/mcool_folder')
-    os.system('mv ./Result/SCpair/*.cool ./Result/cool_folder')
-    for val in os.listdir('./'):
-        if not os.path.isdir(val):
-            if val == fastq + '_logging.log' or val == fastq + '.bam' or val == fastq + '.qc.bam' or val == fastq + '.merged.bam' or val =='trimmed.fastp.json':
-                continue
-            else:
-                print(val)
-                os.remove(val)
-
-
-    
+    mv_Result()
+    # pd.DataFrame(time_log, index=list(time_log.keys())).to_csv('time_log.csv', index=None, sep='\t')
     logging.info('total time: %s' % (time.time() - start))
```

### Comparing `sc3dg-0.0.4/sc3dg/utils/download.py` & `sc3dg-0.0.5/sc3dg/utils/download.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,25 +11,21 @@
 chromosome_size_url = {
     'mm10':'https://hgdownload.soe.ucsc.edu/goldenPath/mm10/bigZips/mm10.chrom.sizes',
     'mm9':'https://hgdownload.soe.ucsc.edu/goldenPath/mm9/bigZips/mm9.chrom.sizes',
     'mm39':'https://hgdownload.soe.ucsc.edu/goldenPath/mm39/bigZips/mm39.chrom.sizes',
     'hg38':'https://hgdownload.soe.ucsc.edu/goldenPath/hg38/bigZips/hg38.chrom.sizes',
     'hg19':'https://hgdownload.soe.ucsc.edu/goldenPath/hg19/bigZips/hg19.chrom.sizes'
 }
-sprite_java = 'https://github.com/caltech-bioinformatics-resource-center/Guttman_Ismagilov_Labs/blob/master/scSPRITE/misc/sprite-pipeline/java/BarcodeIdentification_v1.2.0.jar'
 
-def make_index(path, version='hg38', aligner='bwa', enzyme=None):
+
+def make_index(path, version='hg38', aligner='bwa'):
     if not os.path.exists(path):
         os.makedirs(path)
 
     os.chdir(path)
-    
-    # 下载sprite-config
-    cmd = 'wget %s' % sprite_java
-    os.system(cmd)
 
     # 下载fa
     cmd = 'wget %s' % genome_url[version]
     os.system(cmd)
 
     cmd = 'wget %s' % chromosome_size_url[version]
     os.system(cmd)
@@ -38,23 +34,16 @@
         cmd = 'bwa index %s.fa.gz' % version
         os.system(cmd)
     elif aligner == 'bowtie2':
         cmd = 'bowite2 index %s.fa.gz %s' % (version, version)
         os.system(cmd)
     else:
         sys.exit('aligner should be bwa/bowtie2')
-    print('index done')
-    print('=====================')
-    print('generate enzyme bed')
-    for enz in enzyme.split(','):
-        enz = enz.strip()
-    make_digest(path, enzyme=enz,genome=version)
-
-
 
+    
 def make_digest(path, enzyme='MboI',genome='hg38'):
     if not os.path.exists(path):
         sys.exit('path is not exist')
     print(os.path.exists(path + '/%s.fa' % genome))
     if not os.path.exists(path + '/%s.fa.gz' % genome) and not os.path.exists(path + '/%s.fa' % genome):
         sys.exit('you should run index first')
     if not os.path.exists(path + '/%s.fa.chrom.sizes' % genome):
```

### Comparing `sc3dg-0.0.4/sc3dg/utils/embedding.py` & `sc3dg-0.0.5/sc3dg/utils/embedding.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.4/sc3dg/utils/general.py` & `sc3dg-0.0.5/sc3dg/utils/general.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.4/sc3dg/utils/help.py` & `sc3dg-0.0.5/sc3dg/utils/help.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.4/sc3dg/utils/plot.py` & `sc3dg-0.0.5/sc3dg/utils/plot.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.4/sc3dg/utils/scNano.py` & `sc3dg-0.0.5/sc3dg/utils/scNano.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,17 +9,16 @@
 import time
 import logging
 from pathlib import Path
 from .scNano_barcode import generate_barcode
 from .ReformSAM import reSAM
 from .Generate_scNanoHIC_pairs import WriteCellPairs
 from multiprocessing import Pool
-current_file_path = os.path.abspath(__file__)
-hicCorrectMatrix = os.path.dirname(current_file_path) + '/' + 'correct.py'
-hicCorrectMatrix = 'python ' + hicCorrectMatrix + ' '
+barcodesh = '/cluster/home/Kangwen/Hic/ckw/utils/barcode.sh'
+
 def run_command(command):
     print(command)
     subprocess.run(command, shell=True, timeout=None)
     
 
 def pp(opt, fastq,log_out):
     print('==========run scNano================')
@@ -99,15 +98,15 @@
         print(out, divide_list[i])
         generate_barcode(divide_list[i],PCR, TN5,out)
     
     for fa in bcname:
         node = time.time()
         print(fa)
         cmd = 'nanoplexer -b %s -B 200M -t %s -p %s %s' % (fa, opt['thread'],raw_folder, fq)
-        run_command(cmd)
+        # run_command(cmd)
         print('nanoplexer:%s'% (time.time() - node))
 
     
     # 第一步: 运行 cutadapt 处理所有文件
     for file_name in os.listdir(raw_folder):
         if file_name.endswith(".fastq"):
             input_file = os.path.join(raw_folder, file_name)
@@ -169,14 +168,10 @@
             resolution = int(opt['resolution'])
             cool_file = os.path.join(cool_folder, f"{file_name}.{resolution}.cool")
             KR_cool_file = os.path.join(KRcool_folder, f"{file_name}.{resolution}.KR.cool")
             mcool_file = os.path.join(mcool_folder, f"{file_name}.mcool")
             # 执行 cooler 和 hicCorrectMatrix 命令
             chrom_size = opt['genomesize']
             subprocess.run(["cooler", "cload", "pairs", "-c1", "2", "-p1", "3", "-c2", "4", "-p2", "5", f"{chrom_size}:{resolution}", sorted_pairs, cool_file])
-            cmd = '%s correct --matrix  ' % hicCorrectMatrix + cool_file 
-            cmd += ' --correctionMethod KR --outFileName '
-            cmd += ' ' + KR_cool_file
-            cmd += ' --filterThreshold -1.5 5.0 --chromosomes chr1 chr2 chr3 chr4 chr5 chr6 chr7 chr8 chr9 chr10 chr11 chr12 chr13 chr14 chr15 chr16 chr17 chr18 chr19'
-            print(cmd)
-            os.system(cmd)
-            subprocess.run(['cooler', 'zoomify', KR_cool_file,'-r', opt['zoomify_res'], '-o', mcool_file]) 
+            subprocess.run(["hicCorrectMatrix", "correct", "--matrix", cool_file, "--correctionMethod", "KR", "--outFileName", KR_cool_file, "--filterThreshold", "-1.5", "5.0", "--chromosomes", "chr1", "chr2", "chr3", "chr4", "chr5", "chr6", "chr7", "chr8", "chr9", "chr10", "chr11", "chr12", "chr13", "chr14", "chr15", "chr16", "chr17", "chr18", "chr19"])
+
+            subprocess.run(['cooler', 'zoomify', KR_cool_file,'-r', opt['zoomify_res'], '-o', mcool_file])
```

### Comparing `sc3dg-0.0.4/sc3dg/utils/scNano_barcode.py` & `sc3dg-0.0.5/sc3dg/utils/scNano_barcode.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.4/sc3dg/utils/scSPRITE.py` & `sc3dg-0.0.5/sc3dg/utils/scSPRITE.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,73 +7,66 @@
 import pandas as pd
 import subprocess
 import time
 import logging
 
 
 from multiprocessing import Pool
+
+
 # jar_dir = sys.prefix + '/inHic' 
 # jar_path = jar_dir + '/utils/BarcodeIdentification_v1.2.0.jar'
-current_file_path = os.path.abspath(__file__)
-hicCorrectMatrix = os.path.dirname(current_file_path) + '/' + 'correct.py'
-hicCorrectMatrix = 'python ' + hicCorrectMatrix
+jar_path = '/cluster/home/Kangwen/Hic/seq/4_scSPRITE/Code/BarcodeIdentification_v1.2.0.jar'
 
 def pp(opt, fastq,log_out):
     print('====================scSPRITE====================')
     T = time.time()
     # 移动到工作目录
     os.chdir(opt['output'])
 
     # 创建文件夹tmp,并移动
     if not os.path.exists(opt['type'] + '_' + fastq + '_tmp'): # scHic_sample_tmp
         os.makedirs(opt['type'] + '_' + fastq + '_tmp')
     output = opt['output'] + '/' +opt['type'] + '_' + fastq + '_tmp'
     os.chdir(opt['type'] + '_' + fastq + '_tmp')
-    os.makedirs('./Result', exist_ok=True)
-    
-    os.makedirs('./Result/SCpair', exist_ok=True)
-    os.makedirs('./Result/mcool_folder/', exist_ok=True)
-    os.makedirs('./Result/cool_folder/', exist_ok=True)
+
     fq_r1 = opt['fastq_dir'][opt['fastq_log'].index(fastq)]
     fq_r2 = fq_r1.replace('_1.fastq', '_2.fastq')
 
     # 创建log
     logging.basicConfig(filename=fastq + '_logging.log', level=logging.DEBUG)
     for k in opt.keys():
 
      
         if (k == 'fastq_dir') or (k == 'fastq_log') or (k == 'run_sample'):
             continue
         else:
             logging.debug('# ' + k + ': ' + str(opt[k]))
     
     
+    os.makedirs('./Result', exist_ok=True)
     
+    os.makedirs('./Result/SCpair', exist_ok=True)
+    os.makedirs('./Result/mcool_folder/', exist_ok=True)
+    os.makedirs('./Result/cool_folder/', exist_ok=True)
     for val in os.listdir(opt['output'] + '/' + opt['type'] + '_' + fastq + '_tmp/Result/mcool_folder/'):
         if val.endswith('mcool'):
-            print('==========generated+++++++')
-            return
-    jar_path = ''
-    for val in os.listdir(os.path.dirname(opt['index'])):
-        if val.endswith('jar'):
-            jar_path = os.path.dirname(opt['index']) + '/' + val
-            break
-    if jar_path == '':
-        print('no jar file')
-        sys.exit('no jar file')
+            pass
+            # print('==========generated+++++++')
+            # return
  
     # Generate Barcode Reads
     cmd = 'java -jar ' + jar_path
     cmd += ' ' + '--input1 ' + fq_r1 + ' --input2 ' + fq_r2
     cmd += ' ' + '--output1 ' + fastq + '_1_barcode.fastq.gz'
     cmd += ' ' + '--output2  ' + fastq + '_2_barcode.fastq.gz'
     cmd += ' --config ' + opt['sprite_config']
     t = time.time()
     logging.info(cmd)
-    os.system(cmd)
+    # os.system(cmd)
     logging.info('BarcodeIdentification time: ' + str(time.time() - t))
 
     # Get paird fastq
     cmd = 'fastp --overrepresentation_analysis'
     cmd += ' --correction --thread ' + str(opt['thread'])
     cmd += ' --html trimmed.fastp.html '
     cmd += ' --json trimmed.fastp.json '
@@ -115,24 +108,25 @@
     logging.info('align time: ' + str(time.time() - t))
 
     # sam to bam
     cmd = 'samtools view -@ 8 -S ' + fastq + '.sam -b -o ' + fastq + '.bam'
     t = time.time()
     logging.info(cmd)
     os.system(cmd)
-    logging.info('sam to bam time: ' + str(time.time() - t))
+    logging.info('sam to bam time: ' + str(time.time() - t))  
 
     qc = opt['qc']
 
+    print(123)
 
     cmd = 'samtools view -h -@ ' + str(opt['thread'])
     if qc == 0 :
-        cmd += ' -b  ' + fastq + '.bam > ' + fastq + '.filtered.bam'
+        cmd += ' -b ' + fastq + '.bam > ' + fastq + '.filtered.bam'
     else:
-        cmd += ' -b -q %s' % qc + fastq + '.bam > ' + fastq + '.filtered.bam'
+        cmd += ' -b -q  %s ' % qc + fastq + '.bam > ' + fastq + '.filtered.bam'
     t = time.time()
     logging.info(cmd)
     os.system(cmd)
     logging.info('samtools view time: ' + str(time.time() - t))
 
     cmd = 'bedtools intersect -v -a ' + fastq + '.filtered.bam'
     cmd += ' -b ' + opt['repeat_masker'] + ' > ' + fastq + '.filtered.masked.bam'
@@ -169,55 +163,51 @@
                     'HeadInfo.txt', 
                     opt['species'], 'SCPairCellSummary.txt', 
                     'SCPairClusterSummary.txt',output)
     logging.info('WriteCellPairs time: ' + str(time.time() - t))
 
     mcool_folfer = './Result/mcool_folder'
     os.makedirs('./Result/mcool_folder', exist_ok=True)
-    for val in os.listdir('./Result/SCpair'):
-        if val.endswith('.pairs.gz') and '[' in val and ']' in val:
-            val = val.split('.')[0]
-            cmd = 'cooler cload pairs -c1 2 -p1 3 -c2 4 -p2 5 '
-            cmd += opt['genomesize'] + ':' + str(opt['resolution']) + ' ./Result/SCpair/' + val + '.pairs.gz ./Result/SCpair/' + val  + '_'+str(opt['resolution']) + '.cool'
-            t = time.time()
-            logging.info(cmd)
-            print(cmd)
-            os.system(cmd)
-            logging.info('cooler cload time: ' + str(time.time() - t))
+
+    
+    # for val in os.listdir('./Result/SCpair'):
+    #     if val.endswith('.pairs.gz') and '[' in val and ']' in val:
+    #         val = val.split('.')[0]
+    #         cmd = 'cooler cload pairs -c1 2 -p1 3 -c2 4 -p2 5 '
+    #         cmd += opt['genomesize'] + ':' + str(opt['resolution']) + ' ./Result/SCpair/' + val + '.pairs.gz ./Result/SCpair/' + val  + '_'+str(opt['resolution']) + '.cool'
+    #         t = time.time()
+    #         logging.info(cmd)
+    #         print(cmd)
+    #         os.system(cmd)
+    #         logging.info('cooler cload time: ' + str(time.time() - t))
     
 
-            cmd = '%s correct --matrix  ./Result/SCpair/'%hicCorrectMatrix + val + '_' +   str(opt['resolution']) + '.cool '
-            cmd += ' --correctionMethod KR --outFileName '
-            cmd += ' ./Result/SCpair/' + val + str(opt['resolution']) + '.KR.cool'
-            cmd += ' --filterThreshold -1.5 5.0 --chromosomes chr1 chr2 chr3 chr4 chr5 chr6 chr7 chr8 chr9 chr10 chr11 chr12 chr13 chr14 chr15 chr16 chr17 chr18 chr19'
-            print('14+++++++++++\n', cmd)
-            t = time.time()
-            logging.info(cmd)
-            os.system(cmd)
-            logging.info('hicCorrectMatrix time: ' + str(time.time() - t))
+    #         cmd = 'hicCorrectMatrix correct --matrix  ./Result/SCpair/' + val + '_' +   str(opt['resolution']) + '.cool '
+    #         cmd += ' --correctionMethod KR --outFileName '
+    #         cmd += ' ./Result/SCpair/' + val + str(opt['resolution']) + '.KR.cool'
+    #         cmd += ' --filterThreshold -1.5 5.0 --chromosomes chr1 chr2 chr3 chr4 chr5 chr6 chr7 chr8 chr9 chr10 chr11 chr12 chr13 chr14 chr15 chr16 chr17 chr18 chr19'
+    #         print('14+++++++++++\n', cmd)
+    #         t = time.time()
+    #         logging.info(cmd)
+    #         os.system(cmd)
+    #         logging.info('hicCorrectMatrix time: ' + str(time.time() - t))
         
             
 
-            cmd = 'cooler zoomify ./Result/SCpair/'  + val + str(opt['resolution']) + '.KR.cool -r 10000,40000,100000,500000 -o ./Result/mcool_folder/' + val + '.mcool'
-            print('15+++++++++++\n', cmd)
-            t = time.time()
-            logging.info(cmd)
-            os.system(cmd)
-            logging.info('cooler zoomify time: ' + str(time.time() - t))
+    #         cmd = 'cooler zoomify ./Result/SCpair/'  + val + str(opt['resolution']) + '.KR.cool -r 10000,40000,100000,500000 -o ./Result/mcool_folder/' + val + '.mcool'
+    #         print('15+++++++++++\n', cmd)
+    #         t = time.time()
+    #         logging.info(cmd)
+    #         os.system(cmd)
+    #         logging.info('cooler zoomify time: ' + str(time.time() - t))
 
 
-    os.system('mv ./Resul/SCpair/*.cool ./Result/cool_folder/')
+    os.system('mv ./Resul/SCpair/*.coowl ./Result/cool_folder/')
     os.system('mv ./Resul/SCpair/*.mcool ./Result/mcool_folder/')
-    for val in os.listdir('./'):
-        if not os.path.isdir(val):
-            if val == fastq + '_logging.log' or val == fastq + '.bam' or val == fastq + '.qc.bam' or val == fastq + '.merged.bam' or val =='trimmed.fastp.json':
-                continue
-            else:
-                print(val)
-                os.remove(val)
+    
     logging.info('Total time: ' + str(time.time() - T))
 
 
 
 def WriteSCPairCluster(ScSpriteInfo):
     PairDir = {}
     currentCell = 'None'
@@ -238,28 +228,28 @@
         ReadComponents = line.split("\t")
 
         if currentCell != ReadComponents[1]:
             CellPairCount[currentCell] = [count,0]
             count=0
             currentCell = ReadComponents[1]
 
-            if len(PairDir)> 0:
+            if len(PairDir)> 2000:
                 for key in PairDir.keys():
 
                     split_result = key.split('][')
 
                     # 获取最后符合要求的部分
                     last_three_brackets = '[' + ']['.join(split_result[-3:])
                 
                     if CellPairCount[last_three_brackets][1] ==0:
                         SCPairCellSummary.write(last_three_brackets+"\t"+str(CellPairCount[last_three_brackets][0])+"\n")
                         CellPairCount[last_three_brackets][1] = 1
 
-                    if CellPairCount[last_three_brackets][0] < 1000:
-                        continue
+                    # if CellPairCount[last_three_brackets][0] < 1000:
+                    #     continue
 
 
                     Locs = list(PairDir[key])
                     if len(Locs) < 2 or len(Locs) > 10000:
                         continue
 
                     flag = 0
@@ -293,15 +283,15 @@
 
 def WriteCellPairs(ChromSize, HeadInfo, GenomeInfo, SCPairCellSummary, SCPairClusterSummary,output):
 
     df = pd.read_csv(SCPairCellSummary, delimiter='\t', header=None)
 
     sorted_df = df.sort_values(by=df.columns[1], ascending=False)
 
-    CellList = list(sorted_df.iloc[:, 0])[0:1500]
+    CellList = list(sorted_df.iloc[:, 0])
     ProcessedCell = None
     for line in open(SCPairClusterSummary):
      
         ReadComponents = line[0:-1].split("\t")
 
         split_result = ReadComponents[0].split('][')
         # 获取最后符合要求的部分    
@@ -381,8 +371,8 @@
                 ReadsInfo.write("\t"+ReadComponent[i])
 
             count += 1
             if count % 1000000 == 0:
                 print("%d reads has processed in %f s" % (count, time.time() - startTime))
                 startTime = time.time()
         HeadInfo.close()
-        ReadsInfo.close()
+        ReadsInfo.close()
```

### Comparing `sc3dg-0.0.4/sc3dg/utils/scaffold.py` & `sc3dg-0.0.5/sc3dg/utils/scaffold.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,16 @@
 from Bio.SeqIO.QualityIO import FastqGeneralIterator
 from Bio import SeqIO
 from Levenshtein import hamming
 import gzip
 import logging
 # jar_dir = sys.prefix + '/inHic' 
 # jar_path = jar_dir + '/utils/BarcodeIdentification_v1.2.0.jar'
-current_file_path = os.path.abspath(__file__)
-hicCorrectMatrix = os.path.dirname(current_file_path) + '/' + 'correct.py'
-hicCorrectMatrix = 'python ' + hicCorrectMatrix
+jar_path = '/cluster/home/Kangwen/Hic/seq/4_scSPRITE/Code/BarcodeIdentification_v1.2.0.jar'
+
 
 
 def run_cmd_return_time(cmd):
     t = time.time()
     logging.debug(cmd)
     subprocess.run(cmd, shell=True, executable="/bin/bash")
     return time.time() - t
@@ -124,36 +123,42 @@
     if prefix is not  None:
         cmd += genomesize + ':' + str(res) + ' ' + fastq + '.%s.pairs.gz '%prefix+ fastq + '_' + str(res) + '.cool'
     else:
         cmd += genomesize + ':' + str(res) + ' ' + fastq + '.pairs.gz '+ fastq + '_' + str(res) + '.cool'
     return run_cmd_return_time(cmd)
 
 def KR_correctMatrix(fastq, res):
-    cmd = '%s correct --matrix  ' % hicCorrectMatrix + fastq + '_' + str(res) + '.cool '
+    cmd = 'hicCorrectMatrix correct --matrix  ' + fastq + '_' + str(res) + '.cool '
     cmd += ' --correctionMethod KR --outFileName '
     cmd += ' ' + fastq + '_' + str(res) + '.KR.cool'
     cmd += ' --filterThreshold -1.5 5.0 --chromosomes chr1 chr2 chr3 chr4 chr5 chr6 chr7 chr8 chr9 chr10 chr11 chr12 chr13 chr14 chr15 chr16 chr17 chr18 chr19'
     return run_cmd_return_time(cmd)
 
 def cooelr_zoomify(fastq,res, resz):
     cmd = 'cooler zoomify '  + \
         fastq + '_' +str(res) + \
-        '.KR.cool -r ' + resz + ' -o ' + fastq + '.mcool'
+        '.cool -r ' + resz + ' -o ' + fastq + '.mcool'
     return run_cmd_return_time(cmd)
 
 def find_substring_in_long_string(long_string, substrings):
     long_string = str(long_string)
     pattern = re.compile('|'.join(map(re.escape, substrings)))
     match = pattern.search(long_string)
     if match:
         return match.group()
     else:
         return None
 
-
+def mv_Result():
+    print(os.getcwd())
+    for val in os.listdir('./'):
+        if val.endswith('.mcool') or val.endswith('.cool'):
+            os.system('mv %s Result/' % val)
+        if val.endswith('.dedup.pairs.gz') or val.endswith('.restrict.pairs.gz'):
+            os.system('mv %s Result/' % val)
 
 def GetFastqIndex(srr ,Fastq1_read, Fastq2_read, Barcode1_read, Barcode2_read):
     t = time.time()
  
     Index_name = 'barcode.index'
     All_reads_count = 0
     Barcoded_Reads_count = 0
@@ -312,16 +317,16 @@
     print("*****Start generate single cell pairs files*****")
     cell_count = 0
     scPairsSummary = open("singleCell_HIC_pairs_summary.txt", "w")
     scPairsSummary.write("Cell Num" + "\t" + "Cell Barcode" + "\t" + "Pairs Count" + "\n")
     for i in range(len(SClist)):
         if len(SCPairs[SClist[i]])>1:
             scPairsSummary.write(str(i+1)+"\t"+str(SClist[i])+"\t"+str(len(SCPairs[SClist[i]]))+"\n")
-        if len(SCPairs[SClist[i]])<1000:
-            continue
+        # if len(SCPairs[SClist[i]])<1000:
+        #     continue
         cell_count+=1
         print("Process cell %d,\t"%(cell_count),end='')
         if not os.path.exists(ResultDir):
             os.mkdir(ResultDir)
         fp = gzip.open(ResultDir+"/cell_"+str(cell_count)+"_"+str(i)+".pairs.gz","w+")
         for singel_head in HeadInfo:
             fp.write(singel_head.encode('utf-8'))
@@ -372,21 +377,14 @@
                     else:
                         DirtyFile.write("Reads1\t"+line1[0:-1]+"\tReads2\t"+line2)
                 else:
                     DirtyFile.write("Reads1\t" + line1[0:-1] + "\tReads2\t" + line2)
     fp.close()
     DirtyFile.close()
 
-def sprite_java(fq1, fq2, o1,o2,  config):
-    cmd = 'java -jar ' + java_path
-    cmd += ' ' + '--input1 ' + fq1  +  ' --input2 ' + fq2 
-    cmd += ' ' + '--output1 ' + o1
-    cmd += ' ' + '--output2  ' + o2
-    cmd += ' --config ' + config
-    return run_cmd_return_time(cmd)
 
 def split(fn1, size1, size2):
     if 'gz' in fn1:
             dfh1=gzip.open(fn1,'r')
 
     if 'gz' not in fn1:
         dfh1=open(fn1,'r')
@@ -600,25 +598,25 @@
     target = dir_ + pair
     name = pair.split('.')[0]
     cmd = 'cooler cload pairs -c1 2 -p1 3 -c2 4 -p2 5 '
     cmd += genomesize + ':' + str(res) + ' ' + target + ' ' + dir_  +  name + '_' + str(res) + '.cool'
     # print(cmd)
     time1 = run_cmd_return_time(cmd)
 
-    cmd = '%s correct --matrix  ' % hicCorrectMatrix + dir_ + name + '_' + str(res) + '.cool'
-    cmd += ' --correctionMethod KR --outFileName '
-    cmd += ' ' + dir_ + name + '_' + str(res) + '.KR.cool'
-    cmd += ' --filterThreshold -1.5 5.0 --chromosomes chr1 chr2 chr3 chr4 chr5 chr6 chr7 chr8 chr9 chr10 chr11 chr12 chr13 chr14 chr15 chr16 chr17 chr18 chr19'
-    # print(cmd)
-    time1 = run_cmd_return_time(cmd)
+    # cmd = 'hicCorrectMatrix correct --matrix  ' + dir_ + name + '_' + str(res) + '.cool'
+    # cmd += ' --correctionMethod KR --outFileName '
+    # cmd += ' ' + dir_ + name + '_' + str(res) + '.KR.cool'
+    # cmd += ' --filterThreshold -1.5 5.0 --chromosomes chr1 chr2 chr3 chr4 chr5 chr6 chr7 chr8 chr9 chr10 chr11 chr12 chr13 chr14 chr15 chr16 chr17 chr18 chr19'
+    # # print(cmd)
+    # time1 = run_cmd_return_time(cmd)
 
 
     cmd = 'cooler zoomify '  + \
          dir_ + name + '_' +str(res) + \
-        '.KR.cool -r ' + resz + ' -o ' + dir_ + name + '.mcool'
+        '.cool -r ' + resz + ' -o ' + dir_ + name + '.mcool'
     time1 = run_cmd_return_time(cmd) 
 
 
 
 def snHic_barcode(file1_path, file2_path):
     #####记录barcode对应的reads
     fp = open('barcode.index', "w")
```

### Comparing `sc3dg-0.0.4/sc3dg/utils/sciHic.py` & `sc3dg-0.0.5/sc3dg/utils/sciHic.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.4/sc3dg/utils/sn_m3c.py` & `sc3dg-0.0.5/sc3dg/utils/sn_m3c.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,54 +3,63 @@
 import argparse
 import re
 import numpy as np
 import subprocess
 import time
 import logging
 import os
-current_file_path = os.path.abspath(__file__)
-hicCorrectMatrix = os.path.dirname(current_file_path) + '/' + 'correct.py'
-hicCorrectMatrix = 'python ' + hicCorrectMatrix
+
 
 def pp(opt, fastq,log_out):
 
     
     print('********run sn_m3c*********')
     T = time.time()
     # 移动到工作目录
     os.chdir(opt['output'])
 
-    # 创建文件夹tmp,并移动
+        # 创建文件夹tmp,并移动
     if not os.path.exists(opt['type'] + '_' + fastq + '_tmp'): # scHic_sample_tmp
         os.makedirs(opt['type'] + '_' + fastq + '_tmp')
+    
+
     os.chdir(opt['type'] + '_' + fastq + '_tmp')
-    os.makedirs('./Result', exist_ok=True)
+    if os.path.exists(opt['output'] + '/' + opt['type'] + '_' + fastq + '_tmp/Result/' + fastq +'.mcool'):
+        log_out.info('The result of ' + fastq + ' has been generated')
+        return
+    else:
+        for val in os.listdir(opt['output'] + '/' + opt['type'] + '_' + fastq + '_tmp'):
+            print('rm -r ' + val)
+            os.system('rm -r ' + val)
+            print('clearing done')
+
+    print('********run sn_m3c after clearing*********')
+
     
-    os.makedirs('./Result/SCpair', exist_ok=True)
-    os.makedirs('./Result/mcool_folder/', exist_ok=True)
-    os.makedirs('./Result/cool_folder/', exist_ok=True)
     fq_r1 = opt['fastq_dir'][opt['fastq_log'].index(fastq)]
     fq_r2 = fq_r1.replace('_1.fastq', '_2.fastq')
 
 
     # 创建logging文件
     logging.basicConfig(filename=fastq + '_logging.log', level=logging.DEBUG)
-    if os.path.exists(opt['output'] + '/' + opt['type'] + '_' + fastq + '_tmp/Result/mcool_folder' + fastq +'.mcool'):
-        log_out.info('The result of ' + fastq + ' has been generated')
-        return
+ 
+
+
     for k in opt.keys():
 
      
         if (k == 'fastq_dir') or (k == 'fastq_log') or (k == 'run_sample'):
             continue
         else:
             logging.debug('# ' + k + ': ' + str(opt[k]))
 
- 
-
+    if not os.path.exists('Result'):
+        os.makedirs('Result')
+    if not os.path.exists('Result/SCPair'):
+        os.makedirs('Result/SCPair')
     
     # Get paird fastq
     cmd = 'fastp '
     cmd += '--trim_front1 25 --trim_front2 25 --trim_tail1 3 --trim_tail2 3 '
     cmd += ' -i ' + fq_r1 + ' -I ' + fq_r2
     cmd += ' --out1 trimmed-pair1.fastq.gz --out2 trimmed-pair2.fastq.gz'
     cmd += ' --failed_out failed.fq.gz'
@@ -105,48 +114,49 @@
     cmd += ' --fastq trimmed-pair1.fastq.gz_unmapped_reads.fq.gz_r1.fq --pbat --parallel ' + str(opt['thread'])
     t = time.time()
     logging.info(cmd)
     os.system(cmd)
     logging.info('bismark3 time: ' + str(time.time() - t))
 
     cmd = 'bismark --bowtie2 ' + opt['index']
-    cmd += ' --fastq trimmed-pair2.fastq.gz_unmapped_reads.fq.gz_r1.fq   --pbat --parallel ' + str(opt['thread'])
+    cmd += ' --fastq trimmed-pair2.fastq.gz_unmapped_reads.fq.gz_r1.fq  --parallel ' + str(opt['thread'])
     t = time.time()
     logging.info(cmd)
     os.system(cmd)
     logging.info('bismark4 time: ' + str(time.time() - t))
 
 
     # rm
-    cmd = 'rm *_unmapped_reads.fq.*'
-    logging.info(cmd)
-    t = time.time()
-    os.system(cmd)
-    logging.info('rm time: ' + str(time.time() - t))
+    # cmd = 'rm *_unmapped_reads.fq.*'
+    # logging.info(cmd)
+    # t = time.time()
+    # os.system(cmd)
+    # logging.info('rm time: ' + str(time.time() - t))
     
 
 
     # merge
-    cmd = 'samtools merge *.bam -o ' + fastq + '.merged.bam -f'
+    cmd = 'samtools merge *.bam -o ' + fastq + '.merged.bam'
     logging.info(cmd)
     t = time.time()
     os.system(cmd)
     logging.info('samtools merge time: ' + str(time.time() - t))
 
 
     t = time.time()
-    cmd = 'samtools view -q 30 -@ 10 -b ' + fastq + '.merged.bam -o ' + fastq + '.filtered.bam'
+    qc = opt['qc']
+    cmd = 'samtools view -q %s -@ %s -b ' % (qc,str(opt['thread'])) + fastq + '.merged.bam -o ' + fastq + '.filtered.bam'
     logging.info(cmd)
     os.system(cmd)
 
-    cmd = 'samtools sort -@ 10 -n ' + fastq + '.filtered.bam -o ' + fastq + '.sorted.bam'
+    cmd = 'samtools sort -@ %s -n ' % str(opt['thread']) + fastq + '.filtered.bam -o ' + fastq + '.sorted.bam'
     logging.info(cmd)
     os.system(cmd)
 
-    cmd = 'samtools view -@ 10 -h ' + fastq + '.sorted.bam -o ' + fastq  + '.sorted.sam'
+    cmd = 'samtools view -@ %s -h ' % str(opt['thread']) + fastq + '.sorted.bam -o ' + fastq  + '.sorted.sam'
     logging.info(cmd)
     os.system(cmd)
     logging.info('samtools view time: ' + str(time.time() - t))
 
     logging.info('filtSam')
     t = time.time()
     filtSam(fastq + '.sorted.sam', fastq + '.sam')
@@ -163,25 +173,25 @@
     cmd += ' --nproc-in ' + str(opt['thread']) +  ' --nproc-out ' + str(opt['thread'])
     # print('4++++++++++++\n',cmd)
     t = time.time()
     logging.info(cmd)
     os.system(cmd)
     logging.info('pairtools parse time: ' + str(time.time() - t))
 
-    cmd = 'pairtools restrict -f ' + opt['enzyme_bed'] + ' ' + fastq + '.pairs.gz -o ' + fastq + 'restrict.pairs.gz'
+    cmd = 'pairtools restrict -f ' + opt['enzyme_bed'] + ' ' + fastq + '.pairs.gz -o ' + fastq + '.restrict.pairs.gz'
     # print('4++++++++++++\n',cmd)
     t = time.time()
     logging.info(cmd)
     os.system(cmd)
     logging.info('pairtools restrict time: ' + str(time.time() - t))
 
 
     # #QC select
     cmd = 'pairtools select ' + '\"' + opt['select'] + '\"'
-    cmd += ' ' + fastq + 'restrict.pairs.gz -o ' + fastq + '.filtered.pairs.gz'
+    cmd += ' ' + fastq + '.restrict.pairs.gz -o ' + fastq + '.filtered.pairs.gz'
     # print('5++++++++++\n', cmd)
     t = time.time()
     logging.info(cmd)
     os.system(cmd)
     logging.info('pairtools select time: ' + str(time.time() - t))
 
     # Sort pairs
@@ -241,48 +251,40 @@
     cmd = 'gzip ' + fastq + '.nodups.UU.pairs'
     # print('11+++++++++++\n', cmd)
     t = time.time()
     logging.info(cmd)
     os.system(cmd)
     logging.info('gzip time: ' + str(time.time() - t))
 
-    # KR correction
-    cmd = '%s correct --matrix  ' % hicCorrectMatrix + fastq + str(opt['resolution']) + '.cool '
-    cmd += ' --correctionMethod KR --outFileName '
-    cmd += ' ' + fastq + str(opt['resolution']) + '.KR.cool'
-    cmd += ' --filterThreshold -1.5 5.0 --chromosomes chr1 chr2 chr3 chr4 chr5 chr6 chr7 chr8 chr9 chr10 chr11 chr12 chr13 chr14 chr15 chr16 chr17 chr18 chr19 chrX '
-    # print('12+++++++++++\n', cmd)
-    t = time.time()
-    logging.info(cmd)
-    os.system(cmd)
-    logging.info('hicCorrectMatrix time: ' + str(time.time() - t))
+    # # KR correction
+    # cmd = 'hicCorrectMatrix correct --matrix  ' + fastq + str(opt['resolution']) + '.cool '
+    # cmd += ' --correctionMethod KR --outFileName '
+    # cmd += ' ' + fastq + str(opt['resolution']) + '.KR.cool'
+    # cmd += ' --filterThreshold -1.5 5.0 --chromosomes chr1 chr2 chr3 chr4 chr5 chr6 chr7 chr8 chr9 chr10 chr11 chr12 chr13 chr14 chr15 chr16 chr17 chr18 chr19 chrX '
+    # # print('12+++++++++++\n', cmd)
+    # t = time.time()
+    # logging.info(cmd)
+    # os.system(cmd)
+    # logging.info('hicCorrectMatrix time: ' + str(time.time() - t))
    
     
 
-    cmd = 'cooler zoomify '  + fastq + str(opt['resolution']) + '.KR.cool -r 10000,40000,100000,100000 -o ' + fastq + '.mcool'
+    cmd = 'cooler zoomify '  + fastq + str(opt['resolution']) + '.cool -r %s -o ' % opt['zoomify_res'] + fastq + '.mcool'
     # print('13+++++++++++\n', cmd)
     t = time.time()
     logging.info(cmd)
     os.system(cmd)
     logging.info('cooler zoomify time: ' + str(time.time() - t))
 
 
-    os.system('mv ./*.mcool ./Result/mcool_folder/')
-    os.system('mv ./*.cool ./Result/cool_folder/')
-    os.system('mv ./*restrict.pairs.gz ./Result/SCpair/')
-    os.system('mv ./%s.pairs.gz ./Result/SCpair/'%fastq)
-    os.system('mv ./Result/SCpair/*.mcool ./Result/mcool_folder')
-    os.system('mv ./Result/SCpair/*.cool ./Result/cool_folder')
-    for val in os.listdir('./'):
-        if not os.path.isdir(val):
-            if val == fastq + '_logging.log' or val == fastq + '.bam' or val == fastq + '.qc.bam' or val == fastq + '.merged.bam' or val =='trimmed.fastp.json':
-                continue
-            else:
-                print(val)
-                os.remove(val)
+    os.system('mv ' + fastq + '.mcool ./Result/')
+    os.system('mv ' + fastq + str(opt['resolution']) + '.KR.cool ./Result/')
+    os.system('mv ' + fastq + str(opt['resolution']) + '.cool ./Result/')
+    os.system('mv ' + fastq + '.nodups.pairs.gz ./Result/')
+
     logging.info('total time: ' + str(time.time() - T))
 
 
 
 
 
 
@@ -344,14 +346,22 @@
     for i in range(len(lines)-1):
         if "@" in lines[i]:
             #print(lines[i])
             #print(i)
             fp.write(lines[i])
 
         else:
-            Read_ID1 = lines[i].split("\t")[0].split("_length")[0]
-            Read_ID2 = lines[i+1].split("\t")[0].split("_length")[0]
+            Read_ID1 = lines[i].split("\t")[0].split("_")[0]
+            Read_ID2 = lines[i+1].split("\t")[0].split("_")[0]
+            components_1 = lines[i].split("\t")
+            components_2 = lines[i+1].split("\t")
+
             if Read_ID1 == Read_ID2:
-                fp.write(lines[i]+lines[i+1])
+                components_1[0] = Read_ID1
+                components_2[0] = Read_ID2
+                lines1 = "\t".join(components_1)
+                lines2 = "\t".join(components_2)
+
+                fp.write(lines1+lines2)
                 lines[i+1] = ''
     fp.close()
```

### Comparing `sc3dg-0.0.4/sc3dg/utils/tools.py` & `sc3dg-0.0.5/sc3dg/utils/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,14 @@
     if not opt['type'] == 'sn_m3c':
         if opt['aligner']  == 'bowtie2' :
             if not os.path.exists(opt['index'] + '.1.bt2'):
                 sys.exit('index is not exist/index is not bowtie2 index')
             
         else:
             if not os.path.exists(opt['index'] + '.amb'):
-                print(opt['index'] + '.amb')
                 sys.exit('index is not exist')
     else:
         if not os.path.exists(opt['index'].rsplit('/', 1)[0] + '/Bisulfite_Genome'):
             print('bismark index is not exist')
   
             if not os.path.exists(opt['index'] + '.1.bt2'):
                 sys.exit(opt['index'] + '  is bowtie2 index. fail to create bismark index')
```

### Comparing `sc3dg-0.0.4/sc3dg/utils/visualize.py` & `sc3dg-0.0.5/sc3dg/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `sc3dg-0.0.4/sc3dg.egg-info/requires.txt` & `sc3dg-0.0.5/sc3dg.egg-info/requires.txt`

 * *Files identical despite different names*

