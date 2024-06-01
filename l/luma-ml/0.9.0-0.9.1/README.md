# Comparing `tmp/luma-ml-0.9.0.tar.gz` & `tmp/luma_ml-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luma-ml-0.9.0.tar", last modified: Thu May 30 20:01:40 2024, max compression
+gzip compressed data, was "luma_ml-0.9.1.tar", last modified: Sat Jun  1 18:13:49 2024, max compression
```

## Comparing `luma-ml-0.9.0.tar` & `luma_ml-0.9.1.tar`

### file list

```diff
@@ -1,102 +1,103 @@
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.036328 luma-ml-0.9.0/
--rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma-ml-0.9.0/LICENSE
--rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-05-30 20:01:40.035961 luma-ml-0.9.0/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     4948 2024-05-30 20:00:23.000000 luma-ml-0.9.0/README.md
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.004246 luma-ml-0.9.0/luma/
--rw-r--r--   0 chanlee    (501) staff       (20)    11653 2024-05-30 16:18:18.000000 luma-ml-0.9.0/luma/__import__.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1502 2024-05-26 11:11:06.000000 luma-ml-0.9.0/luma/__init__.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.006842 luma-ml-0.9.0/luma/classifier/
--rw-r--r--   0 chanlee    (501) staff       (20)    12563 2024-05-13 11:38:17.000000 luma-ml-0.9.0/luma/classifier/discriminant.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7935 2024-05-13 11:35:13.000000 luma-ml-0.9.0/luma/classifier/logistic.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-05-23 16:46:06.000000 luma-ml-0.9.0/luma/classifier/naive_bayes.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9070 2024-05-13 11:30:20.000000 luma-ml-0.9.0/luma/classifier/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9174 2024-05-13 11:33:07.000000 luma-ml-0.9.0/luma/classifier/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9806 2024-05-13 11:36:04.000000 luma-ml-0.9.0/luma/classifier/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.009974 luma-ml-0.9.0/luma/clustering/
--rw-r--r--   0 chanlee    (501) staff       (20)    18057 2024-05-13 11:42:50.000000 luma-ml-0.9.0/luma/clustering/affinity.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17889 2024-05-13 11:50:11.000000 luma-ml-0.9.0/luma/clustering/density.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7697 2024-05-13 11:51:42.000000 luma-ml-0.9.0/luma/clustering/hierarchy.py
--rw-r--r--   0 chanlee    (501) staff       (20)    18307 2024-05-13 11:55:03.000000 luma-ml-0.9.0/luma/clustering/kmeans.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8192 2024-05-13 11:55:57.000000 luma-ml-0.9.0/luma/clustering/mixture.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11602 2024-05-13 11:57:37.000000 luma-ml-0.9.0/luma/clustering/spectral.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.011616 luma-ml-0.9.0/luma/core/
--rw-r--r--   0 chanlee    (501) staff       (20)     5924 2024-05-13 11:58:02.000000 luma-ml-0.9.0/luma/core/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)      446 2024-05-13 11:58:51.000000 luma-ml-0.9.0/luma/core/main.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11013 2024-05-13 12:05:21.000000 luma-ml-0.9.0/luma/core/super.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.014590 luma-ml-0.9.0/luma/ensemble/
--rw-r--r--   0 chanlee    (501) staff       (20)    10046 2024-05-13 12:09:42.000000 luma-ml-0.9.0/luma/ensemble/bagging.py
--rw-r--r--   0 chanlee    (501) staff       (20)    19721 2024-05-13 12:15:52.000000 luma-ml-0.9.0/luma/ensemble/boost.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10280 2024-05-13 12:20:38.000000 luma-ml-0.9.0/luma/ensemble/forest.py
--rw-r--r--   0 chanlee    (501) staff       (20)    14109 2024-05-13 12:31:18.000000 luma-ml-0.9.0/luma/ensemble/stack.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6779 2024-05-13 12:36:00.000000 luma-ml-0.9.0/luma/ensemble/vote.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.015968 luma-ml-0.9.0/luma/interface/
--rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-05-13 12:36:06.000000 luma-ml-0.9.0/luma/interface/exception.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7413 2024-05-17 07:30:53.000000 luma-ml-0.9.0/luma/interface/typing.py
--rw-r--r--   0 chanlee    (501) staff       (20)    16347 2024-05-27 18:40:22.000000 luma-ml-0.9.0/luma/interface/util.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.017330 luma-ml-0.9.0/luma/metric/
--rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma-ml-0.9.0/luma/metric/classification.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5917 2024-05-13 15:46:55.000000 luma-ml-0.9.0/luma/metric/clustering.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-05-13 15:46:57.000000 luma-ml-0.9.0/luma/metric/distance.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-05-13 15:46:59.000000 luma-ml-0.9.0/luma/metric/regression.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.017536 luma-ml-0.9.0/luma/migrate/
--rw-r--r--   0 chanlee    (501) staff       (20)     3764 2024-05-13 16:18:47.000000 luma-ml-0.9.0/luma/migrate/port.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.019417 luma-ml-0.9.0/luma/model_selection/
--rw-r--r--   0 chanlee    (501) staff       (20)     3438 2024-05-13 16:20:58.000000 luma-ml-0.9.0/luma/model_selection/cv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8041 2024-05-13 16:29:29.000000 luma-ml-0.9.0/luma/model_selection/fold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12244 2024-05-13 16:35:00.000000 luma-ml-0.9.0/luma/model_selection/search.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5736 2024-05-13 16:40:23.000000 luma-ml-0.9.0/luma/model_selection/split.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.021681 luma-ml-0.9.0/luma/neural/
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.023406 luma-ml-0.9.0/luma/neural/_layers/
--rw-r--r--   0 chanlee    (501) staff       (20)     6748 2024-05-12 09:16:35.000000 luma-ml-0.9.0/luma/neural/_layers/_act.py
--rw-r--r--   0 chanlee    (501) staff       (20)    19314 2024-05-27 19:00:28.000000 luma-ml-0.9.0/luma/neural/_layers/_conv.py
--rw-r--r--   0 chanlee    (501) staff       (20)     4144 2024-05-23 16:58:05.000000 luma-ml-0.9.0/luma/neural/_layers/_drop.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2313 2024-05-12 09:17:05.000000 luma-ml-0.9.0/luma/neural/_layers/_linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    10790 2024-05-30 19:49:07.000000 luma-ml-0.9.0/luma/neural/_layers/_norm.py
--rw-r--r--   0 chanlee    (501) staff       (20)    29777 2024-05-26 11:24:51.000000 luma-ml-0.9.0/luma/neural/_layers/_pool.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.025074 luma-ml-0.9.0/luma/neural/_models/
--rw-r--r--   0 chanlee    (501) staff       (20)    13097 2024-05-29 08:01:04.000000 luma-ml-0.9.0/luma/neural/_models/_alex.py
--rw-r--r--   0 chanlee    (501) staff       (20)    13040 2024-05-30 19:37:12.000000 luma-ml-0.9.0/luma/neural/_models/_inception.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12760 2024-05-29 08:01:42.000000 luma-ml-0.9.0/luma/neural/_models/_lenet.py
--rw-r--r--   0 chanlee    (501) staff       (20)     9639 2024-05-29 08:00:44.000000 luma-ml-0.9.0/luma/neural/_models/_simple.py
--rw-r--r--   0 chanlee    (501) staff       (20)    23952 2024-05-29 08:01:18.000000 luma-ml-0.9.0/luma/neural/_models/_vgg.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12024 2024-05-29 08:04:38.000000 luma-ml-0.9.0/luma/neural/base.py
--rw-r--r--   0 chanlee    (501) staff       (20)    54303 2024-05-30 20:01:17.000000 luma-ml-0.9.0/luma/neural/block.py
--rw-r--r--   0 chanlee    (501) staff       (20)     1319 2024-05-09 19:24:30.000000 luma-ml-0.9.0/luma/neural/init.py
--rw-r--r--   0 chanlee    (501) staff       (20)    34300 2024-05-30 19:15:29.000000 luma-ml-0.9.0/luma/neural/layer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-05-13 19:10:16.000000 luma-ml-0.9.0/luma/neural/loss.py
--rw-r--r--   0 chanlee    (501) staff       (20)    49671 2024-05-30 20:01:31.000000 luma-ml-0.9.0/luma/neural/network.py
--rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-05-09 17:12:02.000000 luma-ml-0.9.0/luma/neural/optimizer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     8582 2024-05-13 19:27:55.000000 luma-ml-0.9.0/luma/neural/single.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.025316 luma-ml-0.9.0/luma/pipe/
--rw-r--r--   0 chanlee    (501) staff       (20)     7308 2024-05-13 19:32:18.000000 luma-ml-0.9.0/luma/pipe/pipeline.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.027259 luma-ml-0.9.0/luma/preprocessing/
--rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma-ml-0.9.0/luma/preprocessing/encoder.py
--rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma-ml-0.9.0/luma/preprocessing/imputer.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3653 2024-05-13 19:32:35.000000 luma-ml-0.9.0/luma/preprocessing/outlier.py
--rw-r--r--   0 chanlee    (501) staff       (20)     2624 2024-05-13 19:33:29.000000 luma-ml-0.9.0/luma/preprocessing/scaler.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.029014 luma-ml-0.9.0/luma/reduction/
--rw-r--r--   0 chanlee    (501) staff       (20)    19163 2024-05-26 19:19:09.000000 luma-ml-0.9.0/luma/reduction/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)    40387 2024-05-13 19:55:48.000000 luma-ml-0.9.0/luma/reduction/manifold.py
--rw-r--r--   0 chanlee    (501) staff       (20)    17019 2024-05-14 09:45:27.000000 luma-ml-0.9.0/luma/reduction/selection.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.032657 luma-ml-0.9.0/luma/regressor/
--rw-r--r--   0 chanlee    (501) staff       (20)    19882 2024-05-14 09:56:22.000000 luma-ml-0.9.0/luma/regressor/general.py
--rw-r--r--   0 chanlee    (501) staff       (20)    12687 2024-05-14 10:03:42.000000 luma-ml-0.9.0/luma/regressor/linear.py
--rw-r--r--   0 chanlee    (501) staff       (20)     6755 2024-05-14 10:04:13.000000 luma-ml-0.9.0/luma/regressor/neighbors.py
--rw-r--r--   0 chanlee    (501) staff       (20)     3098 2024-05-14 10:05:44.000000 luma-ml-0.9.0/luma/regressor/poly.py
--rw-r--r--   0 chanlee    (501) staff       (20)    11070 2024-05-14 14:33:09.000000 luma-ml-0.9.0/luma/regressor/robust.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7805 2024-05-14 14:45:46.000000 luma-ml-0.9.0/luma/regressor/svm.py
--rw-r--r--   0 chanlee    (501) staff       (20)     7415 2024-05-14 14:59:17.000000 luma-ml-0.9.0/luma/regressor/tree.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.033262 luma-ml-0.9.0/luma/visual/
--rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma-ml-0.9.0/luma/visual/eda.py
--rw-r--r--   0 chanlee    (501) staff       (20)    25027 2024-05-23 17:04:49.000000 luma-ml-0.9.0/luma/visual/eval.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.034601 luma-ml-0.9.0/luma_ml.egg-info/
--rw-r--r--   0 chanlee    (501) staff       (20)     5554 2024-05-30 20:01:39.000000 luma-ml-0.9.0/luma_ml.egg-info/PKG-INFO
--rw-r--r--   0 chanlee    (501) staff       (20)     2000 2024-05-30 20:01:39.000000 luma-ml-0.9.0/luma_ml.egg-info/SOURCES.txt
--rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-05-30 20:01:39.000000 luma-ml-0.9.0/luma_ml.egg-info/dependency_links.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-30 20:01:39.000000 luma-ml-0.9.0/luma_ml.egg-info/requires.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-05-30 20:01:39.000000 luma-ml-0.9.0/luma_ml.egg-info/top_level.txt
--rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-05-30 20:01:40.036404 luma-ml-0.9.0/setup.cfg
--rw-r--r--   0 chanlee    (501) staff       (20)      842 2024-05-30 20:00:56.000000 luma-ml-0.9.0/setup.py
-drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-05-30 20:01:40.035282 luma-ml-0.9.0/test/
--rw-r--r--   0 chanlee    (501) staff       (20)      647 2024-04-29 02:58:00.000000 luma-ml-0.9.0/test/__act.py
--rw-r--r--   0 chanlee    (501) staff       (20)      429 2024-05-18 16:19:55.000000 luma-ml-0.9.0/test/__test.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.817218 luma_ml-0.9.1/
+-rw-r--r--   0 chanlee    (501) staff       (20)    35149 2023-11-07 13:17:31.000000 luma_ml-0.9.1/LICENSE
+-rw-r--r--   0 chanlee    (501) staff       (20)     5580 2024-06-01 18:13:49.816916 luma_ml-0.9.1/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     4954 2024-06-01 18:13:31.000000 luma_ml-0.9.1/README.md
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.790861 luma_ml-0.9.1/luma/
+-rw-r--r--   0 chanlee    (501) staff       (20)    11653 2024-05-30 16:18:18.000000 luma_ml-0.9.1/luma/__import__.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1502 2024-05-26 11:11:06.000000 luma_ml-0.9.1/luma/__init__.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.792778 luma_ml-0.9.1/luma/classifier/
+-rw-r--r--   0 chanlee    (501) staff       (20)    12563 2024-05-13 11:38:17.000000 luma_ml-0.9.1/luma/classifier/discriminant.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7935 2024-05-13 11:35:13.000000 luma_ml-0.9.1/luma/classifier/logistic.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5541 2024-05-23 16:46:06.000000 luma_ml-0.9.1/luma/classifier/naive_bayes.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9070 2024-05-13 11:30:20.000000 luma_ml-0.9.1/luma/classifier/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9174 2024-05-13 11:33:07.000000 luma_ml-0.9.1/luma/classifier/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9806 2024-05-13 11:36:04.000000 luma_ml-0.9.1/luma/classifier/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.794936 luma_ml-0.9.1/luma/clustering/
+-rw-r--r--   0 chanlee    (501) staff       (20)    18057 2024-05-13 11:42:50.000000 luma_ml-0.9.1/luma/clustering/affinity.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17889 2024-05-13 11:50:11.000000 luma_ml-0.9.1/luma/clustering/density.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7697 2024-05-13 11:51:42.000000 luma_ml-0.9.1/luma/clustering/hierarchy.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    18307 2024-05-13 11:55:03.000000 luma_ml-0.9.1/luma/clustering/kmeans.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8192 2024-05-13 11:55:57.000000 luma_ml-0.9.1/luma/clustering/mixture.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11602 2024-05-13 11:57:37.000000 luma_ml-0.9.1/luma/clustering/spectral.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.795938 luma_ml-0.9.1/luma/core/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5924 2024-05-13 11:58:02.000000 luma_ml-0.9.1/luma/core/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      446 2024-05-13 11:58:51.000000 luma_ml-0.9.1/luma/core/main.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11013 2024-05-13 12:05:21.000000 luma_ml-0.9.1/luma/core/super.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.797842 luma_ml-0.9.1/luma/ensemble/
+-rw-r--r--   0 chanlee    (501) staff       (20)    10046 2024-05-13 12:09:42.000000 luma_ml-0.9.1/luma/ensemble/bagging.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19721 2024-05-13 12:15:52.000000 luma_ml-0.9.1/luma/ensemble/boost.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10280 2024-05-13 12:20:38.000000 luma_ml-0.9.1/luma/ensemble/forest.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    14109 2024-05-13 12:31:18.000000 luma_ml-0.9.1/luma/ensemble/stack.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6779 2024-05-13 12:36:00.000000 luma_ml-0.9.1/luma/ensemble/vote.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.798700 luma_ml-0.9.1/luma/interface/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1294 2024-05-13 12:36:06.000000 luma_ml-0.9.1/luma/interface/exception.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7413 2024-05-17 07:30:53.000000 luma_ml-0.9.1/luma/interface/typing.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    16347 2024-05-27 18:40:22.000000 luma_ml-0.9.1/luma/interface/util.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.799766 luma_ml-0.9.1/luma/metric/
+-rw-r--r--   0 chanlee    (501) staff       (20)     1654 2024-04-24 15:30:21.000000 luma_ml-0.9.1/luma/metric/classification.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5917 2024-05-13 15:46:55.000000 luma_ml-0.9.1/luma/metric/clustering.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1788 2024-05-13 15:46:57.000000 luma_ml-0.9.1/luma/metric/distance.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1842 2024-05-13 15:46:59.000000 luma_ml-0.9.1/luma/metric/regression.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.800031 luma_ml-0.9.1/luma/migrate/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3764 2024-05-13 16:18:47.000000 luma_ml-0.9.1/luma/migrate/port.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.801104 luma_ml-0.9.1/luma/model_selection/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3438 2024-05-13 16:20:58.000000 luma_ml-0.9.1/luma/model_selection/cv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8041 2024-05-13 16:29:29.000000 luma_ml-0.9.1/luma/model_selection/fold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12244 2024-05-13 16:35:00.000000 luma_ml-0.9.1/luma/model_selection/search.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5736 2024-05-13 16:40:23.000000 luma_ml-0.9.1/luma/model_selection/split.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.804600 luma_ml-0.9.1/luma/neural/
+-rw-r--r--   0 chanlee    (501) staff       (20)      446 2024-06-01 18:11:10.000000 luma_ml-0.9.1/luma/neural/__init__.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.806555 luma_ml-0.9.1/luma/neural/_layers/
+-rw-r--r--   0 chanlee    (501) staff       (20)     6748 2024-06-01 17:44:37.000000 luma_ml-0.9.1/luma/neural/_layers/_act.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    19314 2024-06-01 18:06:53.000000 luma_ml-0.9.1/luma/neural/_layers/_conv.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     4144 2024-05-23 16:58:05.000000 luma_ml-0.9.1/luma/neural/_layers/_drop.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2313 2024-05-12 09:17:05.000000 luma_ml-0.9.1/luma/neural/_layers/_linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    10790 2024-05-30 19:49:07.000000 luma_ml-0.9.1/luma/neural/_layers/_norm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    29777 2024-05-26 11:24:51.000000 luma_ml-0.9.1/luma/neural/_layers/_pool.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.808437 luma_ml-0.9.1/luma/neural/_models/
+-rw-r--r--   0 chanlee    (501) staff       (20)    13097 2024-05-29 08:01:04.000000 luma_ml-0.9.1/luma/neural/_models/_alex.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    13040 2024-05-30 19:37:12.000000 luma_ml-0.9.1/luma/neural/_models/_inception.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12760 2024-05-29 08:01:42.000000 luma_ml-0.9.1/luma/neural/_models/_lenet.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     9639 2024-05-29 08:00:44.000000 luma_ml-0.9.1/luma/neural/_models/_simple.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    23952 2024-05-29 08:01:18.000000 luma_ml-0.9.1/luma/neural/_models/_vgg.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12024 2024-05-29 08:04:38.000000 luma_ml-0.9.1/luma/neural/base.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    54303 2024-05-30 20:01:17.000000 luma_ml-0.9.1/luma/neural/block.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     1319 2024-05-09 19:24:30.000000 luma_ml-0.9.1/luma/neural/init.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    34300 2024-05-30 19:15:29.000000 luma_ml-0.9.1/luma/neural/layer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3111 2024-05-13 19:10:16.000000 luma_ml-0.9.1/luma/neural/loss.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    49671 2024-06-01 12:12:52.000000 luma_ml-0.9.1/luma/neural/network.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    21132 2024-05-09 17:12:02.000000 luma_ml-0.9.1/luma/neural/optimizer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     8582 2024-05-13 19:27:55.000000 luma_ml-0.9.1/luma/neural/single.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.808886 luma_ml-0.9.1/luma/pipe/
+-rw-r--r--   0 chanlee    (501) staff       (20)     7308 2024-05-13 19:32:18.000000 luma_ml-0.9.1/luma/pipe/pipeline.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.810137 luma_ml-0.9.1/luma/preprocessing/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5295 2024-04-21 11:36:14.000000 luma_ml-0.9.1/luma/preprocessing/encoder.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     5533 2024-04-21 11:36:15.000000 luma_ml-0.9.1/luma/preprocessing/imputer.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3653 2024-05-13 19:32:35.000000 luma_ml-0.9.1/luma/preprocessing/outlier.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     2624 2024-05-13 19:33:29.000000 luma_ml-0.9.1/luma/preprocessing/scaler.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.811163 luma_ml-0.9.1/luma/reduction/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19163 2024-05-26 19:19:09.000000 luma_ml-0.9.1/luma/reduction/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    40387 2024-05-13 19:55:48.000000 luma_ml-0.9.1/luma/reduction/manifold.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    17019 2024-05-14 09:45:27.000000 luma_ml-0.9.1/luma/reduction/selection.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.813326 luma_ml-0.9.1/luma/regressor/
+-rw-r--r--   0 chanlee    (501) staff       (20)    19882 2024-05-14 09:56:22.000000 luma_ml-0.9.1/luma/regressor/general.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    12687 2024-05-14 10:03:42.000000 luma_ml-0.9.1/luma/regressor/linear.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     6755 2024-05-14 10:04:13.000000 luma_ml-0.9.1/luma/regressor/neighbors.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     3098 2024-05-14 10:05:44.000000 luma_ml-0.9.1/luma/regressor/poly.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    11070 2024-05-14 14:33:09.000000 luma_ml-0.9.1/luma/regressor/robust.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7805 2024-05-14 14:45:46.000000 luma_ml-0.9.1/luma/regressor/svm.py
+-rw-r--r--   0 chanlee    (501) staff       (20)     7415 2024-05-14 14:59:17.000000 luma_ml-0.9.1/luma/regressor/tree.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.814126 luma_ml-0.9.1/luma/visual/
+-rw-r--r--   0 chanlee    (501) staff       (20)     3045 2024-04-13 08:30:32.000000 luma_ml-0.9.1/luma/visual/eda.py
+-rw-r--r--   0 chanlee    (501) staff       (20)    25027 2024-05-23 17:04:49.000000 luma_ml-0.9.1/luma/visual/eval.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.816481 luma_ml-0.9.1/luma_ml.egg-info/
+-rw-r--r--   0 chanlee    (501) staff       (20)     5580 2024-06-01 18:13:49.000000 luma_ml-0.9.1/luma_ml.egg-info/PKG-INFO
+-rw-r--r--   0 chanlee    (501) staff       (20)     2024 2024-06-01 18:13:49.000000 luma_ml-0.9.1/luma_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)        1 2024-06-01 18:13:49.000000 luma_ml-0.9.1/luma_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       43 2024-06-01 18:13:49.000000 luma_ml-0.9.1/luma_ml.egg-info/requires.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       17 2024-06-01 18:13:49.000000 luma_ml-0.9.1/luma_ml.egg-info/top_level.txt
+-rw-r--r--   0 chanlee    (501) staff       (20)       38 2024-06-01 18:13:49.817273 luma_ml-0.9.1/setup.cfg
+-rw-r--r--   0 chanlee    (501) staff       (20)      803 2024-06-01 18:13:13.000000 luma_ml-0.9.1/setup.py
+drwxr-xr-x   0 chanlee    (501) staff       (20)        0 2024-06-01 18:13:49.816063 luma_ml-0.9.1/test/
+-rw-r--r--   0 chanlee    (501) staff       (20)      647 2024-04-29 02:58:00.000000 luma_ml-0.9.1/test/__act.py
+-rw-r--r--   0 chanlee    (501) staff       (20)      429 2024-05-18 16:19:55.000000 luma_ml-0.9.1/test/__test.py
```

### Comparing `luma-ml-0.9.0/LICENSE` & `luma_ml-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/PKG-INFO` & `luma_ml-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
+Requires-Dist: rich
 
 <!DOCTYPE html>
 <html>
     <body>
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
@@ -120,15 +121,15 @@
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
-                    <td>NumPy, SciPy, Pandas, Matplotlib, Seaborn</td>
+                    <td>NumPy, SciPy, Pandas, Matplotlib, Seaborn, Rich</td>
                 </tr>
                 <tr>
                     <td>Documentation</td>
                     <td>
                         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">LUMA Notion Document</a>
                     </td>
                 </tr>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.9.0 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.9.1 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
