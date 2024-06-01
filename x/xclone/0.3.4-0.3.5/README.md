# Comparing `tmp/xclone-0.3.4.tar.gz` & `tmp/xclone-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xclone-0.3.4.tar", last modified: Thu Apr  6 02:00:17 2023, max compression
+gzip compressed data, was "xclone-0.3.5.tar", last modified: Sat Jun  1 10:24:09 2024, max compression
```

## Comparing `xclone-0.3.4.tar` & `xclone-0.3.5.tar`

### file list

```diff
@@ -1,88 +1,101 @@
-drwxrwxr-x   0 rthuang   (1054) rthuang   (1067)        0 2023-04-06 02:00:17.000000 xclone-0.3.4/
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     2717 2023-04-06 02:00:17.000000 xclone-0.3.4/PKG-INFO
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     1883 2023-04-05 16:47:47.000000 xclone-0.3.4/README.rst
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)       38 2023-04-06 02:00:17.000000 xclone-0.3.4/setup.cfg
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     2311 2022-12-09 02:51:20.000000 xclone-0.3.4/setup.py
-drwxrwxr-x   0 rthuang   (1054) rthuang   (1067)        0 2023-04-06 02:00:17.000000 xclone-0.3.4/xclone/
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)      483 2023-03-24 12:43:33.000000 xclone-0.3.4/xclone/__init__.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    16738 2023-04-01 07:39:44.000000 xclone-0.3.4/xclone/_config.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     1853 2022-11-21 09:00:56.000000 xclone-0.3.4/xclone/_logging.py
-drwxrwxr-x   0 rthuang   (1054) rthuang   (1067)        0 2023-04-06 02:00:17.000000 xclone-0.3.4/xclone/analysis/
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)      505 2023-02-11 05:41:47.000000 xclone-0.3.4/xclone/analysis/__init__.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     2131 2023-02-14 09:27:19.000000 xclone-0.3.4/xclone/analysis/_clustering.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    11302 2023-03-07 03:30:43.000000 xclone-0.3.4/xclone/analysis/evaluation.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     1242 2022-11-21 09:00:56.000000 xclone-0.3.4/xclone/analysis/extract.py
-drwxrwxr-x   0 rthuang   (1054) rthuang   (1067)        0 2023-04-06 02:00:17.000000 xclone-0.3.4/xclone/data/
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)      170 2023-04-04 14:53:17.000000 xclone-0.3.4/xclone/data/__init__.py
-drwxrwxr-x   0 rthuang   (1054) rthuang   (1067)        0 2023-04-06 02:00:17.000000 xclone-0.3.4/xclone/data/demo_datasets/
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)        0 2022-11-22 03:08:43.000000 xclone-0.3.4/xclone/data/demo_datasets/__init__.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     7598 2023-04-04 15:01:44.000000 xclone-0.3.4/xclone/data/demo_datasets/_datasets.py
-drwxrwxr-x   0 rthuang   (1054) rthuang   (1067)        0 2023-04-06 02:00:17.000000 xclone-0.3.4/xclone/model/
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    10415 2023-03-18 11:40:10.000000 xclone-0.3.4/xclone/model/HMM_BB.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    15774 2022-11-21 09:00:56.000000 xclone-0.3.4/xclone/model/HMM_NB.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    17893 2023-01-06 13:25:22.000000 xclone-0.3.4/xclone/model/HMM_base.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    18176 2023-02-14 07:06:41.000000 xclone-0.3.4/xclone/model/XClone_combine.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    19911 2022-12-10 11:07:00.000000 xclone-0.3.4/xclone/model/_BAF.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    14976 2023-03-31 10:42:42.000000 xclone-0.3.4/xclone/model/_BAF_base.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     1228 2023-01-07 13:59:26.000000 xclone-0.3.4/xclone/model/_BAF_process.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     3714 2023-04-03 02:45:04.000000 xclone-0.3.4/xclone/model/_Gaussian_mixture.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     7936 2022-12-21 12:59:58.000000 xclone-0.3.4/xclone/model/_HMM.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    24476 2023-03-30 15:32:23.000000 xclone-0.3.4/xclone/model/_RDR_CNVratio.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)      741 2022-12-09 08:15:05.000000 xclone-0.3.4/xclone/model/_RDR_base.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     6633 2022-11-21 09:00:56.000000 xclone-0.3.4/xclone/model/_RDR_cnv.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    11528 2023-03-06 08:51:26.000000 xclone-0.3.4/xclone/model/_RDR_dispersion.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    30599 2023-03-24 11:17:59.000000 xclone-0.3.4/xclone/model/_RDR_libratio.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     5204 2023-03-21 07:33:39.000000 xclone-0.3.4/xclone/model/_RDR_process.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     1941 2022-12-16 07:27:11.000000 xclone-0.3.4/xclone/model/_RDR_smoothing.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     3836 2023-03-15 12:38:53.000000 xclone-0.3.4/xclone/model/__init__.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     5280 2023-01-10 08:26:39.000000 xclone-0.3.4/xclone/model/_denoise.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    47272 2022-11-21 09:00:56.000000 xclone-0.3.4/xclone/model/analysis_utils.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     1655 2022-11-21 09:00:56.000000 xclone-0.3.4/xclone/model/base_utils.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     4454 2022-12-09 08:15:14.000000 xclone-0.3.4/xclone/model/data_base_utils.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)      223 2023-03-24 12:38:59.000000 xclone-0.3.4/xclone/model/diploid.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    13236 2022-11-21 09:00:56.000000 xclone-0.3.4/xclone/model/mixture.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     5447 2023-01-07 14:10:23.000000 xclone-0.3.4/xclone/model/phasing.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     4282 2023-03-21 03:12:31.000000 xclone-0.3.4/xclone/model/smoothing.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     1151 2022-12-12 07:35:43.000000 xclone-0.3.4/xclone/model/utils.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    23979 2023-03-31 17:48:25.000000 xclone-0.3.4/xclone/model/xclone_baf_wrap.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     9476 2023-03-24 11:27:10.000000 xclone-0.3.4/xclone/model/xclone_combine_wrap.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    15741 2023-03-30 15:29:34.000000 xclone-0.3.4/xclone/model/xclone_rdr_wrap.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)       90 2023-03-24 12:40:17.000000 xclone-0.3.4/xclone/model/xclone_run_wrap.py
-drwxrwxr-x   0 rthuang   (1054) rthuang   (1067)        0 2023-04-06 02:00:17.000000 xclone-0.3.4/xclone/plot/
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    16002 2023-04-01 07:39:41.000000 xclone-0.3.4/xclone/plot/CNV_plot.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     8593 2022-12-23 07:29:07.000000 xclone-0.3.4/xclone/plot/_BAF_debug.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    16358 2023-02-16 06:39:26.000000 xclone-0.3.4/xclone/plot/_BAF_plot.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     9250 2022-12-10 11:26:55.000000 xclone-0.3.4/xclone/plot/_RDR_plot.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     1914 2023-03-15 04:58:49.000000 xclone-0.3.4/xclone/plot/__init__.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     6790 2022-12-10 11:50:13.000000 xclone-0.3.4/xclone/plot/_base_manhattan.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    21593 2023-04-03 10:02:37.000000 xclone-0.3.4/xclone/plot/_base_xanndata.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     1030 2022-12-10 11:36:53.000000 xclone-0.3.4/xclone/plot/_data.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     4378 2022-11-21 09:00:56.000000 xclone-0.3.4/xclone/plot/_explore.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     2012 2022-11-21 09:00:56.000000 xclone-0.3.4/xclone/plot/_plot_style.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)      795 2022-11-21 09:00:56.000000 xclone-0.3.4/xclone/plot/_test.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     9674 2022-12-10 11:48:03.000000 xclone-0.3.4/xclone/plot/_utils.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     7400 2022-12-10 12:13:26.000000 xclone-0.3.4/xclone/plot/_visualize.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     8206 2022-11-21 09:00:56.000000 xclone-0.3.4/xclone/plot/base_plot.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     4284 2023-03-15 05:20:59.000000 xclone-0.3.4/xclone/plot/smooth_plot.py
-drwxrwxr-x   0 rthuang   (1054) rthuang   (1067)        0 2023-04-06 02:00:17.000000 xclone-0.3.4/xclone/preprocessing/
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     2864 2023-03-03 05:50:14.000000 xclone-0.3.4/xclone/preprocessing/_RDR_genes.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     9793 2023-03-07 09:19:28.000000 xclone-0.3.4/xclone/preprocessing/_RDR_preprocess.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     3737 2022-11-21 09:00:56.000000 xclone-0.3.4/xclone/preprocessing/_Xdata_manipulation.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     1599 2023-02-07 12:49:23.000000 xclone-0.3.4/xclone/preprocessing/__init__.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     2312 2022-12-23 06:42:53.000000 xclone-0.3.4/xclone/preprocessing/_anno_data.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     3552 2022-12-09 07:19:23.000000 xclone-0.3.4/xclone/preprocessing/_annotation_prepare.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    14372 2023-01-04 03:57:11.000000 xclone-0.3.4/xclone/preprocessing/_data.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     3438 2022-11-21 09:00:56.000000 xclone-0.3.4/xclone/preprocessing/_demo_data.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)      464 2022-11-21 09:00:56.000000 xclone-0.3.4/xclone/preprocessing/_efficiency.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)    26440 2023-02-07 12:49:21.000000 xclone-0.3.4/xclone/preprocessing/_preprocessing.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)      613 2022-11-21 09:00:56.000000 xclone-0.3.4/xclone/preprocessing/_transformation.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     6557 2022-11-21 09:00:56.000000 xclone-0.3.4/xclone/preprocessing/_utils.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)       61 2022-12-09 07:07:18.000000 xclone-0.3.4/xclone/preprocessing/_utils_base.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     3328 2022-12-05 07:35:56.000000 xclone-0.3.4/xclone/preprocessing/xclone_preprocess_wrap.py
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)       22 2022-12-09 02:52:27.000000 xclone-0.3.4/xclone/version.py
-drwxrwxr-x   0 rthuang   (1054) rthuang   (1067)        0 2023-04-06 02:00:17.000000 xclone-0.3.4/xclone.egg-info/
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     2717 2023-04-06 02:00:17.000000 xclone-0.3.4/xclone.egg-info/PKG-INFO
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)     2190 2023-04-06 02:00:17.000000 xclone-0.3.4/xclone.egg-info/SOURCES.txt
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)        1 2023-04-06 02:00:17.000000 xclone-0.3.4/xclone.egg-info/dependency_links.txt
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)      103 2023-04-06 02:00:17.000000 xclone-0.3.4/xclone.egg-info/requires.txt
--rw-rw-r--   0 rthuang   (1054) rthuang   (1067)        7 2023-04-06 02:00:17.000000 xclone-0.3.4/xclone.egg-info/top_level.txt
+drwxr-x---   0 rthuang  (30012) yuanhua  (30002)        0 2024-06-01 10:24:09.000000 xclone-0.3.5/
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    11357 2023-04-28 03:39:06.000000 xclone-0.3.5/LICENSE
+-rw-r-----   0 rthuang  (30012) yuanhua  (30002)     4569 2024-06-01 10:24:09.000000 xclone-0.3.5/PKG-INFO
+-rw-r-----   0 rthuang  (30012) yuanhua  (30002)     4176 2024-05-26 16:49:55.000000 xclone-0.3.5/README.rst
+-rw-r-----   0 rthuang  (30012) yuanhua  (30002)       38 2024-06-01 10:24:09.000000 xclone-0.3.5/setup.cfg
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     2311 2023-04-28 03:39:13.000000 xclone-0.3.5/setup.py
+drwxr-x---   0 rthuang  (30012) yuanhua  (30002)        0 2024-06-01 10:24:05.000000 xclone-0.3.5/xclone/
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)      483 2023-04-28 03:39:13.000000 xclone-0.3.5/xclone/__init__.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    19107 2024-02-22 04:36:11.000000 xclone-0.3.5/xclone/_config.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     1853 2023-04-28 03:39:13.000000 xclone-0.3.5/xclone/_logging.py
+drwxr-x---   0 rthuang  (30012) yuanhua  (30002)        0 2024-06-01 10:24:05.000000 xclone-0.3.5/xclone/analysis/
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)      659 2024-04-29 01:46:53.000000 xclone-0.3.5/xclone/analysis/__init__.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     2131 2023-04-28 03:39:13.000000 xclone-0.3.5/xclone/analysis/_clustering.py
+-rw-r-----   0 rthuang  (30012) yuanhua  (30002)     1575 2024-04-29 01:46:57.000000 xclone-0.3.5/xclone/analysis/_spatial.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    14409 2024-01-08 22:08:35.000000 xclone-0.3.5/xclone/analysis/evaluation.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     1242 2023-04-28 03:39:13.000000 xclone-0.3.5/xclone/analysis/extract.py
+drwxr-x---   0 rthuang  (30012) yuanhua  (30002)        0 2024-06-01 10:24:05.000000 xclone-0.3.5/xclone/data/
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)      230 2023-12-23 04:31:27.000000 xclone-0.3.5/xclone/data/__init__.py
+drwxr-x---   0 rthuang  (30012) yuanhua  (30002)        0 2024-06-01 10:24:06.000000 xclone-0.3.5/xclone/data/anno_data/
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)  1414391 2023-04-28 03:39:22.000000 xclone-0.3.5/xclone/data/anno_data/annotate_blocks_hg19.txt
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)  1986450 2023-04-28 03:39:37.000000 xclone-0.3.5/xclone/data/anno_data/annotate_blocks_hg19_update.txt
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)  1410683 2023-04-28 03:39:48.000000 xclone-0.3.5/xclone/data/anno_data/annotate_blocks_hg38.txt
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)  1981182 2023-04-28 03:40:04.000000 xclone-0.3.5/xclone/data/anno_data/annotate_blocks_hg38_update.txt
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)  1870850 2023-04-28 03:40:16.000000 xclone-0.3.5/xclone/data/anno_data/annotate_genes_hg19_update.txt
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)  1891086 2023-04-28 03:40:36.000000 xclone-0.3.5/xclone/data/anno_data/annotate_genes_hg38_update.txt
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)  1838625 2023-08-14 12:59:58.000000 xclone-0.3.5/xclone/data/anno_data/annotate_genes_mm10.txt
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     8131 2023-04-28 03:40:36.000000 xclone-0.3.5/xclone/data/anno_data/cellcycle_genes.txt
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)   122002 2023-04-28 03:40:37.000000 xclone-0.3.5/xclone/data/anno_data/housekeeping_genes.txt
+drwxr-x---   0 rthuang  (30012) yuanhua  (30002)        0 2024-06-01 10:24:07.000000 xclone-0.3.5/xclone/data/demo_datasets/
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)        0 2023-04-28 03:40:37.000000 xclone-0.3.5/xclone/data/demo_datasets/__init__.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    12203 2023-12-23 04:31:25.000000 xclone-0.3.5/xclone/data/demo_datasets/_datasets.py
+drwxr-x---   0 rthuang  (30012) yuanhua  (30002)        0 2024-06-01 10:24:08.000000 xclone-0.3.5/xclone/model/
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    11612 2023-05-20 17:19:28.000000 xclone-0.3.5/xclone/model/HMM_BB.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    15774 2023-04-28 03:40:38.000000 xclone-0.3.5/xclone/model/HMM_NB.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    17893 2023-04-28 03:40:38.000000 xclone-0.3.5/xclone/model/HMM_base.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    21534 2024-01-07 05:20:33.000000 xclone-0.3.5/xclone/model/XClone_combine.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    19911 2023-04-28 03:40:39.000000 xclone-0.3.5/xclone/model/_BAF.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    16052 2023-05-18 07:59:00.000000 xclone-0.3.5/xclone/model/_BAF_base.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     1474 2023-11-07 21:17:10.000000 xclone-0.3.5/xclone/model/_BAF_process.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     3714 2023-04-28 03:40:39.000000 xclone-0.3.5/xclone/model/_Gaussian_mixture.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     7936 2023-04-28 03:40:39.000000 xclone-0.3.5/xclone/model/_HMM.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    24714 2023-05-19 09:50:36.000000 xclone-0.3.5/xclone/model/_RDR_CNVratio.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)      741 2023-04-28 03:40:40.000000 xclone-0.3.5/xclone/model/_RDR_base.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     6633 2023-04-28 03:40:41.000000 xclone-0.3.5/xclone/model/_RDR_cnv.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    11528 2023-04-28 03:40:41.000000 xclone-0.3.5/xclone/model/_RDR_dispersion.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    30599 2023-04-28 03:40:41.000000 xclone-0.3.5/xclone/model/_RDR_libratio.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     7148 2023-12-27 15:52:24.000000 xclone-0.3.5/xclone/model/_RDR_process.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     1941 2023-04-28 03:40:41.000000 xclone-0.3.5/xclone/model/_RDR_smoothing.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     4049 2024-04-24 13:26:09.000000 xclone-0.3.5/xclone/model/__init__.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     6587 2023-11-05 22:02:02.000000 xclone-0.3.5/xclone/model/_denoise.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    47272 2023-04-28 03:40:44.000000 xclone-0.3.5/xclone/model/analysis_utils.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     1655 2023-04-28 03:40:44.000000 xclone-0.3.5/xclone/model/base_utils.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     4454 2023-04-28 03:40:44.000000 xclone-0.3.5/xclone/model/data_base_utils.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)      223 2023-04-28 03:40:45.000000 xclone-0.3.5/xclone/model/diploid.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    13236 2023-04-28 03:40:45.000000 xclone-0.3.5/xclone/model/mixture.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     5447 2023-04-28 03:40:45.000000 xclone-0.3.5/xclone/model/phasing.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     4282 2023-04-28 03:40:45.000000 xclone-0.3.5/xclone/model/smoothing.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     1151 2023-04-28 03:40:45.000000 xclone-0.3.5/xclone/model/utils.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    31569 2024-04-24 13:24:55.000000 xclone-0.3.5/xclone/model/xclone_baf_wrap.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    12498 2023-12-23 04:31:15.000000 xclone-0.3.5/xclone/model/xclone_combine_wrap.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    20083 2024-04-24 13:17:47.000000 xclone-0.3.5/xclone/model/xclone_rdr_wrap.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)       90 2023-04-28 03:40:46.000000 xclone-0.3.5/xclone/model/xclone_run_wrap.py
+drwxr-x---   0 rthuang  (30012) yuanhua  (30002)        0 2024-06-01 10:24:09.000000 xclone-0.3.5/xclone/plot/
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    16002 2023-04-28 03:40:47.000000 xclone-0.3.5/xclone/plot/CNV_plot.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     8593 2023-04-28 03:40:47.000000 xclone-0.3.5/xclone/plot/_BAF_debug.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    16358 2023-04-28 03:40:47.000000 xclone-0.3.5/xclone/plot/_BAF_plot.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     9250 2023-04-28 03:40:47.000000 xclone-0.3.5/xclone/plot/_RDR_plot.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     1968 2024-04-25 08:30:29.000000 xclone-0.3.5/xclone/plot/__init__.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     6790 2023-04-28 03:40:48.000000 xclone-0.3.5/xclone/plot/_base_manhattan.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    21593 2023-04-28 03:40:48.000000 xclone-0.3.5/xclone/plot/_base_xanndata.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     1030 2023-04-28 03:40:48.000000 xclone-0.3.5/xclone/plot/_data.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     4378 2023-04-28 03:40:49.000000 xclone-0.3.5/xclone/plot/_explore.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     2012 2023-04-28 03:40:49.000000 xclone-0.3.5/xclone/plot/_plot_style.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)      795 2023-04-28 03:40:49.000000 xclone-0.3.5/xclone/plot/_test.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     9674 2023-04-28 03:40:50.000000 xclone-0.3.5/xclone/plot/_utils.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     7400 2023-04-28 03:40:50.000000 xclone-0.3.5/xclone/plot/_visualize.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     8206 2023-04-28 03:40:50.000000 xclone-0.3.5/xclone/plot/base_plot.py
+-rw-r-----   0 rthuang  (30012) yuanhua  (30002)      826 2023-12-15 06:18:34.000000 xclone-0.3.5/xclone/plot/prob_plot.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     4553 2024-04-24 13:16:58.000000 xclone-0.3.5/xclone/plot/smooth_plot.py
+drwxr-x---   0 rthuang  (30012) yuanhua  (30002)        0 2024-06-01 10:24:09.000000 xclone-0.3.5/xclone/preprocessing/
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     2864 2023-04-28 03:40:50.000000 xclone-0.3.5/xclone/preprocessing/_RDR_genes.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    11136 2023-12-28 20:20:58.000000 xclone-0.3.5/xclone/preprocessing/_RDR_preprocess.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     3737 2023-04-28 03:40:50.000000 xclone-0.3.5/xclone/preprocessing/_Xdata_manipulation.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     1763 2024-01-11 03:32:13.000000 xclone-0.3.5/xclone/preprocessing/__init__.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     2565 2023-08-14 13:09:34.000000 xclone-0.3.5/xclone/preprocessing/_anno_data.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     4921 2023-08-14 13:00:35.000000 xclone-0.3.5/xclone/preprocessing/_annotation_prepare.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    14508 2024-04-25 13:33:57.000000 xclone-0.3.5/xclone/preprocessing/_data.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     3462 2023-08-14 13:05:29.000000 xclone-0.3.5/xclone/preprocessing/_demo_data.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)      464 2023-04-28 03:40:52.000000 xclone-0.3.5/xclone/preprocessing/_efficiency.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)    26440 2023-04-28 03:40:52.000000 xclone-0.3.5/xclone/preprocessing/_preprocessing.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     1092 2023-12-27 20:15:17.000000 xclone-0.3.5/xclone/preprocessing/_transformation.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     6557 2023-04-28 03:40:52.000000 xclone-0.3.5/xclone/preprocessing/_utils.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)       61 2023-04-28 03:40:52.000000 xclone-0.3.5/xclone/preprocessing/_utils_base.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     4731 2024-05-26 16:48:35.000000 xclone-0.3.5/xclone/preprocessing/xclone_preprocess_wrap.py
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)       22 2023-05-18 07:59:00.000000 xclone-0.3.5/xclone/version.py
+drwxr-x---   0 rthuang  (30012) yuanhua  (30002)        0 2024-06-01 10:24:05.000000 xclone-0.3.5/xclone.egg-info/
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     4569 2024-06-01 10:24:04.000000 xclone-0.3.5/xclone.egg-info/PKG-INFO
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)     2692 2024-06-01 10:24:05.000000 xclone-0.3.5/xclone.egg-info/SOURCES.txt
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)        1 2024-06-01 10:24:04.000000 xclone-0.3.5/xclone.egg-info/dependency_links.txt
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)      103 2024-06-01 10:24:04.000000 xclone-0.3.5/xclone.egg-info/requires.txt
+-rw-r--r--   0 rthuang  (30012) yuanhua  (30002)        7 2024-06-01 10:24:04.000000 xclone-0.3.5/xclone.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `xclone-0.3.4/setup.py` & `xclone-0.3.5/setup.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/_config.py` & `xclone-0.3.5/xclone/_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,18 +39,21 @@
     Xdata loading params.
     """
     def __init__(
         self,
         dataset_name = "XClone_scDATA",
         module = "RDR",
         cell_anno_file = None,
+        set_spatial: bool = False,
+        spot_position_file = None,
         rdr_data_dir = None,
         baf_data_dir = None):
         
         self.module = module
+        self.set_spatial = set_spatial
         self.rdr_data_dir = rdr_data_dir
         self.baf_data_dir = baf_data_dir
         self.dataset_name = dataset_name
 
         if self.module == "pre_check":
             self.RDR_barcodes_file = self.rdr_data_dir + "barcodes.tsv"
             self.BAF_barcodes_file = self.baf_data_dir + "xcltk.samples.tsv"
@@ -59,24 +62,29 @@
             self.RDR_file = self.rdr_data_dir + "matrix.mtx"
             self.mtx_barcodes_file = self.rdr_data_dir + "barcodes.tsv"
             self.regions_anno_file = None
             # self.regions_anno_file = self.rdr_data_dir + "features.tsv"
             self.cell_anno_file = cell_anno_file
             self.cell_anno_key = "cell_type"
             self.genome_mode = "hg38_genes"
+            
+            if self.set_spatial:
+                self.spot_position_file = spot_position_file
 
         if self.module == "BAF":
             self.AD_file = self.baf_data_dir + "xcltk.AD.mtx"
             self.DP_file = self.baf_data_dir + "xcltk.DP.mtx"
             self.mtx_barcodes_file = self.baf_data_dir + "xcltk.samples.tsv"
             self.regions_anno_file = None
             # self.regions_anno_file = self.baf_data_dir + "xcltk.region.tsv"
             self.cell_anno_file = cell_anno_file
             self.cell_anno_key = "cell_type"
             self.genome_mode = "hg38_genes"
+            if self.set_spatial:
+                self.spot_position_file = spot_position_file
 
         if self.module == "Combine":
             self.RDR_adata_file = self.rdr_data_dir + "RDR_adata_KNN_HMM_post.h5ad"
             self.BAF_adata_file = self.baf_data_dir + "BAF_merge_Xdata_KNN_HMM_post.h5ad"
     
     def display(self):
         """Display Configuration values."""
@@ -90,24 +98,34 @@
     def __init__(self):
         self.cell_anno_key = "cell_type"
         self.ref_celltype = "N"
         self.exclude_XY = False
         self.remove_guide_XY = False
         # KNN smoothing
         self.KNN_neighbors = 10
+        # Plotting
+        # self.plot_cell_anno_key =  None
+        self.plot_remove_immune = True
+        self.plot_immune_celltype = None
+        self.plot_remove_reference = True
+        self.plot_ref_celltype = None
+
 
 class RDR_General_config():
     def __init__(self):
         """
         RDR params init settings. 
         default for 10X scRNA-seq data.
         """
         self.smart_transform = False
         self.filter_ref_ave = 0.5
+        self.min_gene_keep_num = 3000
+        self.multi_refcelltype = False
         self.marker_group_anno_key = None
+        self.get_marker_genes = True
         self.top_n_marker = 15
         self.remove_marker = True
         self.fit_GLM_libratio = False # default use counts ratio
         self.select_normal_chr_num = 4
         self.dispersion_celltype = None
         self.gene_exp_group = 1
         # active when exp_group larger than 2
@@ -118,14 +136,15 @@
         # [0.00001, 0.96, 0.99999]
         # self.guide_chr_anno_key = "chr"
         # self.guide_qt_lst = [0.00001, 0.96, 0.999]
         ## smoothing
         self.WMA_window_size = 40
         self.WMA_smooth_key = "chr_arm"
         # WMA_smooth_key may update to predefined segment for simple clones
+        
         ## RDR plotting
         self.xclone_plot = True
         self.plot_cell_anno_key =  None
         self.rdr_plot_vmin = -0.7
         self.rdr_plot_vmax = 0.7
         self.set_figtitle = True
 
@@ -135,29 +154,37 @@
         """
         BAF params init settings.
         default for 10X scRNA-seq data.
         """
         self.baf_bias_mode = baf_bias_mode
         if self.baf_bias_mode == 0:
             self.CNV_N_components = 3
+            self.BAF_add = False
         elif self.baf_bias_mode == 1:
             self.CNV_N_components = 5
             self.BAF_add = None
-
+        
+        ## related to RDR
+        self.update_info_from_rdr = True
         self.RDR_file = None
+        self.remove_marker_genes = True
+        self.KNN_connect_use_key = "connectivities_expr"
+        
+        self.get_BAF_KNN_connectivities = False
+        self.KNN_Xlayer = "fill_BAF_phased"
+        
         self.guide_theo_CNV_states = None
         self.theo_neutral_BAF = None
         self.ref_BAF_clip = False
         self.concentration = 100
         self.extreme_count_cap = False
         self.gene_specific_concentration = False
         self.concentration_lower = 20
         self.concentration_upper = 100
-        ## related to RDR
-        self.remove_marker_genes = True
+        
         ## loacal phasing
         self.feature_mode = "GENE"
         # self.init_mode = "warm"
         self.phasing_region_key = "chr"
         self.phasing_len = 100
         self.bin_nproc = 20
         ## smoothing
@@ -180,27 +207,34 @@
     def __init__(self):
         """
         Combination parmas init settings.
         default settings.
         """
         ## combine performing
         self.BAF_denoise = False
+        self.RDR_denoise = False
         self.copyloss_correct = True # default
         self.copyloss_correct_mode = 1
         self.copygain_correct= False # default
         if  self.copygain_correct== False:
             self.copygain_correct_mode = None
+        self.RDR_prior = True
 
         ## combine plotting
+        self.xclone_plot = True
+        self.plot_cell_anno_key =  None
         self.merge_loss = True
         self.merge_loh = True
         self.set_figtitle = True
-        self.xclone_plot = True
-        self.plot_cell_anno_key =  None
         
+        ## function in combine module
+        self.WGD_detection = True
+        self.WGD_detect_genome_level = "chr_arm"
+        self.WGD_prop_value_threshold = 0.9
+        self.WGD_cell_prop_threshold = 50
 
 class HMM_Configs():
     def __init__(self):
         """
         HMM smoothing params init settings.
         default settings.
         """
@@ -254,38 +288,75 @@
             pass
         
         ## general settings
         self.exclude_XY = True
         self.remove_guide_XY = True
         # self.KNN_neighbors = 5
 
+
+class Spatial_Config():
+    def __init__(self):
+        """
+        Spatial transcriptmoics specific config settings.
+        default settings.
+        """
+        if self.module == "RDR":
+            # self.spatail_imputation = True
+            self.smart_transform = False
+            self.spatial_transform = True
+            self.filter_ref_ave = 0.5
+            self.min_gene_keep_num = 1500
+            ## HMM related
+            # self.start_prob = np.array([0.1, 0.8, 0.1])
+            self.start_prob = np.array([0.3, 0.4, 0.3])
+
+        if self.module == "BAF":
+            self.extreme_count_cap = False
+            self.gene_specific_concentration = True
+            if self.gene_specific_concentration == True:
+                self.concentration = None
+
+            ## smoothing related
+            self.WMA_window_size = 6
+        
+        if self.module == "Combine":
+            pass
+        
+        ## general settings
+        self.exclude_XY = True
+        self.remove_guide_XY = True
+        # self.KNN_neighbors = 5
+
+
 ## todo: denoise part
 
 class XCloneConfig():
     """\
     Config manager for xclone.
     """
 
     def __init__(
         self,
         dataset_name: str = "XClone_scDATA",
         set_smartseq: bool = False,
+        set_spatial: bool = False,
         module: str = "RDR",
         baf_bias_mode = 1,
         plot_suffix: str = "",
         file_format_data: str = "h5ad",
         file_format_figs: str = "pdf",
         outdir: Union[str, Path] = "./XCLONE_OUT/",
         _frameon: bool = True,
         _vector_friendly: bool = False
     ):
         """
         """
         self.dataset_name = dataset_name
         self.set_smartseq = set_smartseq
+        self.set_spatial = set_spatial
         if module in ["RDR", "BAF", "Combine"]:
             pass
         else:
             print(module)
             raise ValueError("module is NOT supported in XClone.")
         
         # module specific
@@ -301,14 +372,17 @@
         
         # xclone general config
         Base_settings.__init__(self)
         XCloneGeneral_config.__init__(self)
         
         if self.set_smartseq:
             Smartseq_Config.__init__(self)
+        if self.set_spatial:
+            Spatial_Config.__init__(self)
+
 
         # other general config
         self.plot_suffix = plot_suffix
         self.file_format_data = file_format_data
         self.file_format_figs = file_format_figs
         self.outdir = outdir
         self._frameon = _frameon
```

