# Comparing `tmp/pyod-1.1.3.tar.gz` & `tmp/pyod-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyod-1.1.3.tar", last modified: Fri Feb  9 06:49:55 2024, max compression
+gzip compressed data, was "pyod-2.0.0.tar", last modified: Sat Jun  1 07:33:26 2024, max compression
```

## Comparing `pyod-1.1.3.tar` & `pyod-2.0.0.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxrwxrwx   0        0        0        0 2024-02-09 06:49:55.089030 pyod-1.1.3/
--rw-rw-rw-   0        0        0     1313 2024-02-09 06:49:24.000000 pyod-1.1.3/LICENSE
--rw-rw-rw-   0        0        0      106 2024-02-09 06:49:24.000000 pyod-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0    51702 2024-02-09 06:49:55.089030 pyod-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    49769 2024-02-09 06:49:24.000000 pyod-1.1.3/README.rst
-drwxrwxrwx   0        0        0        0 2024-02-09 06:49:55.002911 pyod-1.1.3/pyod/
--rw-rw-rw-   0        0        0      134 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-09 06:49:55.078517 pyod-1.1.3/pyod/models/
--rw-rw-rw-   0        0        0      701 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/__init__.py
--rw-rw-rw-   0        0        0     9918 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/abod.py
--rw-rw-rw-   0        0        0    24031 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/alad.py
--rw-rw-rw-   0        0        0    16485 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/anogan.py
--rw-rw-rw-   0        0        0    11087 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/auto_encoder.py
--rw-rw-rw-   0        0        0    15366 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/auto_encoder_torch.py
--rw-rw-rw-   0        0        0    20721 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/base.py
--rw-rw-rw-   0        0        0      720 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/base_dl.py
--rw-rw-rw-   0        0        0    13423 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/cblof.py
--rw-rw-rw-   0        0        0     5879 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/cd.py
--rw-rw-rw-   0        0        0     8614 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/cof.py
--rw-rw-rw-   0        0        0     5717 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/combination.py
--rw-rw-rw-   0        0        0    10364 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/copod.py
--rw-rw-rw-   0        0        0    12159 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/deep_svdd.py
--rw-rw-rw-   0        0        0    14003 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/dif.py
--rw-rw-rw-   0        0        0    10493 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/ecod.py
--rw-rw-rw-   0        0        0    15681 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/feature_bagging.py
--rw-rw-rw-   0        0        0     2574 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/gaal_base.py
--rw-rw-rw-   0        0        0     9512 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/gmm.py
--rw-rw-rw-   0        0        0    13758 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/hbos.py
--rw-rw-rw-   0        0        0    11604 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/iforest.py
--rw-rw-rw-   0        0        0     9494 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/inne.py
--rw-rw-rw-   0        0        0     6322 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/kde.py
--rw-rw-rw-   0        0        0    10540 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/knn.py
--rw-rw-rw-   0        0        0    14175 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/kpca.py
--rw-rw-rw-   0        0        0     8285 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/lmdd.py
--rw-rw-rw-   0        0        0     8167 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/loci.py
--rw-rw-rw-   0        0        0     7918 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/loda.py
--rw-rw-rw-   0        0        0     9250 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/lof.py
--rw-rw-rw-   0        0        0    15690 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/lscp.py
--rw-rw-rw-   0        0        0    12627 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/lunar.py
--rw-rw-rw-   0        0        0     5245 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/mad.py
--rw-rw-rw-   0        0        0     8595 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/models/mcd.py
--rw-rw-rw-   0        0        0    10785 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/models/mo_gaal.py
--rw-rw-rw-   0        0        0     8352 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/models/ocsvm.py
--rw-rw-rw-   0        0        0    14866 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/models/pca.py
--rw-rw-rw-   0        0        0     5191 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/models/qmcd.py
--rw-rw-rw-   0        0        0    23604 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/models/rgraph.py
--rw-rw-rw-   0        0        0    16659 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/models/rod.py
--rw-rw-rw-   0        0        0     6805 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/models/sampling.py
--rw-rw-rw-   0        0        0     3621 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/models/sklearn_base.py
--rw-rw-rw-   0        0        0     7670 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/models/so_gaal.py
--rw-rw-rw-   0        0        0     7024 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/models/sod.py
--rw-rw-rw-   0        0        0    10383 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/models/sos.py
--rw-rw-rw-   0        0        0    10197 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/models/suod.py
--rw-rw-rw-   0        0        0    24352 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/models/thresholds.py
--rw-rw-rw-   0        0        0    14081 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/models/vae.py
--rw-rw-rw-   0        0        0    16394 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/models/xgbod.py
-drwxrwxrwx   0        0        0        0 2024-02-09 06:49:55.087030 pyod-1.1.3/pyod/utils/
--rw-rw-rw-   0        0        0      884 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/utils/__init__.py
--rw-rw-rw-   0        0        0    23674 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/utils/data.py
--rw-rw-rw-   0        0        0     6685 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/utils/example.py
--rw-rw-rw-   0        0        0     7630 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/utils/stat_models.py
--rw-rw-rw-   0        0        0      319 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/utils/torch_utility.py
--rw-rw-rw-   0        0        0    17117 2024-02-09 06:49:27.000000 pyod-1.1.3/pyod/utils/utility.py
--rw-rw-rw-   0        0        0      579 2024-02-09 06:49:26.000000 pyod-1.1.3/pyod/version.py
-drwxrwxrwx   0        0        0        0 2024-02-09 06:49:55.009916 pyod-1.1.3/pyod.egg-info/
--rw-rw-rw-   0        0        0    51702 2024-02-09 06:49:54.000000 pyod-1.1.3/pyod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1416 2024-02-09 06:49:54.000000 pyod-1.1.3/pyod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-09 06:49:54.000000 pyod-1.1.3/pyod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       80 2024-02-09 06:49:54.000000 pyod-1.1.3/pyod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2024-02-09 06:49:54.000000 pyod-1.1.3/pyod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       79 2024-02-09 06:49:24.000000 pyod-1.1.3/requirements.txt
--rw-rw-rw-   0        0        0       87 2024-02-09 06:49:55.090030 pyod-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     2076 2024-02-09 06:49:24.000000 pyod-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:33:26.942616 pyod-2.0.0/
+-rw-rw-rw-   0        0        0     1313 2024-06-01 07:33:01.000000 pyod-2.0.0/LICENSE
+-rw-rw-rw-   0        0        0      106 2024-06-01 07:33:02.000000 pyod-2.0.0/MANIFEST.in
+-rw-rw-rw-   0        0        0    50018 2024-06-01 07:33:26.943448 pyod-2.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0    48123 2024-06-01 07:33:01.000000 pyod-2.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2024-06-01 07:33:26.783602 pyod-2.0.0/pyod/
+-rw-rw-rw-   0        0        0      134 2024-06-01 07:33:18.000000 pyod-2.0.0/pyod/__init__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:33:26.929527 pyod-2.0.0/pyod/models/
+-rw-rw-rw-   0        0        0      701 2024-06-01 07:33:18.000000 pyod-2.0.0/pyod/models/__init__.py
+-rw-rw-rw-   0        0        0     9918 2024-06-01 07:33:18.000000 pyod-2.0.0/pyod/models/abod.py
+-rw-rw-rw-   0        0        0    24031 2024-06-01 07:33:18.000000 pyod-2.0.0/pyod/models/alad.py
+-rw-rw-rw-   0        0        0    16485 2024-06-01 07:33:18.000000 pyod-2.0.0/pyod/models/anogan.py
+-rw-rw-rw-   0        0        0    11087 2024-06-01 07:33:18.000000 pyod-2.0.0/pyod/models/auto_encoder.py
+-rw-rw-rw-   0        0        0    15366 2024-06-01 07:33:18.000000 pyod-2.0.0/pyod/models/auto_encoder_torch.py
+-rw-rw-rw-   0        0        0    20578 2024-06-01 07:33:18.000000 pyod-2.0.0/pyod/models/base.py
+-rw-rw-rw-   0        0        0    11464 2024-06-01 07:33:19.000000 pyod-2.0.0/pyod/models/base_dl.py
+-rw-rw-rw-   0        0        0    13423 2024-06-01 07:33:19.000000 pyod-2.0.0/pyod/models/cblof.py
+-rw-rw-rw-   0        0        0     5879 2024-06-01 07:33:19.000000 pyod-2.0.0/pyod/models/cd.py
+-rw-rw-rw-   0        0        0     8614 2024-06-01 07:33:19.000000 pyod-2.0.0/pyod/models/cof.py
+-rw-rw-rw-   0        0        0     5717 2024-06-01 07:33:19.000000 pyod-2.0.0/pyod/models/combination.py
+-rw-rw-rw-   0        0        0    10364 2024-06-01 07:33:19.000000 pyod-2.0.0/pyod/models/copod.py
+-rw-rw-rw-   0        0        0    12159 2024-06-01 07:33:19.000000 pyod-2.0.0/pyod/models/deep_svdd.py
+-rw-rw-rw-   0        0        0    14003 2024-06-01 07:33:19.000000 pyod-2.0.0/pyod/models/dif.py
+-rw-rw-rw-   0        0        0    10493 2024-06-01 07:33:19.000000 pyod-2.0.0/pyod/models/ecod.py
+-rw-rw-rw-   0        0        0    15681 2024-06-01 07:33:19.000000 pyod-2.0.0/pyod/models/feature_bagging.py
+-rw-rw-rw-   0        0        0     2574 2024-06-01 07:33:19.000000 pyod-2.0.0/pyod/models/gaal_base.py
+-rw-rw-rw-   0        0        0     9512 2024-06-01 07:33:19.000000 pyod-2.0.0/pyod/models/gmm.py
+-rw-rw-rw-   0        0        0    13758 2024-06-01 07:33:19.000000 pyod-2.0.0/pyod/models/hbos.py
+-rw-rw-rw-   0        0        0    11604 2024-06-01 07:33:20.000000 pyod-2.0.0/pyod/models/iforest.py
+-rw-rw-rw-   0        0        0     9494 2024-06-01 07:33:20.000000 pyod-2.0.0/pyod/models/inne.py
+-rw-rw-rw-   0        0        0     6322 2024-06-01 07:33:20.000000 pyod-2.0.0/pyod/models/kde.py
+-rw-rw-rw-   0        0        0    10540 2024-06-01 07:33:20.000000 pyod-2.0.0/pyod/models/knn.py
+-rw-rw-rw-   0        0        0    14175 2024-06-01 07:33:20.000000 pyod-2.0.0/pyod/models/kpca.py
+-rw-rw-rw-   0        0        0     8285 2024-06-01 07:33:20.000000 pyod-2.0.0/pyod/models/lmdd.py
+-rw-rw-rw-   0        0        0     8167 2024-06-01 07:33:20.000000 pyod-2.0.0/pyod/models/loci.py
+-rw-rw-rw-   0        0        0     7918 2024-06-01 07:33:20.000000 pyod-2.0.0/pyod/models/loda.py
+-rw-rw-rw-   0        0        0     9250 2024-06-01 07:33:20.000000 pyod-2.0.0/pyod/models/lof.py
+-rw-rw-rw-   0        0        0    15690 2024-06-01 07:33:20.000000 pyod-2.0.0/pyod/models/lscp.py
+-rw-rw-rw-   0        0        0    12627 2024-06-01 07:33:20.000000 pyod-2.0.0/pyod/models/lunar.py
+-rw-rw-rw-   0        0        0     5245 2024-06-01 07:33:20.000000 pyod-2.0.0/pyod/models/mad.py
+-rw-rw-rw-   0        0        0     8595 2024-06-01 07:33:20.000000 pyod-2.0.0/pyod/models/mcd.py
+-rw-rw-rw-   0        0        0    10785 2024-06-01 07:33:20.000000 pyod-2.0.0/pyod/models/mo_gaal.py
+-rw-rw-rw-   0        0        0     8352 2024-06-01 07:33:20.000000 pyod-2.0.0/pyod/models/ocsvm.py
+-rw-rw-rw-   0        0        0    14866 2024-06-01 07:33:21.000000 pyod-2.0.0/pyod/models/pca.py
+-rw-rw-rw-   0        0        0     5191 2024-06-01 07:33:21.000000 pyod-2.0.0/pyod/models/qmcd.py
+-rw-rw-rw-   0        0        0    23604 2024-06-01 07:33:21.000000 pyod-2.0.0/pyod/models/rgraph.py
+-rw-rw-rw-   0        0        0    16659 2024-06-01 07:33:21.000000 pyod-2.0.0/pyod/models/rod.py
+-rw-rw-rw-   0        0        0     6805 2024-06-01 07:33:21.000000 pyod-2.0.0/pyod/models/sampling.py
+-rw-rw-rw-   0        0        0     3602 2024-06-01 07:33:21.000000 pyod-2.0.0/pyod/models/sklearn_base.py
+-rw-rw-rw-   0        0        0     8082 2024-06-01 07:33:21.000000 pyod-2.0.0/pyod/models/so_gaal.py
+-rw-rw-rw-   0        0        0     7024 2024-06-01 07:33:21.000000 pyod-2.0.0/pyod/models/sod.py
+-rw-rw-rw-   0        0        0    10383 2024-06-01 07:33:21.000000 pyod-2.0.0/pyod/models/sos.py
+-rw-rw-rw-   0        0        0    10197 2024-06-01 07:33:21.000000 pyod-2.0.0/pyod/models/suod.py
+-rw-rw-rw-   0        0        0    24352 2024-06-01 07:33:21.000000 pyod-2.0.0/pyod/models/thresholds.py
+-rw-rw-rw-   0        0        0    14081 2024-06-01 07:33:21.000000 pyod-2.0.0/pyod/models/vae.py
+-rw-rw-rw-   0        0        0    16394 2024-06-01 07:33:21.000000 pyod-2.0.0/pyod/models/xgbod.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:33:26.940361 pyod-2.0.0/pyod/utils/
+-rw-rw-rw-   0        0        0      884 2024-06-01 07:33:18.000000 pyod-2.0.0/pyod/utils/__init__.py
+-rw-rw-rw-   0        0        0    23674 2024-06-01 07:33:26.000000 pyod-2.0.0/pyod/utils/data.py
+-rw-rw-rw-   0        0        0     6685 2024-06-01 07:33:26.000000 pyod-2.0.0/pyod/utils/example.py
+-rw-rw-rw-   0        0        0     7630 2024-06-01 07:33:26.000000 pyod-2.0.0/pyod/utils/stat_models.py
+-rw-rw-rw-   0        0        0    18247 2024-06-01 07:33:26.000000 pyod-2.0.0/pyod/utils/torch_utility.py
+-rw-rw-rw-   0        0        0    17117 2024-06-01 07:33:26.000000 pyod-2.0.0/pyod/utils/utility.py
+-rw-rw-rw-   0        0        0      579 2024-06-01 07:33:18.000000 pyod-2.0.0/pyod/version.py
+drwxrwxrwx   0        0        0        0 2024-06-01 07:33:26.797488 pyod-2.0.0/pyod.egg-info/
+-rw-rw-rw-   0        0        0    50018 2024-06-01 07:33:18.000000 pyod-2.0.0/pyod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1416 2024-06-01 07:33:26.000000 pyod-2.0.0/pyod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 07:33:18.000000 pyod-2.0.0/pyod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2024-06-01 07:33:18.000000 pyod-2.0.0/pyod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2024-06-01 07:33:18.000000 pyod-2.0.0/pyod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       75 2024-06-01 07:33:01.000000 pyod-2.0.0/requirements.txt
+-rw-rw-rw-   0        0        0       87 2024-06-01 07:33:26.943448 pyod-2.0.0/setup.cfg
+-rw-rw-rw-   0        0        0     2076 2024-06-01 07:33:17.000000 pyod-2.0.0/setup.py
```

### Comparing `pyod-1.1.3/LICENSE` & `pyod-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/PKG-INFO` & `pyod-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyod
-Version: 1.1.3
+Version: 2.0.0
 Summary: A Comprehensive and Scalable Python Library for Outlier Detection (Anomaly Detection)
 Home-page: https://github.com/yzhao062/pyod
 Author: Yue Zhao
 Author-email: yzhao062@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/yzhao062/pyod/archive/master.zip
 Keywords: outlier detection,anomaly detection,outlier ensembles,data mining,neural networks