-Requires-Dist: seaborn
+Requires-Dist: seaborn Requires-Dist: rich
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
 6.41k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
@@ -36,9 +36,9 @@
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
 Latest Version 0.9.0
 Lines of Code  ~26.5K
 Requirement    Python 3.12 or later
-Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
+Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn, Rich
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.9.0/README.md` & `luma_ml-0.9.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
-                    <td>NumPy, SciPy, Pandas, Matplotlib, Seaborn</td>
+                    <td>NumPy, SciPy, Pandas, Matplotlib, Seaborn, Rich</td>
                 </tr>
                 <tr>
                     <td>Documentation</td>
                     <td>
                         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">LUMA Notion Document</a>
                     </td>
                 </tr>
```

#### html2text {}

```diff
@@ -27,9 +27,9 @@
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
 Latest Version 0.9.0
 Lines of Code  ~26.5K
 Requirement    Python 3.12 or later
-Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
+Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn, Rich
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.9.0/luma/__import__.py` & `luma_ml-0.9.1/luma/__import__.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/__init__.py` & `luma_ml-0.9.1/luma/__init__.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/classifier/discriminant.py` & `luma_ml-0.9.1/luma/classifier/discriminant.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/classifier/logistic.py` & `luma_ml-0.9.1/luma/classifier/logistic.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/classifier/naive_bayes.py` & `luma_ml-0.9.1/luma/classifier/naive_bayes.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/classifier/neighbors.py` & `luma_ml-0.9.1/luma/classifier/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/classifier/svm.py` & `luma_ml-0.9.1/luma/classifier/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/classifier/tree.py` & `luma_ml-0.9.1/luma/classifier/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/clustering/affinity.py` & `luma_ml-0.9.1/luma/clustering/affinity.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/clustering/density.py` & `luma_ml-0.9.1/luma/clustering/density.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/clustering/hierarchy.py` & `luma_ml-0.9.1/luma/clustering/hierarchy.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/clustering/kmeans.py` & `luma_ml-0.9.1/luma/clustering/kmeans.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/clustering/mixture.py` & `luma_ml-0.9.1/luma/clustering/mixture.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/clustering/spectral.py` & `luma_ml-0.9.1/luma/clustering/spectral.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/core/base.py` & `luma_ml-0.9.1/luma/core/base.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/core/super.py` & `luma_ml-0.9.1/luma/core/super.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/ensemble/bagging.py` & `luma_ml-0.9.1/luma/ensemble/bagging.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/ensemble/boost.py` & `luma_ml-0.9.1/luma/ensemble/boost.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/ensemble/forest.py` & `luma_ml-0.9.1/luma/ensemble/forest.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/ensemble/stack.py` & `luma_ml-0.9.1/luma/ensemble/stack.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/ensemble/vote.py` & `luma_ml-0.9.1/luma/ensemble/vote.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/interface/exception.py` & `luma_ml-0.9.1/luma/interface/exception.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/interface/typing.py` & `luma_ml-0.9.1/luma/interface/typing.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/interface/util.py` & `luma_ml-0.9.1/luma/interface/util.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/metric/classification.py` & `luma_ml-0.9.1/luma/metric/classification.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/metric/clustering.py` & `luma_ml-0.9.1/luma/metric/clustering.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/metric/distance.py` & `luma_ml-0.9.1/luma/metric/distance.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/metric/regression.py` & `luma_ml-0.9.1/luma/metric/regression.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/migrate/port.py` & `luma_ml-0.9.1/luma/migrate/port.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/model_selection/cv.py` & `luma_ml-0.9.1/luma/model_selection/cv.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/model_selection/fold.py` & `luma_ml-0.9.1/luma/model_selection/fold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/model_selection/search.py` & `luma_ml-0.9.1/luma/model_selection/search.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/model_selection/split.py` & `luma_ml-0.9.1/luma/model_selection/split.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/_layers/_act.py` & `luma_ml-0.9.1/luma/neural/_layers/_act.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/_layers/_conv.py` & `luma_ml-0.9.1/luma/neural/_layers/_conv.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/_layers/_drop.py` & `luma_ml-0.9.1/luma/neural/_layers/_drop.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/_layers/_linear.py` & `luma_ml-0.9.1/luma/neural/_layers/_linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/_layers/_norm.py` & `luma_ml-0.9.1/luma/neural/_layers/_norm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/_layers/_pool.py` & `luma_ml-0.9.1/luma/neural/_layers/_pool.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/_models/_alex.py` & `luma_ml-0.9.1/luma/neural/_models/_alex.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/_models/_inception.py` & `luma_ml-0.9.1/luma/neural/_models/_inception.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/_models/_lenet.py` & `luma_ml-0.9.1/luma/neural/_models/_lenet.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/_models/_simple.py` & `luma_ml-0.9.1/luma/neural/_models/_simple.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/_models/_vgg.py` & `luma_ml-0.9.1/luma/neural/_models/_vgg.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/base.py` & `luma_ml-0.9.1/luma/neural/base.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/block.py` & `luma_ml-0.9.1/luma/neural/block.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/init.py` & `luma_ml-0.9.1/luma/neural/init.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/layer.py` & `luma_ml-0.9.1/luma/neural/layer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/loss.py` & `luma_ml-0.9.1/luma/neural/loss.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/network.py` & `luma_ml-0.9.1/luma/neural/network.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/optimizer.py` & `luma_ml-0.9.1/luma/neural/optimizer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/neural/single.py` & `luma_ml-0.9.1/luma/neural/single.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/pipe/pipeline.py` & `luma_ml-0.9.1/luma/pipe/pipeline.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/preprocessing/encoder.py` & `luma_ml-0.9.1/luma/preprocessing/encoder.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/preprocessing/imputer.py` & `luma_ml-0.9.1/luma/preprocessing/imputer.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/preprocessing/outlier.py` & `luma_ml-0.9.1/luma/preprocessing/outlier.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/preprocessing/scaler.py` & `luma_ml-0.9.1/luma/preprocessing/scaler.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/reduction/linear.py` & `luma_ml-0.9.1/luma/reduction/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/reduction/manifold.py` & `luma_ml-0.9.1/luma/reduction/manifold.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/reduction/selection.py` & `luma_ml-0.9.1/luma/reduction/selection.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/regressor/general.py` & `luma_ml-0.9.1/luma/regressor/general.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/regressor/linear.py` & `luma_ml-0.9.1/luma/regressor/linear.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/regressor/neighbors.py` & `luma_ml-0.9.1/luma/regressor/neighbors.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/regressor/poly.py` & `luma_ml-0.9.1/luma/regressor/poly.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/regressor/robust.py` & `luma_ml-0.9.1/luma/regressor/robust.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/regressor/svm.py` & `luma_ml-0.9.1/luma/regressor/svm.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/regressor/tree.py` & `luma_ml-0.9.1/luma/regressor/tree.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/visual/eda.py` & `luma_ml-0.9.1/luma/visual/eda.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma/visual/eval.py` & `luma_ml-0.9.1/luma/visual/eval.py`

 * *Files identical despite different names*

### Comparing `luma-ml-0.9.0/luma_ml.egg-info/PKG-INFO` & `luma_ml-0.9.1/luma_ml.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luma-ml
-Version: 0.9.0
+Version: 0.9.1
 Summary: A Comprehensive Python Module for Machine Learning and Data Science
 Home-page: https://github.com/ChanLumerico/luma
 Author: ChanLumerico
 Author-email: greensox284@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