### Comparing `xclone-0.3.4/xclone/_logging.py` & `xclone-0.3.5/xclone/_logging.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/analysis/_clustering.py` & `xclone-0.3.5/xclone/analysis/_clustering.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/analysis/evaluation.py` & `xclone-0.3.5/xclone/analysis/evaluation.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,69 @@
 """Base functions for XClone performance evaluation.
 """
 import numpy as np
 import pandas as pd
 import anndata as ad
 
+
+def prob_adata_generate(data_dir, file_lst = None, method = "xclone"):
+    """
+    Example:
+    data_dir = "/groups/cgsd/xianjie/shared/xclone/GBM_eval_20231104/numbat_raw_genes_tsv/"
+    file_lst = [ "GBM.copy_loss.numbat.prob.gene_scale.extract.cell_x_gene.mtx.rds.tsv" , 
+    "GBM.loh.numbat.prob.gene_scale.extract.cell_x_gene.mtx.rds.tsv", 
+    "GBM.copy_gain.numbat.prob.gene_scale.extract.cell_x_gene.mtx.rds.tsv"]
+    xclone.al.prob_adata_generate(data_dir,file_lst, method = "numbat")
+
+    data_dir = "/home/rthuang/groups/rthuang/Results/GBM/xclone_results/analysis/extracted_data/"
+    xclone.al.prob_adata_generate(data_dir)
+    """
+    if method == "numbat":
+        numbat_file = data_dir + file_lst[0]
+        numbat = pd.read_csv(numbat_file, sep = "\t", index_col = 0)
+        data = numbat.values
+        obs = pd.DataFrame({"cell_barcodes": numbat.index})
+        var = pd.DataFrame({"GeneName": numbat.columns})
+        
+        # Create an AnnData object
+        adata = ad.AnnData(X=data, obs=obs, var=var)
+        adata.obs.set_index(adata.obs["cell_barcodes"], inplace=True)
+        
+        prob_lst = []
+        for file_ in file_lst:
+            numbat_file = data_dir+file_
+            prob_ = pd.read_csv(numbat_file, sep = "\t", index_col = 0)
+            prob_lst.append(prob_) 
+    
+        a_combined = np.stack(prob_lst, axis=-1)
+        adata.layers["numbat_prob"] = a_combined
+
+    if method == "xclone":
+        ## establish prob layer   
+        state_lst = ["prob_combine_copyloss/", "prob_combine_loh/", "prob_combine_copyneutral/", "prob_combine_copygain/"]
+        prob_lst = []
+        for state_ in state_lst:
+            prob_file = data_dir + state_ + "matrix.csv"
+            prob_ = pd.read_csv(prob_file, header = None)
+            prob_lst.append(prob_)
+        a_combined = np.stack(prob_lst, axis=-1)
+
+        obs = pd.read_csv(data_dir + "prob_combine_copyloss/" + "cells.csv", header = None)
+        obs.columns = ["cell_barcodes"]
+        var = pd.read_csv(data_dir + "prob_combine_copyloss/" + "Features.csv")
+        # Create an AnnData object
+        adata = ad.AnnData(X=prob_.values, obs=obs, var=var)
+        adata.obs.set_index(adata.obs["cell_barcodes"], inplace=True)
+        adata.layers["xclone_prob"] = a_combined
+    
+    # Print the AnnData object
+    print(adata)
+    return adata
+
+
 def extract_Xdata(Xdata, use_cell_file, use_gene_file):
     """
     Notes:
     use_cell_file, use_gene_file from xianjie
     
     Example:
     --------
@@ -33,24 +89,15 @@
     return update_Xdata
 
 
 def extract_Xdata1(Xdata, GT_df):
     """
     Notes:
     update for BCH869 dataset.