@@ -27,63 +27,65 @@
 License-File: LICENSE
 
 Python Outlier Detection (PyOD)
 ===============================
 
 **Deployment & Documentation & Stats & License**
 
-.. image:: https://img.shields.io/pypi/v/pyod.svg?color=brightgreen
+|badge_pypi| |badge_anaconda| |badge_docs| |badge_stars| |badge_forks| |badge_downloads| |badge_testing| |badge_coverage| |badge_maintainability| |badge_license| |badge_benchmark|
+
+.. |badge_pypi| image:: https://img.shields.io/pypi/v/pyod.svg?color=brightgreen
    :target: https://pypi.org/project/pyod/
    :alt: PyPI version
 
 
-.. image:: https://anaconda.org/conda-forge/pyod/badges/version.svg
+.. |badge_anaconda| image:: https://anaconda.org/conda-forge/pyod/badges/version.svg
    :target: https://anaconda.org/conda-forge/pyod
    :alt: Anaconda version
 
 
-.. image:: https://readthedocs.org/projects/pyod/badge/?version=latest
+.. |badge_docs| image:: https://readthedocs.org/projects/pyod/badge/?version=latest
    :target: https://pyod.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation status
 
 
-.. image:: https://img.shields.io/github/stars/yzhao062/pyod.svg
+.. |badge_stars| image:: https://img.shields.io/github/stars/yzhao062/pyod.svg
    :target: https://github.com/yzhao062/pyod/stargazers
    :alt: GitHub stars
 
 
