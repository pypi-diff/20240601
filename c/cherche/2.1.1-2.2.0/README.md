# Comparing `tmp/cherche-2.1.1.tar.gz` & `tmp/cherche-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cherche-2.1.1.tar", last modified: Sat Jun  1 14:07:18 2024, max compression
+gzip compressed data, was "cherche-2.2.0.tar", last modified: Sat Jun  1 16:54:51 2024, max compression
```

## Comparing `cherche-2.1.1.tar` & `cherche-2.2.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:07:18.578915 cherche-2.1.1/
--rw-r--r--   0 raphael    (502) staff       (20)     1071 2024-06-01 14:06:46.000000 cherche-2.1.1/LICENSE
--rw-r--r--   0 raphael    (502) staff       (20)    10360 2024-06-01 14:07:18.578749 cherche-2.1.1/PKG-INFO
--rw-r--r--   0 raphael    (502) staff       (20)     7658 2024-06-01 14:06:46.000000 cherche-2.1.1/README.md
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:07:18.561272 cherche-2.1.1/cherche/
--rw-r--r--   0 raphael    (502) staff       (20)      134 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)       63 2024-06-01 14:06:51.000000 cherche-2.1.1/cherche/__version__.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:07:18.562976 cherche-2.1.1/cherche/compose/
--rw-r--r--   0 raphael    (502) staff       (20)      151 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/compose/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)     6368 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/compose/base.py
--rw-r--r--   0 raphael    (502) staff       (20)     8823 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/compose/intersection_union_vote.py
--rw-r--r--   0 raphael    (502) staff       (20)    18160 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/compose/pipeline.py
--rw-r--r--   0 raphael    (502) staff       (20)     4608 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/compose/test_compose.py
--rw-r--r--   0 raphael    (502) staff       (20)     6904 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/compose/test_union_inter.py
--rw-r--r--   0 raphael    (502) staff       (20)     1980 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/compose/test_vote.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:07:18.563495 cherche-2.1.1/cherche/data/
--rw-r--r--   0 raphael    (502) staff       (20)      104 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/data/__init__.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:07:18.569412 cherche-2.1.1/cherche/data/semanlink/
--rw-r--r--   0 raphael    (502) staff       (20)   899186 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/data/semanlink/arxiv.json
--rw-r--r--   0 raphael    (502) staff       (20)  8324401 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/data/semanlink/docs.json
--rw-r--r--   0 raphael    (502) staff       (20)  4587473 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/data/semanlink/tags.json
--rw-r--r--   0 raphael    (502) staff       (20)     3013 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/data/semanlink.py
--rw-r--r--   0 raphael    (502) staff       (20)    29097 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/data/towns.json
--rw-r--r--   0 raphael    (502) staff       (20)     1577 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/data/towns.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:07:18.572057 cherche-2.1.1/cherche/evaluate/
--rw-r--r--   0 raphael    (502) staff       (20)       59 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/evaluate/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)     4094 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/evaluate/evaluate.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:07:18.572317 cherche-2.1.1/cherche/index/
--rw-r--r--   0 raphael    (502) staff       (20)       52 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/index/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)     5056 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/index/faiss_index.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:07:18.572560 cherche-2.1.1/cherche/qa/
--rw-r--r--   0 raphael    (502) staff       (20)       37 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/qa/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)     6442 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/qa/qa.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:07:18.573049 cherche-2.1.1/cherche/query/
--rw-r--r--   0 raphael    (502) staff       (20)      110 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/query/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)     1153 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/query/base.py
--rw-r--r--   0 raphael    (502) staff       (20)     4455 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/query/norvig.py
--rw-r--r--   0 raphael    (502) staff       (20)     5053 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/query/prf.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:07:18.574012 cherche-2.1.1/cherche/rank/
--rw-r--r--   0 raphael    (502) staff       (20)      217 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/rank/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)    10310 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/rank/base.py
--rw-r--r--   0 raphael    (502) staff       (20)     6692 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/rank/cross_encoder.py
--rw-r--r--   0 raphael    (502) staff       (20)     4155 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/rank/dpr.py
--rw-r--r--   0 raphael    (502) staff       (20)     4767 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/rank/embedding.py
--rw-r--r--   0 raphael    (502) staff       (20)     3805 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/rank/encoder.py
--rw-r--r--   0 raphael    (502) staff       (20)     3867 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/rank/test_rank.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:07:18.575338 cherche-2.1.1/cherche/retrieve/
--rw-r--r--   0 raphael    (502) staff       (20)      367 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/retrieve/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)     2438 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/retrieve/base.py
--rw-r--r--   0 raphael    (502) staff       (20)     3609 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/retrieve/bm25.py
--rw-r--r--   0 raphael    (502) staff       (20)     4637 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/retrieve/dpr.py
--rw-r--r--   0 raphael    (502) staff       (20)     4659 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/retrieve/embedding.py
--rw-r--r--   0 raphael    (502) staff       (20)     4495 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/retrieve/encoder.py
--rw-r--r--   0 raphael    (502) staff       (20)     4822 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/retrieve/flash.py
--rw-r--r--   0 raphael    (502) staff       (20)     5047 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/retrieve/fuzz.py
--rw-r--r--   0 raphael    (502) staff       (20)     3455 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/retrieve/lunr.py
--rw-r--r--   0 raphael    (502) staff       (20)     4139 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/retrieve/test_retrieve.py
--rw-r--r--   0 raphael    (502) staff       (20)     7687 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/retrieve/tfidf.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:07:18.575822 cherche-2.1.1/cherche/utils/
--rw-r--r--   0 raphael    (502) staff       (20)      174 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/utils/__init__.py
--rw-r--r--   0 raphael    (502) staff       (20)     1468 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/utils/batch.py
--rw-r--r--   0 raphael    (502) staff       (20)     1754 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/utils/quantize.py
--rw-r--r--   0 raphael    (502) staff       (20)     1983 2024-06-01 14:06:46.000000 cherche-2.1.1/cherche/utils/topk.py
-drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 14:07:18.576047 cherche-2.1.1/cherche.egg-info/
--rw-r--r--   0 raphael    (502) staff       (20)    10360 2024-06-01 14:07:18.000000 cherche-2.1.1/cherche.egg-info/PKG-INFO
--rw-r--r--   0 raphael    (502) staff       (20)     1462 2024-06-01 14:07:18.000000 cherche-2.1.1/cherche.egg-info/SOURCES.txt
--rw-r--r--   0 raphael    (502) staff       (20)        1 2024-06-01 14:07:18.000000 cherche-2.1.1/cherche.egg-info/dependency_links.txt
--rw-r--r--   0 raphael    (502) staff       (20)      788 2024-06-01 14:07:18.000000 cherche-2.1.1/cherche.egg-info/requires.txt
--rw-r--r--   0 raphael    (502) staff       (20)        8 2024-06-01 14:07:18.000000 cherche-2.1.1/cherche.egg-info/top_level.txt
--rw-r--r--   0 raphael    (502) staff       (20)       79 2024-06-01 14:07:18.579212 cherche-2.1.1/setup.cfg
--rw-r--r--   0 raphael    (502) staff       (20)     1767 2024-06-01 14:06:46.000000 cherche-2.1.1/setup.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 16:54:51.406441 cherche-2.2.0/
+-rw-r--r--   0 raphael    (502) staff       (20)     1071 2024-06-01 16:54:16.000000 cherche-2.2.0/LICENSE
+-rw-r--r--   0 raphael    (502) staff       (20)    10360 2024-06-01 16:54:51.406342 cherche-2.2.0/PKG-INFO
+-rw-r--r--   0 raphael    (502) staff       (20)     7658 2024-06-01 16:54:16.000000 cherche-2.2.0/README.md
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 16:54:51.390591 cherche-2.2.0/cherche/
+-rw-r--r--   0 raphael    (502) staff       (20)      134 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)       63 2024-06-01 16:54:44.000000 cherche-2.2.0/cherche/__version__.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 16:54:51.392475 cherche-2.2.0/cherche/compose/
+-rw-r--r--   0 raphael    (502) staff       (20)      151 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/compose/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     6368 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/compose/base.py
+-rw-r--r--   0 raphael    (502) staff       (20)     8823 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/compose/intersection_union_vote.py
+-rw-r--r--   0 raphael    (502) staff       (20)    18160 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/compose/pipeline.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4608 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/compose/test_compose.py
+-rw-r--r--   0 raphael    (502) staff       (20)     6904 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/compose/test_union_inter.py
+-rw-r--r--   0 raphael    (502) staff       (20)     1980 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/compose/test_vote.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 16:54:51.393052 cherche-2.2.0/cherche/data/
+-rw-r--r--   0 raphael    (502) staff       (20)      104 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/data/__init__.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 16:54:51.397540 cherche-2.2.0/cherche/data/semanlink/
+-rw-r--r--   0 raphael    (502) staff       (20)   899186 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/data/semanlink/arxiv.json
+-rw-r--r--   0 raphael    (502) staff       (20)  8324401 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/data/semanlink/docs.json
+-rw-r--r--   0 raphael    (502) staff       (20)  4587473 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/data/semanlink/tags.json
+-rw-r--r--   0 raphael    (502) staff       (20)     3013 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/data/semanlink.py
+-rw-r--r--   0 raphael    (502) staff       (20)    29097 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/data/towns.json
+-rw-r--r--   0 raphael    (502) staff       (20)     1577 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/data/towns.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 16:54:51.399894 cherche-2.2.0/cherche/evaluate/
+-rw-r--r--   0 raphael    (502) staff       (20)       59 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/evaluate/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4094 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/evaluate/evaluate.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 16:54:51.400161 cherche-2.2.0/cherche/index/
+-rw-r--r--   0 raphael    (502) staff       (20)       52 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/index/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     5056 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/index/faiss_index.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 16:54:51.400430 cherche-2.2.0/cherche/qa/
+-rw-r--r--   0 raphael    (502) staff       (20)       37 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/qa/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     6442 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/qa/qa.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 16:54:51.400908 cherche-2.2.0/cherche/query/
+-rw-r--r--   0 raphael    (502) staff       (20)      110 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/query/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     1153 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/query/base.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4455 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/query/norvig.py
+-rw-r--r--   0 raphael    (502) staff       (20)     5053 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/query/prf.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 16:54:51.401834 cherche-2.2.0/cherche/rank/
+-rw-r--r--   0 raphael    (502) staff       (20)      217 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/rank/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)    10310 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/rank/base.py
+-rw-r--r--   0 raphael    (502) staff       (20)     6692 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/rank/cross_encoder.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4155 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/rank/dpr.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4767 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/rank/embedding.py
+-rw-r--r--   0 raphael    (502) staff       (20)     3805 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/rank/encoder.py
+-rw-r--r--   0 raphael    (502) staff       (20)     3867 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/rank/test_rank.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 16:54:51.403284 cherche-2.2.0/cherche/retrieve/
+-rw-r--r--   0 raphael    (502) staff       (20)      367 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/retrieve/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     2438 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/retrieve/base.py
+-rw-r--r--   0 raphael    (502) staff       (20)     3609 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/retrieve/bm25.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4637 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/retrieve/dpr.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4659 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/retrieve/embedding.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4495 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/retrieve/encoder.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4822 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/retrieve/flash.py
+-rw-r--r--   0 raphael    (502) staff       (20)     5047 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/retrieve/fuzz.py
+-rw-r--r--   0 raphael    (502) staff       (20)     3455 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/retrieve/lunr.py
+-rw-r--r--   0 raphael    (502) staff       (20)     4139 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/retrieve/test_retrieve.py
+-rw-r--r--   0 raphael    (502) staff       (20)     7687 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/retrieve/tfidf.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 16:54:51.403802 cherche-2.2.0/cherche/utils/
+-rw-r--r--   0 raphael    (502) staff       (20)      174 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/utils/__init__.py
+-rw-r--r--   0 raphael    (502) staff       (20)     1468 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/utils/batch.py
+-rw-r--r--   0 raphael    (502) staff       (20)     1754 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/utils/quantize.py
+-rw-r--r--   0 raphael    (502) staff       (20)     1983 2024-06-01 16:54:16.000000 cherche-2.2.0/cherche/utils/topk.py
+drwxr-xr-x   0 raphael    (502) staff       (20)        0 2024-06-01 16:54:51.403992 cherche-2.2.0/cherche.egg-info/
+-rw-r--r--   0 raphael    (502) staff       (20)    10360 2024-06-01 16:54:51.000000 cherche-2.2.0/cherche.egg-info/PKG-INFO
+-rw-r--r--   0 raphael    (502) staff       (20)     1462 2024-06-01 16:54:51.000000 cherche-2.2.0/cherche.egg-info/SOURCES.txt
+-rw-r--r--   0 raphael    (502) staff       (20)        1 2024-06-01 16:54:51.000000 cherche-2.2.0/cherche.egg-info/dependency_links.txt
+-rw-r--r--   0 raphael    (502) staff       (20)      788 2024-06-01 16:54:51.000000 cherche-2.2.0/cherche.egg-info/requires.txt
+-rw-r--r--   0 raphael    (502) staff       (20)        8 2024-06-01 16:54:51.000000 cherche-2.2.0/cherche.egg-info/top_level.txt
+-rw-r--r--   0 raphael    (502) staff       (20)       79 2024-06-01 16:54:51.406674 cherche-2.2.0/setup.cfg
+-rw-r--r--   0 raphael    (502) staff       (20)     1767 2024-06-01 16:54:16.000000 cherche-2.2.0/setup.py
```

### Comparing `cherche-2.1.1/LICENSE` & `cherche-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/PKG-INFO` & `cherche-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 Metadata-Version: 2.1
 Name: cherche
