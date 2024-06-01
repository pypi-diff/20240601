# Comparing `tmp/pygda-0.0.3.tar.gz` & `tmp/pygda-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygda-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pygda-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pygda-0.0.3.tar` & `pygda-0.0.4.tar`

### file list

```diff
@@ -1,64 +1,64 @@
--rw-r--r--   0        0        0     5322 2024-05-25 11:50:56.122318 pygda-0.0.3/README.md
--rw-r--r--   0        0        0      172 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/__init__.py
--rw-r--r--   0        0        0      576 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/datasets/__init__.py
--rw-r--r--   0        0        0     2856 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/datasets/airport.py
--rw-r--r--   0        0        0     2393 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/datasets/arxiv.py
--rw-r--r--   0        0        0     2748 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/datasets/blog.py
--rw-r--r--   0        0        0     3237 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/datasets/citation.py
--rw-r--r--   0        0        0     2800 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/datasets/elliptic.py
--rw-r--r--   0        0        0     4523 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/datasets/facebook.py
--rw-r--r--   0        0        0     2416 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/datasets/mag.py
--rw-r--r--   0        0        0     2779 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/datasets/squirrel.py
--rw-r--r--   0        0        0     4370 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/datasets/twitch.py
--rw-r--r--   0        0        0     2421 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/datasets/twitter.py
--rw-r--r--   0        0        0      383 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/metrics/__init__.py
--rw-r--r--   0        0        0     2675 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/metrics/metrics.py
--rw-r--r--   0        0        0      697 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/__init__.py
--rw-r--r--   0        0        0     7414 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/a2gnn.py
--rw-r--r--   0        0        0    11327 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/acdne.py
--rw-r--r--   0        0        0     9514 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/adagcn.py
--rw-r--r--   0        0        0    13352 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/asn.py
--rw-r--r--   0        0        0     4383 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/base.py
--rw-r--r--   0        0        0     8615 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/cwgcn.py
--rw-r--r--   0        0        0    11770 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/dane.py
--rw-r--r--   0        0        0    11852 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/dgda.py
--rw-r--r--   0        0        0    12125 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/dmgnn.py
--rw-r--r--   0        0        0     5895 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/gnn.py
--rw-r--r--   0        0        0     7557 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/grade.py
--rw-r--r--   0        0        0     8903 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/jhgda.py
--rw-r--r--   0        0        0     5961 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/kbl.py
--rw-r--r--   0        0        0    23357 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/pa.py
--rw-r--r--   0        0        0     7477 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/sagda.py
--rw-r--r--   0        0        0    10339 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/specreg.py
--rw-r--r--   0        0        0    18281 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/strurw.py
--rw-r--r--   0        0        0     7827 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/models/udagcn.py
--rw-r--r--   0        0        0     1180 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/__init__.py
--rw-r--r--   0        0        0     2517 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/a2gnn_base.py
--rw-r--r--   0        0        0     4612 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/acdne_base.py
--rw-r--r--   0        0        0     2770 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/adagcn_base.py
--rw-r--r--   0        0        0     6921 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/asn_base.py
--rw-r--r--   0        0        0      469 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/attention.py
--rw-r--r--   0        0        0     4136 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/cached_gcn_conv.py
--rw-r--r--   0        0        0     4107 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/cwgcn_base.py
--rw-r--r--   0        0        0     1926 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/deepwalk_pretrain.py
--rw-r--r--   0        0        0    11050 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/dgda_base.py
--rw-r--r--   0        0        0     9982 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/gmm_clustering.py
--rw-r--r--   0        0        0     3573 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/gnn_base.py
--rw-r--r--   0        0        0     2833 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/grade_base.py
--rw-r--r--   0        0        0    12117 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/jhgda_base.py
--rw-r--r--   0        0        0    39000 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/kbl_base.py
--rw-r--r--   0        0        0     4045 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/mixup_base.py
--rw-r--r--   0        0        0     7526 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/mixup_gcnconv.py
--rw-r--r--   0        0        0     3696 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/ppmi_conv.py
--rw-r--r--   0        0        0     6842 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/prop_gcn_conv.py
--rw-r--r--   0        0        0      303 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/reverse_layer.py
--rw-r--r--   0        0        0    11146 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/reweight_gnn.py
--rw-r--r--   0        0        0     7161 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/sagda_base.py
--rw-r--r--   0        0        0     4303 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/nn/udagcn_base.py
--rw-r--r--   0        0        0       71 2024-05-25 11:50:56.126318 pygda-0.0.3/pygda/utils/__init__.py
--rw-r--r--   0        0        0     2061 2024-05-25 11:50:56.130318 pygda-0.0.3/pygda/utils/mmd.py
--rw-r--r--   0        0        0     1028 2024-05-25 11:50:56.130318 pygda-0.0.3/pygda/utils/svd_transform.py
--rw-r--r--   0        0        0     1912 2024-05-25 11:50:56.130318 pygda-0.0.3/pygda/utils/utility.py
--rw-r--r--   0        0        0       21 2024-05-25 11:50:56.130318 pygda-0.0.3/pygda/version.py
--rw-r--r--   0        0        0      588 2024-05-25 11:50:56.130318 pygda-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     5783 1970-01-01 00:00:00.000000 pygda-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     5808 2024-06-01 03:35:00.328998 pygda-0.0.4/README.md
+-rw-r--r--   0        0        0      172 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/__init__.py
+-rw-r--r--   0        0        0      576 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/datasets/__init__.py
+-rw-r--r--   0        0        0     2856 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/datasets/airport.py
+-rw-r--r--   0        0        0     2393 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/datasets/arxiv.py
+-rw-r--r--   0        0        0     2748 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/datasets/blog.py
+-rw-r--r--   0        0        0     3237 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/datasets/citation.py
+-rw-r--r--   0        0        0     2800 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/datasets/elliptic.py
+-rw-r--r--   0        0        0     4523 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/datasets/facebook.py
+-rw-r--r--   0        0        0     2416 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/datasets/mag.py
+-rw-r--r--   0        0        0     2779 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/datasets/squirrel.py
+-rw-r--r--   0        0        0     4370 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/datasets/twitch.py
+-rw-r--r--   0        0        0     2421 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/datasets/twitter.py
+-rw-r--r--   0        0        0      383 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/metrics/__init__.py
+-rw-r--r--   0        0        0     2675 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/metrics/metrics.py
+-rw-r--r--   0        0        0      697 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/__init__.py
+-rw-r--r--   0        0        0     7555 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/a2gnn.py
+-rw-r--r--   0        0        0    11327 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/acdne.py
+-rw-r--r--   0        0        0     9514 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/adagcn.py
+-rw-r--r--   0        0        0    13467 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/asn.py
+-rw-r--r--   0        0        0     4383 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/base.py
+-rw-r--r--   0        0        0     8619 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/cwgcn.py
+-rw-r--r--   0        0        0    12025 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/dane.py
+-rw-r--r--   0        0        0    11852 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/dgda.py
+-rw-r--r--   0        0        0    12125 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/dmgnn.py
+-rw-r--r--   0        0        0     5895 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/gnn.py
+-rw-r--r--   0        0        0     7557 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/grade.py
+-rw-r--r--   0        0        0     8903 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/jhgda.py
+-rw-r--r--   0        0        0     5961 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/kbl.py
+-rw-r--r--   0        0        0    21669 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/pa.py
+-rw-r--r--   0        0        0     7477 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/sagda.py
+-rw-r--r--   0        0        0    10339 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/specreg.py
+-rw-r--r--   0        0        0    18888 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/strurw.py
+-rw-r--r--   0        0        0     7827 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/models/udagcn.py
+-rw-r--r--   0        0        0     1180 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/nn/__init__.py
+-rw-r--r--   0        0        0     2525 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/nn/a2gnn_base.py
+-rw-r--r--   0        0        0     4612 2024-06-01 03:35:00.332999 pygda-0.0.4/pygda/nn/acdne_base.py
+-rw-r--r--   0        0        0     2771 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/adagcn_base.py
+-rw-r--r--   0        0        0     6922 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/asn_base.py
+-rw-r--r--   0        0        0      469 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/attention.py
+-rw-r--r--   0        0        0     4136 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/cached_gcn_conv.py
+-rw-r--r--   0        0        0     4107 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/cwgcn_base.py
+-rw-r--r--   0        0        0     1926 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/deepwalk_pretrain.py
+-rw-r--r--   0        0        0    11050 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/dgda_base.py
+-rw-r--r--   0        0        0     9982 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/gmm_clustering.py
+-rw-r--r--   0        0        0     3573 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/gnn_base.py
+-rw-r--r--   0        0        0     2834 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/grade_base.py
+-rw-r--r--   0        0        0    12118 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/jhgda_base.py
+-rw-r--r--   0        0        0    39750 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/kbl_base.py
+-rw-r--r--   0        0        0     4045 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/mixup_base.py
+-rw-r--r--   0        0        0     7504 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/mixup_gcnconv.py
+-rw-r--r--   0        0        0     3696 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/ppmi_conv.py
+-rw-r--r--   0        0        0     6842 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/prop_gcn_conv.py
+-rw-r--r--   0        0        0      303 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/reverse_layer.py
+-rw-r--r--   0        0        0    10796 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/reweight_gnn.py
+-rw-r--r--   0        0        0     7162 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/sagda_base.py
+-rw-r--r--   0        0        0     4327 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/nn/udagcn_base.py
+-rw-r--r--   0        0        0       71 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/utils/__init__.py
+-rw-r--r--   0        0        0     2061 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/utils/mmd.py
+-rw-r--r--   0        0        0     1028 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/utils/svd_transform.py
+-rw-r--r--   0        0        0     1912 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/utils/utility.py
+-rw-r--r--   0        0        0       21 2024-06-01 03:35:00.336999 pygda-0.0.4/pygda/version.py
+-rw-r--r--   0        0        0      588 2024-06-01 03:35:00.336999 pygda-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6269 1970-01-01 00:00:00.000000 pygda-0.0.4/PKG-INFO
```