-    
-    Example:
-    --------
-    >>> data_dir = "..."
-    >>> use_cell_file = dat_dir + "GX109.isec.cell.anno.tsv"
-    >>> use_gene_file = dat_dir + "GX109.isec.gene.anno.tsv"
-    >>> RDR_adata = extract_Xdata(RDR_adata,use_cell_file, use_gene_file)
     """
-
-
     use_cell_lst = GT_df.index.tolist()
     use_gene_lst = GT_df.columns.tolist()
     
     cell_flag = Xdata.obs.index.isin(use_cell_lst)
     gene_flag = Xdata.var["GeneName"].isin(use_gene_lst)
     
     update_Xdata = Xdata.copy()
@@ -82,22 +129,25 @@
     gene_index = np.flatnonzero(gene_flag.values)
     cell_index = np.flatnonzero(cell_flag.values)
     
     Ground_truth_mtx[np.repeat(cell_index,len(gene_index)),  np.tile(gene_index, len(cell_index))] = 1
     
     return Ground_truth_mtx
 
-def load_ground_truth(file_path,  out_df = True, BCHdataset = True):
+def load_ground_truth(file_path,  out_df = True, BCHdataset = True, tsv_file = False):
     """
     support for load benchmarking ground truth matrix from .rds file.
     develop base on BCH869 example.
     """
-    import pyreadr
-    result = pyreadr.read_r(file_path) 
-    GT_df = result[None]
+    if tsv_file:
+        GT_df = pd.read_csv(file_path, sep = "\t", index_col = 0)
+    else:
+        import pyreadr
+        result = pyreadr.read_r(file_path) 
+        GT_df = result[None]
     if BCHdataset:
         GT_df.index = GT_df.index.str.replace("BCH", "BT_", regex = False).str.replace(".", "-", regex = False)
     Ground_truth_mtx = GT_df.values
     print("Loading Ground_truth_mtx, shape (cells, genes): ", Ground_truth_mtx.shape)
     if out_df:
         return GT_df
     else:
@@ -106,39 +156,57 @@
 def resort_Ground_truth_mtx(GT_df, Xdata, verbose = True):
     """
     resort Ground_truth_mtx by Xdata order.
     develop base on BCH869 example.
     """
     cell_barcodes = pd.DataFrame(Xdata.obs.index, columns = ["cell_barcodes"])
     gene_names = pd.DataFrame(Xdata.var["GeneName"])
-
+    
+    # if GT_df.shape[1] < Xdata.shape[1]:
+    #     GT_df = GT_df.T.merge(gene_names, left_index=True, right_on = "GeneName", how = "left")
+    #     GT_df.set_index(keys = "GeneName", drop = True, inplace = True)
+    #     arr_ = GT_df.index.isin(gene_names["GeneName"])
+    #     arr_ = np.where(arr_ == None, False, arr_)
+    #     GT_df = GT_df[arr_] 
+    # else:
     GT_df = gene_names.merge(GT_df.T, left_on = "GeneName", right_index=True, how = "left")
     GT_df.set_index(keys = "GeneName", drop = True, inplace = True)
+    
     if verbose:
         print("Ground_truth_mtx reorder genes")
     GT_df = cell_barcodes.merge(GT_df.T, left_on = "cell_barcodes", right_index=True, how = "left")
     GT_df.set_index(keys = "cell_barcodes", drop = True, inplace = True)
     if verbose:
         print("Ground_truth_mtx reorder cells")
     Ground_truth_mtx = GT_df.values
     if verbose:
         print("Ground_truth_mtx shape (cells, genes): ", Ground_truth_mtx.shape)
     return Ground_truth_mtx
 
 
-def base_evaluate_map(adata, ground_truth_file):
+def base_evaluate_map(adata, ground_truth_file, tsv_file = False):
     """
     """
-    GT_df = load_ground_truth(ground_truth_file,  out_df = True, BCHdataset = True)
+    GT_df = load_ground_truth(ground_truth_file,  out_df = True, BCHdataset = True, tsv_file = tsv_file)
     Xdata = extract_Xdata1(adata, GT_df)
     Ground_truth_mtx = resort_Ground_truth_mtx(GT_df, Xdata)
     
     return Ground_truth_mtx, Xdata
 
-def roc_auc_evaluate(Ground_truth_mtx, Xdata, Xlayer = "XC_denoise", state_idx = 0, ROC_show = False):
+def base_evaluate_map1(adata, ground_truth_file, tsv_file = False):
+    """
+    BCHdataset = False
+    """
+    GT_df = load_ground_truth(ground_truth_file,  out_df = True, BCHdataset = False, tsv_file = tsv_file)
+    Xdata = extract_Xdata1(adata, GT_df)
+    Ground_truth_mtx = resort_Ground_truth_mtx(GT_df, Xdata)
+    
+    return Ground_truth_mtx, Xdata
+
+def roc_auc_evaluate(Ground_truth_mtx, Xdata, Xlayer = "XC_denoise", state_idx = 0, ROC_show = False, dpi = 300, save_fig = None):
     """
     ref: # https://github.com/huangyh09/foundation-data-science/blob/main/w10-classification/P3_ROC_NaiveBayes.ipynb
     
     state_idx = 0  copy_loss
     state_idx = 1 loh
     state_idx = 3 copy_gain
     """
@@ -176,16 +244,17 @@
 
         plt.grid(alpha=0.4)
 
         plt.xlabel("False positive rate (1 - specificity)")
         plt.ylabel("True positive rate (sensitivity)")
         plt.title("ROC curve")
         plt.legend()
+        if save_fig:
+            plt.savefig(save_fig, bbox_inches='tight', dpi=dpi)
         plt.show()
-
     return roc_auc
 
 def fast_evaluate(GT_dat_dir, Combine_adata, Xlayer = "XC_denoise", dataset_name = "BCH869", update = False):
     AUC_record = {}
     ## copy gain
     state_name = "copy_gain"
     ground_truth_file = f"{GT_dat_dir}{state_name}/truth/{dataset_name}.isec.copy.gain.binary.matrix.rds"
```

### Comparing `xclone-0.3.4/xclone/analysis/extract.py` & `xclone-0.3.5/xclone/analysis/extract.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/HMM_BB.py` & `xclone-0.3.5/xclone/model/HMM_BB.py`

 * *Files 5% similar despite different names*

```diff
@@ -53,36 +53,66 @@
         ref_ = np.clip(ref_, bd_low, bd_high)
 
     # Xdata.layers[out_layer] = expit(Xmtx_used - ref_)
     Xdata.var[out_anno] = ref_
 
     return Xdata
 
+def get_BAF_ref_limited(Xdata, Xlayer = "BAF_phased_KNN_WMA", out_anno = "ref_BAF_phased", 
+                anno_key = "cell_type", ref_cell = "unclassified", clipping = False):
+    """
+    update for if ref cells are limited.
+    if variance is high, set the corresponding ref baf as 0.5"""
+    Xmtx_used = Xdata.layers[Xlayer].copy()
+    is_ref_ = Xdata.obs[anno_key] == ref_cell
+    ref_ = Xmtx_used[is_ref_].mean(axis = 0)
+
+    baf_variance = np.var(Xmtx_used[is_ref_], axis=0)
+    Xdata.var["baf_variance"] = baf_variance
+    
+    ## do clipping at ref BAF
+    if clipping:
+        print("do clipping at ref BAF")
+        qt_10 = np.quantile(ref_, 0.1)
+        qt_90 = np.quantile(ref_, 0.9)
+        bd_low = max(qt_10, 0.3)
+        bd_high = min(qt_90, 0.7)
+        ref_ = np.clip(ref_, bd_low, bd_high)
+
+    Xdata.var[out_anno] = ref_
+    ## Notes: try to keep confident REF_BAF, and change others to be 0.5.
+    flag_ = Xdata.var["baf_variance"] > 0.001
+    ## Notes: the 0.001 variance cutoff here is based on layer `BAF_phased_KNN_WMA`
+    ## need explore other cutoff if use different layer, e.g., `fill_BAF_phased` 
+    ## (with higher variance in general).
+    print("Set %s bins' baf as 0.5" % (flag_.sum()))
+    Xdata.var[out_anno][flag_] = 0.5
+    return Xdata
+
 def gene_specific_BAF(Xdata,
                       theo_normal_states = 0.5,
-                      theo_states= np.array([0.01, 0.99, 1/3, 2/3]), 
+                      theo_states= np.array([0.01, 1/3, 2/3, 0.99]), 
                       specific_BAF = "ref_BAF_phased", 
                       rescale = False):
     """
-    np.array([0.01, 0.99, 0.5, 1/3, 2/3]) ->
-    np.array([[0.01, 0.99, specific-BAF, 1/3, 2/3],
-              [0.01, 0.99, specific-BAF, 1/3, 2/3]])
+    np.array([0.01,  1/3,  0.5, 2/3, 0.99,]) ->
+    np.array([[0.01, 1/3, specific-BAF, 2/3, 0.99],
+              [0.01, 1/3, specific-BAF, 2/3, 0.99]])
 
     support 3 states: copy loss and copy neutral.
-    np.array([0.01, 0.99, 0.5]) ->
-    np.array([[0.01, 0.99, specific-BAF],
-              [0.01, 0.99, specific-BAF]])
+    np.array([0.01, 0.5, 0.99]) ->
+    np.array([[0.01, specific-BAF, 0.99],
+              [0.01, specific-BAF, 0.99]])
 
     and support rescale.
     """
     from scipy.special import logit, expit
 
     specific_states = Xdata.var[specific_BAF]
     gene_num = Xdata.shape[1]
-    # base_states = np.tile([0.01, 0.99, 1/3, 2/3], gene_num).reshape(gene_num, -1)
     base_states = np.tile(theo_states, gene_num).reshape(gene_num, -1)
     if len(theo_states) == 4:
         used_specific_states = np.insert(base_states, 2, values = specific_states, axis=1)
         if rescale:
             delta1 = logit(specific_states) - logit(theo_normal_states)
             used_specific_states[:,0] = expit(logit(theo_states[0])+ delta1)
             used_specific_states[:,1] = expit(logit(theo_states[1])+ delta1)
```

### Comparing `xclone-0.3.4/xclone/model/HMM_NB.py` & `xclone-0.3.5/xclone/model/HMM_NB.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/HMM_base.py` & `xclone-0.3.5/xclone/model/HMM_base.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/XClone_combine.py` & `xclone-0.3.5/xclone/model/XClone_combine.py`

 * *Files 15% similar despite different names*

```diff
@@ -373,21 +373,81 @@
             prob_[:,:,2,1] += prob_[:,:,1,1]*2/3
             prob_[:,:,1,1] = 0
             prob_[:,:,1,2] += prob_[:,:,1,3]*1/3
             prob_[:,:,2,3] += prob_[:,:,1,3]*2/3
             prob_[:,:,1,3] = 0
     return prob_
 
+def WGD_warning(Xdata,
+                Xlayer = "combine_base_prob",
+                genome_level = "chr_arm", 
+                prop_value_threshold = 0.9,
+                cell_prop_threshold = 30,
+                ):
+    """
+    WGD warning from the `combine_base_prob` signal.
+
+    Parameters
+    ----------
+    prop_value_threshold: 
+        if WGD signal in any chr_arm higher than 
+        threshold, this cell has WGD signal.
+    cell_prop_threshold:
+        if cells with WGD signal more than threshold,
+        xclone raise the WGD warning for this dataset.
+
+    """
+    prob_ = Xdata.layers[Xlayer].copy()
+    prob = prob_.reshape(prob_.shape[0], prob_.shape[1], -1)
+    max_indices = np.argmax(prob, axis=2)
+    
+    if prob_.shape[-1] == 3:
+        WGD_index = 1
+    if prob_.shape[-1] == 5:
+        WGD_index = 2
+    
+    WGD_bool_mtx = max_indices == WGD_index
+    Xdata.layers["WGD_bool"] = WGD_bool_mtx
+    
+#     prop_cell = (max_indices == WGD_index).sum(axis=1)/max_indices.shape[1]
+    
+    Xdata = caluculate_WGD_proportion(Xdata, region_key = genome_level)
+    cells_with_value_over_threshold = np.any(Xdata.obsm["WGD_prop"] > prop_value_threshold, axis=1)
+    if cells_with_value_over_threshold.sum() > cell_prop_threshold:
+        print("[XClone Warning]", "WGD warning,pls check RDR and BAF module for double comfirmation.")
+    return Xdata
+    
+
+def caluculate_WGD_proportion(Xdata, 
+                             region_key = "chr_arm"):
+    """
+    caluculate_WGD_proportion for each chr_arm.
+    """
+    prop_arrays = []
+    region_brk_item = Xdata.var[region_key].drop_duplicates(keep="first")
+    for brk_ in region_brk_item:
+        flag_ = Xdata.var[region_key] == brk_
+        tmp_Xdata = Xdata[:, flag_]
+        prop_chrarm_cell = tmp_Xdata.layers["WGD_bool"].sum(axis=1)/tmp_Xdata.layers["WGD_bool"].shape[1]
+        prop_arrays.append(prop_chrarm_cell)
+
+    # Now vertically stack the arrays from the list
+    stacked_prop_arrays = np.vstack(prop_arrays)
+    Xdata.obsm["WGD_prop"] = stacked_prop_arrays.T
+    return Xdata
+
+
 def CNV_prob_combination(Xdata,
                          RDR_layer = "posterior_mtx",
                          BAF_layer = "BAF_extend_post_prob",
                          copyloss_correct = True,
                          copyloss_correct_mode = 1,
                          copygain_correct = True,
-                         copygain_correct_mode = 2):
+                         copygain_correct_mode = 2,
+                         RDR_prior = True):
     """
     Combine RDR prob with BAF prob.
     """
     rdr_prob_ = Xdata.layers[RDR_layer].copy()
     baf_prob_ = Xdata.layers[BAF_layer].copy()
 
     rdr_prob_ = np.expand_dims(rdr_prob_, axis = -1)
@@ -408,16 +468,20 @@
         corrected_prob = copyloss_corrected(Xdata, "combine_base_prob", mode = copyloss_correct_mode)
         Xdata.layers["corrected_prob"] = corrected_prob
     elif copygain_correct:
         corrected_prob = copygain_corrected(Xdata, "combine_base_prob", mode = copygain_correct_mode)
         Xdata.layers["corrected_prob"] = corrected_prob
     else:
         Xdata.layers["corrected_prob"] = Xdata.layers["combine_base_prob"].copy()
+    
+    if RDR_prior:
+        prob1_merge = CNV_prob_merge(Xdata, "corrected_prob")    
+    else:
+        prob1_merge = CNV_prob_merge2(Xdata, "corrected_prob")
 
-    prob1_merge = CNV_prob_merge(Xdata, "corrected_prob")
     Xdata.layers["prob1_merge"] = prob1_merge
 
     return Xdata
 
 def CNV_prob_merge(Xdata,
                    Xlayer):
     """