-Version: 2.1.1
+Version: 2.2.0
 Summary: Neural Search
 Home-page: https://github.com/raphaelsty/cherche
 Download-URL: https://github.com/user/cherche/archive/v_01.tar.gz
 Author: Raphael Sourty
 Author-email: raphael.sourty@gmail.com
 License: MIT
 Keywords: neural search,information retrieval,question answering,semantic search
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.23.5
-Requires-Dist: scikit-learn>=1.1.2
+Requires-Dist: scikit-learn>=1.5.0
 Requires-Dist: lunr>=0.6.2
 Requires-Dist: rapidfuzz>=3.0.0
 Requires-Dist: flashtext>=2.7
 Requires-Dist: tqdm>=4.62.3
 Requires-Dist: scipy>=1.7.3
-Requires-Dist: lenlp==1.0.5
+Requires-Dist: lenlp==1.1.0
 Provides-Extra: cpu
 Requires-Dist: numpy>=1.23.5; extra == "cpu"
-Requires-Dist: scikit-learn>=1.1.2; extra == "cpu"
+Requires-Dist: scikit-learn>=1.5.0; extra == "cpu"
 Requires-Dist: lunr>=0.6.2; extra == "cpu"
 Requires-Dist: rapidfuzz>=3.0.0; extra == "cpu"
 Requires-Dist: flashtext>=2.7; extra == "cpu"
 Requires-Dist: tqdm>=4.62.3; extra == "cpu"
 Requires-Dist: scipy>=1.7.3; extra == "cpu"