### Comparing `pygda-0.0.3/README.md` & `pygda-0.0.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 ![](docs/pygda_logo.png)
 -----
+[![PyPI version](https://badge.fury.io/py/pygda.svg)](https://badge.fury.io/py/pygda)
+[![Documentation Status](https://readthedocs.org/projects/pygda/badge/?version=stable)](https://pygda.readthedocs.io/en/stable/?badge=stable)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/pygda-team/pygda/issues)
 
 PyGDA is a **Python library** for **Graph Domain Adaptation** built upon [PyTorch](https://pytorch.org/) and [PyG](https://pytorch-geometric.readthedocs.io/en/latest/) to easily train graph domain adaptation models in a [sklearn](https://scikit-learn.org/stable/) style. PyGDA includes **15+** graph domain adaptation models. See examples with PyGDA below!
 
 **Graph Domain Adaptation Using PyGDA with 5 Lines of Code**
 ```
 from pygda.models import A2GNN
```

### Comparing `pygda-0.0.3/pygda/datasets/__init__.py` & `pygda-0.0.4/pygda/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/datasets/airport.py` & `pygda-0.0.4/pygda/datasets/airport.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/datasets/arxiv.py` & `pygda-0.0.4/pygda/datasets/arxiv.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/datasets/blog.py` & `pygda-0.0.4/pygda/datasets/blog.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/datasets/citation.py` & `pygda-0.0.4/pygda/datasets/citation.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/datasets/elliptic.py` & `pygda-0.0.4/pygda/datasets/elliptic.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/datasets/facebook.py` & `pygda-0.0.4/pygda/datasets/facebook.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/datasets/mag.py` & `pygda-0.0.4/pygda/datasets/mag.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/datasets/squirrel.py` & `pygda-0.0.4/pygda/datasets/squirrel.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/datasets/twitch.py` & `pygda-0.0.4/pygda/datasets/twitch.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/datasets/twitter.py` & `pygda-0.0.4/pygda/datasets/twitter.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/metrics/metrics.py` & `pygda-0.0.4/pygda/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/models/__init__.py` & `pygda-0.0.4/pygda/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/models/a2gnn.py` & `pygda-0.0.4/pygda/models/a2gnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -189,17 +189,17 @@
                 epoch_loss += loss.item()
 
                 optimizer.zero_grad()
                 loss.backward()
                 optimizer.step()
 
                 if idx == 0:
-                    epoch_source_logits, epoch_source_labels = self.predict(sampled_source_data)
+                    epoch_source_logits, epoch_source_labels = self.predict(sampled_source_data, source=True)
                 else:
-                    source_logits, source_labels = self.predict(sampled_source_data)
+                    source_logits, source_labels = self.predict(sampled_source_data, source=True)
                     epoch_source_logits = torch.cat((epoch_source_logits, source_logits))
                     epoch_source_labels = torch.cat((epoch_source_labels, source_labels))
             
             epoch_source_preds = epoch_source_logits.argmax(dim=1)
             micro_f1_score = eval_micro_f1(epoch_source_labels, epoch_source_preds)
 
             logger(epoch=epoch,
@@ -208,14 +208,17 @@
                    time=time.time() - start_time,
                    verbose=self.verbose,
                    train=True)
     
     def process_graph(self, data):
         pass
 
-    def predict(self, data):
+    def predict(self, data, source=False):
         self.a2gnn.eval()
 
         with torch.no_grad():
-            logits = self.a2gnn(data, self.s_pnums)
+            if source:
+                logits = self.a2gnn(data, self.s_pnums)
+            else:
+                logits = self.a2gnn(data, self.t_pnums)
 
         return logits, data.y
```

### Comparing `pygda-0.0.3/pygda/models/acdne.py` & `pygda-0.0.4/pygda/models/acdne.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/models/adagcn.py` & `pygda-0.0.4/pygda/models/adagcn.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/models/asn.py` & `pygda-0.0.4/pygda/models/asn.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
 from . import BaseGDA
 from ..nn import ASNBase
 from ..nn import GradReverse
 from ..utils import logger
 from ..metrics import eval_macro_f1, eval_micro_f1
 
+import warnings
+warnings.filterwarnings('ignore', '.*Sparse CSR tensor support is in beta state.*')
 
 class ASN(BaseGDA):
     """
     Adversarial Separation Network for Cross-Network Node Classification (CIKM-21).
 
     Parameters
     ----------
@@ -293,15 +295,15 @@
         """Convert a scipy sparse matrix to a torch sparse tensor."""
         sparse_mx = sparse_mx.tocoo().astype(np.float32)
         indices = torch.from_numpy(
             np.vstack((sparse_mx.row, sparse_mx.col)).astype(np.int64))
         values = torch.from_numpy(sparse_mx.data)
         shape = torch.Size(sparse_mx.shape)
         
-        return torch.sparse.FloatTensor(indices, values, shape).coalesce()
+        return torch.sparse_coo_tensor(indices, values, shape).coalesce().to_sparse_csr()
 
     def agg_tran_prob_mat(self, g, step):
         """aggregated K-step transition probality"""
         g = self.my_scale_sim_mat(g)
         g = csc_matrix.toarray(g)
         a_k = g
         a = g
```

### Comparing `pygda-0.0.3/pygda/models/base.py` & `pygda-0.0.4/pygda/models/base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/models/cwgcn.py` & `pygda-0.0.4/pygda/models/cwgcn.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
             weight_decay=self.weight_decay
         )
 
         start_time = time.time()
 
         print('Step 1, train source data...')
 
-        for epoch in range(self.epoch):
+        for epoch in range(self.epoch * 2):
             epoch_loss = 0
             epoch_source_logits = None
             epoch_source_labels = None
 
             for idx, sampled_source_data in enumerate(source_loader):
                 self.gnn.train()
```

### Comparing `pygda-0.0.3/pygda/models/dane.py` & `pygda-0.0.4/pygda/models/dane.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import copy
 
 import torch.nn as nn
 import scipy.sparse as sp
 import numpy as np
 
 from torch_geometric.loader import NeighborLoader
-from torch_geometric.utils import to_dense_adj
+from torch_geometric.utils import is_undirected, to_undirected
 
 from . import BaseGDA
 from ..nn import GNNBase, GradReverse
 from ..utils import logger
 from ..metrics import eval_macro_f1, eval_micro_f1
 
 
@@ -27,16 +27,16 @@
     ----------
     in_dim :  int
         Input feature dimension.
     hid_dim :  int
         Hidden dimension of model.
     num_classes : int
         Total number of classes.
-    num_layers : int, optional
-        Total number of layers in model. Default: ``2``.
+    num_layers : int
+        Total number of layers in model.
     dropout : float, optional
         Dropout rate. Default: ``0.``.
     gnn : string, optional
         GNN backbone. Default: ``gcn``.
     k : int, optional
         Number of negative samples. Default: ``5``.
     mode : string, optional
@@ -67,15 +67,15 @@
     """
 
     def __init__(
         self,
         in_dim,
         hid_dim,
         num_classes,
-        num_layers=2,
+        num_layers,
         dropout=0.,
         gnn='gcn',
         k=5,
         mode='unsup',
         tgt_rate=0.05,
         act=F.relu,
         weight_decay=1e-5,
@@ -131,14 +131,19 @@
         target_logits = self.gnn(target_data.x, target_data.edge_index)
 
         loss = discriminator_loss + generator_loss
 
         return loss, source_logits, target_logits
 
     def fit(self, source_data, target_data):
+        if not is_undirected(source_data.edge_index):
+            source_data.edge_index = to_undirected(source_data.edge_index)
+        
+        if not is_undirected(target_data.edge_index):
+            target_data.edge_index = to_undirected(target_data.edge_index)
 
         self.sample_size = min(source_data.x.shape[0], target_data.x.shape[0])
 
         if self.batch_size == 0:
             self.source_batch_size = source_data.x.shape[0]
             source_loader = NeighborLoader(source_data,
                                 self.num_neigh,
```

### Comparing `pygda-0.0.3/pygda/models/dgda.py` & `pygda-0.0.4/pygda/models/dgda.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/models/dmgnn.py` & `pygda-0.0.4/pygda/models/dmgnn.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/models/gnn.py` & `pygda-0.0.4/pygda/models/gnn.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/models/grade.py` & `pygda-0.0.4/pygda/models/grade.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/models/jhgda.py` & `pygda-0.0.4/pygda/models/jhgda.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/models/kbl.py` & `pygda-0.0.4/pygda/models/kbl.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/models/pa.py` & `pygda-0.0.4/pygda/models/pa.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 import numpy as np
 import cvxpy as cp
 
 from torch_geometric.loader import NeighborLoader
 from torch_geometric.utils import to_dense_adj
 
 from . import BaseGDA
-from ..nn import ReweightGNN, GradReverse, MixupBase
-from ..utils import logger, MMD
+from ..nn import ReweightGNN
+from ..utils import logger
 from ..metrics import eval_macro_f1, eval_micro_f1
 
 
 class PairAlign(BaseGDA):
     """
 
     Pairwise Alignment Improves Graph Domain Adaptation (ICML-24).
@@ -217,16 +217,18 @@
         label_weight = self.update_lw(source_data, target_data, pred_src, pred_tgt)
         if (epoch + 1) >= self.lw_start and (epoch + 1) % self.lw_freq == 0:
             source_data.lw = label_weight
 
         return loss, pred_src, pred_tgt
 
     def fit(self, source_data, target_data):
-        source_data.edge_weight = torch.ones(source_data.edge_index.shape[1]).to(self.device)
-        target_data.edge_weight = torch.ones(target_data.edge_index.shape[1]).to(self.device)
+        if source_data.edge_weight is None:
+            source_data.edge_weight = torch.ones(source_data.edge_index.shape[1]).to(self.device)
+        if target_data.edge_weight is None:
+            target_data.edge_weight = torch.ones(target_data.edge_index.shape[1]).to(self.device)
 
         if self.batch_size == 0:
             self.source_batch_size = source_data.x.shape[0]
             source_loader = NeighborLoader(source_data,
                                 self.num_neigh,
                                 batch_size=self.source_batch_size)
             self.target_batch_size = target_data.x.shape[0]
@@ -309,41 +311,40 @@
         return torch.mean(loss(pred, label))
 
     def CE_loss_weight(self, pred, label, label_weight, weight_src):
         class_num = len(label.unique())
         label = label.type(torch.int64)
         y_onehot = F.one_hot(label).float().to(self.device)
         p_y = torch.sum(y_onehot, 0) / len(y_onehot)
-        class_weights = torch.tensor(1.0 / p_y, dtype=torch.float, requires_grad=False).to(self.device)
+        class_weights = (1.0 / p_y.clone().detach()).to(self.device)
         if weight_src:
             loss = nn.CrossEntropyLoss(reduction='none', weight=class_weights)
         else:
             loss = nn.CrossEntropyLoss()
         weight = torch.mm(y_onehot, label_weight.view(-1, 1).float())
-        #loss = nn.CrossEntropyLoss(weight= label_weight)
         
         return torch.mean(loss(pred, label).view(-1, 1) * weight)/ class_num
     
     def calc_true_lw(self, src_graph, tgt_graph):
+        print('calc true lw...')
         label_onehot_src = F.one_hot(src_graph.y)
         label_onehot_tgt = F.one_hot(tgt_graph.y)
         num_nodes_src = torch.sum(label_onehot_src, 0)
         label_dis_src = num_nodes_src / src_graph.x.shape[0]
 
         num_nodes_tgt = torch.sum(label_onehot_tgt, 0)
         label_dis_tgt = num_nodes_tgt / tgt_graph.x.shape[0]
 
         label_weight = label_dis_tgt / label_dis_src
         src_graph.true_lw = label_weight.cpu().detach().numpy()
 
         src_graph.lw = np.ones_like(src_graph.true_lw)
-        
-        print("true lw: " + str(src_graph.true_lw))
-    
+            
     def calc_true_beta(self, src_graph, tgt_graph):
+        print('calc true beta...')
         num_classes = self.num_classes
         src_num_edges = src_graph.edge_index.shape[1]
         src_edge_class = np.zeros((src_num_edges, num_classes, num_classes))
         for idx in range(src_num_edges):
             i = src_graph.edge_index[0][idx]
             j = src_graph.edge_index[1][idx]
             src_edge_class[idx, src_graph.y[i], src_graph.y[j]] = 1
@@ -366,31 +367,23 @@
         p_edge_tgt = edge_class_tgt.sum(axis=0) / tgt_num_edges
 
         beta = (p_edge_tgt) / (p_edge_src)
         beta[beta == float('inf')] = 1
         beta = np.nan_to_num(beta, nan = 1)
     
         src_graph.true_beta = beta
-        print("true beta: " + str(beta))
-        print("max: " + str(np.max(beta)) + "; min: " + str(np.min(beta)))
     
     def calc_true_ew(self, src_graph, tgt_graph):
+        print('calc true ew...')
         src_edge_prob, tgt_edge_prob = self.cal_edge_prob_sep(src_graph, tgt_graph)
 
-        #edge_weight = tgt_edge_prob / src_edge_prob
         edge_weight = (tgt_edge_prob + self.gamma_reg) / (src_edge_prob + self.gamma_reg)
-        print(edge_weight.min())
-        print(edge_weight.max())
-
-        # edge_weight[edge_weight == float('inf')] = 1
-        # edge_weight = torch.nan_to_num(edge_weight, nan = 1)
     
         src_graph.true_ew = edge_weight.cpu().detach().numpy()
         src_graph.ew = np.ones_like(src_graph.true_ew)
-        print("true ew: " + str(src_graph.true_ew))
     
     def cal_edge_prob_sep(self, src_graph, tgt_graph):
         src_adj = to_dense_adj(src_graph.edge_index).squeeze().T.detach().cpu().numpy()
         tgt_adj = to_dense_adj(tgt_graph.edge_index).squeeze().T.detach().cpu().numpy()
         num_nodes_src = src_graph.x.shape[0]
         num_nodes_tgt = tgt_graph.x.shape[0]
         src_label = src_graph.y
@@ -400,22 +393,17 @@
         src_label_one_hot = sp.csr_matrix((np.ones(num_nodes_src), (np.arange(num_nodes_src), src_label.cpu().numpy())),
                                       shape=(num_nodes_src, num_class))
         tgt_label_one_hot = sp.csr_matrix((np.ones(num_nodes_tgt), (np.arange(num_nodes_tgt), tgt_label.cpu().numpy())),
                                       shape=(num_nodes_tgt, num_class))
 
         src_node_num = src_label_one_hot.sum(axis=0).T * num_nodes_src
         tgt_node_sum = tgt_label_one_hot.sum(axis=0).T * num_nodes_tgt
-        #print(tgt_pred_node_sum)
-        #print(tgt_node_sum)
 
         src_num_edge = (src_label_one_hot.T * src_adj * src_label_one_hot)
         tgt_num_edge = (tgt_label_one_hot.T * tgt_adj * tgt_label_one_hot)
-        #print(src_num_edge)
-        #print(tgt_pred_num_edge)
-        #print(tgt_true_num_edge)
 
         src_edge_prob = src_num_edge / src_node_num
         tgt_edge_prob = tgt_num_edge / tgt_node_sum
 
         src_edge_prob = torch.from_numpy(np.array(src_edge_prob))
         tgt_edge_prob = torch.from_numpy(np.array(tgt_edge_prob))
 
@@ -435,17 +423,14 @@
             src_num_edges = src_graph.edge_index.shape[1]
             
             edge_weight = np.matmul(self.src_edge_class.reshape(src_num_edges, num_classes**2), edge_rw.reshape(num_classes**2))
             src_data.edge_weight = torch.from_numpy(edge_weight).float().to(self.device)
             src_data.ew = edge_rw
             ew_diff = np.abs(edge_rw - src_data.true_ew.reshape(num_classes, num_classes)).sum()
 
-            # print("ew: "+ str(edge_rw))
-            # print("max: " + str(np.max(edge_rw)) + "; min: " + str(np.min(edge_rw)))
-    
         return 
 
     def calc_edge_rw_pseudo(self, src_graph, tgt_graph, yhat_src, yhat_tgt):
         true_ew = src_graph.true_ew
         true_beta = src_graph.true_beta
         num_classes = self.num_classes
 
@@ -470,104 +455,86 @@
         src_edgeclass = torch.tensor(self.src_edge_class.reshape(-1, num_classes**2)).float().to(self.device)
         C_hat = (src_edgehat.T @ src_edgeclass) / src_num_edges
         muhat_tgt = torch.mean(tgt_edgehat, dim = 0).view(num_classes**2, 1)
         mu_src = torch.mean(src_edgeclass, dim = 0).view(num_classes**2, 1)
     
         w = self.LS_optimization(C_hat, muhat_tgt, mu_src, self.ls_lambda)
         w = np.reshape(w, (num_classes, num_classes))
-        # beta = true_beta
-        print("w: "+ str(np.reshape(w, (num_classes, num_classes))))
-        print("max: " + str(np.max(w)) + "; min: " + str(np.min(w)))
+
         beta_diff = np.abs(w - true_beta.reshape(num_classes, num_classes)).sum()
 
         gamma, p_ei_tgt = self.calc_ratio_weight(src_graph, w, self.gamma_reg)
-        print("gamma: "+ str(gamma))
         edge_rw = gamma
         edge_rw[edge_rw == float('inf')] = 1
         edge_rw = np.nan_to_num(edge_rw, nan = 1)
-        print("calc_ew: " + str(edge_rw))
-        print("max: " + str(np.max(edge_rw)) + "; min: " + str(np.min(edge_rw)))
+
         edge_weight = np.matmul(self.src_edge_class.reshape(src_num_edges, num_classes**2), edge_rw.reshape(num_classes**2))
         src_graph.edge_weight = torch.from_numpy(edge_weight).float().to(self.device)
         src_graph.ew = edge_rw
-        #return edge_weight
 
         diff = np.abs(edge_rw - true_ew.reshape(num_classes, num_classes)).sum()
         
         return diff, beta_diff
     
     def LS_optimization(self, cov, muhat_tgt, mu_src, lambda_reg):
         mu_src = mu_src.cpu().detach().numpy().reshape(-1).astype(np.double)
         muhat_tgt = muhat_tgt.cpu().detach().numpy().reshape(-1).astype(np.double)
         cov = cov.cpu().detach().numpy().astype(np.double)
 
         print("rank of Cov in edge: " + str(np.linalg.matrix_rank(cov)))
-        print("condition number of Cov in edge: " + str(np.linalg.cond(cov)))
         x0 = np.ones(cov.shape[1])  
         x = cp.Variable(cov.shape[1])
 
         objective = cp.Minimize(cp.norm(cov @ x - muhat_tgt, 2)**2 + lambda_reg * cp.norm(x - x0, 2)**2)
         constraints = [mu_src @ x == 1 , 0 <= x]
 
         problem = cp.Problem(objective, constraints)
         problem.solve(solver=cp.SCS)
 
         x_value = x.value
-   
-        print("edge_weight: "+ str(x_value))
-        
+           
         return x_value
     
     def calc_ratio_weight(self, src_graph, kmm_weight, gamma_reg):
         src_num_edges = src_graph.edge_index.shape[1]
         src_num_nodes = src_graph.x.shape[0]
         num_classes = self.num_classes
         p_eij_src = (np.sum(self.src_edge_class.reshape(src_num_edges, num_classes**2), axis=0) / src_num_edges)
         p_eij_tgt = p_eij_src * kmm_weight.reshape(-1)
         p_eij_src_reg = p_eij_src + gamma_reg
         p_eij_tgt_reg = p_eij_tgt + gamma_reg
 
         p_ei_src_reg = np.sum(p_eij_src_reg.reshape(num_classes, num_classes), axis=1)
         p_ei_tgt_reg = np.sum(p_eij_tgt_reg.reshape(num_classes, num_classes), axis=1)
-        # print(p_ei_src)
-        # print(p_ei_tgt)
-        # print("cond_ratio:")
-        # print((p_eij_src.reshape(src_graph.num_classes, src_graph.num_classes).T / p_ei_src).T)
-        # print((p_eij_tgt.reshape(src_graph.num_classes, src_graph.num_classes).T / p_ei_tgt).T)
+
         gamma = ((p_eij_tgt_reg.reshape(num_classes, num_classes).T / p_ei_tgt_reg).T) / ((p_eij_src_reg.reshape(num_classes, num_classes).T / p_ei_src_reg).T)
 
         return gamma, p_ei_tgt_reg
     
     def update_lw(self, src_data, tgt_data, pred_src, pred_tgt):
         yhat_tgt = torch.mean(F.softmax(pred_tgt,dim=1), dim=0)
         y_src_onehot = F.one_hot(src_data.y).float().to(self.device)
         y_src = torch.mean(y_src_onehot, dim=0)
         y_src_pred = F.softmax(pred_src,dim=1)
         cov_mat = torch.mm(y_src_pred.T, y_src_onehot) / src_data.x.shape[0]
-    
-        # print("cov mat rank: "  + str(torch.linalg.matrix_rank(cov_mat)))
-        # print("cov mat condition number: " + str(torch.linalg.cond(cov_mat)))
-        # print()
 
         label_weight = self.calc_label_rw(y_src, yhat_tgt, cov_mat, self.lw_lambda)
 
         return label_weight
     
     def calc_label_rw(self, y_src, y_hat_tgt, cov, lambda_reg):
         y_src = y_src.cpu().detach().numpy().astype(np.double)
         y_hat_tgt = y_hat_tgt.cpu().detach().numpy().astype(np.double)
         cov = cov.cpu().detach().numpy().astype(np.double)
     
         x0 = np.ones(cov.shape[1])
-        #lambda_reg = 0.005  
         x = cp.Variable(cov.shape[1])
 
         objective = cp.Minimize(cp.norm(cov @ x - y_hat_tgt, 2)**2 + lambda_reg * cp.norm(x - x0, 2)**2)
         constraints = [y_src @ x == 1, 0 <= x]
 
         problem = cp.Problem(objective, constraints)
         problem.solve(solver=cp.SCS)
 
         x_value = x.value
-        # print("label_weight: "+ str(x_value))
         
         return x_value
```

### Comparing `pygda-0.0.3/pygda/models/sagda.py` & `pygda-0.0.4/pygda/models/sagda.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/models/specreg.py` & `pygda-0.0.4/pygda/models/specreg.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/models/strurw.py` & `pygda-0.0.4/pygda/models/strurw.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import scipy.sparse as sp
 import numpy as np
 
 from torch_geometric.loader import NeighborLoader
 from torch_geometric.utils import to_dense_adj
 
 from . import BaseGDA
-from ..nn import GNNBase, GradReverse, MixupBase
+from ..nn import ReweightGNN, GradReverse, MixupBase
 from ..utils import logger, MMD
 from ..metrics import eval_macro_f1, eval_micro_f1
 
 
 class StruRW(BaseGDA):
     """
 
@@ -29,18 +29,34 @@
         Input feature dimension.
     hid_dim : int
         Hidden dimension of model.
     num_classes : int
         Total number of classes.
     num_layers : int, optional
         Total number of layers in model. Default: ``2``.
+    cls_dim : int, optional
+        Hidden dimension for classification layer. Default: ``128``.
+    cls_layers : int, optional
+        Total number of cls layers in model. Default: ``2``.
     dropout : float, optional
         Dropout rate. Default: ``0.``.
     gnn : string, optional
-        GNN backbone. Default: ``gcn``.
+        GNN backbone. Default: ``GS``.
+    pooling : string, optional
+        Aggregation in gnn. Default: ``mean``.
+    bn : bool, optional
+        Batch normalization or not. Default: ``False``.
+    reweight : bool, optional
+        Reweight the edge in source graph or not. Default: ``True``.
+    pseudo : bool, optional
+        Use pseudo labels in target graph or not. Default: ``True``.
+    ew_start : int, optional
+        Starting epoch for edge reweighting. Default: ``100``.
+    ew_freq : int, optional
+        Frequency for edge reweighting. Default: ``20``.
     lamb : float, optional
         Trade-off parameter for edge reweight. Default: ``0.8``.
     mode : string, optional
         The training mode of StruRW. Default: ``erm``.
     weight_decay : float, optional
         Weight decay (L2 penalty). Default: ``0.0001``.
     act : callable activation function or None, optional
@@ -66,19 +82,27 @@
 
     def __init__(
         self,
         in_dim,
         hid_dim,
         num_classes,
         num_layers=2,
+        cls_dim=128,
+        cls_layers=2,
         dropout=0.,
-        gnn='gcn',
+        gnn='GS',
+        pooling='mean',
+        reweight=True,
+        pseudo=True,
+        ew_start=100,
+        ew_freq=20,
         lamb=0.8,
         mode='erm',
         act=F.relu,
+        bn=False,
         weight_decay=0.0001,
         lr=0.05,
         epoch=100,
         device='cuda:0',
         batch_size=0,
         num_neigh=-1,
         verbose=2,
@@ -96,76 +120,70 @@
             epoch=epoch,
             device=device,
             batch_size=batch_size,
             num_neigh=num_neigh,
             verbose=verbose,
             **kwargs)
 
-        assert mode in ['erm', 'mixup'], 'unsupport training mode'
+        assert mode in ['erm', 'mixup', 'mmd', 'adv'], 'unsupport training mode'
         
         self.gnn=gnn
         self.lamb=lamb
         self.mode=mode
+        self.bn=bn
+        self.pooling=pooling
+        self.cls_dim=cls_dim
+        self.cls_layers=cls_layers
+        self.reweight=reweight
+        self.ew_freq=ew_freq
+        self.ew_start=ew_start
+        self.pseudo=pseudo
 
     def init_model(self, **kwargs):
 
         if self.mode == 'mixup':
             return MixupBase(
                 in_dim=self.in_dim,
                 hid_dim=self.hid_dim,
                 num_classes=self.num_classes,
                 num_layers=self.num_layers,
                 dropout=self.dropout,
                 rw_lmda=self.lamb,
                 **kwargs
                 ).to(self.device)
         else:
-            return GNNBase(
-                in_dim=self.in_dim,
-                hid_dim=self.hid_dim,
-                num_classes=self.num_classes,
-                num_layers=self.num_layers,
+            return ReweightGNN(
+                input_dim=self.in_dim,
+                gnn_dim=self.hid_dim,
+                output_dim=self.num_classes,
+                cls_dim=self.cls_dim,
+                gnn_layers=self.num_layers,
+                cls_layers=self.cls_layers,
+                backbone=self.gnn,
+                pooling=self.pooling,
                 dropout=self.dropout,
-                gnn=self.gnn,
+                bn=self.bn,
+                rw_lmda=self.lamb,
                 **kwargs
                 ).to(self.device)
 
-    def forward_model(self, source_data, target_data, alpha):
-        target_feat = self.gnn.feat_bottleneck(target_data.x, target_data.edge_index)
-        target_logits = self.gnn.feat_classifier(target_feat, target_data.edge_index)
+    def forward_model(self, source_data, target_data, alpha, epoch):
+        target_feat, target_logits = self.gnn.forward(target_data, target_data.x)
         target_prob = F.softmax(target_logits, dim=1)
         target_pred = torch.max(target_prob, dim=1)[1]
 
-        src_edge_prob, tgt_edge_prob, tgt_true_edge_prob = self.cal_edge_prob_sep(source_data, target_data, target_pred)
-
-        reweight_matrix = torch.div(tgt_edge_prob, src_edge_prob)
-        reweight_matrix[torch.isinf(reweight_matrix)] = 1
-        reweight_matrix[torch.isnan(reweight_matrix)] = 1
-
-        num_nodes = source_data.x.shape[0] + target_data.x.shape[0]
-        label_pred = torch.cat((source_data.y, target_pred))
-        graph_label_one_hot = sp.csr_matrix(
-            (np.ones(num_nodes), (np.arange(num_nodes), label_pred.cpu().numpy())),
-            shape=(num_nodes, self.num_classes))
-        src_label_one_hot = sp.csr_matrix(
-            (np.ones(source_data.x.shape[0]), (np.arange(source_data.x.shape[0]), source_data.y.cpu().numpy())),
-            shape=(source_data.x.shape[0], self.num_classes))
-        
-        edge_weight = torch.ones(source_data.edge_index.shape[1]).to(self.device)
-        for i in range(self.num_classes):
-            for j in range(self.num_classes):
-                idx = np.intersect1d(
-                    np.where(np.in1d(source_data.edge_index[0].cpu().numpy(), graph_label_one_hot.getcol(j).nonzero()[0]))[0],
-                    np.where(np.in1d(source_data.edge_index[1].cpu().numpy(), src_label_one_hot.getcol(i).nonzero()[0]))[0])
-                edge_weight[idx] = reweight_matrix[i][j].item()
+        if self.reweight and (epoch + 1) >= self.ew_start:
+            if self.pseudo:
+                if (epoch + 1) % self.ew_freq == 0:
+                    self.cal_reweight(source_data, target_data, target_pred)
+            else:
+                if epoch == self.ew_start - 1:
+                    self.cal_reweight(source_data, target_data, target_pred)
         
-        edge_weight = (1 - self.lamb) * 1 + self.lamb * edge_weight
-
-        source_feat = self.gnn.feat_bottleneck(source_data.x, source_data.edge_index, edge_weight)
-        source_logits = self.gnn.feat_classifier(source_feat, source_data.edge_index, edge_weight)
+        source_feat, source_logits = self.gnn.forward(source_data, source_data.x)
         source_prob = F.softmax(source_logits, dim=1)
         source_pred = torch.max(source_prob, dim=1)[1]
 
         if self.mode == 'erm':
             loss = F.nll_loss(F.log_softmax(source_logits, dim=1), source_data.y)
         elif self.mode == 'adv':
             source_dlogits = self.domain_discriminator(GradReverse.apply(source_feat, alpha))
@@ -181,55 +199,35 @@
         elif self.mode == 'mmd':
             mmd_loss = MMD(source_feat, target_feat)
             loss = F.nll_loss(F.log_softmax(source_logits, dim=1), source_data.y)
             loss = loss + mmd_loss
 
         return loss, source_logits, target_logits
 
-    def forward_model_mixup(self, source_data, target_data):
-        source_data.edge_weight = torch.ones(source_data.edge_index.shape[1]).to(self.device)
-        target_data.edge_weight = torch.ones(target_data.edge_index.shape[1]).to(self.device)
-
+    def forward_model_mixup(self, source_data, target_data, epoch):
         target_feat = self.gnn.feat_bottleneck(
             target_data.x,
             target_data.edge_index,
             target_data.edge_index,
             1,
             np.arange(target_data.x.shape[0]),
             target_data.edge_weight
         )
         target_logits = self.gnn.feat_classifier(target_feat)
         target_prob = F.softmax(target_logits, dim=1)
         target_pred = torch.max(target_prob, dim=1)[1]
 
-        src_edge_prob, tgt_edge_prob, tgt_true_edge_prob = self.cal_edge_prob_sep(source_data, target_data, target_pred)
-
-        reweight_matrix = torch.div(tgt_edge_prob, src_edge_prob)
-        reweight_matrix[torch.isinf(reweight_matrix)] = 1
-        reweight_matrix[torch.isnan(reweight_matrix)] = 1
-
-        num_nodes = source_data.x.shape[0] + target_data.x.shape[0]
-        label_pred = torch.cat((source_data.y, target_pred))
-        graph_label_one_hot = sp.csr_matrix(
-            (np.ones(num_nodes), (np.arange(num_nodes), label_pred.cpu().numpy())),
-            shape=(num_nodes, self.num_classes))
-        src_label_one_hot = sp.csr_matrix(
-            (np.ones(source_data.x.shape[0]), (np.arange(source_data.x.shape[0]), source_data.y.cpu().numpy())),
-            shape=(source_data.x.shape[0], self.num_classes))
-        
-        edge_weight = torch.ones(source_data.edge_index.shape[1]).to(self.device)
-        for i in range(self.num_classes):
-            for j in range(self.num_classes):
-                idx = np.intersect1d(
-                    np.where(np.in1d(source_data.edge_index[0].cpu().numpy(), graph_label_one_hot.getcol(j).nonzero()[0]))[0],
-                    np.where(np.in1d(source_data.edge_index[1].cpu().numpy(), src_label_one_hot.getcol(i).nonzero()[0]))[0])
-                edge_weight[idx] = reweight_matrix[i][j].item()
+        if self.reweight and (epoch + 1) >= self.ew_start:
+            if self.pseudo:
+                if (epoch + 1) % self.ew_freq == 0:
+                    self.cal_reweight(source_data, target_data, target_pred)
+            else:
+                if epoch == self.ew_start - 1:
+                    self.cal_reweight(source_data, target_data, target_pred)
         
-        edge_weight = (1 - self.lamb) * 1 + self.lamb * edge_weight
-
         lam = np.random.beta(4.0, 4.0)
         data_b, id_new_value_old = self.shuffle_data(source_data)
         data_b = data_b.to(self.device)
 
         source_feat = self.gnn.feat_bottleneck(
             source_data.x,
             source_data.edge_index,
@@ -240,14 +238,18 @@
         source_logits = self.gnn.feat_classifier(source_feat)
 
         loss = F.nll_loss(F.log_softmax(source_logits, dim=1), source_data.y)
 
         return loss, source_logits, target_logits
 
     def fit(self, source_data, target_data):
+        if source_data.edge_weight is None:
+            source_data.edge_weight = torch.ones(source_data.edge_index.shape[1]).to(self.device)
+        if target_data.edge_weight is None:
+            target_data.edge_weight = torch.ones(target_data.edge_index.shape[1]).to(self.device)
 
         if self.batch_size == 0:
             self.source_batch_size = source_data.x.shape[0]
             source_loader = NeighborLoader(source_data,
                                 self.num_neigh,
                                 batch_size=self.source_batch_size)
             self.target_batch_size = target_data.x.shape[0]
@@ -291,17 +293,17 @@
             p = float(epoch) / self.epoch
             alpha = 2. / (1. + np.exp(-10. * p)) - 1
 
             for idx, (sampled_source_data, sampled_target_data) in enumerate(zip(source_loader, target_loader)):
                 self.gnn.train()
                 
                 if self.mode == 'mixup':
-                    loss, source_logits, target_logits = self.forward_model_mixup(sampled_source_data, sampled_target_data)
+                    loss, source_logits, target_logits = self.forward_model_mixup(sampled_source_data, sampled_target_data, epoch)
                 else:
-                    loss, source_logits, target_logits = self.forward_model(sampled_source_data, sampled_target_data, alpha)
+                    loss, source_logits, target_logits = self.forward_model(sampled_source_data, sampled_target_data, alpha, epoch)
                 epoch_loss += loss.item()
 
                 optimizer.zero_grad()
                 loss.backward()
                 optimizer.step()
 
                 if idx == 0:
@@ -316,14 +318,40 @@
 
             logger(epoch=epoch,
                    loss=epoch_loss,
                    source_train_acc=micro_f1_score,
                    time=time.time() - start_time,
                    verbose=self.verbose,
                    train=True)
+    
+    def cal_reweight(self, source_data, target_data, target_pred):
+        print('edge reweight...')
+        src_edge_prob, tgt_edge_prob, tgt_true_edge_prob = self.cal_edge_prob_sep(source_data, target_data, target_pred)
+
+        reweight_matrix = torch.div(tgt_edge_prob, src_edge_prob)
+        reweight_matrix[torch.isinf(reweight_matrix)] = 1
+        reweight_matrix[torch.isnan(reweight_matrix)] = 1
+
+        num_nodes = source_data.x.shape[0] + target_data.x.shape[0]
+        label_pred = torch.cat((source_data.y, target_pred))
+        graph_label_one_hot = sp.csr_matrix(
+            (np.ones(num_nodes), (np.arange(num_nodes), label_pred.cpu().numpy())),
+            shape=(num_nodes, self.num_classes))
+        src_label_one_hot = sp.csr_matrix(
+            (np.ones(source_data.x.shape[0]), (np.arange(source_data.x.shape[0]), source_data.y.cpu().numpy())),
+            shape=(source_data.x.shape[0], self.num_classes))
+        
+        edge_weight = torch.ones(source_data.edge_index.shape[1]).to(self.device)
+        for i in range(self.num_classes):
+            for j in range(self.num_classes):
+                idx = np.intersect1d(
+                    np.where(np.in1d(source_data.edge_index[0].cpu().numpy(), graph_label_one_hot.getcol(j).nonzero()[0]))[0],
+                    np.where(np.in1d(source_data.edge_index[1].cpu().numpy(), src_label_one_hot.getcol(i).nonzero()[0]))[0])
+                edge_weight[idx] = reweight_matrix[i][j].item()
+        source_data.edge_weight = edge_weight
 
     def cal_edge_prob_sep(self, src_graph, tgt_graph, tgt_pred):
         src_adj = to_dense_adj(src_graph.edge_index)[0].cpu().numpy()
         tgt_adj = to_dense_adj(tgt_graph.edge_index)[0].cpu().numpy()
     
         num_class = self.num_classes
         num_nodes_src = src_graph.x.shape[0]
@@ -406,15 +434,15 @@
         self.gnn.eval()
 
         with torch.no_grad():
             if self.mode == 'mixup':
                 data.edge_weight = torch.ones(data.edge_index.shape[1]).to(self.device)
                 logits = self.gnn(data.x, data.edge_index, data.edge_index, 1, np.arange(data.x.shape[0]), data.edge_weight)
             else:
-                logits = self.gnn(data.x, data.edge_index)
+                _, logits = self.gnn(data, data.x)
 
         return logits, data.y
 
     def shuffle_data(self, data):
         data = copy.deepcopy(data).to(self.device)
         id_new_value_old = np.arange(data.x.shape[0])
         idx = np.arange(data.x.shape[0])
```

### Comparing `pygda-0.0.3/pygda/models/udagcn.py` & `pygda-0.0.4/pygda/models/udagcn.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/nn/__init__.py` & `pygda-0.0.4/pygda/nn/__init__.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/nn/a2gnn_base.py` & `pygda-0.0.4/pygda/nn/a2gnn_base.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from .prop_gcn_conv import PropGCNConv
 from .reverse_layer import GradReverse
 
 
 class A2GNNBase(nn.Module):
     """
-    Unsupervised Domain Adaptive Graph Convolutional Networks (WWW-20)
+    Rethinking Propagation for Unsupervised Graph Domain Adaptation (AAAI-24).
 
     Parameters
     ----------
     in_dim : int
         Input dimension of model.
     hid_dim : int
         Hidden dimension of model.
```

### Comparing `pygda-0.0.3/pygda/nn/acdne_base.py` & `pygda-0.0.4/pygda/nn/acdne_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/nn/adagcn_base.py` & `pygda-0.0.4/pygda/nn/adagcn_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
                 x = self.dropout(x)
         
         return x
 
 
 class AdaGCNBase(nn.Module):
     """
-    Graph Transfer Learning via Adversarial Domain Adaptation with Graph Convolution (TKDE-22)
+    Graph Transfer Learning via Adversarial Domain Adaptation with Graph Convolution (TKDE-22).
 
     Parameters
     ----------
     in_dim : int
         Input dimension of model.
     hid_dim : int
         Hidden dimension of model.
```

### Comparing `pygda-0.0.3/pygda/nn/asn_base.py` & `pygda-0.0.4/pygda/nn/asn_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
             return eps.mul(std).add_(mu)
         else:
             return mu
 
 
 class ASNBase(nn.Module):
     """
-    Adversarial Separation Network for Cross-Network Node Classification (CIKM-21)
+    Adversarial Separation Network for Cross-Network Node Classification (CIKM-21).
 
     Parameters
     ----------
     in_dim : int
         Input dimension of model.
     hid_dim : int
         Hidden dimension of model.
```

### Comparing `pygda-0.0.3/pygda/nn/cached_gcn_conv.py` & `pygda-0.0.4/pygda/nn/cached_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/nn/cwgcn_base.py` & `pygda-0.0.4/pygda/nn/cwgcn_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/nn/deepwalk_pretrain.py` & `pygda-0.0.4/pygda/nn/deepwalk_pretrain.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/nn/dgda_base.py` & `pygda-0.0.4/pygda/nn/dgda_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/nn/gmm_clustering.py` & `pygda-0.0.4/pygda/nn/gmm_clustering.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/nn/gnn_base.py` & `pygda-0.0.4/pygda/nn/gnn_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/nn/grade_base.py` & `pygda-0.0.4/pygda/nn/grade_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import torch.nn.functional as F
 
 from torch_geometric.nn import GCNConv
 
 
 class GRADEBase(nn.Module):
     """
-    Non-IID Transfer Learning on Graphs (AAAI-23)
+    Non-IID Transfer Learning on Graphs (AAAI-23).
 
     Parameters
     ----------
     in_dim : int
         Input dimension of model.
     hid_dim : int
         Hidden dimension of model.
```

### Comparing `pygda-0.0.3/pygda/nn/jhgda_base.py` & `pygda-0.0.4/pygda/nn/jhgda_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             A_new = torch.matmul(torch.matmul(S.T, A_old), S)
 
         return S, X_new, A_new, Y_new, Y_new_prob
 
 
 class JHGDABase(nn.Module):
     """
-    Improving Graph Domain Adaptation with Network Hierarchy (CIKM-23)
+    Improving Graph Domain Adaptation with Network Hierarchy (CIKM-23).
 
     Parameters
     ----------
     in_dim : int
         Input dimension of model.
     hid_dim : int
         Hidden dimension of model.
```

### Comparing `pygda-0.0.3/pygda/nn/kbl_base.py` & `pygda-0.0.4/pygda/nn/kbl_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,26 +278,44 @@
     def similarity_cross_domain(self, x_src, x_tar, idx1, idx2):
         z_src = self.lin_self(x_src)
         z_tar = self.lin_self(x_tar)
         alpha = torch.nn.CosineSimilarity(dim=-1)((z_src[idx1] + self.biasatt(z_src[idx1])).unsqueeze(1), z_tar[idx2] + self.biasatt(z_tar[idx2]))
         alpha = torch.sigmoid(alpha)
 
         return alpha
+    
+    def similarity_cross_domain_batch(self, x_src, x_tar, idx1, idx2):
+        z_src = self.lin_self(x_src)
+        z_tar = self.lin_self(x_tar)
+        batch_size = 100
+        batch_alpha = None
+        for i in range(0, len(idx1), batch_size):
+            end = min(i + batch_size, len(idx1))
+            idx1_batch = idx1[i:end]
+            z_src_batch = z_src[idx1_batch]
+            alpha = torch.nn.CosineSimilarity(dim=-1)((z_src_batch + self.biasatt(z_src_batch)).unsqueeze(1), z_tar[idx2] + self.biasatt(z_tar[idx2]))
+            if i == 0:
+                batch_alpha = alpha
+            else:
+                batch_alpha = torch.cat((batch_alpha, alpha), dim=0)
+        alpha = torch.sigmoid(batch_alpha)
+
+        return alpha
 
     def forward_cross_domain(self, x_src, x_tar, idx1, idx2):
         z_src, z_tar = x_src, x_tar
         log_probs_clf_src = log_probs_clf_tar = None
 
         if self.use_clf:
             logits_src = self.lin_clf(F.dropout(F.relu(z_src), p=self.dropout, training=self.training))
             logits_tar = self.lin_clf(F.dropout(F.relu(z_tar), p=self.dropout, training=self.training))
             log_probs_clf_src = F.log_softmax(logits_src, dim=-1)
             log_probs_clf_tar = F.log_softmax(logits_tar, dim=-1)
 
-        alpha = self.similarity_cross_domain(z_src, z_tar, idx1, idx2)
+        alpha = self.similarity_cross_domain_batch(z_src, z_tar, idx1, idx2)
 
         return alpha.unsqueeze(-1), log_probs_clf_src, log_probs_clf_tar
 
     def similarity(self, x, idx1, idx2):
         z = self.lin_self(x)
         alpha = torch.nn.CosineSimilarity(dim=1)(z[idx1] + self.biasatt(z[idx1]), z[idx2] + self.biasatt(z[idx2]))
         alpha = torch.sigmoid(alpha)
```

### Comparing `pygda-0.0.3/pygda/nn/mixup_base.py` & `pygda-0.0.4/pygda/nn/mixup_base.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/nn/mixup_gcnconv.py` & `pygda-0.0.4/pygda/nn/mixup_gcnconv.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,16 +160,15 @@
                         self._cached_adj_t = edge_index
                 else:
                     edge_index = cache
 
         x = self.lin(x)
         
         # propagate_type: (x: Tensor, edge_weight: OptTensor)
-        out = self.propagate(edge_index, x=x, edge_weight=edge_weight,
-                             size=None, lmda = lmda, edge_rw = edge_rw) + self.lin_cen(x_cen)
+        out = self.propagate(edge_index=edge_index, x=x, edge_weight=edge_weight, lmda=lmda, edge_rw=edge_rw, size=None) + self.lin_cen(x_cen)
 
         if self.bias is not None:
             out += self.bias
 
         return out
 
     def message(self, x_j: Tensor, edge_weight: OptTensor, lmda, edge_rw) -> Tensor:
```

### Comparing `pygda-0.0.3/pygda/nn/ppmi_conv.py` & `pygda-0.0.4/pygda/nn/ppmi_conv.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/nn/prop_gcn_conv.py` & `pygda-0.0.4/pygda/nn/prop_gcn_conv.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/nn/reweight_gnn.py` & `pygda-0.0.4/pygda/nn/reweight_gnn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 import torch
 from torch import nn
 import torch.nn.functional as F
-from torch_geometric.nn import MessagePassing
 from torch_geometric.nn.dense.linear import Linear
 from torch_geometric.nn.conv.gcn_conv import gcn_norm
 from torch_sparse import SparseTensor
 import torch_geometric.nn as pyg_nn
 from torch import Tensor
 from torch.nn import Parameter
 from torch_sparse import SparseTensor
 from typing import Optional
-from torch_geometric.nn.conv import MessagePassing
 from torch_geometric.nn.inits import zeros
 from torch_geometric.typing import Adj, OptPairTensor, OptTensor
 from torch_sparse import matmul as torch_sparse_matmul
-from torch_geometric.nn.conv.gcn_conv import gcn_norm
 
 
 def spmm(src: Adj, other: Tensor, reduce: str = "sum") -> Tensor:
     """Matrix product of sparse matrix with dense matrix.
 
     Args:
         src (Tensor or torch_sparse.SparseTensor]): The input sparse matrix,
@@ -39,15 +36,15 @@
     if reduce in ['sum', 'add']:
         return torch.sparse.mm(src, other)
 
     # TODO: Support `mean` reduction for PyTorch SparseTensor
     raise ValueError(f"`{reduce}` reduction is not supported for "
                      f"`torch.sparse.Tensor`.")
 
-class GCN_reweight(MessagePassing):
+class GCN_reweight(pyg_nn.MessagePassing):
     r"""The graph convolutional operator from the `"Semi-supervised
     Classification with Graph Convolutional Networks"
     <https://arxiv.org/abs/1609.02907>`_ paper
 
     .. math::
         \mathbf{X}^{\prime} = \mathbf{\hat{D}}^{-1/2} \mathbf{\hat{A}}
         \mathbf{\hat{D}}^{-1/2} \mathbf{X} \mathbf{\Theta},
@@ -99,38 +96,44 @@
           edge weights :math:`(|\mathcal{E}|)` *(optional)*
         - **output:** node features :math:`(|\mathcal{V}|, F_{out})`
     """
 
     _cached_edge_index: Optional[OptPairTensor]
     _cached_adj_t: Optional[SparseTensor]
 
-    def __init__(self, in_channels: int, out_channels: int, aggr: str,
-                 improved: bool = False, cached: bool = False,
-                 add_self_loops: bool = False, normalize: bool = True,
-                 bias: bool = True, **kwargs):
+    def __init__(
+        self,
+        in_channels: int,
+        out_channels: int,
+        aggr: str,
+        improved: bool = False,
+        cached: bool = False,
+        add_self_loops: bool = False,
+        normalize: bool = True,
+        bias: bool = True,
+        **kwargs
+        ):
 
-        kwargs.setdefault('aggr', "add")
-        super().__init__(**kwargs, flow ="target_to_source")
+        # kwargs.setdefault('aggr', "add")
+        super(GCN_reweight, self).__init__(aggr=aggr, flow ="target_to_source")
 
         self.in_channels = in_channels
         self.out_channels = out_channels
         self.improved = improved
         self.cached = cached
         self.add_self_loops = add_self_loops
         if aggr == "add":
             self.normalize = False
         else:
             self.normalize = True
-        #self.normalize = normalize
-
+        
         self._cached_edge_index = None
         self._cached_adj_t = None
 
-        self.lin = Linear(in_channels, out_channels, bias=False,
-                          weight_initializer='glorot')
+        self.lin = Linear(in_channels, out_channels, bias=False, weight_initializer='glorot')
 
         if bias:
             self.bias = Parameter(torch.Tensor(out_channels))
         else:
             self.register_parameter('bias', None)
 
         self.reset_parameters()
@@ -138,20 +141,17 @@
     def reset_parameters(self):
         self.lin.reset_parameters()
         zeros(self.bias)
         self._cached_edge_index = None
         self._cached_adj_t = None
 
 
-    def forward(self, x: Tensor, edge_index: Adj,
-                edge_weight: OptTensor=None, lmda = 1) -> Tensor:
-        """"""
+    def forward(self, x, edge_index, edge_weight, lmda):
         edge_rw = edge_weight
         edge_weight = torch.ones_like(edge_rw)
-        #edge_weight = None
         if self.normalize:
             if isinstance(edge_index, Tensor):
                 cache = self._cached_edge_index
                 if cache is None:
                     edge_index, edge_weight = gcn_norm(  # yapf: disable
                         edge_index, edge_weight, x.size(self.node_dim),
                         self.improved, self.add_self_loops, dtype=x.dtype)
@@ -170,47 +170,46 @@
                         self._cached_adj_t = edge_index
                 else:
                     edge_index = cache
 
         x = self.lin(x)
 
         # propagate_type: (x: Tensor, edge_weight: OptTensor)
-        out = self.propagate(edge_index, x=x, edge_weight=edge_weight,
-                             size=None, lmda = lmda, edge_rw = edge_rw)
+        out = self.propagate(edge_index, size=None, x=x, edge_weight=edge_weight, edge_rw=edge_rw, lmda=lmda)
 
         if self.bias is not None:
             out = out + self.bias
 
         return out
 
-    def message(self, x_j: Tensor, edge_weight: OptTensor, lmda, edge_rw) -> Tensor:
+    def message(self, x_j, edge_index, edge_weight, edge_rw, lmda):
         x_j = (edge_weight.view(-1, 1) * x_j)
         x_j = (1-lmda) * x_j + (lmda) * (edge_rw.view(-1, 1) * x_j)
         return x_j
 
     def message_and_aggregate(self, adj_t: SparseTensor, x: Tensor) -> Tensor:
         return spmm(adj_t, x, reduce=self.aggr)
 
+
 class GS_reweight(pyg_nn.MessagePassing):
-    def __init__(self, in_channels, out_channels, reducer, 
-                 normalize_embedding=False):
+    def __init__(self, in_channels, out_channels, reducer, normalize_embedding=False):
         super(GS_reweight, self).__init__(aggr=reducer, flow ="target_to_source")
         self.lin = torch.nn.Linear(in_channels, out_channels)
         self.agg_lin = torch.nn.Linear(out_channels + in_channels, out_channels)
 
         self.normalize_emb = normalize_embedding
 
     def forward(self, x, edge_index, edge_weight, lmda):
         num_nodes = x.size(0)
-        return self.propagate(edge_index, size=(num_nodes, num_nodes), x=x, edge_weight = edge_weight, lmda = lmda)
+        return self.propagate(edge_index, size=(num_nodes, num_nodes), x=x, edge_weight=edge_weight, lmda=lmda)
 
     def message(self, x_j, edge_index, edge_weight, lmda):
         x_j = self.lin(x_j)
         x_j = (1-lmda) * x_j + (lmda) * (edge_weight.view(-1, 1) * x_j)
-        #print(lmda)
+
         return x_j
 
     def update(self, aggr_out, x):
         aggr_out = torch.cat((aggr_out, x), dim=-1)
         aggr_out = self.agg_lin(aggr_out)
         aggr_out = F.relu(aggr_out)
 
@@ -270,15 +269,15 @@
             for i in range(cls_layers - 2):
                 self.mlp_classify.append(nn.Linear(cls_dim, cls_dim))
             self.mlp_classify.append(nn.Linear(cls_dim, output_dim))
 
     def forward(self, data, h):
         x, edge_index, edge_weight = h, data.edge_index, data.edge_weight
         for i, layer in enumerate(self.conv):
-            x = layer(x, edge_index, edge_weight=edge_weight, lmda = self.lmda)
+            x = layer(x, edge_index, edge_weight, self.lmda)
             # if self.bn and (i != len(self.conv) - 1):
             #     x = self.bns[i](x)
             x = F.relu(x)
             x = F.dropout(x, p=self.dropout)
 
         y = x
         for i in range(len(self.mlp_classify)):
```

### Comparing `pygda-0.0.3/pygda/nn/sagda_base.py` & `pygda-0.0.4/pygda/nn/sagda_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,15 +105,15 @@
                 x = self.act(x)
                 x = self.dropout_layers[i](x)
         return x
 
 
 class SAGDABase(nn.Module):
     """
-    SA-GDA: Spectral Augmentation for Graph Domain Adaptation (MM-23)
+    SA-GDA: Spectral Augmentation for Graph Domain Adaptation (MM-23).
 
     Parameters
     ----------
     in_dim : int
         Input dimension of model.
     hid_dim : int
         Hidden dimension of model.
```

### Comparing `pygda-0.0.3/pygda/nn/udagcn_base.py` & `pygda-0.0.4/pygda/nn/udagcn_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 x = self.act(x)
                 x = self.dropout_layers[i](x)
         return x
 
 
 class UDAGCNBase(nn.Module):
     """
-    Unsupervised Domain Adaptive Graph Convolutional Networks (WWW-20)
+    Unsupervised Domain Adaptive Graph Convolutional Networks (WWW-20).
 
     Parameters
     ----------
     in_dim : int
         Input dimension of model.
     hid_dim : int
         Hidden dimension of model.
@@ -78,15 +78,15 @@
         super(UDAGCNBase, self).__init__()
 
         self.ppmi = ppmi
 
         self.encoder = GNN(in_dim=in_dim, hid_dim=hid_dim, gnn_type='gcn', act=act, num_layers=num_layers)
         
         if self.ppmi:
-            self.ppmi_encoder = GNN(in_dim=in_dim, hid_dim=hid_dim, base_model=self.encoder, gnn_type='ppmi', path_len=10) 
+            self.ppmi_encoder = GNN(in_dim=in_dim, hid_dim=hid_dim, base_model=self.encoder, num_layers=num_layers, gnn_type='ppmi', path_len=10) 
         
         self.cls_model = nn.Sequential(nn.Linear(hid_dim, num_classes))
 
         self.domain_model = nn.Sequential(
             nn.Linear(hid_dim, adv_dim),
             nn.ReLU(),
             nn.Dropout(0.1),
```

### Comparing `pygda-0.0.3/pygda/utils/mmd.py` & `pygda-0.0.4/pygda/utils/mmd.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/utils/svd_transform.py` & `pygda-0.0.4/pygda/utils/svd_transform.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pygda/utils/utility.py` & `pygda-0.0.4/pygda/utils/utility.py`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/pyproject.toml` & `pygda-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pygda-0.0.3/PKG-INFO` & `pygda-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 Metadata-Version: 2.1
 Name: pygda
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python library for Graph Domain Adaptation
 Author: pygda-team
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: numpy
 Requires-Dist: scikit-learn
 Requires-Dist: scipy
 Requires-Dist: tqdm
 Project-URL: Repository, https://github.com/pygda-team/pygda
 
 ![](docs/pygda_logo.png)
 -----
+[![PyPI version](https://badge.fury.io/py/pygda.svg)](https://badge.fury.io/py/pygda)
+[![Documentation Status](https://readthedocs.org/projects/pygda/badge/?version=stable)](https://pygda.readthedocs.io/en/stable/?badge=stable)
+[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/pygda-team/pygda/issues)
 
 PyGDA is a **Python library** for **Graph Domain Adaptation** built upon [PyTorch](https://pytorch.org/) and [PyG](https://pytorch-geometric.readthedocs.io/en/latest/) to easily train graph domain adaptation models in a [sklearn](https://scikit-learn.org/stable/) style. PyGDA includes **15+** graph domain adaptation models. See examples with PyGDA below!
 
 **Graph Domain Adaptation Using PyGDA with 5 Lines of Code**
 ```
 from pygda.models import A2GNN
```

