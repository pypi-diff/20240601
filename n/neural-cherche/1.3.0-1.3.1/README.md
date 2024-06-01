# Comparing `tmp/neural_cherche-1.3.0.tar.gz` & `tmp/neural_cherche-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neural_cherche-1.3.0.tar", last modified: Thu May 30 21:17:14 2024, max compression
+gzip compressed data, was "neural_cherche-1.3.1.tar", last modified: Sat Jun  1 14:12:02 2024, max compression
```

## Comparing `neural_cherche-1.3.0.tar` & `neural_cherche-1.3.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.676685 neural_cherche-1.3.0/
--rw-r--r--   0 raphael    (502) staff       (20)     1071 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/LICENSE
--rw-r--r--   0 raphael    (502) staff       (20)    11184 2024-05-30 21:17:14.676570 neural_cherche-1.3.0/PKG-INFO
--rw-r--r--   0 raphael    (502) staff       (20)     9504 2024-05-30 21:11:56.000000 neural_cherche-1.3.0/README.md
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.668168 neural_cherche-1.3.0/neural_cherche/
--rw-r--r--   0 raphael    (502) staff       (20)       69 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)       63 2024-05-30 20:50:57.000000 neural_cherche-1.3.0/neural_cherche/__version__.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.669513 neural_cherche-1.3.0/neural_cherche/losses/
--rw-r--r--   0 raphael    (502) staff       (20)      120 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/losses/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)     2794 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/losses/flops.py
--rw-r--r--   0 raphael    (502) staff       (20)     2054 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/losses/ranking.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.670761 neural_cherche-1.3.0/neural_cherche/models/
--rw-r--r--   0 raphael    (502) staff       (20)      142 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/models/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)     4127 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/models/base.py
--rw-r--r--   0 raphael    (502) staff       (20)     9224 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/models/colbert.py
--rw-r--r--   0 raphael    (502) staff       (20)    10137 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/models/sparse_embed.py
--rw-r--r--   0 raphael    (502) staff       (20)    10951 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/models/splade.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.671541 neural_cherche-1.3.0/neural_cherche/rank/
--rw-r--r--   0 raphael    (502) staff       (20)      105 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/rank/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)    10616 2024-05-24 13:32:45.000000 neural_cherche-1.3.0/neural_cherche/rank/colbert.py
--rw-r--r--   0 raphael    (502) staff       (20)    11941 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/rank/sparse_embed.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.672947 neural_cherche-1.3.0/neural_cherche/retrieve/
--rw-r--r--   0 raphael    (502) staff       (20)      230 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/retrieve/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)     5808 2024-05-30 20:34:19.000000 neural_cherche-1.3.0/neural_cherche/retrieve/bm25.py
--rw-r--r--   0 raphael    (502) staff       (20)     6111 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/retrieve/colbert.py
--rw-r--r--   0 raphael    (502) staff       (20)    15777 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/retrieve/sparse_embed.py
--rw-r--r--   0 raphael    (502) staff       (20)     4857 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/retrieve/splade.py
--rw-r--r--   0 raphael    (502) staff       (20)     7034 2024-05-30 20:44:49.000000 neural_cherche-1.3.0/neural_cherche/retrieve/tfidf.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.673782 neural_cherche-1.3.0/neural_cherche/train/
--rw-r--r--   0 raphael    (502) staff       (20)      198 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/train/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)     2937 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/train/train_colbert.py
--rw-r--r--   0 raphael    (502) staff       (20)     4993 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/train/train_sparse_embed.py
--rw-r--r--   0 raphael    (502) staff       (20)     3782 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/train/train_splade.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.675103 neural_cherche-1.3.0/neural_cherche/utils/
--rw-r--r--   0 raphael    (502) staff       (20)      543 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/utils/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)     2456 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/utils/colbert_scores.py
--rw-r--r--   0 raphael    (502) staff       (20)     8255 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/utils/dense_scores.py
--rw-r--r--   0 raphael    (502) staff       (20)     5487 2024-05-30 20:44:19.000000 neural_cherche-1.3.0/neural_cherche/utils/evaluate.py
--rw-r--r--   0 raphael    (502) staff       (20)      544 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/utils/freeze.py
--rw-r--r--   0 raphael    (502) staff       (20)     1844 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/utils/iter.py
--rw-r--r--   0 raphael    (502) staff       (20)     2262 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/utils/sparse_scores.py
--rw-r--r--   0 raphael    (502) staff       (20)      208 2024-05-23 22:30:32.000000 neural_cherche-1.3.0/neural_cherche/utils/warnings.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-05-30 21:17:14.675309 neural_cherche-1.3.0/neural_cherche.egg-info/
--rw-r--r--   0 raphael    (502) staff       (20)    11184 2024-05-30 21:17:14.000000 neural_cherche-1.3.0/neural_cherche.egg-info/PKG-INFO
--rw-r--r--   0 raphael    (502) staff       (20)     1280 2024-05-30 21:17:14.000000 neural_cherche-1.3.0/neural_cherche.egg-info/SOURCES.txt
--rw-r--r--   0 raphael    (502) staff       (20)        1 2024-05-30 21:17:14.000000 neural_cherche-1.3.0/neural_cherche.egg-info/dependency_links.txt
--rw-r--r--   0 raphael    (502) staff       (20)      404 2024-05-30 21:17:14.000000 neural_cherche-1.3.0/neural_cherche.egg-info/requires.txt
--rw-r--r--   0 raphael    (502) staff       (20)       15 2024-05-30 21:17:14.000000 neural_cherche-1.3.0/neural_cherche.egg-info/top_level.txt
--rw-r--r--   0 raphael    (502) staff       (20)       79 2024-05-30 21:17:14.676874 neural_cherche-1.3.0/setup.cfg
--rw-r--r--   0 raphael    (502) staff       (20)     1507 2024-05-30 21:14:35.000000 neural_cherche-1.3.0/setup.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:12:02.682812 neural_cherche-1.3.1/
+-rw-r--r--   0 raphael    (502) staff       (20)     1071 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/LICENSE
+-rw-r--r--   0 raphael    (502) staff       (20)    11184 2024-06-01 14:12:02.682684 neural_cherche-1.3.1/PKG-INFO
+-rw-r--r--   0 raphael    (502) staff       (20)     9504 2024-05-30 21:25:54.000000 neural_cherche-1.3.1/README.md
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:12:02.676563 neural_cherche-1.3.1/neural_cherche/
+-rw-r--r--   0 raphael    (502) staff       (20)       69 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)       63 2024-06-01 14:11:23.000000 neural_cherche-1.3.1/neural_cherche/__version__.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:12:02.677590 neural_cherche-1.3.1/neural_cherche/losses/
+-rw-r--r--   0 raphael    (502) staff       (20)      120 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/losses/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     2794 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/losses/flops.py
+-rw-r--r--   0 raphael    (502) staff       (20)     2054 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/losses/ranking.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:12:02.678326 neural_cherche-1.3.1/neural_cherche/models/
+-rw-r--r--   0 raphael    (502) staff       (20)      142 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/models/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4127 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/models/base.py
+-rw-r--r--   0 raphael    (502) staff       (20)     9224 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/models/colbert.py
+-rw-r--r--   0 raphael    (502) staff       (20)    10137 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/models/sparse_embed.py
+-rw-r--r--   0 raphael    (502) staff       (20)    10951 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/models/splade.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:12:02.678704 neural_cherche-1.3.1/neural_cherche/rank/
+-rw-r--r--   0 raphael    (502) staff       (20)      105 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/rank/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)    10616 2024-05-24 13:32:45.000000 neural_cherche-1.3.1/neural_cherche/rank/colbert.py
+-rw-r--r--   0 raphael    (502) staff       (20)    11941 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/rank/sparse_embed.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:12:02.679508 neural_cherche-1.3.1/neural_cherche/retrieve/
+-rw-r--r--   0 raphael    (502) staff       (20)      230 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/retrieve/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     5808 2024-05-30 20:34:19.000000 neural_cherche-1.3.1/neural_cherche/retrieve/bm25.py
+-rw-r--r--   0 raphael    (502) staff       (20)     6111 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/retrieve/colbert.py
+-rw-r--r--   0 raphael    (502) staff       (20)    15777 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/retrieve/sparse_embed.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4857 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/retrieve/splade.py
+-rw-r--r--   0 raphael    (502) staff       (20)     7034 2024-05-30 20:44:49.000000 neural_cherche-1.3.1/neural_cherche/retrieve/tfidf.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:12:02.680051 neural_cherche-1.3.1/neural_cherche/train/
+-rw-r--r--   0 raphael    (502) staff       (20)      198 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/train/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     2937 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/train/train_colbert.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4993 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/train/train_sparse_embed.py
+-rw-r--r--   0 raphael    (502) staff       (20)     3782 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/train/train_splade.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:12:02.681107 neural_cherche-1.3.1/neural_cherche/utils/
+-rw-r--r--   0 raphael    (502) staff       (20)      543 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/utils/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     2456 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/utils/colbert_scores.py
+-rw-r--r--   0 raphael    (502) staff       (20)     8255 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/utils/dense_scores.py
+-rw-r--r--   0 raphael    (502) staff       (20)     5487 2024-05-30 20:44:19.000000 neural_cherche-1.3.1/neural_cherche/utils/evaluate.py
+-rw-r--r--   0 raphael    (502) staff       (20)      544 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/utils/freeze.py
+-rw-r--r--   0 raphael    (502) staff       (20)     1844 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/utils/iter.py
+-rw-r--r--   0 raphael    (502) staff       (20)     2262 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/utils/sparse_scores.py
+-rw-r--r--   0 raphael    (502) staff       (20)      208 2024-05-23 22:30:32.000000 neural_cherche-1.3.1/neural_cherche/utils/warnings.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:12:02.681298 neural_cherche-1.3.1/neural_cherche.egg-info/
+-rw-r--r--   0 raphael    (502) staff       (20)    11184 2024-06-01 14:12:02.000000 neural_cherche-1.3.1/neural_cherche.egg-info/PKG-INFO
+-rw-r--r--   0 raphael    (502) staff       (20)     1280 2024-06-01 14:12:02.000000 neural_cherche-1.3.1/neural_cherche.egg-info/SOURCES.txt
+-rw-r--r--   0 raphael    (502) staff       (20)        1 2024-06-01 14:12:02.000000 neural_cherche-1.3.1/neural_cherche.egg-info/dependency_links.txt
+-rw-r--r--   0 raphael    (502) staff       (20)      404 2024-06-01 14:12:02.000000 neural_cherche-1.3.1/neural_cherche.egg-info/requires.txt
+-rw-r--r--   0 raphael    (502) staff       (20)       15 2024-06-01 14:12:02.000000 neural_cherche-1.3.1/neural_cherche.egg-info/top_level.txt
+-rw-r--r--   0 raphael    (502) staff       (20)       79 2024-06-01 14:12:02.683088 neural_cherche-1.3.1/setup.cfg
+-rw-r--r--   0 raphael    (502) staff       (20)     1507 2024-06-01 14:11:34.000000 neural_cherche-1.3.1/setup.py
```

### Comparing `neural_cherche-1.3.0/LICENSE` & `neural_cherche-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/PKG-INFO` & `neural_cherche-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural_cherche
-Version: 1.3.0
+Version: 1.3.1
 Summary: Sparse Embeddings for Neural Search.
 Home-page: https://github.com/raphaelsty/neural-cherche
 Download-URL: https://github.com/user/neural-cherche/archive/v_01.tar.gz
 Author: Raphael Sourty
 Author-email: raphael.sourty@gmail.com
 Keywords: neural search,information retrieval,semantic search,SparseEmbed,Google Research,Splade,Stanford,ColBERT
 Classifier: Programming Language :: Python :: 3