-Requires-Dist: lenlp==1.0.5; extra == "cpu"
+Requires-Dist: lenlp==1.1.0; extra == "cpu"
 Requires-Dist: sentence-transformers>=2.2.2; extra == "cpu"
 Requires-Dist: faiss-cpu>=1.7.4; extra == "cpu"
 Provides-Extra: gpu
 Requires-Dist: numpy>=1.23.5; extra == "gpu"
-Requires-Dist: scikit-learn>=1.1.2; extra == "gpu"
+Requires-Dist: scikit-learn>=1.5.0; extra == "gpu"
 Requires-Dist: lunr>=0.6.2; extra == "gpu"
 Requires-Dist: rapidfuzz>=3.0.0; extra == "gpu"
 Requires-Dist: flashtext>=2.7; extra == "gpu"
 Requires-Dist: tqdm>=4.62.3; extra == "gpu"
 Requires-Dist: scipy>=1.7.3; extra == "gpu"
-Requires-Dist: lenlp==1.0.5; extra == "gpu"
+Requires-Dist: lenlp==1.1.0; extra == "gpu"
 Requires-Dist: sentence-transformers>=2.2.2; extra == "gpu"
 Requires-Dist: faiss-gpu>=1.7.4; extra == "gpu"
 Provides-Extra: dev
 Requires-Dist: numpy>=1.23.5; extra == "dev"