-.. image:: https://img.shields.io/github/forks/yzhao062/pyod.svg?color=blue
+.. |badge_forks| image:: https://img.shields.io/github/forks/yzhao062/pyod.svg?color=blue
    :target: https://github.com/yzhao062/pyod/network
    :alt: GitHub forks
 
 
-.. image:: https://pepy.tech/badge/pyod
+.. |badge_downloads| image:: https://pepy.tech/badge/pyod
    :target: https://pepy.tech/project/pyod
    :alt: Downloads
 
-.. image:: https://github.com/yzhao062/pyod/actions/workflows/testing.yml/badge.svg
+.. |badge_testing| image:: https://github.com/yzhao062/pyod/actions/workflows/testing.yml/badge.svg
    :target: https://github.com/yzhao062/pyod/actions/workflows/testing.yml
    :alt: testing
 
 
-.. image:: https://coveralls.io/repos/github/yzhao062/pyod/badge.svg
+.. |badge_coverage| image:: https://coveralls.io/repos/github/yzhao062/pyod/badge.svg
    :target: https://coveralls.io/github/yzhao062/pyod
    :alt: Coverage Status
 
 
-.. image:: https://api.codeclimate.com/v1/badges/bdc3d8d0454274c753c4/maintainability
+.. |badge_maintainability| image:: https://api.codeclimate.com/v1/badges/bdc3d8d0454274c753c4/maintainability
    :target: https://codeclimate.com/github/yzhao062/Pyod/maintainability
    :alt: Maintainability
 
 
-.. image:: https://img.shields.io/github/license/yzhao062/pyod.svg
+.. |badge_license| image:: https://img.shields.io/github/license/yzhao062/pyod.svg
    :target: https://github.com/yzhao062/pyod/blob/master/LICENSE
    :alt: License
 
-.. image:: https://img.shields.io/badge/ADBench-benchmark_results-pink
+.. |badge_benchmark| image:: https://img.shields.io/badge/ADBench-benchmark_results-pink
    :target: https://github.com/Minqi824/ADBench
    :alt: Benchmark
 
 
 -----
 
 
@@ -234,35 +236,30 @@
    cd pyod
    pip install .
 
 
 **Required Dependencies**\ :
 
 
-* Python 3.6 or higher
+* Python 3.8 or higher
 * joblib
 * matplotlib
 * numpy>=1.19
 * numba>=0.51
 * scipy>=1.5.1
 * scikit_learn>=0.22.0
-* six
 
 
 **Optional Dependencies (see details below)**\ :
 
 * combo (optional, required for models/combination.py and FeatureBagging)
 * keras/tensorflow (optional, required for AutoEncoder, and other deep learning models)
 * suod (optional, required for running SUOD model)
 * xgboost (optional, required for XGBOD)