@@ -13,29 +13,29 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=1.13
 Requires-Dist: tqdm>=4.66
 Requires-Dist: transformers>=4.34.0
 Requires-Dist: sentence-transformers>=2.2.2
-Requires-Dist: lenlp>=1.0.3
+Requires-Dist: lenlp==1.0.5
 Provides-Extra: eval
 Requires-Dist: torch>=1.13; extra == "eval"
 Requires-Dist: tqdm>=4.66; extra == "eval"
 Requires-Dist: transformers>=4.34.0; extra == "eval"
 Requires-Dist: sentence-transformers>=2.2.2; extra == "eval"
-Requires-Dist: lenlp>=1.0.3; extra == "eval"
+Requires-Dist: lenlp==1.0.5; extra == "eval"
 Requires-Dist: ranx>=0.3.16; extra == "eval"
 Requires-Dist: beir>=2.0.0; extra == "eval"
 Provides-Extra: dev
 Requires-Dist: torch>=1.13; extra == "dev"
 Requires-Dist: tqdm>=4.66; extra == "dev"
 Requires-Dist: transformers>=4.34.0; extra == "dev"
 Requires-Dist: sentence-transformers>=2.2.2; extra == "dev"
-Requires-Dist: lenlp>=1.0.3; extra == "dev"
+Requires-Dist: lenlp==1.0.5; extra == "dev"
 Requires-Dist: ranx>=0.3.16; extra == "dev"
 Requires-Dist: beir>=2.0.0; extra == "dev"
 Requires-Dist: mkdocs-material==9.2.8; extra == "dev"
 Requires-Dist: mkdocs-awesome-pages-plugin==2.9.2; extra == "dev"
 Requires-Dist: mkdocs-jupyter==0.24.7; extra == "dev"
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: neural_cherche Version: 1.3.0 Summary: Sparse
+Metadata-Version: 2.1 Name: neural_cherche Version: 1.3.1 Summary: Sparse
 Embeddings for Neural Search. Home-page: https://github.com/raphaelsty/neural-
 cherche Download-URL: https://github.com/user/neural-cherche/archive/
 v_01.tar.gz Author: Raphael Sourty Author-email: raphael.sourty@gmail.com
 Keywords: neural search,information retrieval,semantic
 search,SparseEmbed,Google Research,Splade,Stanford,ColBERT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 torch>=1.13 Requires-Dist: tqdm>=4.66 Requires-Dist: transformers>=4.34.0