-Requires-Dist: scikit-learn>=1.1.2; extra == "dev"
+Requires-Dist: scikit-learn>=1.5.0; extra == "dev"
 Requires-Dist: lunr>=0.6.2; extra == "dev"
 Requires-Dist: rapidfuzz>=3.0.0; extra == "dev"
 Requires-Dist: flashtext>=2.7; extra == "dev"
 Requires-Dist: tqdm>=4.62.3; extra == "dev"
 Requires-Dist: scipy>=1.7.3; extra == "dev"
-Requires-Dist: lenlp==1.0.5; extra == "dev"
+Requires-Dist: lenlp==1.1.0; extra == "dev"
 Requires-Dist: sentence-transformers>=2.2.2; extra == "dev"
 Requires-Dist: faiss-cpu>=1.7.4; extra == "dev"
 Requires-Dist: numpydoc>=1.4.0; extra == "dev"
 Requires-Dist: mkdocs_material>=8.3.5; extra == "dev"
 Requires-Dist: mkdocs-awesome-pages-plugin>=2.7.0; extra == "dev"
 Requires-Dist: mkdocs-jupyter>=0.21.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0; extra == "dev"
```

#### html2text {}

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1 Name: cherche Version: 2.1.1 Summary: Neural Search Home-
+Metadata-Version: 2.1 Name: cherche Version: 2.2.0 Summary: Neural Search Home-
 page: https://github.com/raphaelsty/cherche Download-URL: https://github.com/
 user/cherche/archive/v_01.tar.gz Author: Raphael Sourty Author-email:
 raphael.sourty@gmail.com License: MIT Keywords: neural search,information
 retrieval,question answering,semantic search Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: numpy>=1.23.5
-Requires-Dist: scikit-learn>=1.1.2 Requires-Dist: lunr>=0.6.2 Requires-Dist:
+Requires-Dist: scikit-learn>=1.5.0 Requires-Dist: lunr>=0.6.2 Requires-Dist:
 rapidfuzz>=3.0.0 Requires-Dist: flashtext>=2.7 Requires-Dist: tqdm>=4.62.3
-Requires-Dist: scipy>=1.7.3 Requires-Dist: lenlp==1.0.5 Provides-Extra: cpu
+Requires-Dist: scipy>=1.7.3 Requires-Dist: lenlp==1.1.0 Provides-Extra: cpu
 Requires-Dist: numpy>=1.23.5; extra == "cpu" Requires-Dist: scikit-
-learn>=1.1.2; extra == "cpu" Requires-Dist: lunr>=0.6.2; extra == "cpu"
+learn>=1.5.0; extra == "cpu" Requires-Dist: lunr>=0.6.2; extra == "cpu"
 Requires-Dist: rapidfuzz>=3.0.0; extra == "cpu" Requires-Dist: flashtext>=2.7;
 extra == "cpu" Requires-Dist: tqdm>=4.62.3; extra == "cpu" Requires-Dist:
-scipy>=1.7.3; extra == "cpu" Requires-Dist: lenlp==1.0.5; extra == "cpu"
+scipy>=1.7.3; extra == "cpu" Requires-Dist: lenlp==1.1.0; extra == "cpu"
 Requires-Dist: sentence-transformers>=2.2.2; extra == "cpu" Requires-Dist:
 faiss-cpu>=1.7.4; extra == "cpu" Provides-Extra: gpu Requires-Dist:
-numpy>=1.23.5; extra == "gpu" Requires-Dist: scikit-learn>=1.1.2; extra ==
+numpy>=1.23.5; extra == "gpu" Requires-Dist: scikit-learn>=1.5.0; extra ==
 "gpu" Requires-Dist: lunr>=0.6.2; extra == "gpu" Requires-Dist:
 rapidfuzz>=3.0.0; extra == "gpu" Requires-Dist: flashtext>=2.7; extra == "gpu"
 Requires-Dist: tqdm>=4.62.3; extra == "gpu" Requires-Dist: scipy>=1.7.3; extra
-== "gpu" Requires-Dist: lenlp==1.0.5; extra == "gpu" Requires-Dist: sentence-
+== "gpu" Requires-Dist: lenlp==1.1.0; extra == "gpu" Requires-Dist: sentence-
 transformers>=2.2.2; extra == "gpu" Requires-Dist: faiss-gpu>=1.7.4; extra ==
 "gpu" Provides-Extra: dev Requires-Dist: numpy>=1.23.5; extra == "dev"
-Requires-Dist: scikit-learn>=1.1.2; extra == "dev" Requires-Dist: lunr>=0.6.2;
+Requires-Dist: scikit-learn>=1.5.0; extra == "dev" Requires-Dist: lunr>=0.6.2;
 extra == "dev" Requires-Dist: rapidfuzz>=3.0.0; extra == "dev" Requires-Dist:
 flashtext>=2.7; extra == "dev" Requires-Dist: tqdm>=4.62.3; extra == "dev"
-Requires-Dist: scipy>=1.7.3; extra == "dev" Requires-Dist: lenlp==1.0.5; extra
+Requires-Dist: scipy>=1.7.3; extra == "dev" Requires-Dist: lenlp==1.1.0; extra
 == "dev" Requires-Dist: sentence-transformers>=2.2.2; extra == "dev" Requires-
 Dist: faiss-cpu>=1.7.4; extra == "dev" Requires-Dist: numpydoc>=1.4.0; extra ==
 "dev" Requires-Dist: mkdocs_material>=8.3.5; extra == "dev" Requires-Dist:
 mkdocs-awesome-pages-plugin>=2.7.0; extra == "dev" Requires-Dist: mkdocs-
 jupyter>=0.21.0; extra == "dev" Requires-Dist: pytest-cov>=4.0.0; extra ==
 "dev" Requires-Dist: pytest>=7.3.1; extra == "dev" Requires-Dist:
 isort>=5.12.0; extra == "dev" Requires-Dist: ipywidgets>=8.0.6; extra == "dev"
```