@@ -439,14 +503,46 @@
         copy_neutral = prob_[:,:,1,2]
         copy_gain_less = prob_[:,:,1,1] + prob_[:,:,1,3]
         copy_gain = prob_[:,:,2,:].sum(axis = -1) + copy_gain_less
 
     prob_merge = np.stack([copy_loss, loh, copy_neutral, copy_gain], axis = -1)
     return prob_merge
 
+def CNV_prob_merge2(Xdata,
+                   Xlayer):
+    """
+    BAF prior (for some situations, BAF is more accurate than RDR)
+    Then the final prob should bias to the BAF res.
+    Testing stage [not recommend to all cells]
+    But may try to adjust the functions for applying in some cells/regions. 
+    if use this function: combine module config.RDR_prior set False.
+
+    """
+    prob_ = Xdata.layers[Xlayer].copy()
+    
+    ## BAF 3 states
+    if prob_.shape[-1] == 3:
+        copy_loss = prob_[:,:,0,:].sum(axis = -1)
+        loh = prob_[:,:,1,0] + prob_[:,:,1,2]
+        copy_loss = copy_loss + loh
+        copy_neutral = prob_[:,:,1,1] 
+        copy_gain = prob_[:,:,2,:].sum(axis = -1)
+    
+    ## BAF 5 states
+    if prob_.shape[-1] == 5:
+        copy_loss = prob_[:,:,0,:].sum(axis = -1)
+        loh = prob_[:,:,1,0] + prob_[:,:,1,4]
+        copy_loss = copy_loss + loh
+        copy_neutral = prob_[:,:,1,2]
+        copy_gain_less = prob_[:,:,1,1] + prob_[:,:,1,3]
+        copy_gain = prob_[:,:,2,:].sum(axis = -1) + copy_gain_less
+
+    prob_merge = np.stack([copy_loss, loh, copy_neutral, copy_gain], axis = -1)
+    return prob_merge
+
 def CNV_prob_merge_for_plot(Xdata,
                             Xlayer = "corrected_prob"):
     """
     Merge states prob for more detailed evaluation and visualization.
     """
     prob_ = Xdata.layers[Xlayer].copy()
     ## BAF 3 states
```

### Comparing `xclone-0.3.4/xclone/model/_BAF.py` & `xclone-0.3.5/xclone/model/_BAF.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/_BAF_base.py` & `xclone-0.3.5/xclone/model/_BAF_base.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     return Xdata[:,FLAG]
 
 ## Functions for phasing
 ### local phasing
 def process_bin(idx, AD, DP):
     """
     Func:
+    bin: default for 100 genes
     """ 
     ## Z: allele flipping probability
     ad_sum, ad_sum1, dp_sum, Z, thetas, _logLik_new = Local_Phasing(AD, DP)
     is_flip = np.argmax(Z, axis =1)
     
     ## important *
     BD = DP-AD
@@ -103,32 +104,35 @@
             AD_phased = RV_bin["AD_phased"]
             ad_bin_softcnt = RV_bin["ad_bin_softcnt"]
             ad_bin = RV_bin["ad_bin"]
             dp_bin = RV_bin["dp_bin"]
             theta_bin = RV_bin["theta_bin"]
             bin_idx = RV_bin["bin_idx"]
             bin_idx_lst = RV_bin["bin_idx_lst"]
+            allele_flip_local = RV_bin["flip"]
         else:
             AD_phased = np.vstack((AD_phased, RV_bin["AD_phased"]))
             ad_bin_softcnt = np.vstack((ad_bin_softcnt, RV_bin["ad_bin_softcnt"]))
             ad_bin = np.vstack((ad_bin, RV_bin["ad_bin"]))
             dp_bin = np.vstack((dp_bin, RV_bin["dp_bin"]))
             theta_bin = np.vstack((theta_bin, RV_bin["theta_bin"]))
             bin_idx = np.append(bin_idx, RV_bin["bin_idx"])
             bin_idx_lst = np.append(bin_idx_lst, RV_bin["bin_idx_lst"])
+            allele_flip_local = np.append(allele_flip_local, RV_bin["flip"])
 
     ## resolve results for global phasing input
     RV_region = {}
     RV_region["AD_phased"] = AD_phased
 
     RV_region["bin_idx"] = bin_idx
     RV_region["ad_bin_softcnt"] = ad_bin_softcnt
     RV_region["ad_bin"] = ad_bin
     RV_region["dp_bin"] = dp_bin
     RV_region["theta_bin"] = theta_bin
+    RV_region["allele_flip_local"] = allele_flip_local
     
     ## for global phasing record
     RV_region["bin_idx_lst"] = bin_idx_lst
     # return AD_phased
     return RV_region
 
 
@@ -178,33 +182,43 @@
 
             theta_bin = RV_region["theta_bin"]
             bin_idx = RV_region["bin_idx"]
             bin_idx_lst = RV_region["bin_idx_lst"]
             ad_bin_softcnt = RV_region["ad_bin_softcnt"]
             ad_bin = RV_region["ad_bin"]
             dp_bin = RV_region["dp_bin"]
+            allele_flip_local = RV_region["allele_flip_local"]
 
         else:
             AD_phased = np.vstack((AD_phased, RV_region["AD_phased"]))
             
             theta_bin = np.vstack((theta_bin, RV_region["theta_bin"]))
             bin_idx = np.append(bin_idx, RV_region["bin_idx"])
             bin_idx_lst = np.append(bin_idx_lst, RV_region["bin_idx_lst"])
             ad_bin_softcnt = np.vstack((ad_bin_softcnt, RV_region["ad_bin_softcnt"]))
             ad_bin = np.vstack((ad_bin, RV_region["ad_bin"]))
             dp_bin = np.vstack((dp_bin, RV_region["dp_bin"]))
+            allele_flip_local = np.append(allele_flip_local, RV_region["allele_flip_local"])
          
     end_t = datetime.datetime.now()
     elapsed_sec = (end_t - start_t).total_seconds()
     
     print("[XClone-Local_phasing] time_used: " + "{:.2f}".format(elapsed_sec) + "seconds")
 
     update_Xdata = Xdata.copy()
     update_Xdata.layers["AD_phased"] = AD_phased.T
     update_Xdata.var["bin_idx"] = bin_idx_lst
+    update_Xdata.var["allele_flip_local"] = allele_flip_local
+    try:
+        update_Xdata.var["allele_flip_local"].replace({0: False, 1: True}, inplace = True)
+    except Exception as e:
+        print("[XClone Warning]", e)
+    else:
+        print("[XClone hint] get allele flip status from local phasing.")
+    
     update_Xdata.obsm["theta_bin"] = theta_bin.T
     update_Xdata = process_bin_id(update_Xdata, region_key, verbose)
 
     ##check theta_bin reuslts first and there are nan value
     ## save for visualization
     ad_bin_softcnt = sparse.csr_matrix(ad_bin_softcnt)
     ad_bin = sparse.csr_matrix(ad_bin)
@@ -346,15 +360,19 @@
     AD_phased = Xdata.layers["AD_phased"]
     BD_phased = Xdata.layers["DP"] - Xdata.layers["AD_phased"]
     AD_global_phased = AD_phased + 0
     AD_global_phased[:, gene_flip] = BD_phased[: , gene_flip] + 0
 
     update_Xdata = Xdata.copy()
     update_Xdata.layers["AD_global_phased"] = AD_global_phased
-
+    update_Xdata.var["allele_flip_global"] = gene_flip
+    print("[XClone hint] get allele flip status from global phasing.")
+    if {'allele_flip_local', 'allele_flip_global'}.issubset(update_Xdata.var.columns):
+        update_Xdata.var["allele_flip"] =  update_Xdata.var["allele_flip_local"] ^ update_Xdata.var["allele_flip_global"]
+        print("[XClone hint] get final allele flip status.")
 
     ## apply global phasing method on AD_phased bins
     ad_bin_softcnt = bin_Xdata.layers["ad_bin_softcnt"]
     ad_bin = bin_Xdata.layers["ad_bin"]
     dp_bin = bin_Xdata.layers["dp_bin"]
     
     bd_bin_softcnt = dp_bin - ad_bin_softcnt
```

### Comparing `xclone-0.3.4/xclone/model/_BAF_process.py` & `xclone-0.3.5/xclone/model/_BAF_process.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,32 @@
 ## todo get_KNN_connectivities_from_expr and use different name.
+from .base_utils import normalize
+import scipy as sp
+import scanpy as sc
 