@@ -12,14 +12,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: pandas
 Requires-Dist: matplotlib
 Requires-Dist: seaborn
+Requires-Dist: rich
 
 <!DOCTYPE html>
 <html>
     <body>
         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">
             <img src="https://github.com/ChanLumerico/luma/raw/main/others/luma.png" alt="logo" width="75" height="75">
         </a>
@@ -120,15 +121,15 @@
                 </tr>
                 <tr>
                     <td>Requirement</td>
                     <td>Python 3.12 or later</td>
                 </tr>
                 <tr>
                     <td>Dependencies</td>
-                    <td>NumPy, SciPy, Pandas, Matplotlib, Seaborn</td>
+                    <td>NumPy, SciPy, Pandas, Matplotlib, Seaborn, Rich</td>
                 </tr>
                 <tr>
                     <td>Documentation</td>
                     <td>
                         <a href="https://lumerico284.notion.site/LUMA-a467e4a9e885498f87b49c952d0abecd?pvs=74">LUMA Notion Document</a>
                     </td>
                 </tr>
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: luma-ml Version: 0.9.0 Summary: A Comprehensive
+Metadata-Version: 2.1 Name: luma-ml Version: 0.9.1 Summary: A Comprehensive
 Python Module for Machine Learning and Data Science Home-page: https://
 github.com/ChanLumerico/luma Author: ChanLumerico Author-email:
 greensox284@gmail.com Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent Requires-Python: >=3.12
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 numpy Requires-Dist: scipy Requires-Dist: pandas Requires-Dist: matplotlib
-Requires-Dist: seaborn
+Requires-Dist: seaborn Requires-Dist: rich
 _[_l_o_g_o_]
 ************ LLUUMMAA ************
 A Comprehensive Python Module for Machine Learning and Data Science
 [pypi-version][pypi-downloads][https://img.shields.io/badge/total downloads-
 6.41k-red][GitHub code size in bytes][Code Style]
 ******** SSuubbmmoodduulleess ********
 NNaammee                 DDeessccrriippttiioonn