### Comparing `cherche-2.1.1/README.md` & `cherche-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/compose/base.py` & `cherche-2.2.0/cherche/compose/base.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/compose/intersection_union_vote.py` & `cherche-2.2.0/cherche/compose/intersection_union_vote.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/compose/pipeline.py` & `cherche-2.2.0/cherche/compose/pipeline.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/compose/test_compose.py` & `cherche-2.2.0/cherche/compose/test_compose.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/compose/test_union_inter.py` & `cherche-2.2.0/cherche/compose/test_union_inter.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/compose/test_vote.py` & `cherche-2.2.0/cherche/compose/test_vote.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/data/semanlink/arxiv.json` & `cherche-2.2.0/cherche/data/semanlink/arxiv.json`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/data/semanlink/docs.json` & `cherche-2.2.0/cherche/data/semanlink/docs.json`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/data/semanlink/tags.json` & `cherche-2.2.0/cherche/data/semanlink/tags.json`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/data/semanlink.py` & `cherche-2.2.0/cherche/data/semanlink.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/data/towns.json` & `cherche-2.2.0/cherche/data/towns.json`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/data/towns.py` & `cherche-2.2.0/cherche/data/towns.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/evaluate/evaluate.py` & `cherche-2.2.0/cherche/evaluate/evaluate.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/index/faiss_index.py` & `cherche-2.2.0/cherche/index/faiss_index.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/qa/qa.py` & `cherche-2.2.0/cherche/qa/qa.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/query/base.py` & `cherche-2.2.0/cherche/query/base.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/query/norvig.py` & `cherche-2.2.0/cherche/query/norvig.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/query/prf.py` & `cherche-2.2.0/cherche/query/prf.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/rank/base.py` & `cherche-2.2.0/cherche/rank/base.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/rank/cross_encoder.py` & `cherche-2.2.0/cherche/rank/cross_encoder.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/rank/dpr.py` & `cherche-2.2.0/cherche/rank/dpr.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/rank/embedding.py` & `cherche-2.2.0/cherche/rank/embedding.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/rank/encoder.py` & `cherche-2.2.0/cherche/rank/encoder.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/rank/test_rank.py` & `cherche-2.2.0/cherche/rank/test_rank.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/retrieve/base.py` & `cherche-2.2.0/cherche/retrieve/base.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/retrieve/bm25.py` & `cherche-2.2.0/cherche/retrieve/bm25.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/retrieve/dpr.py` & `cherche-2.2.0/cherche/retrieve/dpr.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/retrieve/embedding.py` & `cherche-2.2.0/cherche/retrieve/embedding.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/retrieve/encoder.py` & `cherche-2.2.0/cherche/retrieve/encoder.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/retrieve/flash.py` & `cherche-2.2.0/cherche/retrieve/flash.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/retrieve/fuzz.py` & `cherche-2.2.0/cherche/retrieve/fuzz.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/retrieve/lunr.py` & `cherche-2.2.0/cherche/retrieve/lunr.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/retrieve/test_retrieve.py` & `cherche-2.2.0/cherche/retrieve/test_retrieve.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/retrieve/tfidf.py` & `cherche-2.2.0/cherche/retrieve/tfidf.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/utils/batch.py` & `cherche-2.2.0/cherche/utils/batch.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/utils/quantize.py` & `cherche-2.2.0/cherche/utils/quantize.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche/utils/topk.py` & `cherche-2.2.0/cherche/utils/topk.py`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/cherche.egg-info/PKG-INFO` & `cherche-2.2.0/cherche.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 Metadata-Version: 2.1
 Name: cherche