-def extra_preprocess_BAF(adata, Xlayer = "RDR", run_KNN = False, copy=False):
-    """
+def extra_preprocess_BAF(adata, Xlayer = "fill_BAF_phased",
+                         KNN_neighbors = 10,
+                         run_KNN = False, 
+                         copy=False):
+    """s
     """
     adata = adata.copy() if copy else adata
 
     ## generate KNN graph for smoothing across cell neighbourhood
     if run_KNN:
-        import scanpy as sc
         raw_X = adata.X.copy()
         adata.X = adata.layers[Xlayer].copy()
         sc.pp.pca(adata)
-        sc.pp.neighbors(adata, n_neighbors=10, n_pcs=40)
+        sc.pp.neighbors(adata, n_neighbors= KNN_neighbors, n_pcs=40)
         adata.X = raw_X
+        adata.obsp['connectivities'] = normalize(adata.obsp['connectivities'])
 
     return adata if copy else None
 
+
 def get_KNN_connectivities_from_expr(Xdata, expr_adata):
     """
     """
     ## check data cell order the same
     cell_barcodes_BAF =  Xdata.obs.index.values
     cell_barcodes_RDR =  expr_adata.obs.index.values
```

### Comparing `xclone-0.3.4/xclone/model/_Gaussian_mixture.py` & `xclone-0.3.5/xclone/model/_Gaussian_mixture.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/_HMM.py` & `xclone-0.3.5/xclone/model/_HMM.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/_RDR_CNVratio.py` & `xclone-0.3.5/xclone/model/_RDR_CNVratio.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,15 +235,18 @@
         guide_cnv_ratio[0] = 0.3
         print("[XClone] warning: correct RDR CNV guiding copy loss ratio")
         print("[XClone] hints: can change guide_qt_lst")
     if guide_cnv_ratio[2] > 3:
         print("[XClone] warning: correct RDR CNV guiding copy gain ratio")
         print("[XClone] hints: can change guide_qt_lst")
         guide_cnv_ratio[2] = 3
-    
+    if np.bitwise_or((guide_cnv_ratio[1] < 0.5), (guide_cnv_ratio[1] >1.5)):
+        print("[XClone] warning: correct RDR CNV guiding copy neutral ratio")
+        print("[XClone] hints: can change guide_qt_lst")
+        guide_cnv_ratio[1] = 1
     return guide_cnv_ratio
 
 def guide_CNV_states(RDR_Xdata, 
                      Xlayer = "RDR_smooth", 
                      anno_key = "chr", 
                      chr_lst = ["18", "1", "8"], 
                      qt_lst = [0.00001, 0.96, 0.99999],
```

### Comparing `xclone-0.3.4/xclone/model/_RDR_base.py` & `xclone-0.3.5/xclone/model/_RDR_base.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/_RDR_cnv.py` & `xclone-0.3.5/xclone/model/_RDR_cnv.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/_RDR_dispersion.py` & `xclone-0.3.5/xclone/model/_RDR_dispersion.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/_RDR_libratio.py` & `xclone-0.3.5/xclone/model/_RDR_libratio.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/_RDR_process.py` & `xclone-0.3.5/xclone/model/_RDR_process.py`

 * *Files 26% similar despite different names*

```diff
@@ -37,14 +37,19 @@
     adata.obs['counts_ratio'] = Xmtx.sum(axis=1) / adata.var['ref_avg'].sum()
 
     ## check before generate expected layer
     if depth_key == "library_ratio_capped":
         adata.obs[depth_key] = np.where(np.isinf(adata.obs["library_alpha"]), adata.obs["counts_ratio"], adata.obs[depth_key])
         ## todo capped again; add in later version[not test yet] 20230106
         # adata.obs[depth_key] = np.where(adata.obs[depth_key] < 0.001*adata.obs["counts_ratio"], adata.obs["counts_ratio"], adata.obs[depth_key])
+    
+    ## check cell quality
+    cell_flag = adata.obs[depth_key] > 0 
+    adata = adata[cell_flag,:].copy()
+    Xmtx = Xmtx[cell_flag,:].copy()
 
     ## generate normalised
     X_baseline = (adata.obs[depth_key].values.reshape(-1, 1) *
                   adata.var[avg_key].values.reshape(1, -1))
     adata.layers['ref_normalized'] = (Xmtx / X_baseline)
     
     ## generate lower dimension on residues
@@ -69,23 +74,75 @@
     ## generate KNN graph for smoothing across cell neighbourhood
     if run_KNN:
         import scanpy as sc
         raw_X = adata.X.copy()
         adata.X = np.log(adata.layers['ref_normalized'] + 0.3)
         sc.pp.pca(adata)
         sc.pp.neighbors(adata, n_neighbors = KNN_neighbors, n_pcs=40)
-        ## Notes: connectivities and distances can be slightly different rvery run
+        ## Notes: connectivities and distances can be slightly different every run
         ## even the random_state = 0 (default).
         adata.X = raw_X
         ## connectivities normalization
         adata.obsp['connectivities'] = normalize(adata.obsp['connectivities'])
     
     return adata if copy else None
 
 
+def extra_preprocess2(adata, ref_celltype, cluster_key='cell_type',
+                     avg_layer = "ref_avg", depth_key='counts_ratio', 
+                     copy=True):
+    """
+    Testing stage.[not recommend]
+    If use this, RDR module config.multi_refcelltype set True.
+    """
+    import scipy as sp
+    adata = adata.copy() if copy else adata
+    
+    if sp.sparse.issparse(adata.X):
+        Xmtx = adata.X.A
+    else:
+        Xmtx = adata.X
+
+    if ref_celltype not in list(adata.obs[cluster_key]):
+        print("Error: %s not exist as ref cell type" %(ref_celltype))
+        return None
+        
+    _is_ref = adata.obs[cluster_key] == ref_celltype
+
+    sorted_indices = np.argsort(adata.obsp['connectivities'], axis = -1) # cell*cell
+    sorted_ref_indices = sorted_indices[:, _is_ref] # cell* ref_cell
+    
+    select_num = -1* int(_is_ref.sum()*0.1)
+    # select_num = 30
+    
+    for i in range(sorted_ref_indices.shape[0]):
+        
+        _is_select = sorted_ref_indices[i][select_num:]
+        ref_use = Xmtx[_is_select, :].mean(axis=0)
+        if i == 0:
+            ref_ave = ref_use
+        else:
+            ref_ave = np.vstack((ref_ave, ref_use))
+    
+    adata.layers[avg_layer] = ref_ave
+    # adata.var['ref_avg'] = Xmtx[_is_ref, :].mean(axis=0)
+    # adata.obs['counts_ratio'] = Xmtx.sum(axis=1) / adata.var['ref_avg'].sum()
+
+    ## generate normalised
+    # X_baseline = (adata.obs[depth_key].values.reshape(-1, 1) *
+    #               adata.var[avg_key].values.reshape(1, -1))
+    X_baseline = (adata.obs[depth_key].values.reshape(-1, 1) *
+                  adata.layers[avg_layer])
+    # adata.layers['ref_normalized'] = (Xmtx / X_baseline)
+    # update X_baseline for expected layer
+    adata.layers['expected'] = X_baseline
+
+    return adata if copy else None
+
+
 ## (1) modelling
 from sklearn.decomposition import NMF, PCA
 
 def NMF_confounder(Xdata, 
                    anno_key = "cell_type",
                    normalization_method = "sc",
                    log_transform = True,
```

### Comparing `xclone-0.3.4/xclone/model/_RDR_smoothing.py` & `xclone-0.3.5/xclone/model/_RDR_smoothing.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/__init__.py` & `xclone-0.3.5/xclone/model/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 ##debug
 from ._RDR_cnv import fit_CNV_ratio_update
 
 ## RDR remove ref bio
 from ._RDR_process import NMF_confounder
 ## RDR analysis
-from ._RDR_process import extra_preprocess
+from ._RDR_process import extra_preprocess, extra_preprocess2
 from ._RDR_smoothing import RDR_smoothing_base
 
 ## HMM
 
 from .HMM_base import XHMM_smoothing
 from .HMM_base import XC_HMM_base
 
@@ -73,48 +73,52 @@
 from ._BAF_base import BAF_Local_phasing
 from ._BAF_base import BAF_Global_phasing
 from ._BAF_base import BAF_fillna
 from ._BAF_base import BAF_remove_ref
 
 from .HMM_BB import calculate_Xemm_prob_bb
 from .HMM_BB import generate_bb_logprob
-from .HMM_BB import get_BAF_ref, gene_specific_BAF, specific_BAF
+from .HMM_BB import get_BAF_ref, get_BAF_ref_limited, gene_specific_BAF, specific_BAF
 
 from ._BAF import extrme_count_capping
 from ._BAF import concentration_mapping
 ## optimize BAF theoretical values
 from ._BAF import BAF_theoretical_value_optimization
 
 ## smoothing
 from ._BAF import BAF_smoothing
 from .smoothing import WMA_smooth, KNN_smooth
 from ._BAF_process import get_KNN_connectivities_from_expr
+from ._BAF_process import extra_preprocess_BAF
 
 from ._Gaussian_mixture import get_CNV_states, guide_BAF_theo_states
 
 ## combination
 from .XClone_combine import gene_to_bin_mapping
 # from .XClone_combine import BAF_LOH_merge, BAF_LOH_corrected
 # from .XClone_combine import CNV_states_combination, copyloss_adjust
 # from .XClone_combine import visualize_states_process
 
 from .XClone_combine import bin_to_gene_mapping
 from .XClone_combine import CNV_prob_combination
 from .XClone_combine import CNV_prob_merge_for_plot
 
+from .XClone_combine import WGD_warning
+
 ## post-step[analysis for specific dataset]
 from ._denoise import denoise_gene_scale, merge_denoise_prob
 from ._denoise import denoise_by_cluster
+from ._denoise import denoise_rdr_by_baf
 
 ## wrap
 from .xclone_rdr_wrap import preview_RDR
-from .xclone_rdr_wrap import run_RDR, run_RDR_plot
+from .xclone_rdr_wrap import run_RDR, run_RDR_plot, run_RDR_complex_plot
 from .xclone_rdr_wrap import plot_processed_RDR
 
 from .xclone_baf_wrap import preview_BAF
-from .xclone_baf_wrap import run_BAF, run_BAF_plot
+from .xclone_baf_wrap import run_BAF, run_BAF_plot, run_BAF_complex_plot
 from .xclone_baf_wrap import plot_processed_BAF
 
 from .xclone_combine_wrap import run_combine, run_combine_plot
 
 ## debug-develop-improvement
 from ._HMM import Model_NB, HMM_Frame
```

### Comparing `xclone-0.3.4/xclone/model/_denoise.py` & `xclone-0.3.5/xclone/model/_denoise.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 """Denoise functions for XClone probability.
 """
 
 # Author: Rongting Huang
 
 import numpy as np
 import anndata as ad
+from sklearn.mixture import GaussianMixture
 
 from ..analysis._clustering import XClustering
 
 def denoise_gene_scale(Xdata, Xlayer,
                        neutral_index = 2, 
-                       cnv_index = [0,1,3], 
+                       cnv_index = [0,1,3,4], 
                        GMM_detection = True,
                        gmm_comp = 2,
                        cell_prop_cutoff = 0.05,
                        out_layer = "denoised_gene_prob"):
     """
     default method: GMM detect the cell proportion identified as CNV states for each gene.
     alternative method: set cell_prop_cutoff.
     """
-    import numpy as np
-    from sklearn.mixture import GaussianMixture
     Xmtx = Xdata.layers[Xlayer]
     argmax_ = np.argmax(Xmtx, axis = -1)
 
     neutral_sum = (argmax_ == neutral_index).sum(axis = 0)
     total_sum = argmax_.shape[0]
     proportion_ = (total_sum - neutral_sum)/total_sum
     if GMM_detection:
@@ -41,14 +40,56 @@
     denoise_mtx[:,mask_flag, neutral_index] = 1
     for i in cnv_index:
         denoise_mtx[:,mask_flag, i] = 0
      
     Xdata.layers[out_layer] = denoise_mtx
     return Xdata
 
+def denoise_rdr_by_baf(Xdata, 
+                       RDR_layer, 
+                       BAF_layer, 
+                       out_RDR_layer,
+                       cell_prop_cutoff = 0.999
+                       ):
+    """
+    default method: GMM detect the cell proportion identified as allele bias states, and use the states for rdr denoise.
+    """
+    Xmtx = Xdata.layers[BAF_layer]
+    if Xmtx.shape[-1] == 3:
+        b_neutral_index = 1
+    elif Xmtx.shape[-1] == 5:
+        b_neutral_index = 2
+
+
+    argmax_ = np.argmax(Xmtx, axis = -1)
+
+    neutral_sum = (argmax_ == b_neutral_index).sum(axis = 0)
+    total_sum = argmax_.shape[0]
+    proportion_ = neutral_sum/total_sum
+    mask_flag = proportion_ >= cell_prop_cutoff
+    
+    denoise_mtx  = Xdata.layers[RDR_layer].copy()
+    if denoise_mtx.shape[-1] == 3:
+        r_neutral_index = 1
+        r_cnv_index = [0,2]
+    r_argmax_ = np.argmax(denoise_mtx, axis = -1)
+    r_neutral_sum = (r_argmax_ == r_neutral_index).sum(axis = 0)
+    r_total_sum = r_argmax_.shape[0]
+    r_proportion_ = r_neutral_sum/r_total_sum
+    r_mask_flag = r_proportion_ <=0.2
+
+    mask_flag = mask_flag*r_mask_flag
+
+    denoise_mtx[:,mask_flag, r_neutral_index] = 1
+    for i in r_cnv_index:
+        denoise_mtx[:,mask_flag, i] = 0
+    
+    Xdata.layers[out_RDR_layer] = denoise_mtx
+    return Xdata
+
 def denoise_by_cluster(Xdata, 
                        Xlayer,
                        neutral_index = 2, 
                        cnv_index = [0,1,3],
                        GMM_detection = True,
                        gmm_comp = 2,
                        cell_prop_cutoff = 0.3,
```

### Comparing `xclone-0.3.4/xclone/model/analysis_utils.py` & `xclone-0.3.5/xclone/model/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/base_utils.py` & `xclone-0.3.5/xclone/model/base_utils.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/data_base_utils.py` & `xclone-0.3.5/xclone/model/data_base_utils.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/mixture.py` & `xclone-0.3.5/xclone/model/mixture.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/phasing.py` & `xclone-0.3.5/xclone/model/phasing.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/smoothing.py` & `xclone-0.3.5/xclone/model/smoothing.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/utils.py` & `xclone-0.3.5/xclone/model/utils.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/model/xclone_baf_wrap.py` & `xclone-0.3.5/xclone/model/xclone_baf_wrap.py`

 * *Files 17% similar despite different names*

```diff
@@ -56,16 +56,22 @@
     out_dir = config.outdir
 
     cell_anno_key = config.cell_anno_key
     ref_celltype = config.ref_celltype
     exclude_XY = config.exclude_XY
 
     ## RDR related
+    update_info_from_rdr = config.update_info_from_rdr
     RDR_file = config.RDR_file
     remove_marker_genes = config.remove_marker_genes
+    # ## KNN related
+    KNN_connect_use_key = config.KNN_connect_use_key
+    get_BAF_KNN_connectivities = config.get_BAF_KNN_connectivities
+    KNN_Xlayer = config.KNN_Xlayer
+    KNN_neighbors = config.KNN_neighbors
     
     # BAF settings
     theo_neutral_BAF = config.theo_neutral_BAF
     ref_BAF_clip = config.ref_BAF_clip
     BAF_states_num = config.CNV_N_components
     CNV_N_components = config.CNV_N_components
     gene_specific_concentration = config.gene_specific_concentration
@@ -109,37 +115,55 @@
     
     ### output before CNV calling
     BAF_base_file = out_data_dir + "BAF_base_Xdata.h5ad"
     BAF_merge_base_file = out_data_dir + "BAF_merge_base_Xdata.h5ad"
     ### output after CNV calling
     BAF_final_file = out_data_dir + "BAF_merge_Xdata_KNN_HMM_post.h5ad"
     
-    ### RDR file for BAF module (load preprocessed dataset)
-    ### use RDR connectivities, marker genes, etc.
-    if RDR_file is None:
-        RDR_final_file = out_data_dir + "RDR_adata_KNN_HMM_post.h5ad"
+    if update_info_from_rdr:
+        ### RDR file for BAF module (load preprocessed dataset)
+        ### use RDR connectivities, marker genes, etc.
+        if RDR_file is None:
+            RDR_final_file = out_data_dir + "RDR_adata_KNN_HMM_post.h5ad"
+        else:
+            RDR_final_file = RDR_file
+        
+        remove_marker_genes = True
+        KNN_connect_use_key = "connectivities_expr"
     else:
-        RDR_final_file = RDR_file
+        remove_marker_genes = False
+        get_BAF_KNN_connectivities = True
+        KNN_connect_use_key = "connectivities"
+        
 
     ##------------------------
     main_logger = get_logger("Main BAF module")
     main_logger.info("XClone BAF module Started")
     start_time = datetime.now(timezone.utc)
 
     if run_verbose:
         print("[XClone BAF module running]************************")
     
+    ## check ref_celltype
+    if ref_celltype in BAF_adata.obs[cell_anno_key].values:
+        pass
+    else:
+        raise ValueError(f"[XClone error] Item '{ref_celltype}' not found in the BAF_adata's annotation.")
+    
     if exclude_XY:
         BAF_adata = xclone.pp.exclude_XY_adata(BAF_adata)
         print("[XClone warning] BAF module excelude chr XY analysis.")
     BAF_adata = xclone.pp.check_BAF(BAF_adata, cell_anno_key = cell_anno_key, verbose = verbose)
-
-    RDR_adata = an.read_h5ad(RDR_final_file)
-    ## check validated RDR and BAF
-    xclone.pp.check_RDR_BAF_cellorder(RDR_adata, BAF_adata)
+    
+    if update_info_from_rdr:
+        RDR_adata = an.read_h5ad(RDR_final_file)
+        BAF_adata = BAF_adata[BAF_adata.obs.index.isin(RDR_adata.obs.index),:]
+        ## check validated RDR and BAF
+        xclone.pp.check_RDR_BAF_cellorder(RDR_adata, BAF_adata)
+    
     ## Remove marker genes
     if remove_marker_genes:
         marker_genes = RDR_adata.uns["rank_marker_genes"]
         BAF_adata = xclone.pp.Xdata_region_selection(BAF_adata,
                                                     select = False,
                                                     chr_anno_key = "GeneName",
                                                     chr_lst = marker_genes,
@@ -166,20 +190,27 @@
     merge_Xdata = xclone.pl.calculate_cell_BAF(merge_Xdata, 
                                                AD_key = "ad_bin", DP_key = "dp_bin", BAF_key = "BAF")
     merge_Xdata = xclone.pl.calculate_cell_BAF(merge_Xdata, 
                                                AD_key = "ad_bin_phased", DP_key = "dp_bin", BAF_key = "BAF_phased")
     xclone.model.BAF_fillna(merge_Xdata, Xlayer = "BAF_phased", out_layer = "fill_BAF_phased")
 
     ## smoothing
-    merge_Xdata = xclone.model.get_KNN_connectivities_from_expr(merge_Xdata, RDR_adata)
+    if update_info_from_rdr:
+        merge_Xdata = xclone.model.get_KNN_connectivities_from_expr(merge_Xdata, RDR_adata)
+    else:
+        # KNN_Xlayer = "fill_BAF_phased" # can also update the first `KNN_smooth` func.
+        merge_Xdata = xclone.model.extra_preprocess_BAF(merge_Xdata, Xlayer = KNN_Xlayer,
+                         KNN_neighbors = KNN_neighbors,
+                         run_KNN = get_BAF_KNN_connectivities, 
+                         copy=True)
 
     merge_Xdata = xclone.model.KNN_smooth(merge_Xdata, 
                                           run_KNN = False, 
                                           KNN_Xlayer = None, 
-                                          KNN_connect_use = "connectivities_expr",
+                                          KNN_connect_use = KNN_connect_use_key,
                                           layer = "fill_BAF_phased", 
                                           out_layer='BAF_phased_KNN')
     merge_Xdata = xclone.model.WMA_smooth(merge_Xdata, 
                                           layer="BAF_phased_KNN", 
                                           out_layer='BAF_phased_KNN_WMA', 
                                           window_size = WMA_window_size,
                                           chrom_key = WMA_smooth_key, 
@@ -188,15 +219,15 @@
     merge_Xdata = xclone.model.WMA_smooth(merge_Xdata, 
                                           layer="fill_BAF_phased", 
                                           out_layer='BAF_phased_WMA', 
                                           window_size = WMA_window_size, 
                                           chrom_key = WMA_smooth_key,
                                           verbose=False)
     # merge_Xdata = xclone.model.KNN_smooth(merge_Xdata, 
-    #                                       KNN_connect_use = "connectivities_expr", 
+    #                                       KNN_connect_use = KNN_connect_use_key, 
     #                                       layer="BAF_phased_WMA", 
     #                                       out_layer='BAF_phased_WMA_KNN')
     ## after phasing & smoothing
     try:
         BAF_adata.write(BAF_base_file)
         merge_Xdata.write(BAF_merge_base_file)
     except Exception as e:
@@ -211,26 +242,51 @@
     else:
         CNV_states = xclone.model.get_CNV_states(merge_Xdata, Xlayer = "BAF_phased_WMA",
                                                 n_components = CNV_N_components,
                                                 means_init = None,
                                                 max_iter = 200)
         guide_theo_states = xclone.model.guide_BAF_theo_states(CNV_states)
 
-    ## if you have limited ref cells, you can set theo_baf as 0.5   *important
+    # ## if you have limited ref cells, you can set theo_baf as 0.5   *important
+    ## strategy 1: automatically set all to 0.5(may cause some problem)
+    ## strategy 2: set the genes with high variance ref BAF to 0.5 and keep others
+    # ref_cell_num = (merge_Xdata.obs[cell_anno_key] == ref_celltype).sum()
+    # total_cell_num = merge_Xdata.obs.shape[0]
+    # try:
+    #     ref_prop = ref_cell_num/total_cell_num
+    #     if  ref_prop <= 0.01:
+    #         theo_neutral_BAF = 0.5
+    #         print("[XClone hint] limited ref cells (%s), set theo_BAF as 0.5" % ref_prop)
+    # except Exception as e:
+    #     print("[XClone Warning]", e)
+
     if theo_neutral_BAF is not None:
         merge_Xdata.var["theo_neutral_BAF"] = theo_neutral_BAF
         used_specific_states = xclone.model.gene_specific_BAF(merge_Xdata, 
                             theo_states= guide_theo_states, specific_BAF = "theo_neutral_BAF")
     else:
-        merge_Xdata = xclone.model.get_BAF_ref(merge_Xdata, 
-                                           Xlayer = "fill_BAF_phased", 
+        ref_cell_num = (merge_Xdata.obs[cell_anno_key] == ref_celltype).sum()
+        total_cell_num = merge_Xdata.obs.shape[0]
+        ref_prop = ref_cell_num/total_cell_num
+        ## todo: maybe combine the ref cell nums and prop 
+        ## (limited ref cells num may affect more.)
+        if  ref_prop <= 0.01:
+            merge_Xdata = xclone.model.get_BAF_ref_limited(merge_Xdata, 
+                                           Xlayer = "BAF_phased_KNN_WMA", #BAF_phased_KNN_WMA
                                            out_anno = "ref_BAF_phased",
                                            anno_key = cell_anno_key, 
                                            ref_cell = ref_celltype,
                                            clipping = ref_BAF_clip)
+        else:
+            merge_Xdata = xclone.model.get_BAF_ref(merge_Xdata, 
+                                            Xlayer = "fill_BAF_phased", 
+                                            out_anno = "ref_BAF_phased",
+                                            anno_key = cell_anno_key, 
+                                            ref_cell = ref_celltype,
+                                            clipping = ref_BAF_clip)
 
         used_specific_states = xclone.model.gene_specific_BAF(merge_Xdata, 
                                theo_states= guide_theo_states, specific_BAF = "ref_BAF_phased")
 
     if gene_specific_concentration:
         concentration_lower = config.concentration_lower
         concentration_upper = config.concentration_upper
@@ -243,15 +299,15 @@
                                                       states_num = BAF_states_num,
                                                       gene_specific = gene_specific_concentration, 
                                                       concentration = concentration)
 
     merge_Xdata = xclone.model.BAF_smoothing(merge_Xdata,
                                              inlayer = "bin_phased_BAF_specific_center_emm_prob_log",
                                              outlayer = "bin_phased_BAF_specific_center_emm_prob_log_KNN",
-                                             KNN_connectivities_key = "connectivities_expr",
+                                             KNN_connectivities_key = KNN_connect_use_key,
                                              KNN_smooth = True)
     t = trans_t
     if trans_prob is None:
         if CNV_N_components == 3:
             trans_prob = np.array([[1-2*t, t, t],[t, 1-2*t, t],[t, t, 1-2*t]])
         if CNV_N_components == 5:
             trans_prob = np.array([[1-4*t, t, t, t,t],[t, 1-4*t, t, t,t],[t, t, 1-4*t, t,t], [t, t, t, 1-4*t, t], [t, t, t, t, 1-4*t]])
@@ -263,15 +319,15 @@
                                               emm_inlayer = "bin_phased_BAF_specific_center_emm_prob_log_KNN", 
                                               nproc = 80, 
                                               verbose = False)
     
     # merge_Xdata = xclone.model.BAF_smoothing(merge_Xdata,
     #                                          inlayer = "posterior_mtx_log",
     #                                          outlayer = "posterior_mtx_log_KNN",
-    #                                          KNN_connectivities_key = "connectivities_expr",
+    #                                          KNN_connectivities_key = KNN_connect_use_key,
     #                                          KNN_smooth = True)
     
     # merge_Xdata.layers["posterior_mtx"] = np.exp(merge_Xdata.layers["posterior_mtx_log"])
     
     
     ## try to add 3 states layer for comparasion or denoise or correction. [testing version]
     ### only support BAF 5 states to add 3 states visualization for comparasion now.[testing version] 
@@ -297,34 +353,45 @@
 
         ## if you have limited ref cells, you can set theo_baf as 0.5   *important
         if theo_neutral_BAF is not None:
             merge_Xdata_copy.var["theo_neutral_BAF"] = theo_neutral_BAF
             used_specific_states = xclone.model.gene_specific_BAF(merge_Xdata_copy, 
                             theo_states= guide_theo_states, specific_BAF = "theo_neutral_BAF")
         else:
-            merge_Xdata_copy = xclone.model.get_BAF_ref(merge_Xdata_copy, 
-                                           Xlayer = "fill_BAF_phased", 
+            ref_cell_num = (merge_Xdata_copy.obs[cell_anno_key] == ref_celltype).sum()
+            total_cell_num = merge_Xdata_copy.obs.shape[0]
+            ref_prop = ref_cell_num/total_cell_num
+            if  ref_prop <= 0.01:
+                merge_Xdata_copy = xclone.model.get_BAF_ref_limited(merge_Xdata_copy, 
+                                           Xlayer = "BAF_phased_KNN_WMA", #BAF_phased_KNN_WMA
                                            out_anno = "ref_BAF_phased",
                                            anno_key = cell_anno_key, 
                                            ref_cell = ref_celltype,
                                            clipping = ref_BAF_clip)
+            else:
+                merge_Xdata_copy = xclone.model.get_BAF_ref(merge_Xdata_copy, 
+                                            Xlayer = "fill_BAF_phased", 
+                                            out_anno = "ref_BAF_phased",
+                                            anno_key = cell_anno_key, 
+                                            ref_cell = ref_celltype,
+                                            clipping = ref_BAF_clip)
 
             used_specific_states = xclone.model.gene_specific_BAF(merge_Xdata_copy, 
                                theo_states= guide_theo_states, specific_BAF = "ref_BAF_phased")
         
         merge_Xdata_copy = xclone.model.calculate_Xemm_prob_bb(merge_Xdata_copy, 
                                                       AD_key = "ad_bin_phased", DP_key = "dp_bin",
                                                       outlayer = "correct_emm_prob_log", 
                                                       states = used_specific_states,
                                                       gene_specific = gene_specific_concentration, 
                                                       concentration = concentration)
         merge_Xdata_copy = xclone.model.BAF_smoothing(merge_Xdata_copy,
                                              inlayer = "correct_emm_prob_log",
                                              outlayer = "correct_emm_prob_log_KNN",
-                                             KNN_connectivities_key = "connectivities_expr",
+                                             KNN_connectivities_key = KNN_connect_use_key,
                                              KNN_smooth = True)
         start_prob = np.array([0.3, 0.4, 0.3])                                 
         trans_prob = np.array([[1-2*t, t, t],[t, 1-2*t, t],[t, t, 1-2*t]])
         merge_Xdata_copy = xclone.model.XHMM_smoothing(merge_Xdata_copy,
                                               brk = HMM_brk, 
                                               start_prob = start_prob,  
                                               trans_prob = trans_prob, 
@@ -455,14 +522,100 @@
 
     
     end_time = datetime.now(timezone.utc)
     time_passed = end_time - start_time
     sub_logger.info("BAF plot module finished (%d seconds)" % (time_passed.total_seconds()))
     return None
 
+
+def run_BAF_complex_plot(merge_Xdata,
+                 dataset_name,
+                 plot_cell_anno_key,
+                 set_figtitle = True,
+                 out_dir = None,
+                 **kwargs):
+    """
+    """
+    ## Result output prepare
+    if out_dir is None:
+        cwd = os.getcwd()
+        out_dir = cwd + "/XCLONE_OUT/"
+    
+    out_plot_dir = str(out_dir) + "/plot/"
+    xclone.al.dir_make(out_plot_dir)
+
+    fig_title = ""
+    baf_smooth_fig = out_plot_dir + dataset_name + "_BAF_smooth.png"
+    baf_final_fig1 = out_plot_dir + dataset_name + "_BAF_CNV.png"
+    baf_final_fig2 = out_plot_dir + dataset_name + "_BAF_CNV_denoise.png"
+    baf_final_fig3 = out_plot_dir + dataset_name + "_BAF_CNV_3states.png"
+    baf_final_fig4 = out_plot_dir + dataset_name + "_BAF_CNV_3states_denoise.png"
+
+    sub_logger = get_logger("BAF plot module")
+    sub_logger.info("BAF plot module started")
+    start_time = datetime.now(timezone.utc)
+
+    if set_figtitle:
+        fig_title = dataset_name + " BAF smooth"
+    xclone.pl.BAF_smooth_complex_visualization(merge_Xdata, Xlayer = "BAF_phased_KNN_WMA", 
+                                       cell_anno_key = plot_cell_anno_key, 
+                                       clusters_display_name = plot_cell_anno_key,
+                                       change_colorbar = False, 
+                                       colorbar_name = "BAF",
+                                       title = fig_title,
+                                       save_file = True, 
+                                       out_file = baf_smooth_fig,
+                                       **kwargs)
+    if set_figtitle:
+        fig_title = dataset_name + " BAF module"
+    xclone.pl.Complex_BAF_CNV_visualization(merge_Xdata, weights = False, 
+                                    cell_anno_key = plot_cell_anno_key, 
+                                    clusters_display_name = plot_cell_anno_key, 
+                                    title = fig_title,
+                                    save_file = True, 
+                                    out_file = baf_final_fig1,
+                                    **kwargs)
+                                    
+    
+    if "denoised_posterior_mtx" in merge_Xdata.layers:
+        xclone.pl.Complex_BAF_CNV_visualization(merge_Xdata, Xlayer = "denoised_posterior_mtx",
+                                        weights = False, 
+                                        cell_anno_key = plot_cell_anno_key, 
+                                        clusters_display_name = plot_cell_anno_key,
+                                        title = fig_title + " (denoise)",
+                                        save_file = True, 
+                                        out_file = baf_final_fig2,
+                                        **kwargs)
+    
+    if "add_posterior_mtx" in merge_Xdata.layers:
+        xclone.pl.Complex_BAF_CNV_visualization(merge_Xdata, Xlayer = "add_posterior_mtx",
+                                        weights = False, 
+                                        cell_anno_key = plot_cell_anno_key, 
+                                        clusters_display_name = plot_cell_anno_key,
+                                        title = fig_title,
+                                        save_file = True, 
+                                        out_file = baf_final_fig3,
+                                        **kwargs)
+    if "denoised_add_posterior_mtx" in merge_Xdata.layers:
+        xclone.pl.Complex_BAF_CNV_visualization(merge_Xdata, Xlayer = "denoised_add_posterior_mtx",
+                                        weights = False, 
+                                        cell_anno_key = plot_cell_anno_key, 
+                                        clusters_display_name = plot_cell_anno_key,
+                                        title = fig_title + " (denoise)",
+                                        save_file = True, 
+                                        out_file = baf_final_fig4,
+                                        **kwargs)
+
+    
+    end_time = datetime.now(timezone.utc)
+    time_passed = end_time - start_time
+    sub_logger.info("BAF plot module finished (%d seconds)" % (time_passed.total_seconds()))
+    return None
+
+
 def plot_BAF_module():
     """
     all plots for BAF module.
     """
     pass
 
 def plot_processed_BAF(merge_Xdata,
```

### Comparing `xclone-0.3.4/xclone/model/xclone_combine_wrap.py` & `xclone-0.3.5/xclone/model/xclone_combine_wrap.py`

 * *Files 22% similar despite different names*

```diff
@@ -40,19 +40,22 @@
     dataset_name = config.dataset_name
     
     cell_anno_key = config.cell_anno_key
     exclude_XY = config.exclude_XY
     
     ## RDR BAF settings
     BAF_denoise = config.BAF_denoise
+    RDR_denoise = config.BAF_denoise
     ## combine settings
     copyloss_correct = config.copyloss_correct
     copyloss_correct_mode = config.copyloss_correct_mode
     copygain_correct= config.copygain_correct
     copygain_correct_mode = config.copygain_correct_mode
+    RDR_prior = config.RDR_prior
+    WGD_detection = config.WGD_detection
     
     ## plot settings
     xclone_plot = config.xclone_plot
     plot_cell_anno_key = config.plot_cell_anno_key
     merge_loss = config.merge_loss
     merge_loh = config.merge_loh
     
@@ -92,22 +95,50 @@
         BAF_use_Xlayer = "posterior_mtx"
     
     combine_Xdata = xclone.model.bin_to_gene_mapping(BAF_merge_Xdata,
                         RDR_Xdata,
                         Xlayer = BAF_use_Xlayer,
                         extend_layer = "BAF_extend_post_prob",
                         return_prob = False)
-    
-    combine_Xdata = xclone.model.CNV_prob_combination(combine_Xdata,
-                         RDR_layer = "posterior_mtx",
+    if RDR_denoise:
+        combine_Xdata = xclone.model.denoise_rdr_by_baf(combine_Xdata,
+                                                        RDR_layer = "posterior_mtx",
+                                                        BAF_layer = "BAF_extend_post_prob",
+                                                        out_RDR_layer = "rdr_posterior_mtx_denoised")
+        
+        combine_Xdata = xclone.model.CNV_prob_combination(combine_Xdata,
+                         RDR_layer = "rdr_posterior_mtx_denoised",
                          BAF_layer = "BAF_extend_post_prob",
                          copyloss_correct = copyloss_correct,
                          copyloss_correct_mode = copyloss_correct_mode,
                          copygain_correct = copygain_correct,
-                         copygain_correct_mode = copygain_correct_mode)
+                         copygain_correct_mode = copygain_correct_mode,
+                         RDR_prior = RDR_prior)
+        
+    else:
+
+        combine_Xdata = xclone.model.CNV_prob_combination(combine_Xdata,
+                            RDR_layer = "posterior_mtx",
+                            BAF_layer = "BAF_extend_post_prob",
+                            copyloss_correct = copyloss_correct,
+                            copyloss_correct_mode = copyloss_correct_mode,
+                            copygain_correct = copygain_correct,
+                            copygain_correct_mode = copygain_correct_mode,
+                            RDR_prior = RDR_prior)
+    
+    if WGD_detection:
+        print("[XClone WGD detection performing]")
+        prop_value_threshold = config.WGD_prop_value_threshold
+        cell_prop_threshold = config.WGD_cell_prop_threshold
+        genome_level = config.WGD_detect_genome_level
+        xclone.model.WGD_warning(combine_Xdata, 
+                                 Xlayer = "combine_base_prob", 
+                                 genome_level = genome_level, 
+                                 prop_value_threshold = prop_value_threshold,
+                                 cell_prop_threshold = cell_prop_threshold)
     try:
         combine_Xdata.write(RDR_combine_corrected_file)
     except Exception as e:
         print("[XClone Warning]", e)
     else:
         print("[XClone hint] combine_corrected_file saved in %s." %(out_data_dir))
     
@@ -132,17 +163,53 @@
         if plot_cell_anno_key is None:
             plot_cell_anno_key = cell_anno_key
         run_combine_plot(combine_Xdata, dataset_name, 
                          plot_cell_anno_key, 
                          merge_loss, merge_loh, 
                          set_figtitle,
                          out_dir)
-    
+        if RDR_denoise:
+            rdr_denoise_plot(combine_Xdata, dataset_name, 
+                         plot_cell_anno_key, 
+                         set_figtitle,
+                         out_dir)
+
     return combine_Xdata
 
+def rdr_denoise_plot(combine_Xdata,
+                     dataset_name,
+                     plot_cell_anno_key,
+                     set_figtitle = True,
+                     out_dir = None,
+                     **kwargs):
+    """
+    plotting RDR_Denoised.
+    """
+    ## Result output prepare
+    if out_dir is None:
+        cwd = os.getcwd()
+        out_dir = cwd + "/XCLONE_OUT/"
+    
+    out_plot_dir = str(out_dir) + "/plot/"
+    xclone.al.dir_make(out_plot_dir)
+
+    rdr_final_denoise_fig = out_plot_dir + dataset_name + "_RDR_CNV_denoise.png"
+    if set_figtitle:
+        fig_title = dataset_name + " RDR_CNV_denoise"
+
+
+    xclone.pl.CNV_visualization(combine_Xdata, 
+                                Xlayer = "rdr_posterior_mtx_denoised",
+                                states_weight = np.array([1,2,3]), 
+                                weights = True, 
+                                cell_anno_key = plot_cell_anno_key, 
+                                title = fig_title,
+                                save_file = True, 
+                                out_file = rdr_final_denoise_fig,
+                                **kwargs)
 
 def run_combine_plot(combine_Xdata,
             dataset_name,
             plot_cell_anno_key,
             merge_loss = True,
             merge_loh = True,
             set_figtitle = True,
```

### Comparing `xclone-0.3.4/xclone/model/xclone_rdr_wrap.py` & `xclone-0.3.5/xclone/model/xclone_rdr_wrap.py`

 * *Files 13% similar despite different names*

```diff
@@ -62,16 +62,19 @@
     HMM_brk = config.HMM_brk
     ## optimize 
     max_iter = config.max_iter
     min_iter = config.min_iter
 
     # RDR settings
     filter_ref_ave = config.filter_ref_ave
+    min_gene_keep_num = config.min_gene_keep_num
+    multi_refcelltype = config.multi_refcelltype
     smart_transform = config.smart_transform
     marker_group_anno_key = config.marker_group_anno_key
+    get_marker_genes = config.get_marker_genes
     top_n_marker = config.top_n_marker
     remove_marker = config.remove_marker
     fit_GLM_libratio = config.fit_GLM_libratio
     dispersion_celltype = config.dispersion_celltype
     gene_exp_group = config.gene_exp_group
     gene_exp_ref_log = config.gene_exp_ref_log
     remove_guide_XY = config.remove_guide_XY
@@ -109,36 +112,55 @@
     if exclude_XY:
         RDR_adata = xclone.pp.exclude_XY_adata(RDR_adata)
         print("[XClone warning] RDR module excelude chr XY analysis.")
     ## RDR data preprocessing
     RDR_adata = xclone.pp.check_RDR(RDR_adata, 
     cell_anno_key = cell_anno_key, 
     cell_detection_rate = 0.05, verbose = verbose)
+
+    ## check ref_celltype
+    if ref_celltype in RDR_adata.obs[cell_anno_key].values:
+        pass
+    else:
+        raise ValueError(f"[XClone error] Item '{ref_celltype}' not found in the RDR_adata's annotation.")
     
     ## Transformation for smart-seq data
     RDR_adata = xclone.pp.Xtransformation(RDR_adata, transform = smart_transform, Xlayers = ["raw_expr"])
-    RDR_adata = xclone.pp.Xdata_RDR_preprocess(RDR_adata, filter_ref_ave = filter_ref_ave, 
-    cell_anno_key = cell_anno_key,  ref_celltype = ref_celltype, mode = "FILTER")
+    
+    if config.set_spatial:
+        spatial_transform = config.spatial_transform
+        RDR_adata = xclone.pp.Spatial_Xtransformation(RDR_adata, transform = spatial_transform, Xlayers = ["raw_expr"])
+    
+    ## Consider data coverage before genes filtering (update)
+    RDR_adata = xclone.pp.Xdata_RDR_preprocess(RDR_adata, 
+                                               filter_ref_ave = filter_ref_ave, 
+                                               min_gene_keep_num = min_gene_keep_num,
+                                               cell_anno_key = cell_anno_key,  
+                                               ref_celltype = ref_celltype, 
+                                               mode = "FILTER")
     
     ## marker genes
     if marker_group_anno_key is None:
         marker_group_anno_key = cell_anno_key
-    marker_genes = xclone.pp.get_markers(RDR_adata,
+    if get_marker_genes:
+        marker_genes = xclone.pp.get_markers(RDR_adata,
                                          top_n = top_n_marker,
                                          target_sum=1e4,
                                          rank_group = marker_group_anno_key,
                                          marker_genes_key = "rank_marker_genes",
                                          test_method='wilcoxon')
     ## remove marker genes
     if remove_marker:
         RDR_adata = xclone.pp.filter_markers(RDR_adata, marker_lst = marker_genes)
 
     ## get base bulk and single cell adata
     RDR_adata, RDR_adata_bulk = xclone.pp.Xdata_RDR_preprocess(RDR_adata, filter_ref_ave = None, 
-    cell_anno_key = cell_anno_key, ref_celltype = ref_celltype)
+                                                               min_gene_keep_num = min_gene_keep_num,
+                                                               cell_anno_key = cell_anno_key, 
+                                                               ref_celltype = ref_celltype)
 
     if fit_GLM_libratio:
         ## fit libratio for each cell based on select normal chrs*
         select_normal_chr_num = config.select_normal_chr_num
         RDR_adata_bulk = xclone.model.select_normal_CHR(RDR_adata_bulk, select_chr_num = select_normal_chr_num)
         ### extend the chr index to whole dataset for libratio fitting
         RDR_adata_bulk= xclone.model.extend_chr_index_to_singlecell(RDR_adata_bulk, 
@@ -159,14 +181,21 @@
 
         libsize_key = "library_ratio_capped"
         depth_key = "library_ratio_capped"
     
     else:
         libsize_key = "counts_ratio"
         depth_key = "counts_ratio"
+    
+    ## check cell quality- debug in sapatial transcriptomics, 
+    ## after last step in `xclone.pp.Xdata_RDR_preprocess` 
+    ## may get 0 "counts ratio" again in ST data.
+    cell_flag = RDR_adata.obs[libsize_key] > 0 
+    RDR_adata = RDR_adata[cell_flag,:].copy()
+
     ## fit gene-specific dispersion based on reference celltype
     if dispersion_celltype is None:
         dispersion_celltype = ref_celltype
     RDR_adata_REF = xclone.model.select_celltype(RDR_adata, 
                                                  cell_anno_key = cell_anno_key, 
                                                  select_celltype = dispersion_celltype)
     RDR_adata_REF = xclone.model.fit_Dispersions(RDR_adata_REF, 
@@ -192,14 +221,23 @@
 
     RDR_adata = xclone.model.extra_preprocess(RDR_adata, cluster_key = cell_anno_key,
                                               ref_celltype = ref_celltype,
                                               depth_key=depth_key,
                                               low_dim=False, run_KNN=True, 
                                               KNN_neighbors = KNN_neighbors,
                                               copy=True)
+    
+    if multi_refcelltype:
+        print("multi_refcelltype")
+        # update expected layer
+        RDR_adata = xclone.model.extra_preprocess2(RDR_adata, ref_celltype = ref_celltype, 
+                                   cluster_key=cell_anno_key,
+                                   avg_layer = "ref_avg", 
+                                   depth_key=depth_key, 
+                                   copy=True)
 
     RDR_adata = xclone.model.RDR_smoothing_base(RDR_adata,
                                                 clip = True,
                                                 outlayer = "RDR_smooth",
                                                 cell_anno_key = cell_anno_key,
                                                 ref_celltype = ref_celltype,
                                                 WMA_window_size = WMA_window_size,
@@ -249,19 +287,26 @@
     time_passed = end_time - start_time
     main_logger.info("XClone RDR module finished (%d seconds)" % (time_passed.total_seconds()))
     
     if xclone_plot:
         rdr_plot_vmin = config.rdr_plot_vmin
         rdr_plot_vmax = config.rdr_plot_vmax
         set_figtitle = config.set_figtitle
+
         if run_verbose:
             print("[XClone plotting]")
         if plot_cell_anno_key is None:
             plot_cell_anno_key = cell_anno_key
         
+        plot_remove_immune = config.plot_remove_immune
+        plot_immune_celltype = config.plot_immune_celltype
+        if plot_remove_immune:
+            pass
+
+        
         run_RDR_plot(RDR_adata, dataset_name, 
                      plot_cell_anno_key, 
                      set_figtitle,
                      rdr_plot_vmin, rdr_plot_vmax, 
                      out_dir)
     return RDR_adata                                              
  
@@ -314,14 +359,73 @@
                                 title = fig_title,
                                 save_file = True, 
                                 out_file = rdr_final_fig,
                                 **kwargs)
     
     end_time = datetime.now(timezone.utc)
     time_passed = end_time - start_time
+    sub_logger.info("RDR plot module finished (%d seconds)" % (time_passed.total_seconds()))
+    return None
+
+
+def run_RDR_complex_plot(RDR_adata,
+            dataset_name,
+            plot_cell_anno_key,
+            set_figtitle = True,
+            rdr_plot_vmin = -0.7,
+            rdr_plot_vmax = 0.7,
+            out_dir = None,
+            **kwargs):
+    """
+    """
+    ## Result output prepare
+    if out_dir is None:
+        cwd = os.getcwd()
+        out_dir = cwd + "/XCLONE_OUT/"
+    
+    out_plot_dir = str(out_dir) + "/plot/"
+    xclone.al.dir_make(out_plot_dir)
+
+    # default:XClone
+    fig_title = ""
+    rdr_smooth_fig = out_plot_dir + dataset_name + "_RDR_smooth.png"
+    rdr_final_fig = out_plot_dir + dataset_name + "_RDR_CNV.png"
+
+    sub_logger = get_logger("RDR plot module")
+    sub_logger.info("RDR plot module started")
+    start_time = datetime.now(timezone.utc)
+    
+    if set_figtitle:
+        fig_title = dataset_name + " RDR_smooth (log scale ratio)"
+
+    xclone.pl.RDR_smooth_complex_visualization(RDR_adata, 
+                                       Xlayer = "RDR_smooth", 
+                                       cell_anno_key = plot_cell_anno_key,
+                                       clusters_display_name = plot_cell_anno_key, 
+                                       change_colorbar = False,
+                                       vmin = rdr_plot_vmin, vmax = rdr_plot_vmax,
+                                       title = fig_title,
+                                       save_file = True, 
+                                       out_file = rdr_smooth_fig,
+                                       **kwargs)
+    if set_figtitle:
+        fig_title = dataset_name + " RDR module"
+    
+    xclone.pl.Complex_CNV_visualization(RDR_adata, 
+                                states_weight = np.array([1,2,3]), 
+                                weights = True, 
+                                cell_anno_key = plot_cell_anno_key, 
+                                clusters_display_name = plot_cell_anno_key, 
+                                title = fig_title,
+                                save_file = True, 
+                                out_file = rdr_final_fig,
+                                **kwargs)
+    
+    end_time = datetime.now(timezone.utc)
+    time_passed = end_time - start_time
     sub_logger.info("RDR plot module finished (%d seconds)" % (time_passed.total_seconds()))
     return None
 
 def plot_RDR_module():
     """
     all plots for RDR module.
     """
```

### Comparing `xclone-0.3.4/xclone/plot/CNV_plot.py` & `xclone-0.3.5/xclone/plot/CNV_plot.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/plot/_BAF_debug.py` & `xclone-0.3.5/xclone/plot/_BAF_debug.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/plot/_BAF_plot.py` & `xclone-0.3.5/xclone/plot/_BAF_plot.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/plot/_RDR_plot.py` & `xclone-0.3.5/xclone/plot/_RDR_plot.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/plot/__init__.py` & `xclone-0.3.5/xclone/plot/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,22 +35,24 @@
 from ._BAF_debug import bulk_AF_chr
 
 from ._explore import visualize_prob, compare_prob
 from ._explore import visualize_count
 
 ## smoothing plotting
 from .smooth_plot import raw_ratio_visualization
-from .smooth_plot import smooth_visualization, RDR_smooth_visualization, BAF_smooth_visualization, BAF_smooth_complex_visualization
-from .smooth_plot import smooth_visualization2, smooth_visualization3
+from .smooth_plot import smooth_visualization, RDR_smooth_visualization, RDR_smooth_complex_visualization, BAF_smooth_visualization, BAF_smooth_complex_visualization
+from .smooth_plot import smooth_visualization2
 
 ## CNV plotting
 ### update
 from .CNV_plot import CNV_visualization, Complex_CNV_visualization
 from .CNV_plot import BAF_CNV_visualization, Complex_BAF_CNV_visualization
 from .CNV_plot import Combine_CNV_visualization, Complex_Combine_CNV_visualization
 
 # from .CNV_plot import CNV_visualization, CNV_visualization_complex
 # from .CNV_plot import CNV_visualization2, CNV_visualization2_complex
 # from .CNV_plot import CNV_visualization_combine, complex_CNV_visualization_combine
 
 # from .CNV_plot import CNV_combine_visualization, CNV_combine_visualization_complex
 # from .CNV_plot import CNV_LOH_visualization
+
+from .prob_plot import prob_visualization
```

### Comparing `xclone-0.3.4/xclone/plot/_base_manhattan.py` & `xclone-0.3.5/xclone/plot/_base_manhattan.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/plot/_base_xanndata.py` & `xclone-0.3.5/xclone/plot/_base_xanndata.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/plot/_data.py` & `xclone-0.3.5/xclone/plot/_data.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/plot/_explore.py` & `xclone-0.3.5/xclone/plot/_explore.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/plot/_plot_style.py` & `xclone-0.3.5/xclone/plot/_plot_style.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/plot/_test.py` & `xclone-0.3.5/xclone/plot/_test.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/plot/_utils.py` & `xclone-0.3.5/xclone/plot/_utils.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/plot/_visualize.py` & `xclone-0.3.5/xclone/plot/_visualize.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/plot/base_plot.py` & `xclone-0.3.5/xclone/plot/base_plot.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/plot/smooth_plot.py` & `xclone-0.3.5/xclone/plot/smooth_plot.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,34 +44,40 @@
     Xheatmap(re_Xdata, Xlayer = Xlayer, cell_anno_key = cell_anno_key, 
             vmin=vmin, vmax=vmax,
             colorbar_name = colorbar_name, **kwargs)
 
 
 def smooth_visualization2(Xdata, cell_anno_key = ["cell_type", "Clone"],
                           clusters_display_name = ["Celltype", "Clone"],
-                          Xlayer = "RDR_smooth",vmin=-0.7, vmax=0.7, **kwargs):
+                          Xlayer = "RDR_smooth",vmin=-0.7, vmax=0.7, 
+                          colorbar_name = "RDR smooth (log)", **kwargs):
     """
     can setting colorbar;
     XXheatmap
     """
     re_Xdata = reorder_data_by_cellanno(Xdata, cell_anno_key =cell_anno_key)
     XXheatmap(re_Xdata, Xlayer = Xlayer, cell_anno_key = cell_anno_key, 
               clusters_display_name = clusters_display_name,
-              vmin=vmin, vmax=vmax, **kwargs)
+              vmin=vmin, vmax=vmax, 
+              colorbar_name = colorbar_name, **kwargs)
 
-def smooth_visualization3(Xdata, cell_anno_key = ["cell_type", "Clone"],
+def RDR_smooth_complex_visualization(Xdata, cell_anno_key = ["cell_type", "Clone"],
                           clusters_display_name = ["Celltype", "Clone"],
-                          Xlayer = "RDR_smooth", vmin=-0.7, vmax=0.7, **kwargs):
+                          Xlayer = "RDR_smooth", vmin=-0.7, vmax=0.7, 
+                          colorbar_name = "RDR smooth (log)", **kwargs):
     """