@@ -36,9 +36,9 @@
 luma.visual          Tools for model visualization and data plotting.
 ******** SSttrruuccttuurree ********
 [structure]
 ******** OOtthheerrss ********
 Latest Version 0.9.0
 Lines of Code  ~26.5K
 Requirement    Python 3.12 or later
-Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn
+Dependencies   NumPy, SciPy, Pandas, Matplotlib, Seaborn, Rich
 Documentation  _L_U_M_A_ _N_o_t_i_o_n_ _D_o_c_u_m_e_n_t
```

### Comparing `luma-ml-0.9.0/luma_ml.egg-info/SOURCES.txt` & `luma_ml-0.9.1/luma_ml.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 luma/metric/distance.py
 luma/metric/regression.py
 luma/migrate/port.py
 luma/model_selection/cv.py
 luma/model_selection/fold.py
 luma/model_selection/search.py
 luma/model_selection/split.py
+luma/neural/__init__.py
 luma/neural/base.py
 luma/neural/block.py
 luma/neural/init.py
 luma/neural/layer.py
 luma/neural/loss.py
 luma/neural/network.py
 luma/neural/optimizer.py
```

### Comparing `luma-ml-0.9.0/setup.py` & `luma_ml-0.9.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,29 +2,23 @@
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="luma-ml",
-    version="0.9.0",
+    version="0.9.1",
     author="ChanLumerico",
     author_email="greensox284@gmail.com",
     description="A Comprehensive Python Module for Machine Learning and Data Science",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ChanLumerico/luma",
     packages=setuptools.find_namespace_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.12",
-    install_requires=[
-        "numpy",
-        "scipy",
-        "pandas",
-        "matplotlib",
-        "seaborn",
-    ],
+    install_requires=["numpy", "scipy", "pandas", "matplotlib", "seaborn", "rich"],
 )
```

### Comparing `luma-ml-0.9.0/test/__act.py` & `luma_ml-0.9.1/test/__act.py`

 * *Files identical despite different names*