-Requires-Dist: sentence-transformers>=2.2.2 Requires-Dist: lenlp>=1.0.3
+Requires-Dist: sentence-transformers>=2.2.2 Requires-Dist: lenlp==1.0.5
 Provides-Extra: eval Requires-Dist: torch>=1.13; extra == "eval" Requires-Dist:
 tqdm>=4.66; extra == "eval" Requires-Dist: transformers>=4.34.0; extra ==
 "eval" Requires-Dist: sentence-transformers>=2.2.2; extra == "eval" Requires-
-Dist: lenlp>=1.0.3; extra == "eval" Requires-Dist: ranx>=0.3.16; extra ==
+Dist: lenlp==1.0.5; extra == "eval" Requires-Dist: ranx>=0.3.16; extra ==
 "eval" Requires-Dist: beir>=2.0.0; extra == "eval" Provides-Extra: dev
 Requires-Dist: torch>=1.13; extra == "dev" Requires-Dist: tqdm>=4.66; extra ==
 "dev" Requires-Dist: transformers>=4.34.0; extra == "dev" Requires-Dist:
-sentence-transformers>=2.2.2; extra == "dev" Requires-Dist: lenlp>=1.0.3; extra
+sentence-transformers>=2.2.2; extra == "dev" Requires-Dist: lenlp==1.0.5; extra
 == "dev" Requires-Dist: ranx>=0.3.16; extra == "dev" Requires-Dist:
 beir>=2.0.0; extra == "dev" Requires-Dist: mkdocs-material==9.2.8; extra ==
 "dev" Requires-Dist: mkdocs-awesome-pages-plugin==2.9.2; extra == "dev"
 Requires-Dist: mkdocs-jupyter==0.24.7; extra == "dev"
                          ************ NNeeuurraall--CChheerrcchhee ************
                                  Neural Search
                               [docs/img/logo.png]