+    update from `smooth_visualization3`
     default: change color_bar
+
     """
     re_Xdata = reorder_data_by_cellanno(Xdata, cell_anno_key =cell_anno_key)
     XXheatmap(re_Xdata, Xlayer = Xlayer, cell_anno_key = cell_anno_key, 
               clusters_display_name = clusters_display_name,
               vmin=vmin, vmax=vmax, colorbar_ticks = [vmin, 0, vmax], 
+              colorbar_name = colorbar_name,
               colorbar_label = ["copy loss",  "copy neutral",  "copy gain"],
               **kwargs)
 
 
 def BAF_smooth_visualization(Xdata, cell_anno_key = "cell_type", 
                              Xlayer = "phased_KNN_smoothed", 
                              colorbar_name = "BAF smooth",
```

### Comparing `xclone-0.3.4/xclone/preprocessing/_RDR_genes.py` & `xclone-0.3.5/xclone/preprocessing/_RDR_genes.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/preprocessing/_RDR_preprocess.py` & `xclone-0.3.5/xclone/preprocessing/_RDR_preprocess.py`

 * *Files 17% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 # 2. filtering genes based on ref cells-for raW ratio based following analysis- FUNC `Xdata_RDR_preprocess`
 # 3. filtering nan value in any mtx for genes.(like nan in emm_prob) to solve num issue
 
 ## Part-I data preprocessing part in RDR module
 # YH comment: combine the multiple output adata objects into one
 def Xdata_RDR_preprocess(Xdata, 
                          filter_ref_ave = 0,
+                         min_gene_keep_num = 3000,
                          cell_anno_key = "cell_type", 
                          ref_celltype = None,
                          var_key = "ref_avg",
                          obs_key = "counts_ratio",
                          mode = "ALL"):
     """
     Xdata_RDR_preprocess
