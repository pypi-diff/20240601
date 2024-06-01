# Comparing `tmp/mbapy-0.7.4.tar.gz` & `tmp/mbapy-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbapy-0.7.4.tar", last modified: Fri May 10 13:06:23 2024, max compression
+gzip compressed data, was "mbapy-0.8.0.tar", last modified: Sat Jun  1 12:01:51 2024, max compression
```

## Comparing `mbapy-0.7.4.tar` & `mbapy-0.8.0.tar`

### file list

```diff
@@ -1,109 +1,124 @@
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.646023 mbapy-0.7.4/
--rw-rw-rw-   0        0        0     1085 2023-09-30 06:15:47.000000 mbapy-0.7.4/LICENSE
--rw-rw-rw-   0        0        0      214 2024-04-21 10:41:48.000000 mbapy-0.7.4/MANIFEST.in
--rw-rw-rw-   0        0        0    10206 2024-05-10 13:06:23.644024 mbapy-0.7.4/PKG-INFO
--rw-rw-rw-   0        0        0     8039 2024-04-30 02:19:58.000000 mbapy-0.7.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.461975 mbapy-0.7.4/mbapy/
--rw-rw-rw-   0        0        0     1203 2024-01-04 08:03:01.000000 mbapy-0.7.4/mbapy/__init__.py
--rw-rw-rw-   0        0        0      402 2024-05-10 13:06:01.000000 mbapy-0.7.4/mbapy/__version__.py
--rw-rw-rw-   0        0        0    27309 2024-04-25 14:59:13.000000 mbapy-0.7.4/mbapy/base.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.523398 mbapy-0.7.4/mbapy/bio/
--rw-rw-rw-   0        0        0      133 2024-01-08 14:19:44.000000 mbapy-0.7.4/mbapy/bio/__init__.py
--rw-rw-rw-   0        0        0    21230 2024-04-29 08:59:11.000000 mbapy-0.7.4/mbapy/bio/peptide.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.537643 mbapy-0.7.4/mbapy/dl_torch/
--rw-rw-rw-   0        0        0      361 2024-01-11 01:58:53.000000 mbapy-0.7.4/mbapy/dl_torch/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.541641 mbapy-0.7.4/mbapy/dl_torch/arch/
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.547202 mbapy-0.7.4/mbapy/dl_torch/arch/CL/
--rw-rw-rw-   0        0        0       34 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/arch/CL/__init__.py
--rw-rw-rw-   0        0        0    16559 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/arch/CL/builder.py
--rw-rw-rw-   0        0        0     2423 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/arch/CL/trainer.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.552198 mbapy-0.7.4/mbapy/dl_torch/arch/CLIP/
--rw-rw-rw-   0        0        0       32 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/arch/CLIP/__init__.py
--rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.4/mbapy/dl_torch/arch/CLIP/builder.py
--rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.7.4/mbapy/dl_torch/arch/CLIP/trainer.py
--rw-rw-rw-   0        0        0      203 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/arch/__init__.py
--rw-rw-rw-   0        0        0    26096 2024-01-05 08:43:17.000000 mbapy-0.7.4/mbapy/dl_torch/bb.py
--rw-rw-rw-   0        0        0     6352 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/data.py
--rw-rw-rw-   0        0        0     1063 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/hyper_search.py
--rw-rw-rw-   0        0        0     4113 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/loss.py
--rw-rw-rw-   0        0        0    13191 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/m.py
--rw-rw-rw-   0        0        0     4661 2023-12-11 09:26:16.000000 mbapy-0.7.4/mbapy/dl_torch/optim.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.553255 mbapy-0.7.4/mbapy/dl_torch/paper/
--rw-rw-rw-   0        0        0       18 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/paper/__init__.py
--rw-rw-rw-   0        0        0     2917 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/dl_torch/paper/bb.py
--rw-rw-rw-   0        0        0    17600 2024-01-11 07:34:28.000000 mbapy-0.7.4/mbapy/dl_torch/utils.py
--rw-rw-rw-   0        0        0    22088 2024-04-21 10:54:51.000000 mbapy-0.7.4/mbapy/file.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.557255 mbapy-0.7.4/mbapy/file_utils/
--rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.4/mbapy/file_utils/__init__.py
--rw-rw-rw-   0        0        0     7095 2023-12-18 14:29:23.000000 mbapy-0.7.4/mbapy/file_utils/image.py
--rw-rw-rw-   0        0        0    11531 2024-03-10 02:50:26.000000 mbapy-0.7.4/mbapy/file_utils/video.py
--rw-rw-rw-   0        0        0    25377 2024-02-23 13:27:31.000000 mbapy-0.7.4/mbapy/game.py
--rw-rw-rw-   0        0        0     3364 2023-12-18 14:29:23.000000 mbapy-0.7.4/mbapy/paper.py
--rw-rw-rw-   0        0        0    11217 2024-05-04 10:36:23.000000 mbapy-0.7.4/mbapy/plot.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.564867 mbapy-0.7.4/mbapy/plot_utils/
--rw-rw-rw-   0        0        0        0 2024-04-21 13:25:30.000000 mbapy-0.7.4/mbapy/plot_utils/__init__.py
--rw-rw-rw-   0        0        0    15028 2024-04-24 01:25:33.000000 mbapy-0.7.4/mbapy/plot_utils/bar_utils.py
--rw-rw-rw-   0        0        0        0 2024-04-21 13:26:21.000000 mbapy-0.7.4/mbapy/plot_utils/line_utils.py
--rw-rw-rw-   0        0        0    11533 2024-04-23 03:04:53.000000 mbapy-0.7.4/mbapy/plot_utils/scatter_utils.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.569496 mbapy-0.7.4/mbapy/sci_utils/
--rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.7.4/mbapy/sci_utils/__init__.py
--rw-rw-rw-   0        0        0    10594 2024-01-20 12:03:17.000000 mbapy-0.7.4/mbapy/sci_utils/paper_download.py
--rw-rw-rw-   0        0        0    23045 2023-12-11 09:26:16.000000 mbapy-0.7.4/mbapy/sci_utils/paper_parse.py
--rw-rw-rw-   0        0        0    16559 2024-04-25 15:14:19.000000 mbapy-0.7.4/mbapy/sci_utils/paper_search.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.606990 mbapy-0.7.4/mbapy/scripts/
--rw-rw-rw-   0        0        0      153 2024-01-08 13:31:52.000000 mbapy-0.7.4/mbapy/scripts/__init__.py
--rw-rw-rw-   0        0        0       68 2024-01-08 13:31:52.000000 mbapy-0.7.4/mbapy/scripts/__main__.py
--rw-rw-rw-   0        0        0     2821 2024-04-21 10:45:32.000000 mbapy-0.7.4/mbapy/scripts/_main_.py
--rw-rw-rw-   0        0        0     1628 2024-05-02 13:29:19.000000 mbapy-0.7.4/mbapy/scripts/_script_utils_.py
--rw-rw-rw-   0        0        0     5549 2024-02-23 13:27:31.000000 mbapy-0.7.4/mbapy/scripts/avif.py
--rw-rw-rw-   0        0        0     1947 2024-01-22 08:25:16.000000 mbapy-0.7.4/mbapy/scripts/cluster.py
--rw-rw-rw-   0        0        0    13566 2024-01-08 13:31:52.000000 mbapy-0.7.4/mbapy/scripts/cnipa.py
--rw-rw-rw-   0        0        0     2741 2024-02-23 13:27:31.000000 mbapy-0.7.4/mbapy/scripts/cp.py
--rw-rw-rw-   0        0        0     4806 2024-04-24 02:05:38.000000 mbapy-0.7.4/mbapy/scripts/duitang.py
--rw-rw-rw-   0        0        0     3175 2024-05-03 09:21:25.000000 mbapy-0.7.4/mbapy/scripts/extract-dir.py
--rw-rw-rw-   0        0        0     2637 2024-01-08 13:31:52.000000 mbapy-0.7.4/mbapy/scripts/extract_paper.py
--rw-rw-rw-   0        0        0     3781 2024-04-15 15:02:22.000000 mbapy-0.7.4/mbapy/scripts/file-size.py
--rw-rw-rw-   0        0        0    28801 2024-05-06 09:11:10.000000 mbapy-0.7.4/mbapy/scripts/hplc.py
--rw-rw-rw-   0        0        0    26861 2024-05-10 09:08:25.000000 mbapy-0.7.4/mbapy/scripts/mass.py
--rw-rw-rw-   0        0        0     2614 2024-02-23 13:27:31.000000 mbapy-0.7.4/mbapy/scripts/mv.py
--rw-rw-rw-   0        0        0    29037 2024-05-10 08:37:48.000000 mbapy-0.7.4/mbapy/scripts/peptide.py
--rw-rw-rw-   0        0        0     1679 2024-01-12 08:11:59.000000 mbapy-0.7.4/mbapy/scripts/reviz.py
--rw-rw-rw-   0        0        0     2101 2024-02-23 13:27:31.000000 mbapy-0.7.4/mbapy/scripts/rm.py
--rw-rw-rw-   0        0        0     5392 2024-01-08 13:31:52.000000 mbapy-0.7.4/mbapy/scripts/scihub.py
--rw-rw-rw-   0        0        0     8636 2024-01-08 13:31:52.000000 mbapy-0.7.4/mbapy/scripts/scihub_selenium.py
--rw-rw-rw-   0        0        0     5633 2024-02-23 13:27:31.000000 mbapy-0.7.4/mbapy/scripts/splash_img.py
--rw-rw-rw-   0        0        0     9128 2024-03-14 08:21:47.000000 mbapy-0.7.4/mbapy/scripts/video.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.618525 mbapy-0.7.4/mbapy/stats/
--rw-rw-rw-   0        0        0     2839 2023-10-04 07:59:59.000000 mbapy-0.7.4/mbapy/stats/__init__.py
--rw-rw-rw-   0        0        0    30529 2023-10-06 03:00:11.000000 mbapy-0.7.4/mbapy/stats/cluster.py
--rw-rw-rw-   0        0        0    15779 2024-04-09 06:03:49.000000 mbapy-0.7.4/mbapy/stats/df.py
--rw-rw-rw-   0        0        0    19333 2023-09-30 06:15:47.000000 mbapy-0.7.4/mbapy/stats/geography.py
--rw-rw-rw-   0        0        0     4009 2024-04-23 02:29:03.000000 mbapy-0.7.4/mbapy/stats/reg.py
--rw-rw-rw-   0        0        0    16955 2024-04-05 10:19:56.000000 mbapy-0.7.4/mbapy/stats/test.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.629536 mbapy-0.7.4/mbapy/storage/
--rw-rw-rw-   0        0        0    69698 2024-01-11 01:58:53.000000 mbapy-0.7.4/mbapy/storage/libsci.dll
--rw-rw-rw-   0        0        0    15864 2024-01-11 01:58:53.000000 mbapy-0.7.4/mbapy/storage/libsci.so
--rw-rw-rw-   0        0        0    40252 2024-01-11 01:58:53.000000 mbapy-0.7.4/mbapy/storage/libstats.dll
--rw-rw-rw-   0        0        0    16752 2024-01-11 01:58:53.000000 mbapy-0.7.4/mbapy/storage/libstats.so
--rw-rw-rw-   0        0        0     7557 2024-04-26 14:00:52.000000 mbapy-0.7.4/mbapy/storage/mbapy-cli-scripts-list.json
--rw-rw-rw-   0        0        0     1565 2023-12-18 14:29:23.000000 mbapy-0.7.4/mbapy/web.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.637075 mbapy-0.7.4/mbapy/web_utils/
--rw-rw-rw-   0        0        0        0 2023-07-27 10:19:54.000000 mbapy-0.7.4/mbapy/web_utils/__init__.py
--rw-rw-rw-   0        0        0     4133 2023-11-06 08:06:25.000000 mbapy-0.7.4/mbapy/web_utils/parse.py
--rw-rw-rw-   0        0        0    35800 2024-04-25 03:11:33.000000 mbapy-0.7.4/mbapy/web_utils/request.py
--rw-rw-rw-   0        0        0    31544 2024-04-25 01:49:36.000000 mbapy-0.7.4/mbapy/web_utils/spider.py
--rw-rw-rw-   0        0        0    20128 2024-05-01 10:43:48.000000 mbapy-0.7.4/mbapy/web_utils/task.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.520358 mbapy-0.7.4/mbapy.egg-info/
--rw-rw-rw-   0        0        0    10206 2024-05-10 13:06:23.000000 mbapy-0.7.4/mbapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2231 2024-05-10 13:06:23.000000 mbapy-0.7.4/mbapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-10 13:06:23.000000 mbapy-0.7.4/mbapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2024-05-10 13:06:23.000000 mbapy-0.7.4/mbapy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      990 2024-05-10 13:06:23.000000 mbapy-0.7.4/mbapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-10 13:06:23.000000 mbapy-0.7.4/mbapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      976 2024-05-03 13:01:37.000000 mbapy-0.7.4/requirements.json
--rw-rw-rw-   0        0        0       42 2024-05-10 13:06:23.646023 mbapy-0.7.4/setup.cfg
--rw-rw-rw-   0        0        0     3400 2024-05-10 13:06:15.000000 mbapy-0.7.4/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-10 13:06:23.642026 mbapy-0.7.4/test/
--rw-rw-rw-   0        0        0     2028 2024-01-11 01:58:53.000000 mbapy-0.7.4/test/test_base.py
--rw-rw-rw-   0        0        0     1575 2023-10-20 09:14:56.000000 mbapy-0.7.4/test/test_game.py
--rw-rw-rw-   0        0        0     1742 2024-01-11 01:58:53.000000 mbapy-0.7.4/test/test_web.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.534071 mbapy-0.8.0/
+-rw-rw-rw-   0        0        0     1085 2023-09-30 06:15:47.000000 mbapy-0.8.0/LICENSE
+-rw-rw-rw-   0        0        0      214 2024-04-21 10:41:48.000000 mbapy-0.8.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    10206 2024-06-01 12:01:51.533074 mbapy-0.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8039 2024-04-30 02:19:58.000000 mbapy-0.8.0/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.328690 mbapy-0.8.0/mbapy/
+-rw-rw-rw-   0        0        0     1219 2024-05-20 13:22:29.000000 mbapy-0.8.0/mbapy/__init__.py
+-rw-rw-rw-   0        0        0      402 2024-06-01 12:01:39.000000 mbapy-0.8.0/mbapy/__version__.py
+-rw-rw-rw-   0        0        0    27309 2024-04-25 14:59:13.000000 mbapy-0.8.0/mbapy/base.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.363380 mbapy-0.8.0/mbapy/bio/
+-rw-rw-rw-   0        0        0      133 2024-01-08 14:19:44.000000 mbapy-0.8.0/mbapy/bio/__init__.py
+-rw-rw-rw-   0        0        0    21230 2024-04-29 08:59:11.000000 mbapy-0.8.0/mbapy/bio/peptide.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.375792 mbapy-0.8.0/mbapy/dl_torch/
+-rw-rw-rw-   0        0        0      361 2024-01-11 01:58:53.000000 mbapy-0.8.0/mbapy/dl_torch/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.375792 mbapy-0.8.0/mbapy/dl_torch/arch/
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.379791 mbapy-0.8.0/mbapy/dl_torch/arch/CL/
+-rw-rw-rw-   0        0        0       34 2023-09-30 06:15:47.000000 mbapy-0.8.0/mbapy/dl_torch/arch/CL/__init__.py
+-rw-rw-rw-   0        0        0    16559 2023-09-30 06:15:47.000000 mbapy-0.8.0/mbapy/dl_torch/arch/CL/builder.py
+-rw-rw-rw-   0        0        0     2423 2023-09-30 06:15:47.000000 mbapy-0.8.0/mbapy/dl_torch/arch/CL/trainer.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.383837 mbapy-0.8.0/mbapy/dl_torch/arch/CLIP/
+-rw-rw-rw-   0        0        0       32 2023-09-30 06:15:47.000000 mbapy-0.8.0/mbapy/dl_torch/arch/CLIP/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.8.0/mbapy/dl_torch/arch/CLIP/builder.py
+-rw-rw-rw-   0        0        0        0 2023-07-10 08:31:51.000000 mbapy-0.8.0/mbapy/dl_torch/arch/CLIP/trainer.py
+-rw-rw-rw-   0        0        0      203 2023-09-30 06:15:47.000000 mbapy-0.8.0/mbapy/dl_torch/arch/__init__.py
+-rw-rw-rw-   0        0        0    26096 2024-01-05 08:43:17.000000 mbapy-0.8.0/mbapy/dl_torch/bb.py
+-rw-rw-rw-   0        0        0     6352 2023-09-30 06:15:47.000000 mbapy-0.8.0/mbapy/dl_torch/data.py
+-rw-rw-rw-   0        0        0     1063 2023-09-30 06:15:47.000000 mbapy-0.8.0/mbapy/dl_torch/hyper_search.py
+-rw-rw-rw-   0        0        0     4113 2023-09-30 06:15:47.000000 mbapy-0.8.0/mbapy/dl_torch/loss.py
+-rw-rw-rw-   0        0        0    13191 2023-09-30 06:15:47.000000 mbapy-0.8.0/mbapy/dl_torch/m.py
+-rw-rw-rw-   0        0        0     4661 2023-12-11 09:26:16.000000 mbapy-0.8.0/mbapy/dl_torch/optim.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.401792 mbapy-0.8.0/mbapy/dl_torch/paper/
+-rw-rw-rw-   0        0        0       18 2023-09-30 06:15:47.000000 mbapy-0.8.0/mbapy/dl_torch/paper/__init__.py
+-rw-rw-rw-   0        0        0     2917 2023-09-30 06:15:47.000000 mbapy-0.8.0/mbapy/dl_torch/paper/bb.py
+-rw-rw-rw-   0        0        0    17600 2024-01-11 07:34:28.000000 mbapy-0.8.0/mbapy/dl_torch/utils.py
+-rw-rw-rw-   0        0        0    22088 2024-04-21 10:54:51.000000 mbapy-0.8.0/mbapy/file.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.405589 mbapy-0.8.0/mbapy/file_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.8.0/mbapy/file_utils/__init__.py
+-rw-rw-rw-   0        0        0     7095 2023-12-18 14:29:23.000000 mbapy-0.8.0/mbapy/file_utils/image.py
+-rw-rw-rw-   0        0        0    11531 2024-03-10 02:50:26.000000 mbapy-0.8.0/mbapy/file_utils/video.py
+-rw-rw-rw-   0        0        0    25377 2024-02-23 13:27:31.000000 mbapy-0.8.0/mbapy/game.py
+-rw-rw-rw-   0        0        0     3364 2023-12-18 14:29:23.000000 mbapy-0.8.0/mbapy/paper.py
+-rw-rw-rw-   0        0        0    11328 2024-06-01 09:05:32.000000 mbapy-0.8.0/mbapy/plot.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.411404 mbapy-0.8.0/mbapy/plot_utils/
+-rw-rw-rw-   0        0        0        0 2024-04-21 13:25:30.000000 mbapy-0.8.0/mbapy/plot_utils/__init__.py
+-rw-rw-rw-   0        0        0    15028 2024-04-24 01:25:33.000000 mbapy-0.8.0/mbapy/plot_utils/bar_utils.py
+-rw-rw-rw-   0        0        0        0 2024-04-21 13:26:21.000000 mbapy-0.8.0/mbapy/plot_utils/line_utils.py
+-rw-rw-rw-   0        0        0    11533 2024-04-23 03:04:53.000000 mbapy-0.8.0/mbapy/plot_utils/scatter_utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.415382 mbapy-0.8.0/mbapy/sci_instrument/
+-rw-rw-rw-   0        0        0        0 2024-05-20 08:58:47.000000 mbapy-0.8.0/mbapy/sci_instrument/__init__.py
+-rw-rw-rw-   0        0        0     5310 2024-05-31 15:08:38.000000 mbapy-0.8.0/mbapy/sci_instrument/_base.py
+-rw-rw-rw-   0        0        0     2058 2024-06-01 11:55:07.000000 mbapy-0.8.0/mbapy/sci_instrument/_utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.421393 mbapy-0.8.0/mbapy/sci_instrument/hplc/
+-rw-rw-rw-   0        0        0     2170 2024-05-31 13:28:59.000000 mbapy-0.8.0/mbapy/sci_instrument/hplc/SCIEX.py
+-rw-rw-rw-   0        0        0      473 2024-05-21 13:58:09.000000 mbapy-0.8.0/mbapy/sci_instrument/hplc/__init__.py
+-rw-rw-rw-   0        0        0     1369 2024-05-31 13:28:59.000000 mbapy-0.8.0/mbapy/sci_instrument/hplc/_base.py
+-rw-rw-rw-   0        0        0     8383 2024-05-31 13:28:33.000000 mbapy-0.8.0/mbapy/sci_instrument/hplc/_utils.py
+-rw-rw-rw-   0        0        0     3584 2024-05-22 01:55:33.000000 mbapy-0.8.0/mbapy/sci_instrument/hplc/waters.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.425396 mbapy-0.8.0/mbapy/sci_instrument/mass/
+-rw-rw-rw-   0        0        0     4332 2024-06-01 08:33:17.000000 mbapy-0.8.0/mbapy/sci_instrument/mass/SCIEX.py
+-rw-rw-rw-   0        0        0      390 2024-05-30 09:23:25.000000 mbapy-0.8.0/mbapy/sci_instrument/mass/__init__.py
+-rw-rw-rw-   0        0        0     7963 2024-06-01 06:31:25.000000 mbapy-0.8.0/mbapy/sci_instrument/mass/_base.py
+-rw-rw-rw-   0        0        0     5475 2024-06-01 11:56:09.000000 mbapy-0.8.0/mbapy/sci_instrument/mass/_utils.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.433439 mbapy-0.8.0/mbapy/sci_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-20 02:35:49.000000 mbapy-0.8.0/mbapy/sci_utils/__init__.py
+-rw-rw-rw-   0        0        0    10594 2024-01-20 12:03:17.000000 mbapy-0.8.0/mbapy/sci_utils/paper_download.py
+-rw-rw-rw-   0        0        0    23045 2023-12-11 09:26:16.000000 mbapy-0.8.0/mbapy/sci_utils/paper_parse.py
+-rw-rw-rw-   0        0        0    16559 2024-04-25 15:14:19.000000 mbapy-0.8.0/mbapy/sci_utils/paper_search.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.461709 mbapy-0.8.0/mbapy/scripts/
+-rw-rw-rw-   0        0        0      153 2024-01-08 13:31:52.000000 mbapy-0.8.0/mbapy/scripts/__init__.py
+-rw-rw-rw-   0        0        0       68 2024-01-08 13:31:52.000000 mbapy-0.8.0/mbapy/scripts/__main__.py
+-rw-rw-rw-   0        0        0     2821 2024-04-21 10:45:32.000000 mbapy-0.8.0/mbapy/scripts/_main_.py
+-rw-rw-rw-   0        0        0     1628 2024-05-02 13:29:19.000000 mbapy-0.8.0/mbapy/scripts/_script_utils_.py
+-rw-rw-rw-   0        0        0     5549 2024-02-23 13:27:31.000000 mbapy-0.8.0/mbapy/scripts/avif.py
+-rw-rw-rw-   0        0        0     1947 2024-01-22 08:25:16.000000 mbapy-0.8.0/mbapy/scripts/cluster.py
+-rw-rw-rw-   0        0        0    13566 2024-01-08 13:31:52.000000 mbapy-0.8.0/mbapy/scripts/cnipa.py
+-rw-rw-rw-   0        0        0     2741 2024-02-23 13:27:31.000000 mbapy-0.8.0/mbapy/scripts/cp.py
+-rw-rw-rw-   0        0        0     4806 2024-04-24 02:05:38.000000 mbapy-0.8.0/mbapy/scripts/duitang.py
+-rw-rw-rw-   0        0        0     3175 2024-05-03 09:21:25.000000 mbapy-0.8.0/mbapy/scripts/extract-dir.py
+-rw-rw-rw-   0        0        0     2637 2024-01-08 13:31:52.000000 mbapy-0.8.0/mbapy/scripts/extract_paper.py
+-rw-rw-rw-   0        0        0     3781 2024-04-15 15:02:22.000000 mbapy-0.8.0/mbapy/scripts/file-size.py
+-rw-rw-rw-   0        0        0    26472 2024-05-22 01:58:16.000000 mbapy-0.8.0/mbapy/scripts/hplc.py
+-rw-rw-rw-   0        0        0    20997 2024-06-01 11:56:40.000000 mbapy-0.8.0/mbapy/scripts/mass.py
+-rw-rw-rw-   0        0        0     2614 2024-02-23 13:27:31.000000 mbapy-0.8.0/mbapy/scripts/mv.py
+-rw-rw-rw-   0        0        0    29037 2024-05-10 08:37:48.000000 mbapy-0.8.0/mbapy/scripts/peptide.py
+-rw-rw-rw-   0        0        0     1679 2024-01-12 08:11:59.000000 mbapy-0.8.0/mbapy/scripts/reviz.py
+-rw-rw-rw-   0        0        0     2101 2024-02-23 13:27:31.000000 mbapy-0.8.0/mbapy/scripts/rm.py
+-rw-rw-rw-   0        0        0     5392 2024-01-08 13:31:52.000000 mbapy-0.8.0/mbapy/scripts/scihub.py
+-rw-rw-rw-   0        0        0     8636 2024-01-08 13:31:52.000000 mbapy-0.8.0/mbapy/scripts/scihub_selenium.py
+-rw-rw-rw-   0        0        0     5633 2024-02-23 13:27:31.000000 mbapy-0.8.0/mbapy/scripts/splash_img.py
+-rw-rw-rw-   0        0        0     9128 2024-03-14 08:21:47.000000 mbapy-0.8.0/mbapy/scripts/video.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.494786 mbapy-0.8.0/mbapy/stats/
+-rw-rw-rw-   0        0        0     2839 2023-10-04 07:59:59.000000 mbapy-0.8.0/mbapy/stats/__init__.py
+-rw-rw-rw-   0        0        0    30529 2023-10-06 03:00:11.000000 mbapy-0.8.0/mbapy/stats/cluster.py
+-rw-rw-rw-   0        0        0    15779 2024-04-09 06:03:49.000000 mbapy-0.8.0/mbapy/stats/df.py
+-rw-rw-rw-   0        0        0    19333 2023-09-30 06:15:47.000000 mbapy-0.8.0/mbapy/stats/geography.py
+-rw-rw-rw-   0        0        0     4009 2024-04-23 02:29:03.000000 mbapy-0.8.0/mbapy/stats/reg.py
+-rw-rw-rw-   0        0        0    16955 2024-04-05 10:19:56.000000 mbapy-0.8.0/mbapy/stats/test.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.505663 mbapy-0.8.0/mbapy/storage/
+-rw-rw-rw-   0        0        0    69698 2024-01-11 01:58:53.000000 mbapy-0.8.0/mbapy/storage/libsci.dll
+-rw-rw-rw-   0        0        0    15864 2024-01-11 01:58:53.000000 mbapy-0.8.0/mbapy/storage/libsci.so
+-rw-rw-rw-   0        0        0    40252 2024-01-11 01:58:53.000000 mbapy-0.8.0/mbapy/storage/libstats.dll
+-rw-rw-rw-   0        0        0    16752 2024-01-11 01:58:53.000000 mbapy-0.8.0/mbapy/storage/libstats.so
+-rw-rw-rw-   0        0        0     7557 2024-04-26 14:00:52.000000 mbapy-0.8.0/mbapy/storage/mbapy-cli-scripts-list.json
+-rw-rw-rw-   0        0        0     1565 2023-12-18 14:29:23.000000 mbapy-0.8.0/mbapy/web.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.527077 mbapy-0.8.0/mbapy/web_utils/
+-rw-rw-rw-   0        0        0        0 2023-07-27 10:19:54.000000 mbapy-0.8.0/mbapy/web_utils/__init__.py
+-rw-rw-rw-   0        0        0     4133 2023-11-06 08:06:25.000000 mbapy-0.8.0/mbapy/web_utils/parse.py
+-rw-rw-rw-   0        0        0    35800 2024-04-25 03:11:33.000000 mbapy-0.8.0/mbapy/web_utils/request.py
+-rw-rw-rw-   0        0        0    31544 2024-04-25 01:49:36.000000 mbapy-0.8.0/mbapy/web_utils/spider.py
+-rw-rw-rw-   0        0        0    20700 2024-05-26 14:29:21.000000 mbapy-0.8.0/mbapy/web_utils/task.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.361383 mbapy-0.8.0/mbapy.egg-info/
+-rw-rw-rw-   0        0        0    10206 2024-06-01 12:01:51.000000 mbapy-0.8.0/mbapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2649 2024-06-01 12:01:51.000000 mbapy-0.8.0/mbapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 12:01:51.000000 mbapy-0.8.0/mbapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2024-06-01 12:01:51.000000 mbapy-0.8.0/mbapy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      990 2024-06-01 12:01:51.000000 mbapy-0.8.0/mbapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-06-01 12:01:51.000000 mbapy-0.8.0/mbapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      976 2024-05-03 13:01:37.000000 mbapy-0.8.0/requirements.json
+-rw-rw-rw-   0        0        0       42 2024-06-01 12:01:51.534392 mbapy-0.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     3400 2024-06-01 12:01:47.000000 mbapy-0.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 12:01:51.531074 mbapy-0.8.0/test/
+-rw-rw-rw-   0        0        0     2028 2024-01-11 01:58:53.000000 mbapy-0.8.0/test/test_base.py
+-rw-rw-rw-   0        0        0     1575 2023-10-20 09:14:56.000000 mbapy-0.8.0/test/test_game.py
+-rw-rw-rw-   0        0        0     1742 2024-01-11 01:58:53.000000 mbapy-0.8.0/test/test_web.py
```

### Comparing `mbapy-0.7.4/LICENSE` & `mbapy-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/PKG-INFO` & `mbapy-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbapy
-Version: 0.7.4
+Version: 0.8.0
 Summary: MyBA in Python
 Home-page: https://github.com/BHM-Bob/BA_PY
 Author: BHM-Bob G
 Author-email: bhmfly@foxmail.com
 License: MIT Licence
 Description: <!--
          * @Author: BHM-Bob 2262029386@qq.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mbapy Version: 0.7.4 Summary: MyBA in Python Home-