```

### Comparing `neural_cherche-1.3.0/README.md` & `neural_cherche-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/losses/flops.py` & `neural_cherche-1.3.1/neural_cherche/losses/flops.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/losses/ranking.py` & `neural_cherche-1.3.1/neural_cherche/losses/ranking.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/models/base.py` & `neural_cherche-1.3.1/neural_cherche/models/base.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/models/colbert.py` & `neural_cherche-1.3.1/neural_cherche/models/colbert.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/models/sparse_embed.py` & `neural_cherche-1.3.1/neural_cherche/models/sparse_embed.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/models/splade.py` & `neural_cherche-1.3.1/neural_cherche/models/splade.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/rank/colbert.py` & `neural_cherche-1.3.1/neural_cherche/rank/colbert.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/rank/sparse_embed.py` & `neural_cherche-1.3.1/neural_cherche/rank/sparse_embed.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/retrieve/bm25.py` & `neural_cherche-1.3.1/neural_cherche/retrieve/bm25.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/retrieve/colbert.py` & `neural_cherche-1.3.1/neural_cherche/retrieve/colbert.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/retrieve/sparse_embed.py` & `neural_cherche-1.3.1/neural_cherche/retrieve/sparse_embed.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/retrieve/splade.py` & `neural_cherche-1.3.1/neural_cherche/retrieve/splade.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/retrieve/tfidf.py` & `neural_cherche-1.3.1/neural_cherche/retrieve/tfidf.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/train/train_colbert.py` & `neural_cherche-1.3.1/neural_cherche/train/train_colbert.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/train/train_sparse_embed.py` & `neural_cherche-1.3.1/neural_cherche/train/train_sparse_embed.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/train/train_splade.py` & `neural_cherche-1.3.1/neural_cherche/train/train_splade.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/utils/__init__.py` & `neural_cherche-1.3.1/neural_cherche/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/utils/colbert_scores.py` & `neural_cherche-1.3.1/neural_cherche/utils/colbert_scores.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/utils/dense_scores.py` & `neural_cherche-1.3.1/neural_cherche/utils/dense_scores.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/utils/evaluate.py` & `neural_cherche-1.3.1/neural_cherche/utils/evaluate.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/utils/freeze.py` & `neural_cherche-1.3.1/neural_cherche/utils/freeze.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/utils/iter.py` & `neural_cherche-1.3.1/neural_cherche/utils/iter.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche/utils/sparse_scores.py` & `neural_cherche-1.3.1/neural_cherche/utils/sparse_scores.py`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/neural_cherche.egg-info/PKG-INFO` & `neural_cherche-1.3.1/neural_cherche.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neural_cherche
-Version: 1.3.0
+Version: 1.3.1
 Summary: Sparse Embeddings for Neural Search.
 Home-page: https://github.com/raphaelsty/neural-cherche
 Download-URL: https://github.com/user/neural-cherche/archive/v_01.tar.gz
 Author: Raphael Sourty
 Author-email: raphael.sourty@gmail.com
 Keywords: neural search,information retrieval,semantic search,SparseEmbed,Google Research,Splade,Stanford,ColBERT
 Classifier: Programming Language :: Python :: 3
@@ -13,29 +13,29 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: torch>=1.13
 Requires-Dist: tqdm>=4.66
 Requires-Dist: transformers>=4.34.0
 Requires-Dist: sentence-transformers>=2.2.2
-Requires-Dist: lenlp>=1.0.3
+Requires-Dist: lenlp==1.0.5
 Provides-Extra: eval
 Requires-Dist: torch>=1.13; extra == "eval"
 Requires-Dist: tqdm>=4.66; extra == "eval"
 Requires-Dist: transformers>=4.34.0; extra == "eval"
 Requires-Dist: sentence-transformers>=2.2.2; extra == "eval"
-Requires-Dist: lenlp>=1.0.3; extra == "eval"
+Requires-Dist: lenlp==1.0.5; extra == "eval"
 Requires-Dist: ranx>=0.3.16; extra == "eval"
 Requires-Dist: beir>=2.0.0; extra == "eval"
 Provides-Extra: dev
 Requires-Dist: torch>=1.13; extra == "dev"
 Requires-Dist: tqdm>=4.66; extra == "dev"
 Requires-Dist: transformers>=4.34.0; extra == "dev"
 Requires-Dist: sentence-transformers>=2.2.2; extra == "dev"
-Requires-Dist: lenlp>=1.0.3; extra == "dev"
+Requires-Dist: lenlp==1.0.5; extra == "dev"
 Requires-Dist: ranx>=0.3.16; extra == "dev"
 Requires-Dist: beir>=2.0.0; extra == "dev"
 Requires-Dist: mkdocs-material==9.2.8; extra == "dev"
 Requires-Dist: mkdocs-awesome-pages-plugin==2.9.2; extra == "dev"
 Requires-Dist: mkdocs-jupyter==0.24.7; extra == "dev"
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: neural_cherche Version: 1.3.0 Summary: Sparse
+Metadata-Version: 2.1 Name: neural_cherche Version: 1.3.1 Summary: Sparse
 Embeddings for Neural Search. Home-page: https://github.com/raphaelsty/neural-
 cherche Download-URL: https://github.com/user/neural-cherche/archive/
 v_01.tar.gz Author: Raphael Sourty Author-email: raphael.sourty@gmail.com
 Keywords: neural search,information retrieval,semantic
 search,SparseEmbed,Google Research,Splade,Stanford,ColBERT Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.6
 Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
 torch>=1.13 Requires-Dist: tqdm>=4.66 Requires-Dist: transformers>=4.34.0
-Requires-Dist: sentence-transformers>=2.2.2 Requires-Dist: lenlp>=1.0.3
+Requires-Dist: sentence-transformers>=2.2.2 Requires-Dist: lenlp==1.0.5
 Provides-Extra: eval Requires-Dist: torch>=1.13; extra == "eval" Requires-Dist:
 tqdm>=4.66; extra == "eval" Requires-Dist: transformers>=4.34.0; extra ==
 "eval" Requires-Dist: sentence-transformers>=2.2.2; extra == "eval" Requires-
-Dist: lenlp>=1.0.3; extra == "eval" Requires-Dist: ranx>=0.3.16; extra ==
+Dist: lenlp==1.0.5; extra == "eval" Requires-Dist: ranx>=0.3.16; extra ==
 "eval" Requires-Dist: beir>=2.0.0; extra == "eval" Provides-Extra: dev
 Requires-Dist: torch>=1.13; extra == "dev" Requires-Dist: tqdm>=4.66; extra ==
 "dev" Requires-Dist: transformers>=4.34.0; extra == "dev" Requires-Dist:
-sentence-transformers>=2.2.2; extra == "dev" Requires-Dist: lenlp>=1.0.3; extra
+sentence-transformers>=2.2.2; extra == "dev" Requires-Dist: lenlp==1.0.5; extra
 == "dev" Requires-Dist: ranx>=0.3.16; extra == "dev" Requires-Dist:
 beir>=2.0.0; extra == "dev" Requires-Dist: mkdocs-material==9.2.8; extra ==
 "dev" Requires-Dist: mkdocs-awesome-pages-plugin==2.9.2; extra == "dev"
 Requires-Dist: mkdocs-jupyter==0.24.7; extra == "dev"
                          ************ NNeeuurraall--CChheerrcchhee ************
                                  Neural Search
                               [docs/img/logo.png]
```

### Comparing `neural_cherche-1.3.0/neural_cherche.egg-info/SOURCES.txt` & `neural_cherche-1.3.1/neural_cherche.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neural_cherche-1.3.0/setup.py` & `neural_cherche-1.3.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 base_packages = [
     "torch >= 1.13",
     "tqdm >= 4.66",
     "transformers >= 4.34.0",
     "sentence-transformers >= 2.2.2",
-    "lenlp >= 1.0.3",
+    "lenlp == 1.0.5",
 ]
 
 
 eval = ["ranx >= 0.3.16", "beir >= 2.0.0"]
 
 dev = [
     "mkdocs-material == 9.2.8",
```