-* pythresh (optional, required for thresholding)
-
-**Warning**\ :
-PyOD includes several neural network-based models, such as AutoEncoders, implemented in Tensorflow and PyTorch. These deep learning libraries are not automatically installed by PyOD to avoid conflicts with existing installations. If you plan to use neural-net based models, please ensure these libraries are installed. See the `neural-net FAQ <https://github.com/yzhao062/pyod/wiki/Setting-up-Keras-and-Tensorflow-for-Neural-net-Based-models>`_ for guidance. Additionally, xgboost is not installed by default but is required for models like XGBOD.
-
+* pythresh (optional, required for thresholding)optional
 
 ----
 
 
 API Cheatsheet & Reference
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
@@ -591,49 +588,14 @@
 
 .. image:: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png
    :target: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png
    :alt: kNN example figure
 
 ----
 
-How to Contribute
-^^^^^^^^^^^^^^^^^
-
-You are welcome to contribute to this exciting project:
-
-
-* Please first check Issue lists for "help wanted" tag and comment the one
-  you are interested. We will assign the issue to you.
-
-* Fork the master branch and add your improvement/modification/fix.
-
-* Create a pull request to **development branch** and follow the pull request template `PR template <https://github.com/yzhao062/pyod/blob/master/PULL_REQUEST_TEMPLATE.md>`_
-
-* Automatic tests will be triggered. Make sure all tests are passed. Please make sure all added modules are accompanied with proper test functions.
-
-
-To make sure the code has the same style and standard, please refer to abod.py, hbos.py, or feature_bagging.py for example.
-
-You are also welcome to share your ideas by opening an issue or dropping me an email at zhaoy@cmu.edu :)
-
-
-Inclusion Criteria
-^^^^^^^^^^^^^^^^^^
-
-Similarly to `scikit-learn <https://scikit-learn.org/stable/faq.html#what-are-the-inclusion-criteria-for-new-algorithms>`_,
-We mainly consider well-established algorithms for inclusion.
-A rule of thumb is at least two years since publication, 50+ citations, and usefulness.
-
-However, we encourage the author(s) of newly proposed models to share and add your implementation into PyOD
-for boosting ML accessibility and reproducibility.
-This exception only applies if you could commit to the maintenance of your model for at least two year period.
-
-
-----
-
 Reference
 ^^^^^^^^^
 
 
 .. [#Aggarwal2015Outlier] Aggarwal, C.C., 2015. Outlier analysis. In Data mining (pp. 237-263). Springer, Cham.
 
 .. [#Aggarwal2015Theoretical] Aggarwal, C.C. and Sathe, S., 2015. Theoretical foundations and algorithms for outlier ensembles.\ *ACM SIGKDD Explorations Newsletter*\ , 17(1), pp.24-47.
```

### Comparing `pyod-1.1.3/README.rst` & `pyod-2.0.0/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,61 +1,63 @@
 Python Outlier Detection (PyOD)
 ===============================
 
 **Deployment & Documentation & Stats & License**
 
-.. image:: https://img.shields.io/pypi/v/pyod.svg?color=brightgreen
+|badge_pypi| |badge_anaconda| |badge_docs| |badge_stars| |badge_forks| |badge_downloads| |badge_testing| |badge_coverage| |badge_maintainability| |badge_license| |badge_benchmark|
+
+.. |badge_pypi| image:: https://img.shields.io/pypi/v/pyod.svg?color=brightgreen
    :target: https://pypi.org/project/pyod/
    :alt: PyPI version
 
 
-.. image:: https://anaconda.org/conda-forge/pyod/badges/version.svg
+.. |badge_anaconda| image:: https://anaconda.org/conda-forge/pyod/badges/version.svg
    :target: https://anaconda.org/conda-forge/pyod
    :alt: Anaconda version
 
 
-.. image:: https://readthedocs.org/projects/pyod/badge/?version=latest
+.. |badge_docs| image:: https://readthedocs.org/projects/pyod/badge/?version=latest
    :target: https://pyod.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation status
 
 
-.. image:: https://img.shields.io/github/stars/yzhao062/pyod.svg
+.. |badge_stars| image:: https://img.shields.io/github/stars/yzhao062/pyod.svg
    :target: https://github.com/yzhao062/pyod/stargazers
    :alt: GitHub stars
 
 
-.. image:: https://img.shields.io/github/forks/yzhao062/pyod.svg?color=blue
+.. |badge_forks| image:: https://img.shields.io/github/forks/yzhao062/pyod.svg?color=blue
    :target: https://github.com/yzhao062/pyod/network
    :alt: GitHub forks
 
 
-.. image:: https://pepy.tech/badge/pyod
+.. |badge_downloads| image:: https://pepy.tech/badge/pyod
    :target: https://pepy.tech/project/pyod
    :alt: Downloads
 
-.. image:: https://github.com/yzhao062/pyod/actions/workflows/testing.yml/badge.svg
+.. |badge_testing| image:: https://github.com/yzhao062/pyod/actions/workflows/testing.yml/badge.svg
    :target: https://github.com/yzhao062/pyod/actions/workflows/testing.yml
    :alt: testing
 
 
-.. image:: https://coveralls.io/repos/github/yzhao062/pyod/badge.svg
+.. |badge_coverage| image:: https://coveralls.io/repos/github/yzhao062/pyod/badge.svg
    :target: https://coveralls.io/github/yzhao062/pyod
    :alt: Coverage Status
 
 
-.. image:: https://api.codeclimate.com/v1/badges/bdc3d8d0454274c753c4/maintainability
+.. |badge_maintainability| image:: https://api.codeclimate.com/v1/badges/bdc3d8d0454274c753c4/maintainability
    :target: https://codeclimate.com/github/yzhao062/Pyod/maintainability
    :alt: Maintainability
 
 
-.. image:: https://img.shields.io/github/license/yzhao062/pyod.svg
+.. |badge_license| image:: https://img.shields.io/github/license/yzhao062/pyod.svg
    :target: https://github.com/yzhao062/pyod/blob/master/LICENSE
    :alt: License
 
-.. image:: https://img.shields.io/badge/ADBench-benchmark_results-pink
+.. |badge_benchmark| image:: https://img.shields.io/badge/ADBench-benchmark_results-pink
    :target: https://github.com/Minqi824/ADBench
    :alt: Benchmark
 
 
 -----
 
 
@@ -206,35 +208,30 @@
    cd pyod
    pip install .
 
 
 **Required Dependencies**\ :
 
 
-* Python 3.6 or higher
+* Python 3.8 or higher
 * joblib
 * matplotlib
 * numpy>=1.19
 * numba>=0.51
 * scipy>=1.5.1
 * scikit_learn>=0.22.0
-* six
 
 
 **Optional Dependencies (see details below)**\ :
 
 * combo (optional, required for models/combination.py and FeatureBagging)
 * keras/tensorflow (optional, required for AutoEncoder, and other deep learning models)
 * suod (optional, required for running SUOD model)
 * xgboost (optional, required for XGBOD)
-* pythresh (optional, required for thresholding)
-
-**Warning**\ :
-PyOD includes several neural network-based models, such as AutoEncoders, implemented in Tensorflow and PyTorch. These deep learning libraries are not automatically installed by PyOD to avoid conflicts with existing installations. If you plan to use neural-net based models, please ensure these libraries are installed. See the `neural-net FAQ <https://github.com/yzhao062/pyod/wiki/Setting-up-Keras-and-Tensorflow-for-Neural-net-Based-models>`_ for guidance. Additionally, xgboost is not installed by default but is required for models like XGBOD.
-
+* pythresh (optional, required for thresholding)optional
 
 ----
 
 
 API Cheatsheet & Reference
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
@@ -563,49 +560,14 @@
 
 .. image:: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png
    :target: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png
    :alt: kNN example figure
 
 ----
 
-How to Contribute
-^^^^^^^^^^^^^^^^^
-
-You are welcome to contribute to this exciting project:
-
-
-* Please first check Issue lists for "help wanted" tag and comment the one
-  you are interested. We will assign the issue to you.
-
-* Fork the master branch and add your improvement/modification/fix.
-
-* Create a pull request to **development branch** and follow the pull request template `PR template <https://github.com/yzhao062/pyod/blob/master/PULL_REQUEST_TEMPLATE.md>`_
-
-* Automatic tests will be triggered. Make sure all tests are passed. Please make sure all added modules are accompanied with proper test functions.
-
-
-To make sure the code has the same style and standard, please refer to abod.py, hbos.py, or feature_bagging.py for example.
-
-You are also welcome to share your ideas by opening an issue or dropping me an email at zhaoy@cmu.edu :)
-
-
-Inclusion Criteria
-^^^^^^^^^^^^^^^^^^
-
-Similarly to `scikit-learn <https://scikit-learn.org/stable/faq.html#what-are-the-inclusion-criteria-for-new-algorithms>`_,
-We mainly consider well-established algorithms for inclusion.
-A rule of thumb is at least two years since publication, 50+ citations, and usefulness.
-
-However, we encourage the author(s) of newly proposed models to share and add your implementation into PyOD
-for boosting ML accessibility and reproducibility.
-This exception only applies if you could commit to the maintenance of your model for at least two year period.
-
-
-----
-
 Reference
 ^^^^^^^^^
 
 
 .. [#Aggarwal2015Outlier] Aggarwal, C.C., 2015. Outlier analysis. In Data mining (pp. 237-263). Springer, Cham.
 
 .. [#Aggarwal2015Theoretical] Aggarwal, C.C. and Sathe, S., 2015. Theoretical foundations and algorithms for outlier ensembles.\ *ACM SIGKDD Explorations Newsletter*\ , 17(1), pp.24-47.
```

### Comparing `pyod-1.1.3/pyod/models/__init__.py` & `pyod-2.0.0/pyod/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/abod.py` & `pyod-2.0.0/pyod/models/abod.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/alad.py` & `pyod-2.0.0/pyod/models/alad.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/anogan.py` & `pyod-2.0.0/pyod/models/anogan.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/auto_encoder.py` & `pyod-2.0.0/pyod/models/auto_encoder.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/auto_encoder_torch.py` & `pyod-2.0.0/pyod/models/auto_encoder_torch.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/base.py` & `pyod-2.0.0/pyod/models/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,35 +9,30 @@
 
 import abc
 import warnings
 from collections import defaultdict
 from inspect import signature
 
 import numpy as np
-import six
 from numpy import percentile
 from scipy.special import erf
 from scipy.stats import binom
 from sklearn.metrics import roc_auc_score
 from sklearn.preprocessing import MinMaxScaler
 from sklearn.utils import deprecated
 from sklearn.utils.multiclass import check_classification_targets
 from sklearn.utils.validation import check_is_fitted
 
 from .sklearn_base import _pprint
 from ..utils.utility import precision_n_scores
 
 
-@six.add_metaclass(abc.ABCMeta)
-class BaseDetector(object):
+class BaseDetector(metaclass=abc.ABCMeta):
     """Abstract class for all outlier detection algorithms.
 
-    .. warning::
-    pyod would stop supporting Python 2 in the future. Consider move to
-    Python 3.5+.
 
     Parameters
     ----------
     contamination : float in (0., 0.5), optional (default=0.1)
         The amount of contamination of the data set,
         i.e. the proportion of outliers in the data set. Used when fitting to
         define the threshold on the decision function.
@@ -247,23 +242,23 @@
             raise ValueError(method,
                              'is not a valid probability conversion method')
 
     def predict_confidence(self, X):
         """Predict the model's confidence in making the same prediction
         under slightly different training sets.
         See :cite:`perini2020quantifying`.
-        
+
         Parameters
         -------
         X : numpy array of shape (n_samples, n_features)
             The input samples.
 
         Returns
         -------
-        confidence : numpy array of shape (n_samples,) 
+        confidence : numpy array of shape (n_samples,)
             For each observation, tells how consistently the model would
             make the same prediction if the training set was perturbed.
             Return a probability, ranging in [0,1].
 
         """
 
         check_is_fitted(self, ['decision_scores_', 'threshold_', 'labels_'])
```

### Comparing `pyod-1.1.3/pyod/models/cblof.py` & `pyod-2.0.0/pyod/models/cblof.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/cd.py` & `pyod-2.0.0/pyod/models/cd.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/cof.py` & `pyod-2.0.0/pyod/models/cof.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/combination.py` & `pyod-2.0.0/pyod/models/combination.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/copod.py` & `pyod-2.0.0/pyod/models/copod.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/deep_svdd.py` & `pyod-2.0.0/pyod/models/deep_svdd.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/dif.py` & `pyod-2.0.0/pyod/models/dif.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/ecod.py` & `pyod-2.0.0/pyod/models/ecod.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/feature_bagging.py` & `pyod-2.0.0/pyod/models/feature_bagging.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/gaal_base.py` & `pyod-2.0.0/pyod/models/gaal_base.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/gmm.py` & `pyod-2.0.0/pyod/models/gmm.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/hbos.py` & `pyod-2.0.0/pyod/models/hbos.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/iforest.py` & `pyod-2.0.0/pyod/models/iforest.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/inne.py` & `pyod-2.0.0/pyod/models/inne.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/kde.py` & `pyod-2.0.0/pyod/models/kde.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/knn.py` & `pyod-2.0.0/pyod/models/knn.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/kpca.py` & `pyod-2.0.0/pyod/models/kpca.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/lmdd.py` & `pyod-2.0.0/pyod/models/lmdd.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/loci.py` & `pyod-2.0.0/pyod/models/loci.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/loda.py` & `pyod-2.0.0/pyod/models/loda.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/lof.py` & `pyod-2.0.0/pyod/models/lof.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/lscp.py` & `pyod-2.0.0/pyod/models/lscp.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/lunar.py` & `pyod-2.0.0/pyod/models/lunar.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/mad.py` & `pyod-2.0.0/pyod/models/mad.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/mcd.py` & `pyod-2.0.0/pyod/models/mcd.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/mo_gaal.py` & `pyod-2.0.0/pyod/models/mo_gaal.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/ocsvm.py` & `pyod-2.0.0/pyod/models/ocsvm.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/pca.py` & `pyod-2.0.0/pyod/models/pca.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/qmcd.py` & `pyod-2.0.0/pyod/models/qmcd.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/rgraph.py` & `pyod-2.0.0/pyod/models/rgraph.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/rod.py` & `pyod-2.0.0/pyod/models/rod.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/sampling.py` & `pyod-2.0.0/pyod/models/sampling.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/sklearn_base.py` & `pyod-2.0.0/pyod/models/sklearn_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,18 +4,16 @@
 # Author: Yue Zhao <zhaoy@cmu.edu>
 # License: BSD 2 clause
 
 from __future__ import division
 from __future__ import print_function
 
 import numpy as np
-import six
 from joblib.parallel import cpu_count
 
-
 def _get_n_jobs(n_jobs):
     """Get number of jobs for the computation.
     See sklearn/utils/__init__.py for more information.
 
     This function reimplements the logic of joblib to determine the actual
     number of jobs depending on the cpu count. If -1 all CPUs are used.
     If 1 is given, no parallel computing code is used at all, which is useful
@@ -75,15 +73,15 @@
 
     # Do a multi-line justified repr:
     options = np.get_printoptions()
     np.set_printoptions(precision=5, threshold=64, edgeitems=2)
     params_list = list()
     this_line_length = offset
     line_sep = ',\n' + (1 + offset // 2) * ' '
-    for i, (k, v) in enumerate(sorted(six.iteritems(params))):
+    for i, (k, v) in enumerate(sorted(params.items())):
         if type(v) is float:
             # use str for representing floating point numbers
             # this way we get consistent representation across
             # architectures and versions.
             this_repr = '%s=%s' % (k, str(v))
         else:
             # use repr of the rest
```

### Comparing `pyod-1.1.3/pyod/models/so_gaal.py` & `pyod-2.0.0/pyod/models/so_gaal.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,56 @@
-# -*- coding: utf-8 -*-
 """Single-Objective Generative Adversarial Active Learning.
 Part of the codes are adapted from
 https://github.com/leibinghe/GAAL-based-outlier-detection
 """
-# Author: Winston Li <jk_zhengli@hotmail.com>
+# Author: Sihan Chen <schen976@usc.edu>
 # License: BSD 2 clause
 
-from __future__ import division
-from __future__ import print_function
-
+import math
 from collections import defaultdict
 
-import numpy as np
+import torch
+import torch.nn as nn
+import torch.nn.functional as F
+import torch.optim as optim
 from sklearn.utils import check_array
 from sklearn.utils.validation import check_is_fitted
+from torch.utils.data import DataLoader, TensorDataset
 
 from .base import BaseDetector
-from .base_dl import _get_tensorflow_version
-from .gaal_base import create_discriminator
-from .gaal_base import create_generator
-
-# if tensorflow 2, import from tf directly
-if _get_tensorflow_version() < 200:
-    from keras.layers import Input
-    from keras.models import Model
-    from keras.optimizers import SGD
-elif 200 <= _get_tensorflow_version() <= 209:
-    from tensorflow.keras.layers import Input
-    from tensorflow.keras.models import Model
-    from tensorflow.keras.optimizers import SGD
-else:
-    from tensorflow.keras.layers import Input
-    from tensorflow.keras.models import Model
-    from tensorflow.keras.optimizers.legacy import SGD
+
+
+class Generator(nn.Module):
+    def __init__(self, latent_size):
+        super(Generator, self).__init__()
+        self.layer1 = nn.Linear(latent_size, latent_size)
+        self.layer2 = nn.Linear(latent_size, latent_size)
+        nn.init.eye_(self.layer1.weight)
+        nn.init.eye_(self.layer2.weight)
+
+    def forward(self, x):
+        x = F.relu(self.layer1(x))
+        x = F.relu(self.layer2(x))
+        return x
+
+
+class Discriminator(nn.Module):
+    def __init__(self, latent_size, data_size):
+        super(Discriminator, self).__init__()
+        self.layer1 = nn.Linear(latent_size, math.ceil(math.sqrt(data_size)))
+        self.layer2 = nn.Linear(math.ceil(math.sqrt(data_size)), 1)
+        nn.init.kaiming_normal_(self.layer1.weight, mode='fan_in',
+                                nonlinearity='relu')
+        nn.init.kaiming_normal_(self.layer2.weight, mode='fan_in',
+                                nonlinearity='sigmoid')
+
+    def forward(self, x):
+        x = F.relu(self.layer1(x))
+        x = torch.sigmoid(self.layer2(x))
+        return x
 
 
 class SO_GAAL(BaseDetector):
     """Single-Objective Generative Adversarial Active Learning.
 
     SO-GAAL directly generates informative potential outliers to assist the
     classifier in describing a boundary that can separate outliers from normal
@@ -51,15 +65,16 @@
     ----------
     contamination : float in (0., 0.5), optional (default=0.1)
         The amount of contamination of the data set, i.e.
         the proportion of outliers in the data set. Used when fitting to
         define the threshold on the decision function.
 
     stop_epochs : int, optional (default=20)
-        The number of epochs of training. The number of total epochs equals to three times of stop_epochs.
+        The number of epochs of training. The number of total epochs equals to
+         three times of stop_epochs.
 
     lr_d : float, optional (default=0.01)
         The learn rate of the discriminator.
 
     lr_g : float, optional (default=0.0001)
         The learn rate of the generator.
 
@@ -81,15 +96,16 @@
 
     labels_ : int, either 0 or 1
         The binary labels of the training data. 0 stands for inliers
         and 1 for outliers/anomalies. It is generated by applying
         ``threshold_`` on ``decision_scores_``.
     """
 
-    def __init__(self, stop_epochs=20, lr_d=0.01, lr_g=0.0001, momentum=0.9, contamination=0.1):
+    def __init__(self, stop_epochs=20, lr_d=0.01, lr_g=0.0001, momentum=0.9,
+                 contamination=0.1):
         super(SO_GAAL, self).__init__(contamination=contamination)
         self.stop_epochs = stop_epochs
         self.lr_d = lr_d
         self.lr_g = lr_g
         self.momentum = momentum
 
     def fit(self, X, y=None):
@@ -112,73 +128,79 @@
         self._set_n_classes(y)
         latent_size = X.shape[1]
         data_size = X.shape[0]
         stop = 0
         epochs = self.stop_epochs * 3
         self.train_history = defaultdict(list)
 
-        self.discriminator = create_discriminator(latent_size, data_size)
-        self.discriminator.compile(
-            optimizer=SGD(lr=self.lr_d, momentum=self.momentum), loss='binary_crossentropy')
-
-        self.generator = create_generator(latent_size)
-        latent = Input(shape=(latent_size,))
-        fake = self.generator(latent)
-        self.discriminator.trainable = False
-        fake = self.discriminator(fake)
-        self.combine_model = Model(latent, fake)
-        self.combine_model.compile(
-            optimizer=SGD(lr=self.lr_g, momentum=self.momentum), loss='binary_crossentropy')
+        self.discriminator = Discriminator(latent_size, data_size)
+        self.generator = Generator(latent_size)
+
+        optimizer_d = optim.SGD(self.discriminator.parameters(), lr=self.lr_d,
+                                momentum=self.momentum)
+        optimizer_g = optim.SGD(self.generator.parameters(), lr=self.lr_g,
+                                momentum=self.momentum)
+        criterion = nn.BCELoss()
+
+        dataloader = DataLoader(
+            TensorDataset(torch.tensor(X, dtype=torch.float32)),
+            batch_size=min(500, data_size),
+            shuffle=True)
 
-        # Start iteration
         for epoch in range(epochs):
             print('Epoch {} of {}'.format(epoch + 1, epochs))
-            batch_size = min(500, data_size)
-            num_batches = int(data_size / batch_size)
 
-            for index in range(num_batches):
-                print('\nTesting for epoch {} index {}:'.format(epoch + 1,
-                                                                index + 1))
+            for data_batch in dataloader:
+                data_batch = data_batch[0]
+                batch_size = data_batch.size(0)
 
-                # Generate noise
-                noise_size = batch_size
-                noise = np.random.uniform(0, 1, (int(noise_size), latent_size))
+                # Train Discriminator
+                noise = torch.rand(batch_size, latent_size)
+                generated_data = self.generator(noise)
 
-                # Get training data
-                data_batch = X[index * batch_size: (index + 1) * batch_size]
+                real_labels = torch.ones(batch_size, 1)
+                fake_labels = torch.zeros(batch_size, 1)
 
-                # Generate potential outliers
-                generated_data = self.generator.predict(noise, verbose=0)
+                outputs_real = self.discriminator(data_batch)
+                outputs_fake = self.discriminator(generated_data)
 
-                # Concatenate real data to generated data
-                x = np.concatenate((data_batch, generated_data))
-                y = np.array([1] * batch_size + [0] * int(noise_size))
+                d_loss_real = criterion(outputs_real, real_labels)
+                d_loss_fake = criterion(outputs_fake, fake_labels)
 
-                # Train discriminator
-                discriminator_loss = self.discriminator.train_on_batch(x, y)
-                self.train_history['discriminator_loss'].append(
-                    discriminator_loss)
+                d_loss = d_loss_real + d_loss_fake
+
+                optimizer_d.zero_grad()
+                d_loss.backward()
+                optimizer_d.step()
+
+                self.train_history['discriminator_loss'].append(d_loss.item())
 
-                # Train generator
                 if stop == 0:
-                    trick = np.array([1] * noise_size)
-                    generator_loss = self.combine_model.train_on_batch(noise,
-                                                                       trick)
-                    self.train_history['generator_loss'].append(generator_loss)
+                    # Train Generator
+                    trick_labels = torch.ones(batch_size, 1)
+                    g_loss = criterion(
+                        self.discriminator(self.generator(noise)),
+                        trick_labels)
+
+                    optimizer_g.zero_grad()
+                    g_loss.backward()
+                    optimizer_g.step()
+
+                    self.train_history['generator_loss'].append(g_loss.item())
                 else:
-                    trick = np.array([1] * noise_size)
-                    generator_loss = self.combine_model.evaluate(noise, trick)
-                    self.train_history['generator_loss'].append(generator_loss)
+                    g_loss = criterion(
+                        self.discriminator(self.generator(noise)),
+                        trick_labels)
+                    self.train_history['generator_loss'].append(g_loss.item())
 
-            # Stop training generator
             if epoch + 1 > self.stop_epochs:
                 stop = 1
 
-        # Detection result
-        self.decision_scores_ = self.discriminator.predict(X).ravel()
+        self.decision_scores_ = self.discriminator(
+            torch.tensor(X, dtype=torch.float32)).detach().numpy().ravel()
         self._process_decision_scores()
         return self
 
     def decision_function(self, X):
         """Predict raw anomaly score of X using the fitted detector.
 
         The anomaly score of an input sample is computed based on different
@@ -194,9 +216,10 @@
         Returns
         -------
         anomaly_scores : numpy array of shape (n_samples,)
             The anomaly score of the input samples.
         """
         check_is_fitted(self, ['discriminator'])
         X = check_array(X)
-        pred_scores = self.discriminator.predict(X).ravel()
+        pred_scores = self.discriminator(
+            torch.tensor(X, dtype=torch.float32)).detach().numpy().ravel()
         return pred_scores
```

### Comparing `pyod-1.1.3/pyod/models/sod.py` & `pyod-2.0.0/pyod/models/sod.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/sos.py` & `pyod-2.0.0/pyod/models/sos.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/suod.py` & `pyod-2.0.0/pyod/models/suod.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/thresholds.py` & `pyod-2.0.0/pyod/models/thresholds.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/vae.py` & `pyod-2.0.0/pyod/models/vae.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/models/xgbod.py` & `pyod-2.0.0/pyod/models/xgbod.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/utils/__init__.py` & `pyod-2.0.0/pyod/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/utils/data.py` & `pyod-2.0.0/pyod/utils/data.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/utils/example.py` & `pyod-2.0.0/pyod/utils/example.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/utils/stat_models.py` & `pyod-2.0.0/pyod/utils/stat_models.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/utils/utility.py` & `pyod-2.0.0/pyod/utils/utility.py`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/pyod/version.py` & `pyod-2.0.0/pyod/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # X.YbN # Beta release
 # X.YrcN # Release Candidate
 # X.Y # Final release
 #
 # Dev branch marker is: 'X.Y.dev' or 'X.Y.devN' where N is an integer.
 # 'X.Y.dev0' is the canonical version of 'X.Y.dev'
 #
-__version__ = '1.1.3'  # pragma: no cover
+__version__ = '2.0.0'  # pragma: no cover
```

### Comparing `pyod-1.1.3/pyod.egg-info/PKG-INFO` & `pyod-2.0.0/pyod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyod
-Version: 1.1.3
+Version: 2.0.0
 Summary: A Comprehensive and Scalable Python Library for Outlier Detection (Anomaly Detection)
 Home-page: https://github.com/yzhao062/pyod
 Author: Yue Zhao
 Author-email: yzhao062@gmail.com
 License: UNKNOWN
 Download-URL: https://github.com/yzhao062/pyod/archive/master.zip
 Keywords: outlier detection,anomaly detection,outlier ensembles,data mining,neural networks
@@ -27,63 +27,65 @@
 License-File: LICENSE
 
 Python Outlier Detection (PyOD)
 ===============================
 
 **Deployment & Documentation & Stats & License**
 
-.. image:: https://img.shields.io/pypi/v/pyod.svg?color=brightgreen
+|badge_pypi| |badge_anaconda| |badge_docs| |badge_stars| |badge_forks| |badge_downloads| |badge_testing| |badge_coverage| |badge_maintainability| |badge_license| |badge_benchmark|
+
+.. |badge_pypi| image:: https://img.shields.io/pypi/v/pyod.svg?color=brightgreen
    :target: https://pypi.org/project/pyod/
    :alt: PyPI version
 
 
-.. image:: https://anaconda.org/conda-forge/pyod/badges/version.svg
+.. |badge_anaconda| image:: https://anaconda.org/conda-forge/pyod/badges/version.svg
    :target: https://anaconda.org/conda-forge/pyod
    :alt: Anaconda version
 
 
-.. image:: https://readthedocs.org/projects/pyod/badge/?version=latest
+.. |badge_docs| image:: https://readthedocs.org/projects/pyod/badge/?version=latest
    :target: https://pyod.readthedocs.io/en/latest/?badge=latest
    :alt: Documentation status
 
 
-.. image:: https://img.shields.io/github/stars/yzhao062/pyod.svg
+.. |badge_stars| image:: https://img.shields.io/github/stars/yzhao062/pyod.svg
    :target: https://github.com/yzhao062/pyod/stargazers
    :alt: GitHub stars
 
 
-.. image:: https://img.shields.io/github/forks/yzhao062/pyod.svg?color=blue
+.. |badge_forks| image:: https://img.shields.io/github/forks/yzhao062/pyod.svg?color=blue
    :target: https://github.com/yzhao062/pyod/network
    :alt: GitHub forks
 
 
-.. image:: https://pepy.tech/badge/pyod
+.. |badge_downloads| image:: https://pepy.tech/badge/pyod
    :target: https://pepy.tech/project/pyod
    :alt: Downloads
 
-.. image:: https://github.com/yzhao062/pyod/actions/workflows/testing.yml/badge.svg
+.. |badge_testing| image:: https://github.com/yzhao062/pyod/actions/workflows/testing.yml/badge.svg
    :target: https://github.com/yzhao062/pyod/actions/workflows/testing.yml
    :alt: testing
 
 
-.. image:: https://coveralls.io/repos/github/yzhao062/pyod/badge.svg
+.. |badge_coverage| image:: https://coveralls.io/repos/github/yzhao062/pyod/badge.svg
    :target: https://coveralls.io/github/yzhao062/pyod
    :alt: Coverage Status
 
 
-.. image:: https://api.codeclimate.com/v1/badges/bdc3d8d0454274c753c4/maintainability
+.. |badge_maintainability| image:: https://api.codeclimate.com/v1/badges/bdc3d8d0454274c753c4/maintainability
    :target: https://codeclimate.com/github/yzhao062/Pyod/maintainability
    :alt: Maintainability
 
 
-.. image:: https://img.shields.io/github/license/yzhao062/pyod.svg
+.. |badge_license| image:: https://img.shields.io/github/license/yzhao062/pyod.svg
    :target: https://github.com/yzhao062/pyod/blob/master/LICENSE
    :alt: License
 
-.. image:: https://img.shields.io/badge/ADBench-benchmark_results-pink
+.. |badge_benchmark| image:: https://img.shields.io/badge/ADBench-benchmark_results-pink
    :target: https://github.com/Minqi824/ADBench
    :alt: Benchmark
 
 
 -----
 
 
@@ -234,35 +236,30 @@
    cd pyod
    pip install .
 
 
 **Required Dependencies**\ :
 
 
-* Python 3.6 or higher
+* Python 3.8 or higher
 * joblib
 * matplotlib
 * numpy>=1.19
 * numba>=0.51
 * scipy>=1.5.1
 * scikit_learn>=0.22.0
-* six
 
 
 **Optional Dependencies (see details below)**\ :
 
 * combo (optional, required for models/combination.py and FeatureBagging)
 * keras/tensorflow (optional, required for AutoEncoder, and other deep learning models)
 * suod (optional, required for running SUOD model)
 * xgboost (optional, required for XGBOD)
-* pythresh (optional, required for thresholding)
-
-**Warning**\ :
-PyOD includes several neural network-based models, such as AutoEncoders, implemented in Tensorflow and PyTorch. These deep learning libraries are not automatically installed by PyOD to avoid conflicts with existing installations. If you plan to use neural-net based models, please ensure these libraries are installed. See the `neural-net FAQ <https://github.com/yzhao062/pyod/wiki/Setting-up-Keras-and-Tensorflow-for-Neural-net-Based-models>`_ for guidance. Additionally, xgboost is not installed by default but is required for models like XGBOD.
-
+* pythresh (optional, required for thresholding)optional
 
 ----
 
 
 API Cheatsheet & Reference
 ^^^^^^^^^^^^^^^^^^^^^^^^^^
 
@@ -591,49 +588,14 @@
 
 .. image:: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png
    :target: https://raw.githubusercontent.com/yzhao062/pyod/master/examples/KNN.png
    :alt: kNN example figure
 
 ----
 
-How to Contribute
-^^^^^^^^^^^^^^^^^
-
-You are welcome to contribute to this exciting project:
-
-
-* Please first check Issue lists for "help wanted" tag and comment the one
-  you are interested. We will assign the issue to you.
-
-* Fork the master branch and add your improvement/modification/fix.
-
-* Create a pull request to **development branch** and follow the pull request template `PR template <https://github.com/yzhao062/pyod/blob/master/PULL_REQUEST_TEMPLATE.md>`_
-
-* Automatic tests will be triggered. Make sure all tests are passed. Please make sure all added modules are accompanied with proper test functions.
-
-
-To make sure the code has the same style and standard, please refer to abod.py, hbos.py, or feature_bagging.py for example.
-
-You are also welcome to share your ideas by opening an issue or dropping me an email at zhaoy@cmu.edu :)
-
-
-Inclusion Criteria
-^^^^^^^^^^^^^^^^^^
-
-Similarly to `scikit-learn <https://scikit-learn.org/stable/faq.html#what-are-the-inclusion-criteria-for-new-algorithms>`_,
-We mainly consider well-established algorithms for inclusion.
-A rule of thumb is at least two years since publication, 50+ citations, and usefulness.
-
-However, we encourage the author(s) of newly proposed models to share and add your implementation into PyOD
-for boosting ML accessibility and reproducibility.
-This exception only applies if you could commit to the maintenance of your model for at least two year period.
-
-
-----
-
 Reference
 ^^^^^^^^^
 
 
 .. [#Aggarwal2015Outlier] Aggarwal, C.C., 2015. Outlier analysis. In Data mining (pp. 237-263). Springer, Cham.
 
 .. [#Aggarwal2015Theoretical] Aggarwal, C.C. and Sathe, S., 2015. Theoretical foundations and algorithms for outlier ensembles.\ *ACM SIGKDD Explorations Newsletter*\ , 17(1), pp.24-47.
```

### Comparing `pyod-1.1.3/pyod.egg-info/SOURCES.txt` & `pyod-2.0.0/pyod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyod-1.1.3/setup.py` & `pyod-2.0.0/setup.py`

 * *Files identical despite different names*