@@ -90,46 +91,66 @@
     # reference data preprocessing
     if ref_celltype is None:
         raise ValueError("ref_celltype should be assigned! Pls check!")
 
     ref_flag = Xdata.obs[cell_anno_key] == ref_celltype
     ref_Xdata = Xdata[ref_flag,:]
 
-    Xdata.var['ref_avg'] = ref_Xdata.X.A.mean(axis=0)
+    Xdata.var[var_key] = ref_Xdata.X.A.mean(axis=0)
 
-    
     ## filter genes based on ref_average counts
     ### if filter_ref_ave is None, skip the filtering step*
     ### if mode == "FILTER", just do the filter step*
     gene_num = Xdata.var.shape[0]
+    cell_num = Xdata.obs.shape[0]
     if filter_ref_ave is None:
         gene_flag = np.ones((gene_num), dtype=bool)
     else:
-        gene_flag = Xdata.var['ref_avg'] > filter_ref_ave
+        gene_flag = Xdata.var[var_key] > filter_ref_ave
+        if gene_flag.sum() < min_gene_keep_num:
+            # make sure at least default 3000 genes,in case low coverage data filter out too much genes
+            quantile_value = min_gene_keep_num/Xdata.shape[1]
+            if quantile_value > 1:
+                quantile_value = 1
+            filter_ref_ave_recomend = np.quantile(Xdata.var[var_key], quantile_value)
+            print("filter_ref_ave_recomend", filter_ref_ave_recomend)
+            if filter_ref_ave_recomend > 0:
+                gene_flag = Xdata.var[var_key] > filter_ref_ave_recomend
+            else:
+                gene_flag = Xdata.var[var_key] > 0
+                print("[XClone hint]: just filter the genes (ref_avg=0)")
     
     # mode="FILTER"
     update_Xdata = Xdata[:, gene_flag].copy()
     ## cell counts_ratio to be compared with learned libratio