-Version: 2.1.1
+Version: 2.2.0
 Summary: Neural Search
 Home-page: https://github.com/raphaelsty/cherche
 Download-URL: https://github.com/user/cherche/archive/v_01.tar.gz
 Author: Raphael Sourty
 Author-email: raphael.sourty@gmail.com
 License: MIT
 Keywords: neural search,information retrieval,question answering,semantic search
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.23.5
-Requires-Dist: scikit-learn>=1.1.2
+Requires-Dist: scikit-learn>=1.5.0
 Requires-Dist: lunr>=0.6.2
 Requires-Dist: rapidfuzz>=3.0.0
 Requires-Dist: flashtext>=2.7
 Requires-Dist: tqdm>=4.62.3
 Requires-Dist: scipy>=1.7.3
-Requires-Dist: lenlp==1.0.5
+Requires-Dist: lenlp==1.1.0
 Provides-Extra: cpu
 Requires-Dist: numpy>=1.23.5; extra == "cpu"
-Requires-Dist: scikit-learn>=1.1.2; extra == "cpu"
+Requires-Dist: scikit-learn>=1.5.0; extra == "cpu"
 Requires-Dist: lunr>=0.6.2; extra == "cpu"
 Requires-Dist: rapidfuzz>=3.0.0; extra == "cpu"
 Requires-Dist: flashtext>=2.7; extra == "cpu"
 Requires-Dist: tqdm>=4.62.3; extra == "cpu"
 Requires-Dist: scipy>=1.7.3; extra == "cpu"