+Metadata-Version: 2.1 Name: mbapy Version: 0.8.0 Summary: MyBA in Python Home-
 page: https://github.com/BHM-Bob/BA_PY Author: BHM-Bob G Author-email:
 bhmfly@foxmail.com License: MIT Licence Description:
 ************ BBAA__PPYY:: OOppttiimmiizzee YYoouurr WWoorrkkffllooww wwiitthh PPyytthhoonn!! ************
 [Downloads][Downloads][Downloads]
 _[_r_e_p_o_ _s_i_z_e_]_[_c_o_d_e_ _s_i_z_e_]_[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_G_i_t_H_u_b_ _C_o_m_m_i_t_ _A_c_t_i_v_i_t_y_]
 [GitHub last commit]
 _[_P_y_P_I_ _S_t_a_t_u_s_]_[_P_y_P_I_]_[_p_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
```

### Comparing `mbapy-0.7.4/README.md` & `mbapy-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/__init__.py` & `mbapy-0.8.0/mbapy/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-11-01 22:16:49
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2023-10-19 22:01:01
+LastEditTime: 2024-05-20 21:22:29
 Description: some helpful python scripts in plot, stats and deeplearning
 '''
 import os
 
 # os.environ.__getitem__(self, key), no default value
 if 'MBAPY_AUTO_IMPORT_TORCH' not in os.environ:
     os.environ['MBAPY_AUTO_IMPORT_TORCH'] = 'True'
 if 'MBAPY_FAST_LOAD' not in os.environ:
     os.environ['MBAPY_FAST_LOAD'] = 'False'
     
 if os.environ['MBAPY_FAST_LOAD'] == 'False':
-    from . import base, file, paper, plot, stats, web
+    from . import base, file, paper, plot, stats, web, sci_instrument
     
 from .__version__ import (__author__, __author_email__, __build__,
                           __description__, __license__, __title__, __url__,
                           __version__)
 
 try:
     if 'MBAPY_AUTO_IMPORT_TORCH' in os.environ and\
```

### Comparing `mbapy-0.7.4/mbapy/base.py` & `mbapy-0.8.0/mbapy/base.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/bio/peptide.py` & `mbapy-0.8.0/mbapy/bio/peptide.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/dl_torch/arch/CL/builder.py` & `mbapy-0.8.0/mbapy/dl_torch/arch/CL/builder.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/dl_torch/arch/CL/trainer.py` & `mbapy-0.8.0/mbapy/dl_torch/arch/CL/trainer.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/dl_torch/bb.py` & `mbapy-0.8.0/mbapy/dl_torch/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/dl_torch/data.py` & `mbapy-0.8.0/mbapy/dl_torch/data.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/dl_torch/hyper_search.py` & `mbapy-0.8.0/mbapy/dl_torch/hyper_search.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/dl_torch/loss.py` & `mbapy-0.8.0/mbapy/dl_torch/loss.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/dl_torch/m.py` & `mbapy-0.8.0/mbapy/dl_torch/m.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/dl_torch/optim.py` & `mbapy-0.8.0/mbapy/dl_torch/optim.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/dl_torch/paper/bb.py` & `mbapy-0.8.0/mbapy/dl_torch/paper/bb.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/dl_torch/utils.py` & `mbapy-0.8.0/mbapy/dl_torch/utils.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/file.py` & `mbapy-0.8.0/mbapy/file.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/file_utils/image.py` & `mbapy-0.8.0/mbapy/file_utils/image.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/file_utils/video.py` & `mbapy-0.8.0/mbapy/file_utils/video.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/game.py` & `mbapy-0.8.0/mbapy/game.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/paper.py` & `mbapy-0.8.0/mbapy/paper.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/plot.py` & `mbapy-0.8.0/mbapy/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     from .plot_utils.line_utils import *
     from .plot_utils.scatter_utils import plot_reg, plot_scatter, add_scatter_legend
 
 # plt.rcParams['font.sans-serif'] = ['SimHei'] #用来正常显示中文
 plt.rcParams["font.family"] = 'Times New Roman'
 plt.rcParams['axes.unicode_minus'] = False #用来正常显示负号
 colors = plt.rcParams['axes.prop_cycle'].by_key()['color']
+PLT_MARKERS = ('o', 'v', '^', '<', '>', '8', 's', 'p', '*', 'h', 'H', 'D', 'd', 'P', 'X')
 
 def rgb2hex(r, g, b):
   return '#'+('{:02X}' * 3).format(r, g, b)
 def hex2rgb(hex:str):
   return [int(hex[i:i+2], 16) for i in (1, 3, 5)]
 def rgbs2hexs(rgbs:List[Tuple[float]]):
     """
@@ -139,26 +140,26 @@
         if 'tick_size' in kwargs:
             axs[-1].tick_params(labelsize = kwargs['tick_size'])
         if 'label_size' in kwargs:
             axs[-1].set_xlabel('Theoretical Quantiles', fontsize = kwargs['label_size'])
             axs[-1].set_ylabel('Sample Quantiles', fontsize = kwargs['label_size'])
     return axs
             
-def save_show(path:str, dpi = 300, bbox_inches = 'tight', show: bool = True):
+def save_show(path:str, dpi = 300, bbox_inches = 'tight', show: bool = True, **kwargs):
     """
     Saves the current matplotlib figure to a file at the specified path and displays the figure.
 
     Parameters:
         - path (str): The path where the figure will be saved.
         - dpi (int, optional): The resolution of the saved figure in dots per inch. Default is 300.
         - bbox_inches (str or Bbox, optional): The portion of the figure to save. Default is 'tight'.
         - show (bool, optional): Whether to show the figure after saving. Default is True.
     """
     plt.tight_layout()
-    plt.gcf().savefig(path, dpi=dpi, bbox_inches = bbox_inches)
+    plt.gcf().savefig(path, dpi=dpi, bbox_inches = bbox_inches, **kwargs)
     if show:
         plt.show()
     
 def plot_stats_star(x1: float, x2: float, h: float, endpoint: float, p_value: float,
                     ax = plt, p2star: Callable[[float], str] = p_value_to_stars):
     """
     Params
```

### Comparing `mbapy-0.7.4/mbapy/plot_utils/bar_utils.py` & `mbapy-0.8.0/mbapy/plot_utils/bar_utils.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/plot_utils/scatter_utils.py` & `mbapy-0.8.0/mbapy/plot_utils/scatter_utils.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/sci_utils/paper_download.py` & `mbapy-0.8.0/mbapy/sci_utils/paper_download.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/sci_utils/paper_parse.py` & `mbapy-0.8.0/mbapy/sci_utils/paper_parse.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/sci_utils/paper_search.py` & `mbapy-0.8.0/mbapy/sci_utils/paper_search.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/_main_.py` & `mbapy-0.8.0/mbapy/scripts/_main_.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/_script_utils_.py` & `mbapy-0.8.0/mbapy/scripts/_script_utils_.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/avif.py` & `mbapy-0.8.0/mbapy/scripts/avif.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/cluster.py` & `mbapy-0.8.0/mbapy/scripts/cluster.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/cnipa.py` & `mbapy-0.8.0/mbapy/scripts/cnipa.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/cp.py` & `mbapy-0.8.0/mbapy/scripts/cp.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/duitang.py` & `mbapy-0.8.0/mbapy/scripts/duitang.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/extract-dir.py` & `mbapy-0.8.0/mbapy/scripts/extract-dir.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/extract_paper.py` & `mbapy-0.8.0/mbapy/scripts/extract_paper.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/file-size.py` & `mbapy-0.8.0/mbapy/scripts/file-size.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/hplc.py` & `mbapy-0.8.0/mbapy/scripts/hplc.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,356 +1,269 @@
 import argparse
 import os
+from collections import OrderedDict
 from functools import partial
 from pathlib import Path
-from typing import Dict, List
+from typing import Dict, List, Union, Tuple, Callable
 
 import scipy
 import numpy as np
 import pandas as pd
 import matplotlib.pyplot as plt
 
 os.environ['MBAPY_AUTO_IMPORT_TORCH'] = 'False'
 os.environ['MBAPY_FAST_LOAD'] = 'True'
 from mbapy.base import put_err
 from mbapy.plot import get_palette, save_show
 from mbapy.file import decode_bits_to_str, get_paths_with_extension, get_valid_file_path
+from mbapy.sci_instrument.hplc import HplcData, WatersData, SciexData, SciexTicData
+from mbapy.sci_instrument.hplc._utils import plot_hplc as _plot_hplc, process_file_labels, process_peak_labels
 from mbapy.scripts._script_utils_ import clean_path, Command, excute_command
 
-                
+
 class plot_hplc(Command):
+    SUPPORT_SYSTEMS = {'waters', 'SCIEX', 'SCIEX-TIC'}
     def __init__(self, args: argparse.Namespace, printf=print) -> None:
         super().__init__(args, printf)
         self.dfs = {}
-        self.SUPPORT_SYSTEMS = {'waters'}
+        self.sys2suffix = {'waters': 'arw', 'SCIEX': 'txt', 'SCIEX-TIC': 'txt'}
+        self.sys2model: Dict[str, HplcData] = {'waters': WatersData, 'SCIEX': SciexData, 'SCIEX-TIC': SciexTicData}
         
     @staticmethod
     def make_args(args: argparse.ArgumentParser):
         args.add_argument('-i', '--input', type = str, default='.',
                           help="data file directory, default is %(default)s.")
         args.add_argument('-s', '--system', type = str, default='waters',
-                          help="HPLC system. Default is %(default)s, only accept arw file exported by Waters.")
+                          help=f"HPLC system. Default is %(default)s, those systems are supported: {plot_hplc.SUPPORT_SYSTEMS}")
         args.add_argument('-r', '--recursive', action='store_true', default=False,
                           help='search input directory recursively, default is %(default)s.')
         args.add_argument('-merge', action='store_true', default=False,
                           help='merge multi files into one plot, default is %(default)s.')
         args.add_argument('-o', '--output', type = str, default=None,
                           help="output file dir or path. Default is %(default)s, means same as input dir")
         # set draw argument
         args.add_argument('--min-peak-width', type = float, default=4,
                           help='filter peaks with min width in hplc/Charge plot, default is %(default)s.')
         args.add_argument('-xlim', type = str, default='0,None',
                           help='set x-axis limit, input as "0,15", default is %(default)s.')
-        args.add_argument('-cols', '--colors', type = str, default='black',
-                          help='draw color, default is %(default)s.')
-        args.add_argument('-labels', '--labels', type = str, default='',
-                          help='labels, input as 1000,Pep1;1050,Pep2, default is %(default)s.')
         args.add_argument('-flabels', '--file-labels', type = str, default='',
                           help='labels, input as 228,blue;304,red, default is %(default)s.')
-        args.add_argument('--labels-eps', type = float, default=0.5,
-                          help='eps to recognize labels, default is %(default)s.')
-        args.add_argument('-expand', '--expand', type = float, default=0.2,
-                          help='how much the x-axis and y-axisto be expanded, default is %(default)s.')
-        args.add_argument('-lpos', '--legend-pos', type = str, default='upper center',
-                          help='legend position, can be string as "upper center", or be float as 0.1,0.2, default is %(default)s')
-        args.add_argument('-lposbbox1', '--legend-pos-bbox1', type = float, default=1.1,
+        args.add_argument('-lpos', '--file-legend-pos', type = str, default='upper center',
+                          help='legend position, can be string as "upper center", default is %(default)s')
+        args.add_argument('-lposbbox', '--file-legend-bbox', type = str, default='1.3,0.5',
                           help='legend position bbox 1 to anchor, default is %(default)s')
-        args.add_argument('-lposbbox2', '--legend-pos-bbox2', type = float, default=1,
-                          help='legend position bbox 2 to anchor, default is %(default)s')
+        args.add_argument('-dpi', type = int, default=600,
+                          help='set dpi of output image, default is %(default)s.')
+        args.add_argument('-show', action='store_true', default=False,
+                          help='show plot window, default is %(default)s.')
         return args
-    
-    @staticmethod
-    def load_arw_file(path: Path, content: str = None):
-        content = content or path.read_text()
-        lines = content.splitlines()
-        info_df = pd.DataFrame([lines[1].split('\t')], columns = lines[0].split('\t'))
-        data_df = pd.DataFrame([line.split('\t') for line in lines[2:]],
-                            columns = ['Time', 'Absorbance'])
-        return info_df, data_df.astype({'Time': float, 'Absorbance': float})
-    
-    def process_file_labels(self, labels: str):
-        labels = '' if labels is None else labels
-        col_mode = self.args.__dict__.get('file_col_mode', 'hls')
-        file_labels, colors = [], get_palette(len(labels.split(';')), mode = 'hls')
-        for idx, i in enumerate(labels.split(';')):
-            if i:
-                pack = i.split(',')
-                label, color = pack[0], pack[1] if len(pack) == 2 else colors[idx]
-                file_labels.append([label, color])
-        return file_labels
-    
+
     def load_dfs_from_data_file(self):
-        if self.args.system == 'waters':
-            paths = get_paths_with_extension(self.args.input, ['arw'], recursive=self.args.recursive)
-            load_data = plot_hplc.load_arw_file
-        dfs = {path:load_data(Path(path)) for path in paths}
-        return {k:v for k,v in dfs.items() if v is not None}
-    
+        paths = get_paths_with_extension(self.args.input, [self.sys2suffix[self.args.system]], recursive=self.args.recursive)
+        dfs = [self.data_model(path) for path in paths]
+        dfs = {data.get_tag():data for data in dfs if data.SUCCEED_LOADED}
+        return dfs
+
     def process_args(self):
-        assert self.args.system in {'waters'}, f'not support HPLC system: {self.args.system}'
+        assert self.args.system in self.SUPPORT_SYSTEMS, f'not support HPLC system: {self.args.system}'
         # process self.args
         self.args.input = clean_path(self.args.input)
         self.args.output = clean_path(self.args.output) if self.args.output else self.args.input
         if not os.path.isdir(self.args.output):
             print(f'given output {self.args.output} is a file, change it to parent dir')
             self.args.output = self.args.output.parent
-        # labels
-        labels, colors = {}, get_palette(len(self.args.labels.split(';')), mode = 'hls')
-        for idx, i in enumerate(self.args.labels.split(';')):
-            if i:
-                pack = i.split(',')
-                mass, label, color = pack[0], pack[1], pack[2] if len(pack) == 3 else colors[idx]
-                labels[float(mass)] = [label, color]
-        self.args.labels = labels
+        self.args.file_legend_bbox = eval(f'({self.args.file_legend_bbox})') # NOTE: can be invoked
+        self.data_model = self.sys2model[self.args.system]
         # file labels
-        self.args.file_labels = self.process_file_labels(self.args.file_labels)
-        
-    @staticmethod
-    def process_waters_data(path: str, df, args: argparse.Namespace, save_df: bool = True, show_df: bool = True):
-        info_df, data_df = df
-        # output csv
-        sample_name, sample_time, sample_channle = info_df['"样品名称"'][0], info_df['"采集日期"'][0], info_df['"通道"'][0]
-        csv_name = f'{sample_name} - {sample_time} - {sample_channle}'.replace('"', '')
-        if save_df:
-            csv_name = get_valid_file_path(csv_name.replace('/', '-'), valid_len=500).replace(':', '-')
-            info_df.to_csv(str(path.parent / get_valid_file_path(csv_name + ' - info.csv')))
-            data_df.to_csv(str(path.parent / get_valid_file_path(csv_name + ' - data.csv')))
-        if show_df:
-            print(f'plot {path.stem}: {csv_name}')
-            print(info_df.T)
-        return csv_name, info_df, data_df, args
-        
-    @staticmethod
-    def plot_waters(file_name:str, info_df: pd.DataFrame, data_df: pd.DataFrame, args):
-        fig, ax = plt.subplots(figsize=(10, 6))
-        xlim = args.xlim.split(',')
-        if isinstance(info_df, pd.DataFrame):
-            au_units = info_df['"检测单位"'][0].replace('"', '')
-            xlim = [float(xlim[0]), data_df['Time'].max() if xlim[1] == 'None' else float(xlim[1])]
-            ax.plot(data_df['Time'], data_df['Absorbance'], color = args.color, label = info_df[''])
-        else:
-            au_units = info_df[0]['"检测单位"'][0].replace('"', '')
-            xlim_max = data_df[0]['Time'].max()
-            for label, info_df_i, data_df_i in zip(args.file_labels, info_df, data_df):
-                label_string, color = label
-                ax.plot(data_df_i['Time'], data_df_i['Absorbance'], color = color, label = label_string)
-                xlim_max = max(xlim_max, data_df_i['Time'].max())
-            xlim = [float(xlim[0]), xlim_max if xlim[1] == 'None' else float(xlim[1])]
-        plt.xticks(size = 20)
-        plt.yticks(size = 20)
-        ax.set_xlabel('Time (min)', fontsize=25)
-        ax.set_ylabel(f'Absorbance ({au_units})', fontsize=25)
-        ax.set_xlim(xlim[0], xlim[1])
-        plt.legend(fontsize=15, loc = args.legend_pos, bbox_to_anchor = (args.legend_pos_bbox1, args.legend_pos_bbox2), draggable = True)
-        save_show(os.path.join(args.output, f'{file_name} absorbance.png'), dpi = 600)
-    
+        self.args.file_labels = process_file_labels(self.args.file_labels)
+
     def main_process(self):
+        def _save_fig(root, name, dpi, show, bbox_extra_artists):
+            path = get_valid_file_path(os.path.join(root, f"{name.replace('/', '-')}.png"))
+            print(f'saving plot to {path}')
+            save_show(path, dpi, show=show, bbox_extra_artists = bbox_extra_artists)
         # load origin dfs from data file
         self.dfs = self.load_dfs_from_data_file()
         if not self.dfs:
             raise FileNotFoundError(f'can not find data files in {self.args.input}')
         # show data general info and output peak list DataFrame
         if self.args.merge:
-            if self.args.system == 'waters':
-                dfs = list(self.dfs.values())
-                info_df, data_df = [d[0] for d in dfs], [d[1] for d in dfs]
-                plot_hplc.plot_waters('merge', info_df, data_df, self.args)
+            dfs = list(self.dfs.values())
+            ax, legends = _plot_hplc(dfs, **self.args.__dict__)
+            _save_fig(self.args.output, "merge.png", self.args.dpi, self.args.show, legends)
         else:
-            for path, df in self.dfs.items():
-                path = Path(path).resolve()
-                # plot each df
-                process_fn = getattr(self, f'process_{self.args.system}_data')
-                plot_fn = getattr(self, f'plot_{self.args.system}')
-                plot_fn(*process_fn(path, df, self.args))
+            for tag, data in self.dfs.items():
+                print(f'plotting data for {tag}')
+                data.save_processed_data()
+                ax, legends = _plot_hplc(data, **self.args.__dict__)
+                _save_fig(self.args.output, f"{tag.replace('/', '-')}.png", self.args.dpi, self.args.show, legends)
 
 
 class explore_hplc(plot_hplc):
     from nicegui import ui
     def __init__(self, args: argparse.Namespace, printf=print) -> None:
         super().__init__(args, printf)
         self.now_name = ''
         self.fig = None
+        self.dfs = OrderedDict()
         self.dfs_checkin = {}
+        self.dfs_refinment_x = {}
+        self.dfs_refinment_y = {}
         self.stored_dfs = {}
         self._expansion = []
-        self._time_tik_per_min = {'waters':1/60} # a min time unit is how many minutes
+        self._bbox_extra_artists = None
+        self.is_bind_lim = False
+        self.xlim_number_min = None
+        self.xlim_number_max = None
+        self.xlim_search_number_min = None
+        self.xlim_search_number_max = None
         
     @staticmethod
     def make_args(args: argparse.ArgumentParser):
         args.add_argument('-i', '--input', type = str, default='.',
                           help="data file directory, default is %(default)s.")
         args.add_argument('-s', '--system', type = str, default='waters',
-                          help="HPLC system. Default is %(default)s, only accept arw file exported by Waters.")
+                          help="HPLC system. Default is %(default)s, those systems are supported: {plot_hplc.SUPPORT_SYSTEMS}")
+        args.add_argument('-url', '--url', type = str, default='localhost',
+                          help="url to connect to, default is %(default)s.")
+        args.add_argument('-port', '--port', type = int, default=8011,
+                          help="port to connect to, default is %(default)s.")
         return args
     
     def process_args(self):
+        assert self.args.system in self.SUPPORT_SYSTEMS, f'not support HPLC system: {self.args.system}'
         self.args.input = clean_path(self.args.input)
-        assert self.args.system in {'waters'}, f'not support HPLC system: {self.args.system}'
+        self.data_model = self.sys2model[self.args.system]
         
     async def load_data(self, event):
         from nicegui import ui
         for name, content in zip(event.names, event.contents):
-            if self.args.system == 'waters':
-                if name.endswith('.arw'):
-                    content = decode_bits_to_str(content.read())
-                    info_df, data_df = plot_hplc.load_arw_file(None, content)
-                    name, info_df, data_df, _ = plot_hplc.process_waters_data(name, (info_df, data_df), None, save_df=False, show_df=False)
-                    self.stored_dfs[name] = (info_df, data_df)
-                else:
-                    ui.notify(f'{name} is not a arw file')
+            if name.endswith(self.sys2suffix[self.args.system]):
+                df = self.data_model()
+                df.raw_data = df.load_raw_data_from_bytes(content.read())
+                df.processed_data = df.process_raw_data()
+                df.data_file_path = name
+                if df.check_processed_data_empty():
+                    ui.notify(f'{name} is not a valid {self.args.system} file, skip')
                     continue
+                self.stored_dfs[df.make_tag()] = df
+            else:
+                ui.notify(f'{name} is not a arw file, skip')
+                continue
             ui.notify(f'loaded {name}')
         self.make_tabs.refresh()
         
+    def load_data_from_dir(self):
+        for name, dfs in self.load_dfs_from_data_file().items():
+            self.stored_dfs[name] = dfs
+        self.make_tabs.refresh()
+        
     def _push_df_from_tabs(self, event):
         if event.value:
             self.dfs[event.sender.text] = self.stored_dfs[event.sender.text]
         else:
             self.dfs.pop(event.sender.text, None)
+        self._ui_refinment_numbers.refresh()
         
     @ui.refreshable
     def make_tabs(self):
         from nicegui import ui
         with ui.card().classes('h-full'):
-            for name in self.stored_dfs:
+            for name in sorted(self.stored_dfs):
                 if name not in self.dfs_checkin:
                     self.dfs_checkin[name] = False
                 ui.checkbox(text = name, value = self.dfs_checkin[name],
                             on_change=self._push_df_from_tabs).bind_value_to(self.dfs_checkin, name)
                 
-    def process_peak_labels(self, peak_labels: str):
-        peak_labels = '' if peak_labels is None else peak_labels
-        labels, cols = {}, get_palette(len(peak_labels.split(';')), mode = self.args.peak_col_mode)
-        for i, label in enumerate(peak_labels.split(';')):
-            if label:
-                items = label.split(',')
-                if len(items) == 2:
-                    (t, label), color = items, cols[i]
-                elif len(items) == 3:
-                    t, label, color = items
-                labels[float(t)] = [label, color]
-        return labels
-                
-    def plot_waters(self, ax: plt.Axes):
-        from nicegui import ui
-        names, info_df, data_df = [], [], []
-        for name, df in self.dfs.items():
-            names.append(name)
-            info_df.append(df[0])
-            data_df.append(df[1])
-        # check if no data
-        if len(info_df) == 0:
-            return ui.notify('no data to plot')
-        # process file labels
-        file_labels = self.process_file_labels(self.args.file_labels)
-        if not file_labels or len(file_labels) != len(names):
-            ui.notify(f'only {len(file_labels)} labels found, should be {len(names)} labels, use name instead')
-            file_labels = self.process_file_labels(';'.join(names))
-            if len(file_labels) == 1:
-                file_labels[0][1] = 'black'
-        # process peak labels
-        peak_labels = self.process_peak_labels(self.args.peak_labels)
-        peak_labels_v = np.array(list(peak_labels.keys()))
-        # plot each
-        ax.figure.set_dpi(self.args.dpi)
-        lines, scatters, sc_labels = [], [], []
-        for label, info_df_i, data_df_i in zip(file_labels, info_df, data_df):
-            label_string, color = label
-            line = ax.plot(data_df_i['Time'], data_df_i['Absorbance'], color = color, label = label_string)[0]
-            lines.append(line)
-            # search peaks
-            st = int(self.args.start_search_time * 60) # start_search_time is in minutes
-            peaks_idx, peak_props = scipy.signal.find_peaks(data_df_i['Absorbance'], rel_height = 1,
-                                                        prominence =self.args.min_height,
-                                                        width = self.args.min_peak_width)
-            peaks_idx = peaks_idx[peaks_idx > st]
-            peak_df = data_df_i.iloc[peaks_idx, :]
-            for t, a in zip(peak_df['Time'], peak_df['Absorbance']):                    
-                matched = np.where(np.abs(peak_labels_v - t) < self.args.labels_eps)[0]
-                if matched.size > 0:
-                    label, col = peak_labels[peak_labels_v[matched[0]]]
-                    sc = ax.scatter(t+self.args.marker_offset[0], a+self.args.marker_offset[1], marker='*', s = self.args.marker_size, color = col)
-                    scatters.append(sc)
-                    sc_labels.append(label)
-                else:
-                    ax.scatter(t+self.args.marker_offset[0], a+self.args.marker_offset[1], marker=11, s = self.args.marker_size, color = 'black')
-                if self.args.show_tag_text:
-                    ax.text(t+self.args.tag_offset[0], a+self.args.tag_offset[1], f'{t:.2f}', fontsize=self.args.tag_fontsize)
-        # style fix
-        ax.tick_params(axis='both', which='major', labelsize=self.args.axis_ticks_fontsize)
-        ax.set_xlabel(self.args.xlabel, fontsize=self.args.axis_label_fontsize)
-        ax.set_ylabel(self.args.ylabel, fontsize=self.args.axis_label_fontsize)
-        # set file labels legend
-        if self.args.show_file_legend:
-            file_legend = plt.legend(fontsize=self.args.legend_fontsize, loc = self.args.legend_pos,
-                                    bbox_to_anchor = (self.args.bbox1, self.args.bbox2), draggable = True)
-            ax.add_artist(file_legend)
-        # set peak labels legend
-        if scatters and self.args.show_tag_legend:
-            [line.set_label(None) for line in lines]
-            [sc.set_label(l) for sc, l in zip(scatters, sc_labels)]
-            peak_legend = plt.legend(fontsize=self.args.legend_fontsize, loc = self.args.legend_pos,
-                                     bbox_to_anchor = (self.args.bbox1, self.args.bbox2), draggable = True)
-            ax.add_artist(peak_legend)
-        # saving
-        ax.set_xlim(left=self.args.xlim[0], right=self.args.xlim[1])
-        ax.set_ylim(bottom=self.args.ylim[0], top=self.args.ylim[1])
-        plt.tight_layout()
-                
     @ui.refreshable
     def make_fig(self):
         from nicegui import ui
         plt.close(self.fig)
-        with ui.pyplot(figsize=(self.args.fig_w, self.args.fig_h), close=False) as fig:
+        with ui.pyplot(figsize=self.args.fig_size, close=False) as fig:
             self.fig = fig.fig
-            getattr(self, f'plot_{self.args.system}')(fig.fig.gca())
+            if self.dfs:
+                ax, self._bbox_extra_artists = _plot_hplc(list(self.dfs.values()), ax = self.fig.gca(),
+                                                          dfs_refinment_x=self.dfs_refinment_x,
+                                                          dfs_refinment_y=self.dfs_refinment_y,
+                                                          file_label_fn=partial(process_file_labels, file_col_mode=self.args.file_col_mode),
+                                                          peak_label_fn=partial(process_peak_labels, peak_col_mode=self.args.peak_col_mode),
+                                                          **self.args.__dict__)
+                ax.tick_params(axis='both', which='major', labelsize=self.args.axis_ticks_fontsize)
+                ax.set_xlabel(self.args.xlabel, fontsize=self.args.axis_label_fontsize)
+                ax.set_ylabel(self.args.ylabel, fontsize=self.args.axis_label_fontsize)
+                ax.set_xlim(left=self.args.xlim[0], right=self.args.xlim[1])
+                ax.set_ylim(bottom=self.args.ylim[0], top=self.args.ylim[1])
+                plt.tight_layout()
             
     def _ui_only_one_expansion(self, e):
         if e.value:
             for expansion in self._expansion:
                 if expansion != e.sender:
-                    expansion.value = False
+                    expansion.set_value(False)
+                    
+    @ui.refreshable
+    def _ui_refinment_numbers(self):
+        from nicegui import ui
+        # update dfs_refinment
+        self.dfs_refinment_x = {n: (0 if n not in self.dfs_refinment_x else self.dfs_refinment_x[n]) for n in self.dfs}
+        self.dfs_refinment_y = {n: (0 if n not in self.dfs_refinment_y else self.dfs_refinment_y[n]) for n in self.dfs}
+        # update refinment numbers GUI
+        for (n, x), (_, y) in zip(self.dfs_refinment_x.items(), self.dfs_refinment_y.items()):
+            ui.label(n).tooltip(n)
+            with ui.row():
+                ui.number(label='x', value=x, step=0.01, format='%.4f').bind_value_to(self.dfs_refinment_x, n).classes('w-2/5')
+                ui.number(label='y', value=y, step=0.01, format='%.4f').bind_value_to(self.dfs_refinment_y, n).classes('w-2/5')
+            
+    def _ui_bind_xlim_onchange(self, e):
+        if self.is_bind_lim:
+            if e.sender == self.xlim_number_min:
+                self.xlim_search_number_min.set_value(e.value)
+            elif e.sender == self.xlim_search_number_min:
+                self.xlim_number_min.set_value(e.value)
+            elif e.sender == self.xlim_number_max:
+                self.xlim_search_number_max.set_value(e.value)
+            elif e.sender == self.xlim_search_number_max:
+                self.xlim_number_max.set_value(e.value)
                     
     def save_fig(self):
         from nicegui import ui
         path = os.path.join('./', self.args.file_name)
         ui.notify(f'saving figure to {path}')
-        save_show(path, dpi = self.args.dpi, show = False)
+        save_show(path, dpi = self.args.dpi, show = False, bbox_extra_artists = self._bbox_extra_artists)
         
     @staticmethod
     def _apply_v2list(v, lst, idx):
         lst[idx] = v
     
     def main_process(self):
         from nicegui import app, ui
         from mbapy.game import BaseInfo
         # make global settings
         # do not support xlim because it makes confusion with peak searching
         self.args = BaseInfo(file_labels = '', peak_labels = '', merge = False, recursive = False,
-                             min_peak_width = 1, min_height = 0, start_search_time = 0,
+                             min_peak_width = 0.1, min_height = 0.01, start_search_time = 0, end_search_time = None,
                              show_tag_text = True, labels_eps = 0.1,
-                             legend_pos = 'upper right', bbox1 = 1.2, bbox2 = 1,
+                             file_legend_pos = 'upper right', file_legend_bbox = [1.3, 0.75],
+                             peak_legend_pos = 'upper right', peak_legend_bbox = [1.3, 1],
                              title = '', xlabel = 'Time (min)', ylabel = 'Absorbance (AU)',
                              axis_ticks_fontsize = 20,axis_label_fontsize = 25, 
                              file_col_mode = 'hls', peak_col_mode = 'Set1',
                              show_tag_legend = True, show_file_legend = True,
                              tag_fontsize = 15, tag_offset = [0.05,0.05], marker_size = 80, marker_offset = [0,0.05],
-                             title_fontsize = 25, legend_fontsize = 15,
+                             title_fontsize = 25, legend_fontsize = 15, line_width = 2,
                              xlim = [0, None], ylim = [None, None],
-                             fig_w = 10, fig_h = 8, fig = None, dpi = 600, file_name = '',
+                             fig_size = [10, 8], fig = None, dpi = 600, file_name = '',
                              **self.args.__dict__)
-        # load dfs from input dir
-        for name, dfs in self.load_dfs_from_data_file().items():
-            process_fn = getattr(self, f'process_{self.args.system}_data')
-            name, info_df, data_df, _ = process_fn(name, dfs, None, save_df=False, show_df=False)
-            self.stored_dfs[name] = (info_df, data_df)
+        # load dfs from input dir to stored_dfs
+        self.load_data_from_dir()
         # GUI
         with ui.header(elevated=True).style('background-color: #3874c8'):
             ui.label('mbapy-cli HPLC | HPLC Data Explorer').classes('text-h4')
             ui.space()
+            ui.checkbox('bind lim', value=self.is_bind_lim).bind_value_to(self, 'is_bind_lim').tooltip('bind value of search-lim and plot-lim')
             ui.checkbox('merge', value=self.args.merge).bind_value_to(self.args,'merge').bind_value_from(self, 'dfs', lambda dfs: len(dfs) > 1)
             ui.button('Plot', on_click=self.make_fig.refresh, icon='refresh').props('no-caps')
             ui.button('Save', on_click=self.save_fig, icon='save').props('no-caps')
             ui.button('Show', on_click=plt.show, icon='open_in_new').props('no-caps')
             ui.button('Exit', on_click=app.shutdown, icon='power')
         with ui.splitter(value = 20).classes('w-full h-full h-56') as splitter:
             with splitter.before:
@@ -358,21 +271,27 @@
                 tabs = self.make_tabs()
             with splitter.after:
                 with ui.row().classes('w-full h-full'):
                     with ui.column().classes('h-full'):
                         # data filtering configs
                         with ui.expansion('Data Filtering', icon='filter_alt', value=True, on_value_change=self._ui_only_one_expansion) as expansion1:
                             self._expansion.append(expansion1)
-                            ui.select(list(self.SUPPORT_SYSTEMS), label='HPLC System', value=self.args.system).bind_value_to(self.args,'system').classes('w-full')
-                            ui.number('min peak width', value=self.args.min_peak_width, min = 0, step = 0.10).bind_value_to(self.args,'min_peak_width')
+                            ui.select(sorted(list(self.SUPPORT_SYSTEMS)), label='HPLC System', value=self.args.system).bind_value_to(self.args,'system').bind_value_to(self, 'data_model', lambda s: self.sys2model[s]).on_value_change(self.load_data_from_dir).classes('w-full')
+                            ui.number('min peak width', value=self.args.min_peak_width, min = 0, step = 0.10).bind_value_to(self.args,'min_peak_width').tooltip('in minutes')
                             ui.number('min height', value=self.args.min_height, min = 0, step=0.01).bind_value_to(self.args, 'min_height')
-                            ui.number('start search time', value=self.args.start_search_time, min = 0).bind_value_to(self.args,'start_search_time').tooltip('in minutes')
-                        # configs for fontsize
-                        with ui.expansion('Configs for Fontsize', icon='format_size', on_value_change=self._ui_only_one_expansion) as expansion2:
+                            ui.number('labels eps', value=self.args.labels_eps, min=0, format='%.2f').bind_value_to(self.args, 'labels_eps')
+                            self.xlim_search_number_min = ui.number('start search time', value=self.args.start_search_time, min = 0, on_change=self._ui_bind_xlim_onchange).bind_value_to(self.args,'start_search_time').tooltip('in minutes')
+                            self.xlim_search_number_max = ui.number('end search time', value=self.args.end_search_time, min = 0, on_change=self._ui_bind_xlim_onchange).bind_value_to(self.args, 'end_search_time').tooltip('in minutes')
+                        # data refinment configs
+                        with ui.expansion('Data Refinment', icon='auto_fix_high', on_value_change=self._ui_only_one_expansion) as expansion2:
                             self._expansion.append(expansion2)
+                            self._ui_refinment_numbers()
+                        # configs for fontsize
+                        with ui.expansion('Configs for Fontsize', icon='format_size', on_value_change=self._ui_only_one_expansion) as expansion3:
+                            self._expansion.append(expansion3)
                             with ui.row().classes('w-full'):
                                 ui.input('title', value=self.args.title).bind_value_to(self.args, 'title')
                                 ui.number('title fontsize', value=self.args.title_fontsize, min=0, step=0.5, format='%.1f').bind_value_to(self.args, 'title_fontsize')
                             with ui.row().classes('w-full'):
                                 ui.input('xlabel', value=self.args.xlabel).bind_value_to(self.args, 'xlabel')
                                 ui.input('ylabel', value=self.args.ylabel).bind_value_to(self.args, 'ylabel')
                             with ui.row().classes('w-full'):
@@ -384,52 +303,58 @@
                                 ui.number('marker size', value=self.args.marker_size, min=0, step=5, format='%.1f').bind_value_to(self.args,'marker_size')
                             with ui.row().classes('w-full'):
                                 ui.number('tag offset x', value=self.args.tag_offset[0], step=0.01, format='%.2f').on_value_change(lambda e: self._apply_v2list(e.value, self.args.tag_offset, 0))
                                 ui.number('marker offset x', value=self.args.marker_offset[0], step=0.01, format='%.2f').on_value_change(lambda e: self._apply_v2list(e.value, self.args.marker_offset, 0))
                             with ui.row().classes('w-full'):
                                 ui.number('tag offset y', value=self.args.tag_offset[1], step=0.01, format='%.2f').on_value_change(lambda e: self._apply_v2list(e.value, self.args.tag_offset, 1))
                                 ui.number('marker offset y', value=self.args.marker_offset[1], step=0.01, format='%.2f').on_value_change(lambda e: self._apply_v2list(e.value, self.args.marker_offset, 1))
+                            ui.number('line width', value=self.args.line_width, min=0, step=0.5, format='%.1f').bind_value_to(self.args, 'line_width')
                         # configs for legend
-                        with ui.expansion('Configs for Legend', icon='more', on_value_change=self._ui_only_one_expansion) as expansion3:
-                            self._expansion.append(expansion3)
+                        with ui.expansion('Configs for Legend', icon='more', on_value_change=self._ui_only_one_expansion) as expansion4:
+                            self._expansion.append(expansion4)
                             with ui.row().classes('w-full'):
                                 ui.checkbox('show file legend', value=self.args.show_file_legend).bind_value_to(self.args,'show_file_legend')
                                 ui.checkbox('show peak legend', value=self.args.show_tag_legend).bind_value_to(self.args,'show_tag_legend')
                             with ui.row().classes('w-full'):
                                 ui.textarea('file labels').bind_value_to(self.args, 'file_labels').props('clearable').tooltip('input as label1,color1;label2,color2')
                                 ui.textarea('peak labels').bind_value_to(self.args, 'peak_labels').props('clearable').tooltip('input as peaktime,label,color;...')
-                            col_mode_option = ['hls', 'Set1', 'Set2', 'Set3', 'Dark2', 'Paired', 'Pastel1', 'Pastel2', 'tab10', 'tab20', 'tab20b', 'tab20c']
                             with ui.row().classes('w-full'):
-                                ui.select(label='file col mode', options = col_mode_option, value=self.args.file_col_mode).bind_value_to(self.args, 'file_col_mode').classes('w-32')
-                                ui.select(label='peak col mode', options = col_mode_option, value=self.args.peak_col_mode).bind_value_to(self.args, 'peak_col_mode').classes('w-32')
-                            ui.number('labels eps', value=self.args.labels_eps, min=0, format='%.1f').bind_value_to(self.args, 'labels_eps')
-                            ui.number('legend fontsize', value=self.args.legend_fontsize, min=0, step=0.5, format='%.1f').bind_value_to(self.args, 'legend_fontsize')
-                            ui.input('legend loc', value=self.args.legend_pos).bind_value_to(self.args, 'legend_pos')
+                                col_mode_option = ['hls', 'Set1', 'Set2', 'Set3', 'Dark2', 'Paired', 'Pastel1', 'Pastel2', 'tab10', 'tab20', 'tab20b', 'tab20c']
+                                ui.select(label='file col mode', options = col_mode_option, value=self.args.file_col_mode).bind_value_to(self.args, 'file_col_mode').classes('w-2/5')
+                                ui.select(label='peak col mode', options = col_mode_option, value=self.args.peak_col_mode).bind_value_to(self.args, 'peak_col_mode').classes('w-2/5')
+                            ui.number('legend fontsize', value=self.args.legend_fontsize, min=0, step=0.5, format='%.2f').bind_value_to(self.args, 'legend_fontsize')
+                            with ui.row().classes('w-full'):
+                                all_loc = ['best', 'upper right', 'upper left', 'lower left', 'lower right', 'right', 'center left', 'center right', 'lower center', 'upper center', 'center']
+                                ui.select(label='file legend loc', options=all_loc, value=self.args.file_legend_pos).bind_value_to(self.args, 'file_legend_pos').classes('w-2/5')
+                                ui.select(label='peak legend loc', options=all_loc, value=self.args.peak_legend_pos).bind_value_to(self.args, 'peak_legend_pos').classes('w-2/5')
                             with ui.row().classes('w-full'):
-                                ui.number('bbox1', value=self.args.bbox1, min=0, step=0.1, format='%.1f').bind_value_to(self.args, 'bbox1').classes('w-32')
-                                ui.number('bbox2', value=self.args.bbox2, min=0, step=0.1, format='%.1f').bind_value_to(self.args, 'bbox2').classes('w-32')
+                                ui.number('file bbox1', value=self.args.file_legend_bbox[0], step=0.01, format='%.2f').on_value_change(lambda e: self._apply_v2list(e.value, self.args.file_legend_bbox, 0)).classes('w-2/5')
+                                ui.number('peak bbox1', value=self.args.peak_legend_bbox[0], step=0.01, format='%.2f').on_value_change(lambda e: self._apply_v2list(e.value, self.args.peak_legend_bbox, 0)).classes('w-2/5')
+                            with ui.row().classes('w-full'):
+                                ui.number('file bbox2', value=self.args.file_legend_bbox[1], step=0.01, format='%.2f').on_value_change(lambda e: self._apply_v2list(e.value, self.args.file_legend_bbox, 1)).classes('w-2/5')
+                                ui.number('peak bbox2', value=self.args.peak_legend_bbox[1], step=0.01, format='%.2f').on_value_change(lambda e: self._apply_v2list(e.value, self.args.peak_legend_bbox, 1)).classes('w-2/5')
                         # configs for saving
-                        with ui.expansion('Configs for Saving', icon='save', on_value_change=self._ui_only_one_expansion) as expansion4:
-                            self._expansion.append(expansion4)
+                        with ui.expansion('Configs for Saving', icon='save', on_value_change=self._ui_only_one_expansion) as expansion5:
+                            self._expansion.append(expansion5)
                             with ui.row().classes('w-full'):
-                                ui.number('xlim-min', value=self.args.xlim[0], min=0, step=0.1, format='%.1f').on_value_change(lambda e: self._apply_v2list(e.value, self.args.xlim, 0))
-                                ui.number('xlim-max', value=self.args.xlim[1], min=0, step=0.1, format='%.1f').on_value_change(lambda e: self._apply_v2list(e.value, self.args.xlim, 1))
+                                self.xlim_number_min = ui.number('xlim-min', value=self.args.xlim[0], step=0.1, format='%.2f', on_change=self._ui_bind_xlim_onchange).on_value_change(lambda e: self._apply_v2list(e.value, self.args.xlim, 0))
+                                self.xlim_number_max = ui.number('xlim-max', value=self.args.xlim[1], step=0.1, format='%.2f', on_change=self._ui_bind_xlim_onchange).on_value_change(lambda e: self._apply_v2list(e.value, self.args.xlim, 1))
                             with ui.row().classes('w-full'):
-                                ui.number('ylim-min', value=self.args.ylim[0], min=0, step=0.1, format='%.1f').on_value_change(lambda e: self._apply_v2list(e.value, self.args.ylim, 0))
-                                ui.number('ylim-max', value=self.args.ylim[1], min=0, step=0.1, format='%.1f').on_value_change(lambda e: self._apply_v2list(e.value, self.args.ylim, 1))
-                            ui.number('figure width', value=self.args.fig_w, min=1, step=0.5, format='%.1f').bind_value_to(self.args, 'fig_w')
-                            ui.number('figure height', value=self.args.fig_h, min=1, step=0.5, format='%.1f').bind_value_to(self.args, 'fig_h')
+                                ui.number('ylim-min', value=self.args.ylim[0], step=0.01, format='%.2f').on_value_change(lambda e: self._apply_v2list(e.value, self.args.ylim, 0))
+                                ui.number('ylim-max', value=self.args.ylim[1], step=0.01, format='%.2f').on_value_change(lambda e: self._apply_v2list(e.value, self.args.ylim, 1))
+                            ui.number('figure width', value=self.args.fig_size[0], min=1, step=0.5, format='%.2f').on_value_change(lambda e: self._apply_v2list(e.value, self.args.fig_size, 0)).classes('w-2/5')
+                            ui.number('figure height', value=self.args.fig_size[1], min=1, step=0.5, format='%.2f').on_value_change(lambda e: self._apply_v2list(e.value, self.args.fig_size, 1)).classes('w-2/5')
                             dpi_input = ui.number('DPI', value=self.args.dpi, min=100, step=100, format='%d').bind_value_to(self.args, 'dpi')
                             ui.select(options=[100, 300, 600], value=dpi_input.value, label='Quick Set DPI').bind_value_to(dpi_input).classes('w-full')
                             ui.input('figure file name', value=self.args.file_name).bind_value_to(self.args, 'file_name')
                     with ui.card():
                         ui.label(f'selected {len(self.dfs)} data files').classes('text-h6').bind_text_from(self, 'dfs', lambda dfs: f'selected {len(dfs)} data files')
                         self.make_fig()
         ## run GUI
-        ui.run(host = 'localhost', port = 8011, title = 'HPLC Data Explorer', reload=False)
+        ui.run(host = self.args.url, port = self.args.port, title = 'HPLC Data Explorer', reload=False)
         
 
 _str2func = {
     'plot-hplc': plot_hplc,
     'explore-hplc': explore_hplc
 }
 
@@ -440,10 +365,10 @@
     plot_hplc_args = plot_hplc.make_args(subparsers.add_parser('plot-hplc', description='plot hplc spectrum'))
     explore_hplc_args = explore_hplc.make_args(subparsers.add_parser('explore-hplc', description='explore hplc spectrum data'))
 
     excute_command(args_paser, sys_args, _str2func)
 
 if __name__ == "__main__":
     # dev code, MUST COMMENT OUT BEFORE RELEASE
-    # main('explore-hplc -i data_tmp/scripts/hplc'.split())
+    # main('explore-hplc -i data_tmp/scripts/mass'.split())
     
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mbapy-0.7.4/mbapy/scripts/mass.py` & `mbapy-0.8.0/mbapy/scripts/mass.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,380 +1,260 @@
 import argparse
-import glob
+import itertools
 import os
+from copy import deepcopy
 from functools import partial
 from pathlib import Path
 from typing import Dict, List
 
-import scipy
+import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-import matplotlib.pyplot as plt
+import scipy
 
 os.environ['MBAPY_AUTO_IMPORT_TORCH'] = 'False'
 os.environ['MBAPY_FAST_LOAD'] = 'True'
 
-# if __name__ == '__main__':
-from mbapy.base import put_err
-from mbapy.plot import get_palette, save_show
+from mbapy.base import Configs, put_err
 from mbapy.file import get_paths_with_extension, get_valid_file_path
-from mbapy.scripts._script_utils_ import clean_path, Command, excute_command, show_args
-# else:
-#     from ..base import put_err
-#     from ..plot import get_palette, save_show
-#     from ..file import get_paths_with_extension, get_valid_file_path
-#     from ._script_utils_ import clean_path, excute_command, show_args
+from mbapy.plot import get_palette, save_show, PLT_MARKERS
+from mbapy.sci_instrument.mass import MassData, SciexOriData, SciexPeakListData
+from mbapy.sci_instrument.mass import plot_mass as _plot_mass
+from mbapy.sci_instrument.mass import process_peak_labels
+from mbapy.scripts._script_utils_ import Command, clean_path, excute_command
+from mbapy.web import TaskPool
 
 
-def _plot_vlines(x, y, col, label = None):
-    plt.vlines(x, 0, y, colors = [col] * len(x), label = label)
-    plt.scatter(x, y, c = col)
-    
+process_peak_labels = partial(process_peak_labels, markers = PLT_MARKERS[1:]) # because the first marker is used for the noraml peak
+
 class plot_mass(Command):
     def __init__(self, args: argparse.Namespace, printf=print) -> None:
         super().__init__(args, printf)
-        self.use_recursive_output = False
-        self.original_output = None
-        
-    @staticmethod
-    def process_labels(labels: str):
-        result, colors = {}, get_palette(len(labels.split(';')), mode = 'hls')
-        for idx, i in enumerate(labels.split(';')):
-            if i:
-                pack = i.split(',')
-                mass, label, color = pack[0], pack[1], pack[2] if len(pack) == 3 else colors[idx]
-                result[float(mass)] = [label, color]
-        return result
+        self.task_pool: TaskPool = None
+        self.dfs: Dict[str, MassData] = {}
+        self.SUPPORT_SYS: Dict[str, MassData] = {'SCIEX-PeakList': SciexPeakListData, 'SCIEX-Ori': SciexOriData}
     
-    def process_args(self):          
+    def process_args(self):
         # process input and output args
         # after process, output whether be str or be None if recursive
         self.args.dir = clean_path(self.args.dir)
         if self.args.output is None:
             self.args.output = self.args.dir
             if not os.path.isdir(self.args.output):
                 print(f'given output {self.args.output} is a file, change it to parent dir')
                 self.args.output = self.args.output.parent
         if self.args.recursive and self.args.output:
             self.args.output = None
         self.use_recursive_output = self.args.recursive and self.args.output is None
-        # process labels args
-        self.args.labels = self.process_labels(self.args.labels)
-        if ',' in self.args.legend_pos:
-            self.args.legend_pos = self.args.legend_pos.split(',')
-            self.args.legend_pos = (float(self.args.legend_pos[0]), float(self.args.legend_pos[1]))
-            
-    @staticmethod
-    def load_file(path: Path):
-        lines = path.read_text().splitlines()
-        df = pd.DataFrame([line.split('\t') for line in lines[1:]],
-                            columns = lines[0].split('\t'))
-        if df.shape[1] == 2 and df.columns[0] == 'Time' and df.columns[1] == 'Intensity':
-            # setattr(df, '_content_type', 'base peak') # NOTE: this does not work
-            df._attrs['content_type'] = 'base peak'
-            return df.astype(float)
-        elif df.shape[1] == 2 and df.columns[0] == 'Time' and df.columns[1] == 'Absorbance':
-            df._attrs['content_type'] = 'absorbance'
-            return df.astype(float)
-        elif df.shape[1] == 2 and df.columns[0] == 'Mass/Charge' and df.columns[1] == 'Intensity':
-            df._attrs['content_type'] = 'mass-charge'
-            return df.astype(float)
-        elif df.shape[1] == 10:
-            df._attrs['content_type'] = 'peak list'
-            df =  df.astype({'Mass/Charge':float, 'Height':float, 'Charge':int,
-                            'Monoisotopic':str, 'Mass (charge)':str,
-                            'Mass/charge (charge)':str})
-            df['Mass (charge)'] = df['Mass (charge)'].str.extract(r'(\d+\.\d+)', expand=False).astype(float)
-            df['Mass/charge (charge)'] = df['Mass/charge (charge)'].str.extract(r'(\d+\.\d+)', expand=False).astype(float)
-            return df
-        else:
-            return put_err(f'Can not recognizable txt file: {path}, skip.')
+        # process others
+        self.args.labels = process_peak_labels(self.args.labels)
+        self.args.xlim = eval(f'[{self.args.xlim}]') if self.args.xlim else None
         
     @staticmethod
     def filter_peaklist_data(df: pd.DataFrame, args):
         df['mass_data'] = df['Mass (charge)'] if args.mass else df['Mass/charge (charge)']
         drop_idx = df[df['Height'] < args.min_height].index
         if not drop_idx.empty:
             print(f'drop data with min-height: {args.min_height} and only these data remained:\n',
                 df[df['Height'] >= args.min_height])
             df.drop(drop_idx, axis = 0, inplace = True)
         return df
+    
+    def load_suffix_data(self, dir: str, suffix: List[str], recursive):
+        for path in get_paths_with_extension(dir, suffix, recursive):
+            path_obj = Path(path)
+            if path_obj.stem in self.dfs:
+                print(f'{path} already loaded as {type(self.dfs[path_obj.stem])} data type, skip')
+                continue
+            for n, model in self.SUPPORT_SYS.items():
+                if path_obj.suffix in model.DATA_FILE_SUFFIX:
+                    tmp_err_warning_level = Configs.err_warning_level
+                    Configs.err_warning_level = 1
+                    data = model(path)
+                    Configs.err_warning_level = tmp_err_warning_level
+                    if data.SUCCEED_LOADED:
+                        print(f'loaded {path} as {n} data type')
+                        self.dfs[data.get_tag()] = data
+                        break
             
-    @staticmethod
-    def load_data(dir: str, recursive: bool):
-        # find base peak file and peak list file
-        paths = get_paths_with_extension(dir, ['txt'], recursive)
-        dfs = {path:plot_mass.load_file(Path(path)) for path in paths}
-        dfs = {k:v for k,v in dfs.items() if v is not None}
-        if not dfs:
+    def load_data(self, dir: str, recursive: bool):
+        suffixs_r = list(set([model.RECOMENDED_DATA_FILE_SUFFIX for model in self.SUPPORT_SYS.values()]))
+        suffixs = list(set(itertools.chain(*[model.DATA_FILE_SUFFIX for model in self.SUPPORT_SYS.values()])) - set(suffixs_r))
+        self.load_suffix_data(dir, suffixs_r, recursive)
+        self.load_suffix_data(dir, suffixs, recursive)
+        if not self.dfs:
             raise FileNotFoundError(f'can not find txt files in {dir}')
-        return dfs
-    
-    @staticmethod
-    def plot_basepeak(name:str, base_peak: pd.DataFrame, args, ax):
-        ax.plot(base_peak['Time'], base_peak['Intensity'], color = args.color)
-        plt.yscale('log')
-        ax.set_title(f'{name} (TIC of TOF MS)', fontsize=25)
-        ax.set_xlabel('Time (min)', fontsize=25)
-        ax.set_ylabel('Intensity (cps)', fontsize=25)
-        
-    @staticmethod
-    def plot_absorbance(name:str, df: pd.DataFrame, args, ax):
-        ax.plot(df['Time'], df['Absorbance'], color = args.color)
-        ax.set_title(f'{name} (Absorbance)', fontsize=25)
-        ax.set_xlabel('Time (min)', fontsize=25)
-        au_units = ('m' if df['Absorbance'].max() > 10 else '') + 'AU'
-        ax.set_ylabel(f'Absorbance ({au_units})', fontsize=25)
-        ax.set_xlim(0, df['Time'].max())
-        
-    @staticmethod
-    def plot_peaklist(name:str, df: pd.DataFrame, args, ax):
-        if args.xlim:
-            xlim = [float(i) for i in args.xlim.split(',')]
-            df = df[(df['Mass/Charge'] >= xlim[0]) & (df['Mass/Charge'] <= xlim[1])]
-            print(f'x-axis data limit set to {xlim}')
-        idx = df['Monoisotopic'] == 'Yes'
-        _plot_vlines(df['mass_data'], df['Height'], args.color)
-        labels_ms = np.array(list(args.labels.keys()))
-        text_col = args.color
-        for ms, h, c in zip(df['mass_data'][idx], df['Height'][idx],
-                            df['Charge'][idx]):
-            matched = np.where(np.abs(labels_ms - ms) < args.labels_eps)[0]
-            if matched.size > 0:
-                label, text_col = args.labels.get(labels_ms[matched[0]])
-                _plot_vlines([ms], [h], text_col, label)
-            else:
-                text_col = args.color
-            ax.text(ms, h, f'* {ms:.2f}({c:d})',
-                    fontsize=args.__dict__.get('tag_fontsize', 15), color = text_col)
-        plt.yscale('log')
-        axis_lim = (1-args.expand, 1+args.expand)
-        plt.xlim(df['mass_data'].min() * axis_lim[0], df['mass_data'].max() * axis_lim[1])
-        plt.ylim(df['Height'].min() * axis_lim[0], df['Height'].max() * axis_lim[1])
-        ax.set_title(f'{name} (Peak List of TOF MS)', fontsize=25)
-        ax.set_xlabel(f'Mass{"" if args.mass else "/charge"}', fontsize=25)
-        ax.set_ylabel('Intensity (cps)', fontsize=25)
-        
-    @staticmethod
-    def plot_masscharge(name: str, df: pd.DataFrame, args, ax):
-        # find peaks
-        peaks_cache_path = os.path.join(args.output, f'{name} peaks.cache.npy')
-        if args.use_peaks_cache and os.path.exists(peaks_cache_path):
-            peaks = np.load(peaks_cache_path)
-            print(f'loaded peaks from cache: {peaks_cache_path}')
-        else:
-            print('searching peaks...')
-            peaks = scipy.signal.find_peaks_cwt(df['Intensity'], args.min_peak_width)
-            np.save(peaks_cache_path, peaks)
-        # filter peaks
-        if peaks.any():
-            df = df.iloc[peaks, :]
-        if args.xlim:
-            xlim = [float(i) for i in args.xlim.split(',')]
-            if xlim[0] > xlim[1]:
-                xlim = xlim[::-1]
-                put_err('x-axis limit error, xlim should be in ascending order, change it to [min, max]')
-            df = df[(df['Mass/Charge'] >= xlim[0]) & (df['Mass/Charge'] <= xlim[1])]
-            print(f'x-axis data limit set to {xlim}')
-        min_height = df['Intensity'].max() * args.min_height_percent / 100
-        df = df[(df['Intensity'] >= min_height) & (df['Intensity'] >= args.min_height)]
-        print(f'min-height set to {min_height}')
-        print(f'searching done. {len(df)} peaks found.')
-        df.to_csv(os.path.join(args.output, f'{name} {df._attrs["content_type"]}.csv'))
-        # plot
-        _plot_vlines(df['Mass/Charge'], df['Intensity'], args.color)
-        labels_ms = np.array(list(args.labels.keys()))
-        text_col = args.color
-        for ms, h in zip(df['Mass/Charge'], df['Intensity']):
-            matched = np.where(np.abs(labels_ms - ms) < args.labels_eps)[0]
-            if matched.size > 0:
-                label, text_col = args.labels.get(labels_ms[matched[0]])
-                _plot_vlines([ms], [h], text_col, label)
-            else:
-                text_col = args.color
-            ax.text(ms, h, f'* {ms:.2f}',
-                    fontsize=args.__dict__.get('tag_fontsize', 15), color = text_col)
-        # fix style
-        plt.yscale('log')
-        axis_lim = (1-args.expand, 1+args.expand)
-        plt.xlim(df['Mass/Charge'].min() * axis_lim[0], df['Mass/Charge'].max() * axis_lim[1])
-        plt.ylim(df['Intensity'].min() * axis_lim[0], df['Intensity'].max() * axis_lim[1])
-        ax.set_title(f'{name} (Mass/Charge of TOF MS)', fontsize=25)
-        ax.set_xlabel(f'Mass/Charge', fontsize=25)
-        ax.set_ylabel('Intensity (cps)', fontsize=25)
+        return self.dfs
     
     def main_process(self):
-        dfs = self.load_data(self.args.dir, self.args.recursive)
+        self.load_data(self.args.dir, self.args.recursive)
+        if self.args.multi_process > 1:
+            self.task_pool = TaskPool('process', self.args.multi_process).run()
+            print(f'created task pool with {self.args.multi_process} processes')
         # show data general info and output peak list DataFrame
-        for n,df in dfs.items():
-            path = Path(n).resolve()
-            name = path.stem
-            if self.use_recursive_output:
-                self.original_output = self.args.output
-                self.args.output = str(path.parent)
-            print(f'\n\n\n\n\n{name}: {df._attrs["content_type"]}:\n', df)
-            df.to_csv(os.path.join(self.args.output, f'{name} {df._attrs["content_type"]}.csv'))
-            # process Mass (charge) and identify mass
-            if df._attrs['content_type'] == 'peak list':
-                df = self.filter_peaklist_data(df, self.args)
-            if not df.empty:
-                # plot each df
-                print(f'plotting {name}: {df._attrs["content_type"]}')
-                fig, ax = plt.subplots(figsize=(10, 6))
-                if df._attrs["content_type"] == 'base peak':
-                    self.plot_basepeak(name, df, self.args, ax)
-                elif df._attrs["content_type"] == 'absorbance':
-                    self.plot_absorbance(name, df, self.args, ax)
-                elif df._attrs["content_type"] == 'peak list': # avoid drop all data but still draw
-                    self.plot_peaklist(name, df, self.args, ax)
-                elif df._attrs["content_type"] =='mass-charge':
-                    self.plot_masscharge(name, df, self.args, ax)
-                # style adjust and save
-                plt.xticks(size = 20);plt.yticks(size = 20)
-                plt.legend(fontsize=15, loc = self.args.legend_pos,
-                           bbox_to_anchor = (self.args.legend_pos_bbox1, self.args.legend_pos_bbox2),
-                           draggable = True)
-                save_show(os.path.join(self.args.output, f'{name} {df._attrs["content_type"]}.png'),
-                          dpi = 600, show = self.args.show_fig)
-            else:
-                print(f'no data left after filtering, skip {name}: {df._attrs["content_type"]}')
-            # recovery output path
-            if self.use_recursive_output:
-                self.output = self.original_output
-            
+        for n, data in self.dfs.items():
+            if data.peak_df is None or data.check_processed_data_empty(data.peak_df):
+                print(f'{n}: search peaks...')
+                data.search_peaks(self.args.xlim, self.args.min_peak_width,
+                                  self.task_pool, self.args.multi_process)
+                data.filter_peaks(self.args.xlim, self.args.min_height, self.args.min_height_percent)
+            data.save_processed_data()
+            print(f'{n}: processed data saved to {data.processed_data_path}')
+            _plot_mass(data, xlim=self.args.xlim, labels=self.args.labels, labels_eps=self.args.labels_eps)
+            # style adjust and save
+            plt.xticks(size = 20);plt.yticks(size = 20)
+            png_path = Path(data.data_file_path).with_suffix('.png')
+            save_show(png_path, dpi = 600, show = self.args.show_fig)
+            print(f'{n}: plot saved to {png_path}')
+        self.task_pool.close()
+
 
 class explore_mass(plot_mass):
     from nicegui import ui
     def __init__(self, args: argparse.Namespace, printf=print) -> None:
         super().__init__(args, printf)
         self.labels_string = args.labels
         self.fig = None
         self._expansion = []
+        self._bbox_extra_artists = None
         
     def _ui_only_one_expansion(self, e):
         if e.value:
             for expansion in self._expansion:
                 if expansion != e.sender:
                     expansion.value = False
         
     @ui.refreshable
     def make_fig(self):
         from nicegui import ui
         plt.close(self.fig)
         with ui.pyplot(figsize=(self.args.fig_w, self.args.fig_h), close = False) as fig:
-            # process labels
-            self.args.labels = self.process_labels(self.args.labels_string)
-            # process io path
-            if self.use_recursive_output:
-                self.original_output = self.args.output
-                self.args.output = os.path.dirname(self.args.now_name)
-            df = self.args.dfs[self.args.now_name].copy() # avoid modify original data
-            name = Path(self.args.now_name).resolve().stem # same as plot-mass
+            # process args
+            self.args.labels = process_peak_labels(self.args.labels_string)
+            self.args.xlim = eval(f'[{self.args.xlim}]') if isinstance(self.args.xlim, str) else self.args.xlim
             # plot
-            print(f'plotting {name}: {df._attrs["content_type"]}')
             ax = fig.fig.gca()
-            if df._attrs["content_type"] == 'peak list': # avoid drop all data but still draw
-                df = self.filter_peaklist_data(df, self.args)
-                if not df.empty:
-                    self.plot_peaklist(name, df, self.args, ax)
-                else:
-                    ui.notify(f'no data left after filtering, skip {name}: {df._attrs["content_type"]}')
-            elif df._attrs["content_type"] =='mass-charge':
-                self.plot_masscharge(name, df, self.args, ax)
-            # fix style
+            data = self.args.dfs[self.args.now_name]
+            ## choose mass data
+            if self.args.mass and data.X_M_HEADER is not None:
+                data.X_HEADER = data.X_M_HEADER
+            elif not self.args.mass:
+                data.X_HEADER = data.X_MZ_HEADER
+            ## search peaks
+            if data.peak_df is None or data.check_processed_data_empty(data.peak_df):
+                ui.notify(f'{data.get_tag()}: search peaks...')
+                data.search_peaks(self.args.xlim, self.args.min_peak_width,
+                                  self.task_pool, self.args.multi_process)
+            tmp_data = deepcopy(data) # filter from original data
+            tmp_data.filter_peaks(self.args.xlim, self.args.min_height, self.args.min_height_percent)
+            ## plot
+            ax, self._bbox_extra_artists = _plot_mass(tmp_data, ax = ax, xlim=self.args.xlim,
+                                                      labels=self.args.labels, labels_eps=self.args.labels_eps,
+                                                      legend_bbox=(self.args.legend_pos_bbox1, self.args.legend_pos_bbox2),
+                                                      legend_pos=self.args.legend_pos, marker_size=self.args.marker_size)
+            x_axis_exp = (1-self.args.xaxis_expand, 1+self.args.xaxis_expand)
+            y_axis_exp = (1-self.args.yaxis_expand, 1+self.args.yaxis_expand)
+            plt.xlim(tmp_data.peak_df[tmp_data.X_HEADER].min() * x_axis_exp[0], tmp_data.peak_df[tmp_data.X_HEADER].max() * x_axis_exp[1])
+            plt.ylim(tmp_data.peak_df[tmp_data.Y_HEADER].min() * y_axis_exp[0], tmp_data.peak_df[tmp_data.Y_HEADER].max() * y_axis_exp[1])
             plt.xticks(size = self.args.xticks_fontsize)
             plt.yticks(size = self.args.yticks_fontsize)
             plt.title(self.args.title, fontsize=self.args.title_fontsize)
             plt.xlabel(self.args.xlabel, fontsize=self.args.axis_label_fontsizes)
             plt.ylabel(self.args.ylabel, fontsize=self.args.axis_label_fontsizes)
-            plt.legend(fontsize=self.args.legend_fontsize, loc=self.args.legend_pos,
-                       bbox_to_anchor=(self.args.legend_pos_bbox1, self.args.legend_pos_bbox2), draggable = True)
-            # recovery output path
-            if self.use_recursive_output:
-                self.output = self.original_output
-        self.fig = fig.fig
+            self.fig = fig.fig
         
     def save_fig(self):
         from nicegui import ui
-        path = os.path.join(self.args.output, self.args.file_name + ('' if self.args.file_name.endswith('.png') else '.png'))
-        ui.notify(f'saving figure to {path}')
-        save_show(path, dpi = self.args.dpi, show = self.args.show_fig)
+        png_path = Path(self.args.dfs[self.args.now_name].data_file_path).with_suffix('.png')
+        ui.notify(f'saving figure to {png_path}')
+        save_show(png_path, dpi = self.args.dpi, show = self.args.show_fig)
         
     def main_process(self):
         from nicegui import app, ui
+
         from mbapy.game import BaseInfo
+
+        # set task pool
+        if self.args.multi_process > 1:
+            self.task_pool = TaskPool('process', self.args.multi_process).run()
+            print(f'created task pool with {self.args.multi_process} processes')
         # process args and load data
-        dfs = self.load_data(self.args.dir, self.args.recursive)
-        dfs = {k:v for k,v in dfs.items() if v is not None and v._attrs['content_type'] in ['peak list','mass-charge']}
-        if not dfs:
+        self.load_data(self.args.dir, self.args.recursive)
+        self.dfs = {data.data_file_path:data for data in self.dfs.values()}
+        if not self.dfs:
             raise FileNotFoundError(f'can not find peak-list or mass-charge txt files in {self.args.dir}')
         # make global settings
-        self.args = BaseInfo(now_name = list(dfs.keys())[0], dfs = dfs,
+        self.args = BaseInfo(now_name = list(self.dfs.keys())[0], dfs = self.dfs,
                             #  instance_refresh = False, # instance refresh not implemented yet
                             labels_string = self.labels_string,
                             title = '', xlabel = 'Mass/Charge', ylabel = 'Intensity (cps)',
                             xticks_fontsize = 20, yticks_fontsize = 20, tag_fontsize = 15,
                             axis_label_fontsizes = 25, title_fontsize = 25, legend_fontsize = 15,
-                            fig_w = 10, fig_h = 8, dpi = 600, file_name = '',
+                            fig_w = 12, fig_h = 7, dpi = 600, file_name = '',
+                            xaxis_expand = 0.2, yaxis_expand = 0.1,
+                            legend_pos_bbox1 = 1.0, legend_pos_bbox2 = 1.0, legend_pos = 'upper right',
                             **self.args.__dict__)
         # GUI
         with ui.header(elevated=True).style('background-color: #3874c8'):
             ui.label('mbapy-cli mass | Mass Data Explorer').classes('text-h4')
             ui.space()
             # ui.checkbox('Instance refresh', value=self.args.instance_refresh).bind_value_to(self.args, 'instance_refresh')
             ui.button('Refresh', on_click=self.make_fig.refresh, icon='refresh').props('no-caps')
             ui.button('Save', on_click=self.save_fig, icon='save').props('no-caps')
             ui.button('Show', on_click=plt.show, icon='open_in_new').props('no-caps')
             ui.button('Exit', on_click=app.shutdown, icon='power')
         with ui.splitter(value = 15).classes('w-full h-full h-56') as splitter:
             with splitter.before:
-                df_short_names = [n.replace(os.path.join(self.args.dir, ''), '') for n in dfs]
+                df_short_names = [n.replace(os.path.join(self.args.dir, ''), '') for n in self.dfs]
                 with ui.tabs(value = df_short_names[0]).props('vertical').classes('w-full h-full') as tabs:
                     df_tabs = [ui.tab(n).props('no-caps').classes('w-full') for n in df_short_names]
                 tabs.bind_value_to(self.args, 'now_name', lambda short_name: os.path.join(self.args.dir, short_name))
                 # tabs.on_value_change(self.make_fig) # instance refresh not implemented yet
             with splitter.after:
                 with ui.row().classes('w-full h-full'):
                     with ui.column().classes('h-full'):
                         # data filtering configs
                         with ui.expansion('Data Filtering', icon='filter_alt', value=True, on_value_change=self._ui_only_one_expansion) as expansion1:
                             self._expansion.append(expansion1)
                             ui.checkbox('use peaks cache', value=self.args.use_peaks_cache).bind_value_to(self.args, 'use_peaks_cache')
-                            ui.checkbox('filter by mass', value=self.args.mass).bind_value_to(self.args,'mass')
-                            ui.number('min peak width', value=self.args.min_peak_width, min = 1).bind_value_to(self.args,'min_peak_width')
+                            ui.checkbox('filter by mass', value=self.args.mass).bind_value_to(self.args, 'mass')
                             ui.number('min height', value=self.args.min_height, min = 0).bind_value_to(self.args, 'min_height')
                             ui.number('min height percent', value=self.args.min_height_percent, min = 0, max = 100).bind_value_to(self.args,'min_height_percent').classes('w-full')
                             ui.input('xlim', value=self.args.xlim).bind_value_to(self.args, 'xlim')
                         # configs for fontsize
                         with ui.expansion('Configs for Fontsize', icon='format_size', on_value_change=self._ui_only_one_expansion) as expansion2:
                             self._expansion.append(expansion2)
                             ui.number('xticks fontsize', value=self.args.xticks_fontsize, min=0, step=0.5, format='%.1f').bind_value_to(self.args, 'xticks_fontsize')
                             ui.number('yticks fontsize', value=self.args.yticks_fontsize, min=0, step=0.5, format='%.1f').bind_value_to(self.args, 'yticks_fontsize')
                             ui.number('title fontsize', value=self.args.title_fontsize, min=0, step=0.5, format='%.1f').bind_value_to(self.args, 'title_fontsize')
                             ui.number('axis label fontsize', value=self.args.axis_label_fontsizes, min=0, step=0.5, format='%.1f').bind_value_to(self.args, 'axis_label_fontsizes')
                             ui.number('tag fontsize', value=self.args.tag_fontsize, min=0, step=0.5, format='%.1f').bind_value_to(self.args, 'tag_fontsize')
+                            ui.number('marker size', value=self.args.marker_size, min=0, step=10, format='%.1f').bind_value_to(self.args,'marker_size')
                             ui.input('title', value=self.args.title).bind_value_to(self.args, 'title')
                             ui.input('xlabel', value=self.args.xlabel).bind_value_to(self.args, 'xlabel')
                             ui.input('ylabel', value=self.args.ylabel).bind_value_to(self.args, 'ylabel')
                         # configs for legend
                         with ui.expansion('Configs for Legend', icon='more', on_value_change=self._ui_only_one_expansion) as expansion3:
                             self._expansion.append(expansion3)
                             ui.textarea('labels', value=self.args.labels_string).bind_value_to(self.args, 'labels_string').props('clearable')
-                            ui.number('labels eps', value=self.args.labels_eps, min=0, step=0.1, format='%.1f').bind_value_to(self.args, 'labels_eps')
+                            ui.number('labels eps', value=self.args.labels_eps, min=0, step=0.1, format='%.6f').bind_value_to(self.args, 'labels_eps')
                             ui.number('legend fontsize', value=self.args.legend_fontsize, min=0, step=0.5, format='%.1f').bind_value_to(self.args, 'legend_fontsize')
                             ui.input('legend loc', value=self.args.legend_pos).bind_value_to(self.args, 'legend_pos')
-                            ui.number('bbox1', value=self.args.legend_pos_bbox1, min=0, step=0.1, format='%.1f').bind_value_to(self.args, 'legend_pos_bbox1')
-                            ui.number('bbox2', value=self.args.legend_pos_bbox2, min=0, step=0.1, format='%.1f').bind_value_to(self.args, 'legend_pos_bbox2')
+                            with ui.row().classes('w-full'):
+                                ui.number('bbox1', value=self.args.legend_pos_bbox1, min=0, step=0.1, format='%.3f').bind_value_to(self.args, 'legend_pos_bbox1')
+                                ui.number('bbox2', value=self.args.legend_pos_bbox2, min=0, step=0.1, format='%.3f').bind_value_to(self.args, 'legend_pos_bbox2')
                         # configs for saving
                         with ui.expansion('Configs for Saving', icon='save', on_value_change=self._ui_only_one_expansion) as expansion4:
                             self._expansion.append(expansion4)
                             ui.checkbox('show figure', value=self.args.show_fig).bind_value_to(self.args,'show_fig')
-                            ui.number('axis expand', value=self.args.expand, min=0, max=1, step=0.01, format='%.3f').bind_value_to(self.args, 'expand')
-                            ui.number('figure width', value=self.args.fig_w, min=1, step=0.5, format='%.1f').bind_value_to(self.args, 'fig_w')
-                            ui.number('figure height', value=self.args.fig_h, min=1, step=0.5, format='%.1f').bind_value_to(self.args, 'fig_h')
+                            with ui.row().classes('w-full'):
+                                ui.number('x axis expand', value=self.args.xaxis_expand, min=0, max=1, step=0.01, format='%.3f').classes('w-2/5').bind_value_to(self.args, 'xaxis_expand')
+                                ui.number('y axis expand', value=self.args.yaxis_expand, min=0, max=1, step=0.01, format='%.3f').classes('w-2/5').bind_value_to(self.args, 'yaxis_expand')
+                            ui.number('figure width', value=self.args.fig_w, min=1, step=0.5, format='%.3f').bind_value_to(self.args, 'fig_w')
+                            ui.number('figure height', value=self.args.fig_h, min=1, step=0.5, format='%.3f').bind_value_to(self.args, 'fig_h')
                             ui.number('DPI', value=self.args.dpi, min=1, step=1, format='%d').bind_value_to(self.args, 'dpi')
                             ui.input('figure file name', value=self.args.file_name).bind_value_to(self.args, 'file_name')
                     with ui.card():
                         ui.label(f'{df_short_names[0]}').classes('text-h6').bind_text_from(tabs, 'value')
                         self.make_fig()
         ## run GUI
         ui.run(host = 'localhost', port = 8010, title = 'Mass Data Explorer', reload=False)
@@ -402,45 +282,42 @@
     # set draw argument
     plot_mass_args.add_argument('--use-peaks-cache', action='store_true', default=False,
                                 help='use peaks cache to speed up plot, default is %(default)s')
     plot_mass_args.add_argument('-m', '--mass', action='store_true', default=False,
                                 help='draw Mass instead of Mass/charge which is Mass+z, default is %(default)s')
     plot_mass_args.add_argument('-min', '--min-height', type = int, default=0,
                                 help='filter data with min height in peak list plot, default is %(default)s')
-    plot_mass_args.add_argument('-minp', '--min-height-percent', type = float, default=10,
+    plot_mass_args.add_argument('-minp', '--min-height-percent', type = float, default=1,
                                 help='filter data with min height percent to hightest in mass/charge plot, default is %(default)s')
     plot_mass_args.add_argument('--min-peak-width', type = float, default=4,
                                 help='filter peaks with min width in Mass/Charge plot, default is %(default)s')
     plot_mass_args.add_argument('-xlim', type = str, default=None,
                                 help='set x-axis limit, input as "200,2000", default is %(default)s')
     plot_mass_args.add_argument('-col', '--color', type = str, default='black',
                                 help='draw color, default is %(default)s')
+    plot_mass_args.add_argument('--marker-size', type = float, default=120,
+                                help='marker size, default is %(default)s')
     plot_mass_args.add_argument('-labels', '--labels', type = str, default='',
-                                help='labels, input as 1000,Pep1;1050,Pep2, default is %(default)s')
+                                help='labels, input as 1000,Pep1,red;1050,Pep2, default is %(default)s')
     plot_mass_args.add_argument('--labels-eps', type = float, default=0.5,
                                 help='eps to recognize labels, default is %(default)s')
-    plot_mass_args.add_argument('-expand', '--expand', type = float, default=0.2,
-                                help='how much the x-axis and y-axisto be expanded, default is %(default)s')
-    plot_mass_args.add_argument('-lpos', '--legend-pos', type = str, default='upper center',
-                                help='legend position, can be string as "upper center", or be float as 0.1,0.2, default is %(default)s')
-    plot_mass_args.add_argument('-lposbbox1', '--legend-pos-bbox1', type = float, default=1.2,
-                                help='legend position bbox 1 to anchor, default is %(default)s')
-    plot_mass_args.add_argument('-lposbbox2', '--legend-pos-bbox2', type = float, default=1,
-                                help='legend position bbox 2 to anchor, default is %(default)s')
     plot_mass_args.add_argument('-sf', '--show-fig', action='store_true', default=False,
                                 help='automatically show figure, default is %(default)s')
+    plot_mass_args.add_argument('-mp', '--multi-process', type = int, default=4,
+                                help='multi-process to speed up plot, default is %(default)s')
 
     explore_mass_args = subparsers.add_parser('explore-mass', description='explore mass spectrum data')
     for action in plot_mass_args._actions:
         if action.dest == 'use_peaks_cache':
             action.default = True
         if action.dest not in ['help']:
             explore_mass_args._add_action(action)
 
-    excute_command(args_paser, sys_args, _str2func)
-
+    if __name__ in ['__main__', 'mbapy.scripts.mass']:
+        # '__main__' is debug, 'mbapy.scripts.mass' is user running
+        excute_command(args_paser, sys_args, _str2func)
 
 if __name__ in {"__main__", "__mp_main__"}:
     # dev code, MUST COMMENT OUT BEFORE RELEASE
     # main('explore-mass -d data_tmp/scripts/mass'.split())
     
     main()
```

### Comparing `mbapy-0.7.4/mbapy/scripts/mv.py` & `mbapy-0.8.0/mbapy/scripts/mv.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/peptide.py` & `mbapy-0.8.0/mbapy/scripts/peptide.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/reviz.py` & `mbapy-0.8.0/mbapy/scripts/reviz.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/rm.py` & `mbapy-0.8.0/mbapy/scripts/rm.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/scihub.py` & `mbapy-0.8.0/mbapy/scripts/scihub.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/scihub_selenium.py` & `mbapy-0.8.0/mbapy/scripts/scihub_selenium.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/splash_img.py` & `mbapy-0.8.0/mbapy/scripts/splash_img.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/scripts/video.py` & `mbapy-0.8.0/mbapy/scripts/video.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/stats/__init__.py` & `mbapy-0.8.0/mbapy/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/stats/cluster.py` & `mbapy-0.8.0/mbapy/stats/cluster.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/stats/df.py` & `mbapy-0.8.0/mbapy/stats/df.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/stats/geography.py` & `mbapy-0.8.0/mbapy/stats/geography.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/stats/reg.py` & `mbapy-0.8.0/mbapy/stats/reg.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/stats/test.py` & `mbapy-0.8.0/mbapy/stats/test.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/storage/libsci.dll` & `mbapy-0.8.0/mbapy/storage/libsci.dll`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/storage/libsci.so` & `mbapy-0.8.0/mbapy/storage/libsci.so`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/storage/libstats.dll` & `mbapy-0.8.0/mbapy/storage/libstats.dll`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/storage/libstats.so` & `mbapy-0.8.0/mbapy/storage/libstats.so`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/storage/mbapy-cli-scripts-list.json` & `mbapy-0.8.0/mbapy/storage/mbapy-cli-scripts-list.json`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/web.py` & `mbapy-0.8.0/mbapy/web.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/web_utils/parse.py` & `mbapy-0.8.0/mbapy/web_utils/parse.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/web_utils/request.py` & `mbapy-0.8.0/mbapy/web_utils/request.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/web_utils/spider.py` & `mbapy-0.8.0/mbapy/web_utils/spider.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/mbapy/web_utils/task.py` & `mbapy-0.8.0/mbapy/web_utils/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import _thread
 import asyncio
+import multiprocessing
 import os
 import re
-import time
 import threading
-import multiprocessing
+import time
 from collections import namedtuple
 from enum import Enum
 from functools import partial
 from queue import Queue
-from typing import Any, Callable, Dict, List, Tuple, Union
+from typing import Any, Callable, Dict, List, Literal, Set, Tuple, Union
 from uuid import uuid4
 
 from tqdm import tqdm
 
 if __name__ == '__main__':
     # dev mode
-    from mbapy.base import put_err, put_log, parameter_checker
+    from mbapy.base import parameter_checker, put_err, put_log
 else:
-    from ..base import put_err, put_log, parameter_checker
+    from ..base import parameter_checker, put_err, put_log
 
 statuesQue = Queue()
 Key2Action = namedtuple('Key2Action', ['statue', 'func', 'args', 'kwgs',
                                        'is_reg', 'lock'],
                         defaults=[False, None])
 
 def _wait_for_quit(statuesQue, key2action: Dict[str, List[Key2Action]]):
@@ -330,23 +330,24 @@
         return getattr(self, f'_add_task_{mode}')(name, coro_func, *args, **kwargs)
 
     def _query_async_task_callback(self, future: asyncio.Future, task_name: str):
         try:
             self._thread_result_queue.put((task_name, future.result(),
                                            TaskStatus.SUCCEED))
         except Exception as e:
+            put_err(f'error {e} when get result from queue') 
             self._thread_result_queue.put((task_name, e, TaskStatus.NOT_SUCCEEDED))
             
     def _query_task_queue(self, block: bool = True, timeout: int = 3):
         while not self._thread_result_queue.empty():
             try:
                 _name, result, statue = self._thread_result_queue.get(block, timeout)
                 self.tasks[_name] = (_name, result, statue)
             except Exception as e:
-                put_err(f'error {e} when get result from queue')        
+                put_err(f'error {e} when get result from queue')
         
     def query_task(self, name, block: bool = False, timeout: int = 3):
         # short-cut for not found
         if name not in self.tasks:
             return self.TASK_NOT_FOUND
         # retrive finished results
         self._query_task_queue(block=block, timeout=timeout)
@@ -418,21 +419,27 @@
         """
         st = time.time()
         if verbose:
             bar =tqdm(desc='waiting', total=len(self.tasks), initial=self.count_done_tasks())
         while not condition_func(*args, **kwargs):
             if timeout is not None and time.time() - st > timeout:
                 return False
+            done = self.count_done_tasks()
             if verbose:
-                done = self.count_done_tasks()
                 bar.set_description(f'done/sum: {done}/{len(self.tasks)}')
                 bar.update(self.count_done_tasks() - bar.n)
             time.sleep(wait_each_loop)
         return self
     
+    def wait_till_tasks_done(self, task_names: List[str],
+                             wait_each_loop: float = 0.5) -> Dict[str, Union[Any, Literal[TaskStatus.NOT_FOUND], Literal[TaskStatus.NOT_FINISHED]]]:
+        self.wait_till(lambda names: names.issubset(set([r[0] for r in self.tasks.values() if r != TaskStatus.NOT_RETURNED])),
+                       wait_each_loop = wait_each_loop, verbose=False, names=set(task_names))
+        return {name: self.query_task(name) for name in task_names}
+    
     def close(self):
         """close the thread and event loop, join the thread"""
         # close async pool
         if self.MODE == 'async':
             self._async_loop.call_soon_threadsafe(self._async_loop.stop)
             self._async_loop.close()
         # close thread and join it
```

### Comparing `mbapy-0.7.4/mbapy.egg-info/PKG-INFO` & `mbapy-0.8.0/mbapy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbapy
-Version: 0.7.4
+Version: 0.8.0
 Summary: MyBA in Python
 Home-page: https://github.com/BHM-Bob/BA_PY
 Author: BHM-Bob G
 Author-email: bhmfly@foxmail.com
 License: MIT Licence
 Description: <!--
          * @Author: BHM-Bob 2262029386@qq.com
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mbapy Version: 0.7.4 Summary: MyBA in Python Home-
+Metadata-Version: 2.1 Name: mbapy Version: 0.8.0 Summary: MyBA in Python Home-
 page: https://github.com/BHM-Bob/BA_PY Author: BHM-Bob G Author-email:
 bhmfly@foxmail.com License: MIT Licence Description:
 ************ BBAA__PPYY:: OOppttiimmiizzee YYoouurr WWoorrkkffllooww wwiitthh PPyytthhoonn!! ************
 [Downloads][Downloads][Downloads]
 _[_r_e_p_o_ _s_i_z_e_]_[_c_o_d_e_ _s_i_z_e_]_[_G_i_t_H_u_b_ _r_e_l_e_a_s_e_ _(_l_a_t_e_s_t_ _b_y_ _d_a_t_e_)_]_[_G_i_t_H_u_b_ _C_o_m_m_i_t_ _A_c_t_i_v_i_t_y_]
 [GitHub last commit]
 _[_P_y_P_I_ _S_t_a_t_u_s_]_[_P_y_P_I_]_[_p_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
```

### Comparing `mbapy-0.7.4/mbapy.egg-info/SOURCES.txt` & `mbapy-0.8.0/mbapy.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -39,14 +39,26 @@
 mbapy/file_utils/__init__.py
 mbapy/file_utils/image.py
 mbapy/file_utils/video.py
 mbapy/plot_utils/__init__.py
 mbapy/plot_utils/bar_utils.py
 mbapy/plot_utils/line_utils.py
 mbapy/plot_utils/scatter_utils.py
+mbapy/sci_instrument/__init__.py
+mbapy/sci_instrument/_base.py
+mbapy/sci_instrument/_utils.py
+mbapy/sci_instrument/hplc/SCIEX.py
+mbapy/sci_instrument/hplc/__init__.py
+mbapy/sci_instrument/hplc/_base.py
+mbapy/sci_instrument/hplc/_utils.py
+mbapy/sci_instrument/hplc/waters.py
+mbapy/sci_instrument/mass/SCIEX.py
+mbapy/sci_instrument/mass/__init__.py
+mbapy/sci_instrument/mass/_base.py
+mbapy/sci_instrument/mass/_utils.py
 mbapy/sci_utils/__init__.py
 mbapy/sci_utils/paper_download.py
 mbapy/sci_utils/paper_parse.py
 mbapy/sci_utils/paper_search.py
 mbapy/scripts/__init__.py
 mbapy/scripts/__main__.py
 mbapy/scripts/_main_.py
```

### Comparing `mbapy-0.7.4/mbapy.egg-info/requires.txt` & `mbapy-0.8.0/mbapy.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/requirements.json` & `mbapy-0.8.0/requirements.json`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/setup.py` & `mbapy-0.8.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 '''
 Author: BHM-Bob 2262029386@qq.com
 Date: 2022-11-01 18:30:01
 LastEditors: BHM-Bob 2262029386@qq.com
-LastEditTime: 2024-05-10 21:06:14
+LastEditTime: 2024-06-01 20:01:47
 Description: 
 '''
 """
 something is from https://github.com/pypa/sampleproject
 thanks to https://zetcode.com/python/package/
 thanks to https://github.com/gaogaotiantian/viztracer/blob/master/setup.py
 """
@@ -104,8 +104,8 @@
         'full': requirements['std'] + requirements['full'],
         },
 )
 
 # pip install .
 
 # python setup.py sdist
-# twine upload dist/mbapy-0.7.4.tar.gz
+# twine upload dist/mbapy-0.8.0.tar.gz
```

### Comparing `mbapy-0.7.4/test/test_base.py` & `mbapy-0.8.0/test/test_base.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/test/test_game.py` & `mbapy-0.8.0/test/test_game.py`

 * *Files identical despite different names*

### Comparing `mbapy-0.7.4/test/test_web.py` & `mbapy-0.8.0/test/test_web.py`

 * *Files identical despite different names*