-    update_Xdata.obs[obs_key] = update_Xdata.X.A.sum(axis=1) / update_Xdata.var['ref_avg'].sum()
+    update_Xdata.obs[obs_key] = update_Xdata.X.A.sum(axis=1) / update_Xdata.var[var_key].sum()
     
     if mode == "FILTER":
-        
+        ## filter genes
         print("[XClone-RDR preprocessing] Filter out %d genes / %d total genes, remain %d genes" 
                %(gene_num - gene_flag.sum(), gene_num, gene_flag.sum()))
+        
+        ## filter cells/spots with no counts
+        cell_flag = update_Xdata.obs[obs_key] > 0
+        update_Xdata = update_Xdata[cell_flag, :]
+
+        print("[XClone-RDR preprocessing] Filter out %d cells / %d total cells, remain %d cells" 
+               %(cell_num - cell_flag.sum(), cell_num, cell_flag.sum()))
         return update_Xdata
     
     # mode="ALL"
     ## process both cellbased data and celltype based data.
     celltype_ad = rr_ad_celltype_processing(update_Xdata, ref_celltype, cell_anno_key)
     is_ref = celltype_ad.obs[cell_anno_key] == ref_celltype
 
-    celltype_ad.var["ref_avg"] = celltype_ad[is_ref,:].X.toarray()[0]
+    celltype_ad.var[var_key] = celltype_ad[is_ref,:].X.toarray()[0]
 
     rr_cell_ad = rr_ad_cell_processing(update_Xdata, ref_celltype, cell_anno_key)
     update_Xdata.layers["raw_ratio"] = rr_cell_ad.X
+    update_Xdata.layers["test_ratio"] = rr_cell_ad.layers["test_ratio"]
 
     return update_Xdata, celltype_ad
 
 ### Sub part-For visualization -RDR raw ratio
 
 def rr_ad_celltype_processing(Xdata, ref_celltype, cell_anno_key):
     """
@@ -185,15 +206,18 @@
     
     # 02-cell based anndata
     ## calculate ratio-cell
     cell_lib = obs_Xdata.X.A.sum(axis=1, keepdims=True)
     # raw_ratio = np.log((obs_Xdata.X.A + 0.1) / (cell_lib*ref_norm)) ## add small value 0.1 for visualization
     raw_ratio = np.log((obs_Xdata.X.A + 1e-8) / (cell_lib*ref_norm)) ## add small value 1e-6 for visualization
 
+    test_ratio = np.log((np.sqrt(obs_Xdata.X.A + 1) + np.sqrt(obs_Xdata.X.A) + 1e-8) / (cell_lib*ref_norm))
+
     rr_cell_ad = ad.AnnData(raw_ratio, var=obs_Xdata.var.copy(), obs = obs_Xdata.obs.copy())
+    rr_cell_ad.layers["test_ratio"] = test_ratio
     
     print("output anndata is not sparse matrix.")
     return rr_cell_ad
 
 
 ## Part-II libsize ratio estimation part in RDR module
 ## see _RDR_libratio
```

### Comparing `xclone-0.3.4/xclone/preprocessing/_Xdata_manipulation.py` & `xclone-0.3.5/xclone/preprocessing/_Xdata_manipulation.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/preprocessing/__init__.py` & `xclone-0.3.5/xclone/preprocessing/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 """XClone preprocessing.
 """
 
-
+from ._annotation_prepare import add_cytoband
 from ._annotation_prepare import resort_chr_df, get_chr_arm_df, concat_df
-from ._anno_data import load_anno, load_hg38_genes, load_hg19_genes, load_cc_genes, load_hk_genes
-from ._demo_data import load_TNBC1_BAF, load_TNBC1_RDR
+from ._anno_data import load_anno, load_hg38_genes, load_hg19_genes, load_mm10_genes
+from ._anno_data import load_cc_genes, load_hk_genes
+# from ._demo_data import load_TNBC1_BAF, load_TNBC1_RDR
 
 from ._data import process_barcodes
 from ._data import check_RDR_BAF_anno
 from ._data import resort_mtx_bychr
 from ._data import resort_mtx_bycell
 
 from ._data import xclonedata
 from ._data import extra_anno
 from ._data import exclude_XY_adata
 from ._data import check_RDR, check_BAF
 from ._data import check_RDR_BAF_cellorder, check_data_combine
 
 
 # RDR
-from ._transformation import Xtransformation
+from ._transformation import Xtransformation, Spatial_Xtransformation
 from ._RDR_preprocess import Xdata_RDR_preprocess, gene_length_scale
 ## RDR genes
 from ._RDR_genes import get_markers
 from ._RDR_genes import filter_markers
 
 from ._preprocessing import valid_cell, gene_filter
 from ._preprocessing import filter_nulldata, filter_2nulldata, tidy_Xdata
@@ -40,8 +41,11 @@
 from ._utils import annotate_node
 # from ._utils import get_region_position
 
 from ._efficiency import efficiency_preview
 
 from ._Xdata_manipulation import Xdata_region_selection, Xdata_cell_selection
 
-from .xclone_preprocess_wrap import load_Xdata
+from .xclone_preprocess_wrap import load_Xdata
+
+## spatial
+# from._spatial_data import load_visium
```

### Comparing `xclone-0.3.4/xclone/preprocessing/_anno_data.py` & `xclone-0.3.5/xclone/preprocessing/_anno_data.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,14 +23,16 @@
         stream = pkg_resources.resource_stream(__name__, '../data/anno_data/annotate_genes_hg38_update.txt')
     if genome_mode == "hg38_blocks":
         stream = pkg_resources.resource_stream(__name__, '../data/anno_data/annotate_blocks_hg38_update.txt')
     if genome_mode == "hg19_genes":
         stream = pkg_resources.resource_stream(__name__, '../data/anno_data/annotate_genes_hg19_update.txt')
     if genome_mode == "hg19_blocks":
         stream = pkg_resources.resource_stream(__name__, '../data/anno_data/annotate_blocks_hg19_update.txt')
+    if genome_mode == "mm10_genes":
+        stream = pkg_resources.resource_stream(__name__, '../data/anno_data/annotate_genes_mm10.txt')
     return pd.read_table(stream)#encoding='latin-1'
 
 
 def load_hg38_genes():
     """Return a genes list of hg38.
     ## example usage of load_anno
     usage: from xclone.utils import load_hg38_genes
@@ -54,14 +56,19 @@
     """Return a genes list of hg19.
     ## example usage of load_anno
     usage: from xclone.utils import load_hg19_genes
     load_hg19_genes()
     """
     return load_anno("hg19_genes")['GeneName']
 
+def load_mm10_genes():
+    """Return a genes list of mm10.
+    """
+    return load_anno("mm10_genes")['GeneName']
+
 def load_cc_genes():
     """Return a list of cell cycle genes.
     """
     stream = pkg_resources.resource_stream(__name__, '../data/anno_data/cellcycle_genes.txt')
     return pd.read_table(stream)
```

### Comparing `xclone-0.3.4/xclone/preprocessing/_annotation_prepare.py` & `xclone-0.3.5/xclone/preprocessing/_annotation_prepare.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Base functions for XClone annotation data 
 preprocessing/preparation.
 """
 
 # Author: Rongting Huang
 # Date: 2021/05/04
 # update: 2021/07/21
+# extend to mouse annotation: 20230814
 
 
 import pandas as pd
 import numpy as np
 
 ## Part I: For hg19/38 blocks/genes chr_region annotation preprocessing (2021/05/05)
 def resort_chr_df(chr_df):
@@ -99,7 +100,41 @@
         print("Error! Pls check chromosome order!")
     out_put_df = concat_df.drop(columns=['another_chr'])
     return out_put_df
 
 
 
 ## chr info prepare
+
+## Part II: For mm10 genes chr_region annotation preprocessing (2023/08/14)
+
+def add_cytoband(sort_genes_region, cytoband, out_file):
+    """
+    Func:
+        add cytoband info in annotated genes.
+    Example:
+    add_cytoband(sort_genes_region, cytoband, out_file)
+    """
+    
+    def cytoband_fun(r_series):
+        """
+        Func:
+        add cytoband info in separate chr region.
+
+        Example:
+        band_results = sort_genes_region.apply(cytoband_fun, axis=1)
+        """
+        chr_specific_band = cytoband[cytoband["chr"] == r_series["chr"]]
+        start_pos = r_series["start"]
+        stop_pos = r_series["stop"]
+        chr_specific_band["start_flag"] = (chr_specific_band["start"] <= start_pos)
+        chr_specific_band["stop_flag"] = (chr_specific_band["stop"] >= stop_pos)
+        flag = chr_specific_band["start_flag"] & chr_specific_band["stop_flag"]
+        band_info = chr_specific_band[flag]["arm_info"]
+        return band_info
+    
+    band_results = sort_genes_region.apply(cytoband_fun, axis=1)
+    band_results_lst = band_results.iloc[:,0].dropna()
+    for i in range(1, band_results.shape[1]):
+        band_results_lst = band_results_lst.append(band_results.iloc[:,i].dropna())
+    sort_genes_region["band"] = band_results_lst
+    sort_genes_region.to_csv(out_file, sep = "\t", index = False)
```

### Comparing `xclone-0.3.4/xclone/preprocessing/_data.py` & `xclone-0.3.5/xclone/preprocessing/_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 def get_Xmtx(X, genome_mode):
     """
     Function: prepare data format for XClone
     ------
     params:
     X: csr_mtx /csr_mtx path
-    genome_mode: hg38_genes/hg38_blocks/hg19_genes/hg19_blocks
+    genome_mode: hg38_genes/hg38_blocks/hg19_genes/hg19_blocks/mm10_genes
     default: hg38_genes
     ------
     usage:
     from xclone.model.preprocessing_utils import get_Xmtx
     dat_dir = '/storage/yhhuang/users/rthuang/processed_data/xcltk/
     xianjie-cpos/kat_022621/TNBC1-csp-post/phase-snp-even/'
     X = dat_dir + 'kat-csp-post.50kb.block.AD.mtx'
@@ -42,14 +42,16 @@
         X_data = sp.io.mmread(X).tocsr()
     ## use chr1-22+XY, 
     ## can be updated if xcltk output change[Note1]
     if genome_mode=="hg19_genes":
         X_data = X_data[0:32696,:]
     if genome_mode=="hg38_genes":
         X_data = X_data[0:33472,:]
+    if genome_mode=="mm10_genes":
+        X_data = X_data[0:32195,:]
     return X_data.T
 
 def resort_mtx_bychr(mtx_file, features_file, assign_sort_index=None, out_file = None, keep_all = True):
     """
     Function:
     sort the mtx as the assignned chromosome index.
     For thr output gene based mtx is not in order.
@@ -202,15 +204,15 @@
     prepare data format for XClone
     
     Params:
     -------
     X: csr_mtx/csr_mtx path, can be list
     data_mode: 'BAF' OR 'RDR'
     mtx_barcodes_file: barcodes_file path
-    genome_mode: hg38_genes/hg38_blocks/hg19_genes/hg19_blocks
+    genome_mode: hg38_genes/hg38_blocks/hg19_genes/hg19_blocks/mm10_genes
     default: hg38_genes
     
     Example:
     --------
     * Load xclonedata
     >>> import xclone
     >>> dat_dir = '/storage/yhhuang/users/rthuang/processed_data/xcltk/
@@ -288,14 +290,16 @@
     anno_data = pd.read_csv(anno_file, sep = sep)
     # merge annotaion
     anno_data_update = Xdata.obs.merge(anno_data.set_index(barcodes_key), left_index=True, right_index=True, how = "left")
     
     if isinstance(cell_anno_key, list):
         for key_ in cell_anno_key:
             anno_data_update[key_] = anno_data_update[key_].astype('category')
+    elif cell_anno_key is None:
+        pass
     else:
         anno_data_update[cell_anno_key] = anno_data_update[cell_anno_key].astype('category')
     
     Xdata.obs = anno_data_update
     return Xdata if copy else None
 
 ## Part III: check data validity
```

### Comparing `xclone-0.3.4/xclone/preprocessing/_demo_data.py` & `xclone-0.3.5/xclone/preprocessing/_demo_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Base functions for XClone demo data loading.
 """
 
 # Author: Rongting Huang
 # Date: 2021/07/15
 # update: 2022/07/13
+# deprecated 2023/08/14
 
 import pkg_resources
 import pandas as pd
 import scipy as sp
 
 from ._data import xclonedata
 # import anndata as an
```

### Comparing `xclone-0.3.4/xclone/preprocessing/_preprocessing.py` & `xclone-0.3.5/xclone/preprocessing/_preprocessing.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone/preprocessing/_transformation.py` & `xclone-0.3.5/xclone/preprocessing/_transformation.py`

 * *Files 27% similar despite different names*

```diff
@@ -12,13 +12,27 @@
 ## scRNA-seq data; smart-seq
 def Xtransformation(Xdata, transform = True, Xlayers = ["raw_expr"]):
     """
     Expression transformation for smart-seq scRNA count.
     Xlayers for transformation.
     """
     if transform:
-        Xdata.X = sparse.csr_matrix(np.round(np.log(Xdata.X.A + 1)))
         for layer_ in Xlayers:
-            Xdata.layers[layer_] = Xdata.X
+            Xdata.layers[layer_] = Xdata.X.copy()
+        
+        Xdata.X = sparse.csr_matrix(np.round(np.log(Xdata.X.A + 1)))
     return Xdata
 
-## scATAC-seq data 
+## scATAC-seq data
+
+## scRNA-seq data; smart-seq
+def Spatial_Xtransformation(Xdata, transform = True, Xlayers = ["raw_expr"]):
+    """
+    Expression transformation for smart-seq scRNA count.
+    Xlayers for transformation.
+    """
+    if transform:
+        for layer_ in Xlayers:
+            Xdata.layers[layer_] = Xdata.X.copy()
+            trans_data = np.log(np.sqrt(Xdata.X.A + 1) + np.sqrt(Xdata.X.A))
+        Xdata.X = sparse.csr_matrix(np.round(trans_data))
+    return Xdata
```

### Comparing `xclone-0.3.4/xclone/preprocessing/_utils.py` & `xclone-0.3.5/xclone/preprocessing/_utils.py`

 * *Files identical despite different names*

### Comparing `xclone-0.3.4/xclone.egg-info/SOURCES.txt` & `xclone-0.3.5/xclone.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,34 @@
+LICENSE
 README.rst
 setup.py
 xclone/__init__.py
 xclone/_config.py
 xclone/_logging.py
 xclone/version.py
 xclone.egg-info/PKG-INFO
 xclone.egg-info/SOURCES.txt
 xclone.egg-info/dependency_links.txt
 xclone.egg-info/requires.txt
 xclone.egg-info/top_level.txt
 xclone/analysis/__init__.py
 xclone/analysis/_clustering.py
+xclone/analysis/_spatial.py
 xclone/analysis/evaluation.py
 xclone/analysis/extract.py
 xclone/data/__init__.py
+xclone/data/anno_data/annotate_blocks_hg19.txt
+xclone/data/anno_data/annotate_blocks_hg19_update.txt
+xclone/data/anno_data/annotate_blocks_hg38.txt
+xclone/data/anno_data/annotate_blocks_hg38_update.txt
+xclone/data/anno_data/annotate_genes_hg19_update.txt
+xclone/data/anno_data/annotate_genes_hg38_update.txt
+xclone/data/anno_data/annotate_genes_mm10.txt
+xclone/data/anno_data/cellcycle_genes.txt
+xclone/data/anno_data/housekeeping_genes.txt
 xclone/data/demo_datasets/__init__.py
 xclone/data/demo_datasets/_datasets.py
 xclone/model/HMM_BB.py
 xclone/model/HMM_NB.py
 xclone/model/HMM_base.py
 xclone/model/XClone_combine.py
 xclone/model/_BAF.py
@@ -56,14 +67,15 @@
 xclone/plot/_data.py
 xclone/plot/_explore.py
 xclone/plot/_plot_style.py
 xclone/plot/_test.py
 xclone/plot/_utils.py
 xclone/plot/_visualize.py
 xclone/plot/base_plot.py
+xclone/plot/prob_plot.py
 xclone/plot/smooth_plot.py
 xclone/preprocessing/_RDR_genes.py
 xclone/preprocessing/_RDR_preprocess.py
 xclone/preprocessing/_Xdata_manipulation.py
 xclone/preprocessing/__init__.py
 xclone/preprocessing/_anno_data.py
 xclone/preprocessing/_annotation_prepare.py
```