-Requires-Dist: lenlp==1.0.5; extra == "cpu"
+Requires-Dist: lenlp==1.1.0; extra == "cpu"
 Requires-Dist: sentence-transformers>=2.2.2; extra == "cpu"
 Requires-Dist: faiss-cpu>=1.7.4; extra == "cpu"
 Provides-Extra: gpu
 Requires-Dist: numpy>=1.23.5; extra == "gpu"
-Requires-Dist: scikit-learn>=1.1.2; extra == "gpu"
+Requires-Dist: scikit-learn>=1.5.0; extra == "gpu"
 Requires-Dist: lunr>=0.6.2; extra == "gpu"
 Requires-Dist: rapidfuzz>=3.0.0; extra == "gpu"
 Requires-Dist: flashtext>=2.7; extra == "gpu"
 Requires-Dist: tqdm>=4.62.3; extra == "gpu"
 Requires-Dist: scipy>=1.7.3; extra == "gpu"
-Requires-Dist: lenlp==1.0.5; extra == "gpu"
+Requires-Dist: lenlp==1.1.0; extra == "gpu"
 Requires-Dist: sentence-transformers>=2.2.2; extra == "gpu"
 Requires-Dist: faiss-gpu>=1.7.4; extra == "gpu"
 Provides-Extra: dev
 Requires-Dist: numpy>=1.23.5; extra == "dev"
-Requires-Dist: scikit-learn>=1.1.2; extra == "dev"
+Requires-Dist: scikit-learn>=1.5.0; extra == "dev"
 Requires-Dist: lunr>=0.6.2; extra == "dev"
 Requires-Dist: rapidfuzz>=3.0.0; extra == "dev"
 Requires-Dist: flashtext>=2.7; extra == "dev"
 Requires-Dist: tqdm>=4.62.3; extra == "dev"
 Requires-Dist: scipy>=1.7.3; extra == "dev"
-Requires-Dist: lenlp==1.0.5; extra == "dev"
+Requires-Dist: lenlp==1.1.0; extra == "dev"
 Requires-Dist: sentence-transformers>=2.2.2; extra == "dev"
 Requires-Dist: faiss-cpu>=1.7.4; extra == "dev"
 Requires-Dist: numpydoc>=1.4.0; extra == "dev"
 Requires-Dist: mkdocs_material>=8.3.5; extra == "dev"
 Requires-Dist: mkdocs-awesome-pages-plugin>=2.7.0; extra == "dev"
 Requires-Dist: mkdocs-jupyter>=0.21.0; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0; extra == "dev"
```

#### html2text {}

```diff
@@ -1,36 +1,36 @@
-Metadata-Version: 2.1 Name: cherche Version: 2.1.1 Summary: Neural Search Home-
+Metadata-Version: 2.1 Name: cherche Version: 2.2.0 Summary: Neural Search Home-
 page: https://github.com/raphaelsty/cherche Download-URL: https://github.com/
 user/cherche/archive/v_01.tar.gz Author: Raphael Sourty Author-email:
 raphael.sourty@gmail.com License: MIT Keywords: neural search,information
 retrieval,question answering,semantic search Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Requires-Python: >=3.6 Description-Content-
 Type: text/markdown License-File: LICENSE Requires-Dist: numpy>=1.23.5
-Requires-Dist: scikit-learn>=1.1.2 Requires-Dist: lunr>=0.6.2 Requires-Dist:
+Requires-Dist: scikit-learn>=1.5.0 Requires-Dist: lunr>=0.6.2 Requires-Dist:
 rapidfuzz>=3.0.0 Requires-Dist: flashtext>=2.7 Requires-Dist: tqdm>=4.62.3
-Requires-Dist: scipy>=1.7.3 Requires-Dist: lenlp==1.0.5 Provides-Extra: cpu
+Requires-Dist: scipy>=1.7.3 Requires-Dist: lenlp==1.1.0 Provides-Extra: cpu
 Requires-Dist: numpy>=1.23.5; extra == "cpu" Requires-Dist: scikit-
-learn>=1.1.2; extra == "cpu" Requires-Dist: lunr>=0.6.2; extra == "cpu"
+learn>=1.5.0; extra == "cpu" Requires-Dist: lunr>=0.6.2; extra == "cpu"
 Requires-Dist: rapidfuzz>=3.0.0; extra == "cpu" Requires-Dist: flashtext>=2.7;
 extra == "cpu" Requires-Dist: tqdm>=4.62.3; extra == "cpu" Requires-Dist:
-scipy>=1.7.3; extra == "cpu" Requires-Dist: lenlp==1.0.5; extra == "cpu"
+scipy>=1.7.3; extra == "cpu" Requires-Dist: lenlp==1.1.0; extra == "cpu"
 Requires-Dist: sentence-transformers>=2.2.2; extra == "cpu" Requires-Dist:
 faiss-cpu>=1.7.4; extra == "cpu" Provides-Extra: gpu Requires-Dist:
-numpy>=1.23.5; extra == "gpu" Requires-Dist: scikit-learn>=1.1.2; extra ==
+numpy>=1.23.5; extra == "gpu" Requires-Dist: scikit-learn>=1.5.0; extra ==
 "gpu" Requires-Dist: lunr>=0.6.2; extra == "gpu" Requires-Dist:
 rapidfuzz>=3.0.0; extra == "gpu" Requires-Dist: flashtext>=2.7; extra == "gpu"
 Requires-Dist: tqdm>=4.62.3; extra == "gpu" Requires-Dist: scipy>=1.7.3; extra
-== "gpu" Requires-Dist: lenlp==1.0.5; extra == "gpu" Requires-Dist: sentence-
+== "gpu" Requires-Dist: lenlp==1.1.0; extra == "gpu" Requires-Dist: sentence-
 transformers>=2.2.2; extra == "gpu" Requires-Dist: faiss-gpu>=1.7.4; extra ==
 "gpu" Provides-Extra: dev Requires-Dist: numpy>=1.23.5; extra == "dev"
-Requires-Dist: scikit-learn>=1.1.2; extra == "dev" Requires-Dist: lunr>=0.6.2;
+Requires-Dist: scikit-learn>=1.5.0; extra == "dev" Requires-Dist: lunr>=0.6.2;
 extra == "dev" Requires-Dist: rapidfuzz>=3.0.0; extra == "dev" Requires-Dist:
 flashtext>=2.7; extra == "dev" Requires-Dist: tqdm>=4.62.3; extra == "dev"
-Requires-Dist: scipy>=1.7.3; extra == "dev" Requires-Dist: lenlp==1.0.5; extra
+Requires-Dist: scipy>=1.7.3; extra == "dev" Requires-Dist: lenlp==1.1.0; extra
 == "dev" Requires-Dist: sentence-transformers>=2.2.2; extra == "dev" Requires-
 Dist: faiss-cpu>=1.7.4; extra == "dev" Requires-Dist: numpydoc>=1.4.0; extra ==
 "dev" Requires-Dist: mkdocs_material>=8.3.5; extra == "dev" Requires-Dist:
 mkdocs-awesome-pages-plugin>=2.7.0; extra == "dev" Requires-Dist: mkdocs-
 jupyter>=0.21.0; extra == "dev" Requires-Dist: pytest-cov>=4.0.0; extra ==
 "dev" Requires-Dist: pytest>=7.3.1; extra == "dev" Requires-Dist:
 isort>=5.12.0; extra == "dev" Requires-Dist: ipywidgets>=8.0.6; extra == "dev"
```

### Comparing `cherche-2.1.1/cherche.egg-info/SOURCES.txt` & `cherche-2.2.0/cherche.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cherche-2.1.1/setup.py` & `cherche-2.2.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 from cherche.__version__ import __version__
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 base_packages = [
     "numpy >= 1.23.5",
-    "scikit-learn >= 1.1.2",
+    "scikit-learn >= 1.5.0",
     "lunr >= 0.6.2",
     "rapidfuzz >= 3.0.0",
     "flashtext >= 2.7",
     "tqdm >= 4.62.3",
     "scipy >= 1.7.3",
-    "lenlp == 1.0.5",
+    "lenlp == 1.1.0",
 ]
 
 cpu = ["sentence-transformers >= 2.2.2", "faiss-cpu >= 1.7.4"]
 gpu = ["sentence-transformers >= 2.2.2", "faiss-gpu >= 1.7.4"]
 dev = [
     "numpydoc >= 1.4.0",
     "mkdocs_material >= 8.3.5",
```

