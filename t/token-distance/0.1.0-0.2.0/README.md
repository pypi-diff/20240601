# Comparing `tmp/token_distance-0.1.0.tar.gz` & `tmp/token_distance-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "token_distance-0.1.0.tar", max compression
+gzip compressed data, was "token_distance-0.2.0.tar", max compression
```

## Comparing `token_distance-0.1.0.tar` & `token_distance-0.2.0.tar`

### file list

```diff
@@ -1,31 +1,33 @@
--rw-r--r--   0        0        0     1500 2024-05-30 19:12:33.055149 token_distance-0.1.0/LICENSE
--rw-r--r--   0        0        0     2913 2024-05-30 18:42:54.715737 token_distance-0.1.0/README.md
--rw-r--r--   0        0        0     1746 2024-05-30 19:25:25.518031 token_distance-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      115 2024-05-30 17:41:10.440748 token_distance-0.1.0/token_distance/__init__.py
--rw-r--r--   0        0        0        0 2024-05-28 17:29:22.296777 token_distance-0.1.0/token_distance/algorithms/__init__.py
--rw-r--r--   0        0        0      199 2024-05-28 19:17:13.394638 token_distance-0.1.0/token_distance/algorithms/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     9351 2024-05-30 17:29:21.204724 token_distance-0.1.0/token_distance/algorithms/__pycache__/token_distance.cpython-311.pyc
--rw-r--r--   0        0        0     6483 2024-05-30 17:18:55.726135 token_distance-0.1.0/token_distance/algorithms/token_distance.py
--rw-r--r--   0        0        0     1065 2024-05-28 20:00:04.417553 token_distance-0.1.0/token_distance/means/__init__.py
--rw-r--r--   0        0        0     1935 2024-05-28 20:00:04.689554 token_distance-0.1.0/token_distance/means/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3240 2024-05-28 19:22:11.539819 token_distance-0.1.0/token_distance/means/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1808 2024-05-28 19:22:11.386819 token_distance-0.1.0/token_distance/means/base.py
--rw-r--r--   0        0        0     1930 2024-05-30 19:03:56.499593 token_distance-0.1.0/token_distance/similarities/__init__.py
--rw-r--r--   0        0        0     3466 2024-05-30 19:03:57.490598 token_distance-0.1.0/token_distance/similarities/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3217 2024-05-28 19:17:13.372638 token_distance-0.1.0/token_distance/similarities/__pycache__/base.cpython-311.pyc
--rw-r--r--   0        0        0     1890 2024-05-28 18:34:20.980855 token_distance-0.1.0/token_distance/similarities/base.py
--rw-r--r--   0        0        0        0 2024-05-28 17:29:54.171174 token_distance-0.1.0/token_distance/types/__init__.py
--rw-r--r--   0        0        0      194 2024-05-28 19:17:13.369638 token_distance-0.1.0/token_distance/types/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     3864 2024-05-28 19:59:53.152504 token_distance-0.1.0/token_distance/types/__pycache__/registry.cpython-311.pyc
--rw-r--r--   0        0        0     6921 2024-05-30 16:16:29.351940 token_distance-0.1.0/token_distance/types/__pycache__/token.cpython-311.pyc
--rw-r--r--   0        0        0     2017 2024-05-28 19:55:09.686277 token_distance-0.1.0/token_distance/types/registry.py
--rw-r--r--   0        0        0     4240 2024-05-30 16:11:30.314719 token_distance-0.1.0/token_distance/types/token.py
--rw-r--r--   0        0        0        0 2024-05-30 16:20:30.192971 token_distance-0.1.0/token_distance/ui/__init__.py
--rw-r--r--   0        0        0      191 2024-05-30 17:06:02.405925 token_distance-0.1.0/token_distance/ui/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     5744 2024-05-30 17:31:46.388343 token_distance-0.1.0/token_distance/ui/__pycache__/console.cpython-311.pyc
--rw-r--r--   0        0        0     3322 2024-05-30 17:31:46.031342 token_distance-0.1.0/token_distance/ui/console.py
--rw-r--r--   0        0        0      766 2024-05-28 20:00:21.463626 token_distance-0.1.0/token_distance/weights/__init__.py
--rw-r--r--   0        0        0     1624 2024-05-28 20:00:21.740628 token_distance-0.1.0/token_distance/weights/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1921 2024-05-28 19:17:13.377638 token_distance-0.1.0/token_distance/weights/__pycache__/common.cpython-311.pyc
--rw-r--r--   0        0        0      938 2024-05-28 19:06:54.955227 token_distance-0.1.0/token_distance/weights/common.py
--rw-r--r--   0        0        0     4511 1970-01-01 00:00:00.000000 token_distance-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1500 2024-05-30 19:12:33.055149 token_distance-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3178 2024-06-01 16:32:13.699322 token_distance-0.2.0/README.md
+-rw-r--r--   0        0        0     1746 2024-06-01 16:05:45.386564 token_distance-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      228 2024-06-01 16:28:05.851957 token_distance-0.2.0/token_distance/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:29:22.296777 token_distance-0.2.0/token_distance/algorithms/__init__.py
+-rw-r--r--   0        0        0      199 2024-05-28 19:17:13.394638 token_distance-0.2.0/token_distance/algorithms/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     7729 2024-06-01 16:09:17.094876 token_distance-0.2.0/token_distance/algorithms/__pycache__/token_distance.cpython-311.pyc
+-rw-r--r--   0        0        0     7200 2024-06-01 16:09:17.095876 token_distance-0.2.0/token_distance/algorithms/__pycache__/token_matching.cpython-311.pyc
+-rw-r--r--   0        0        0     5175 2024-06-01 16:00:30.234955 token_distance-0.2.0/token_distance/algorithms/token_distance.py
+-rw-r--r--   0        0        0     5105 2024-06-01 16:04:47.122242 token_distance-0.2.0/token_distance/algorithms/token_matching.py
+-rw-r--r--   0        0        0     1065 2024-05-28 20:00:04.417553 token_distance-0.2.0/token_distance/means/__init__.py
+-rw-r--r--   0        0        0     1935 2024-05-28 20:00:04.689554 token_distance-0.2.0/token_distance/means/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3240 2024-05-28 19:22:11.539819 token_distance-0.2.0/token_distance/means/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1808 2024-05-28 19:22:11.386819 token_distance-0.2.0/token_distance/means/base.py
+-rw-r--r--   0        0        0     1929 2024-06-01 15:40:21.445068 token_distance-0.2.0/token_distance/similarities/__init__.py
+-rw-r--r--   0        0        0     3465 2024-06-01 15:43:50.932082 token_distance-0.2.0/token_distance/similarities/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     3217 2024-05-28 19:17:13.372638 token_distance-0.2.0/token_distance/similarities/__pycache__/base.cpython-311.pyc
+-rw-r--r--   0        0        0     1890 2024-05-28 18:34:20.980855 token_distance-0.2.0/token_distance/similarities/base.py
+-rw-r--r--   0        0        0        0 2024-05-28 17:29:54.171174 token_distance-0.2.0/token_distance/types/__init__.py
+-rw-r--r--   0        0        0      194 2024-05-28 19:17:13.369638 token_distance-0.2.0/token_distance/types/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4737 2024-06-01 16:09:17.099876 token_distance-0.2.0/token_distance/types/__pycache__/registry.cpython-311.pyc
+-rw-r--r--   0        0        0     7413 2024-06-01 16:37:06.347941 token_distance-0.2.0/token_distance/types/__pycache__/token.cpython-311.pyc
+-rw-r--r--   0        0        0     2676 2024-06-01 16:00:30.221955 token_distance-0.2.0/token_distance/types/registry.py
+-rw-r--r--   0        0        0     4699 2024-06-01 16:37:05.463936 token_distance-0.2.0/token_distance/types/token.py
+-rw-r--r--   0        0        0        0 2024-05-30 16:20:30.192971 token_distance-0.2.0/token_distance/ui/__init__.py
+-rw-r--r--   0        0        0      191 2024-05-30 17:06:02.405925 token_distance-0.2.0/token_distance/ui/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     5744 2024-05-30 17:31:46.388343 token_distance-0.2.0/token_distance/ui/__pycache__/console.cpython-311.pyc
+-rw-r--r--   0        0        0     3322 2024-05-30 17:31:46.031342 token_distance-0.2.0/token_distance/ui/console.py
+-rw-r--r--   0        0        0      766 2024-05-28 20:00:21.463626 token_distance-0.2.0/token_distance/weights/__init__.py
+-rw-r--r--   0        0        0     1624 2024-05-28 20:00:21.740628 token_distance-0.2.0/token_distance/weights/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1921 2024-05-28 19:17:13.377638 token_distance-0.2.0/token_distance/weights/__pycache__/common.cpython-311.pyc
+-rw-r--r--   0        0        0      938 2024-05-28 19:06:54.955227 token_distance-0.2.0/token_distance/weights/common.py
+-rw-r--r--   0        0        0     4776 1970-01-01 00:00:00.000000 token_distance-0.2.0/PKG-INFO
```

### Comparing `token_distance-0.1.0/LICENSE` & `token_distance-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `token_distance-0.1.0/README.md` & `token_distance-0.2.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -8,16 +8,15 @@
 reflects its importance, which could depend on factors like token length or predefined criteria.
 
 For each search token, token-distance identifies the most similar token in the target text based on these weights. The
 core of the library's functionality lies in how it calculates similarity: it pairs each search token with the best
 matching token in the target text and computes a weighted average of these pairings to produce a final similarity score.
 
 The operations of token-distance are summarized in the chart below, which illustrates the step-by-step process from
-tokenization to the calculation of similarity scores. This visual aid helps users understand how inputs are transformed
-into meaningful outputs.
+tokenization to the calculation of similarity scores. 
 
 
 ![](source/_static/schema.png)
 
 
 ## Installation
 
@@ -63,7 +62,17 @@
 
 calculate_distance: Callable[[str, str], float] = from_config(Config(mean='geometric'))
 ````
 
 This configuration uses a geometric mean to compute the similarity score between tokens, which is useful for certain
 types of textual analysis.
 
+token-distance can also obtain information about the actual matching of the tokens, if those are of interest:
+
+````python
+from collections.abc import Callable, Collection
+from token_distance import match_from_config, MatchConfig, RecordingToken
+
+get_best_matches: Callable[[str, str], Collection[RecordingToken]] = match_from_config(MatchConfig())
+````
+
+
```

### Comparing `token_distance-0.1.0/pyproject.toml` & `token_distance-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "token-distance"
-version = "0.1.0"
+version = "0.2.0"
 description = "Python library designed to perform fuzzy token matching within text documents. Utilizing advanced algorithms, this tool allows developers and data scientists to search and compare tokens based on flexible criteria, beyond exact matches. The library supports tokenization through whitespace, regular expressions, or custom functions, and provides weighted comparisons for nuanced analysis."
 authors = ["voidpointercast <voidpointercast@justmail.de>"]
 repository = "https://gitlab.com/patrick.daniel.gress/token-distance"
 homepage = "https://gitlab.com/patrick.daniel.gress/token-distance"
 documentation = "https://token-distance.readthedocs.io/en/latest/"
 license = "BSD"
 readme = "README.md"
```

### Comparing `token_distance-0.1.0/token_distance/algorithms/__pycache__/token_distance.cpython-311.pyc` & `token_distance-0.2.0/token_distance/algorithms/__pycache__/token_distance.cpython-311.pyc`

 * *Files 20% similar despite different names*

#### Python bytecode

```diff
@@ -1,32 +1,31 @@
 magic:    0xa70d0d0a
-moddate:  0xffb45866 (Thu May 30 17:18:55 2024 UTC)
-files sz: 6483
+moddate:  0x9e455b66 (Sat Jun  1 16:00:30 2024 UTC)
+files sz: 5175
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 12
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
       055a050100640064036c066d075a070100640064046c086d095a09010064
-      0064056c0a6d0b5a0b0100640064066c0c6d0d5a0d6d0e5a0e0100640064
+      0064056c0a6d0b5a0b6d0c5a0c0100640064066c0d6d0e5a0e0100640064
       076c0f6d105a106d115a116d125a120100640064086c136d145a146d155a
-      156d165a166d175a176d185a180100640064096c196d1a5a1a6d1b5a1b6d
-      1c5a1c6d1d5a1d6d1e5a1e6d1f5a1f01006400640a6c206d215a216d225a
-      226d235a230100640b6514640c6510640d6521640e6501651b1900000000
-      0000000000640f650165241900000000000000000064106525660c641184
-      045a26640b6514640c6510640d6521640e6501651b190000000000000000
-      00640f650165241900000000000000000064106525660c641284045a2765
-      0502004700641384006414a6020000ab020000000000000000a6000000ab
-      0000000000000000005a280200650d6415a6010000ab0100000000000000
-      005a29641665026524670165296602190000000000000000006417652965
-      247a070000641065296606641884045a2a0200470064198400641a650ea6
-      030000ab0300000000000000005a2b02006528a6000000ab000000000000
-      0000006601641b65286410652b6604641c84055a2c641d5300
+      156d165a160100640064096c176d185a1801006400640a6c196d1a5a1a6d
+      1b5a1b6d1c5a1c6d1d5a1d6d1e5a1e01006400640b6c1f6d205a206d215a
+      216d225a220100640c6514640d6510640e6520640f6501651b1900000000
+      00000000006410650165231900000000000000000064116524660c641284
+      045a25640c6514640d6510640e6520640f6501651b190000000000000000
+      006410650165231900000000000000000064116524660c641384045a2665
+      0502004700641484006415a6020000ab020000000000000000a6000000ab
+      0000000000000000005a270200650b6416a6010000ab0100000000000000
+      005a2802004700641784006418650ca6030000ab0300000000000000005a
+      2902006527a6000000ab0000000000000000006601641965276411652966
+      04641a84055a2a641b5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
                  4 LOAD_CONST               1 (('Collection', 'Callable', 'Sequence'))
                  6 IMPORT_NAME              0 (collections.abc)
                  8 IMPORT_FROM              1 (Collection)
                 10 STORE_NAME               1 (Collection)
@@ -47,232 +46,216 @@
                 36 LOAD_CONST               3 (('partial',))
                 38 IMPORT_NAME              6 (functools)
                 40 IMPORT_FROM              7 (partial)
                 42 STORE_NAME               7 (partial)
                 44 POP_TOP
    
      4          46 LOAD_CONST               0 (0)
-                48 LOAD_CONST               4 (('attrgetter',))
-                50 IMPORT_NAME              8 (operator)
-                52 IMPORT_FROM              9 (attrgetter)
-                54 STORE_NAME               9 (attrgetter)
+                48 LOAD_CONST               4 (('Pattern',))
+                50 IMPORT_NAME              8 (re)
+                52 IMPORT_FROM              9 (Pattern)
+                54 STORE_NAME               9 (Pattern)
                 56 POP_TOP
    
      5          58 LOAD_CONST               0 (0)
-                60 LOAD_CONST               5 (('Pattern',))
-                62 IMPORT_NAME             10 (re)
-                64 IMPORT_FROM             11 (Pattern)
-                66 STORE_NAME              11 (Pattern)
-                68 POP_TOP
-   
-     6          70 LOAD_CONST               0 (0)
-                72 LOAD_CONST               6 (('TypeVar', 'Protocol'))
-                74 IMPORT_NAME             12 (typing)
-                76 IMPORT_FROM             13 (TypeVar)
-                78 STORE_NAME              13 (TypeVar)
-                80 IMPORT_FROM             14 (Protocol)
-                82 STORE_NAME              14 (Protocol)
+                60 LOAD_CONST               5 (('TypeVar', 'Protocol'))
+                62 IMPORT_NAME             10 (typing)
+                64 IMPORT_FROM             11 (TypeVar)
+                66 STORE_NAME              11 (TypeVar)
+                68 IMPORT_FROM             12 (Protocol)
+                70 STORE_NAME              12 (Protocol)
+                72 POP_TOP
+   
+     7          74 LOAD_CONST               0 (0)
+                76 LOAD_CONST               6 (('match_tokens',))
+                78 IMPORT_NAME             13 (token_distance.algorithms.token_matching)
+                80 IMPORT_FROM             14 (match_tokens)
+                82 STORE_NAME              14 (match_tokens)
                 84 POP_TOP
    
      8          86 LOAD_CONST               0 (0)
                 88 LOAD_CONST               7 (('Mean', 'average', 'get_mean_by_name'))
                 90 IMPORT_NAME             15 (token_distance.means)
                 92 IMPORT_FROM             16 (Mean)
                 94 STORE_NAME              16 (Mean)
                 96 IMPORT_FROM             17 (average)
                 98 STORE_NAME              17 (average)
                100 IMPORT_FROM             18 (get_mean_by_name)
                102 STORE_NAME              18 (get_mean_by_name)
                104 POP_TOP
    
      9         106 LOAD_CONST               0 (0)
-               108 LOAD_CONST               8 (('Similarity', 'as_recording', 'RecordingSimilarity', 'jaro_winkler', 'get_similarity_by_name'))
+               108 LOAD_CONST               8 (('Similarity', 'jaro_winkler', 'get_similarity_by_name'))
                110 IMPORT_NAME             19 (token_distance.similarities)
                112 IMPORT_FROM             20 (Similarity)
                114 STORE_NAME              20 (Similarity)
-               116 IMPORT_FROM             21 (as_recording)
-               118 STORE_NAME              21 (as_recording)
-               120 IMPORT_FROM             22 (RecordingSimilarity)
-               122 STORE_NAME              22 (RecordingSimilarity)
-               124 IMPORT_FROM             23 (jaro_winkler)
-               126 STORE_NAME              23 (jaro_winkler)
-               128 IMPORT_FROM             24 (get_similarity_by_name)
-               130 STORE_NAME              24 (get_similarity_by_name)
-               132 POP_TOP
-   
-    11         134 LOAD_CONST               0 (0)
-               136 LOAD_CONST               9 (('WeightedToken', 'Token', 'EvaluatedToken', 'RecordingToken', 'split_text_by', 'parse_token'))
-               138 IMPORT_NAME             25 (token_distance.types.token)
-               140 IMPORT_FROM             26 (WeightedToken)
-               142 STORE_NAME              26 (WeightedToken)
-               144 IMPORT_FROM             27 (Token)
-               146 STORE_NAME              27 (Token)
-               148 IMPORT_FROM             28 (EvaluatedToken)
-               150 STORE_NAME              28 (EvaluatedToken)
-               152 IMPORT_FROM             29 (RecordingToken)
-               154 STORE_NAME              29 (RecordingToken)
-               156 IMPORT_FROM             30 (split_text_by)
-               158 STORE_NAME              30 (split_text_by)
-               160 IMPORT_FROM             31 (parse_token)
-               162 STORE_NAME              31 (parse_token)
+               116 IMPORT_FROM             21 (jaro_winkler)
+               118 STORE_NAME              21 (jaro_winkler)
+               120 IMPORT_FROM             22 (get_similarity_by_name)
+               122 STORE_NAME              22 (get_similarity_by_name)
+               124 POP_TOP
+   
+    10         126 LOAD_CONST               0 (0)
+               128 LOAD_CONST               9 (('get_if_needed',))
+               130 IMPORT_NAME             23 (token_distance.types.registry)
+               132 IMPORT_FROM             24 (get_if_needed)
+               134 STORE_NAME              24 (get_if_needed)
+               136 POP_TOP
+   
+    11         138 LOAD_CONST               0 (0)
+               140 LOAD_CONST              10 (('WeightedToken', 'Token', 'EvaluatedToken', 'split_text_by', 'parse_token'))
+               142 IMPORT_NAME             25 (token_distance.types.token)
+               144 IMPORT_FROM             26 (WeightedToken)
+               146 STORE_NAME              26 (WeightedToken)
+               148 IMPORT_FROM             27 (Token)
+               150 STORE_NAME              27 (Token)
+               152 IMPORT_FROM             28 (EvaluatedToken)
+               154 STORE_NAME              28 (EvaluatedToken)
+               156 IMPORT_FROM             29 (split_text_by)
+               158 STORE_NAME              29 (split_text_by)
+               160 IMPORT_FROM             30 (parse_token)
+               162 STORE_NAME              30 (parse_token)
                164 POP_TOP
    
     12         166 LOAD_CONST               0 (0)
-               168 LOAD_CONST              10 (('Weight', 'even_weight', 'get_weight_by_name'))
-               170 IMPORT_NAME             32 (token_distance.weights)
-               172 IMPORT_FROM             33 (Weight)
-               174 STORE_NAME              33 (Weight)
-               176 IMPORT_FROM             34 (even_weight)
-               178 STORE_NAME              34 (even_weight)
-               180 IMPORT_FROM             35 (get_weight_by_name)
-               182 STORE_NAME              35 (get_weight_by_name)
+               168 LOAD_CONST              11 (('Weight', 'even_weight', 'get_weight_by_name'))
+               170 IMPORT_NAME             31 (token_distance.weights)
+               172 IMPORT_FROM             32 (Weight)
+               174 STORE_NAME              32 (Weight)
+               176 IMPORT_FROM             33 (even_weight)
+               178 STORE_NAME              33 (even_weight)
+               180 IMPORT_FROM             34 (get_weight_by_name)
+               182 STORE_NAME              34 (get_weight_by_name)
                184 POP_TOP
    
-    15         186 LOAD_CONST              11 ('similarity')
+    15         186 LOAD_CONST              12 ('similarity')
    
     16         188 LOAD_NAME               20 (Similarity)
    
-    15         190 LOAD_CONST              12 ('mean')
+    15         190 LOAD_CONST              13 ('mean')
    
     17         192 LOAD_NAME               16 (Mean)
    
-    15         194 LOAD_CONST              13 ('weight')
+    15         194 LOAD_CONST              14 ('weight')
    
-    18         196 LOAD_NAME               33 (Weight)
+    18         196 LOAD_NAME               32 (Weight)
    
-    15         198 LOAD_CONST              14 ('tokens')
+    15         198 LOAD_CONST              15 ('tokens')
    
     19         200 LOAD_NAME                1 (Collection)
                202 LOAD_NAME               27 (Token)
                204 BINARY_SUBSCR
    
-    15         214 LOAD_CONST              15 ('candidates')
+    15         214 LOAD_CONST              16 ('candidates')
    
     20         216 LOAD_NAME                1 (Collection)
-               218 LOAD_NAME               36 (str)
+               218 LOAD_NAME               35 (str)
                220 BINARY_SUBSCR
    
-    15         230 LOAD_CONST              16 ('return')
+    15         230 LOAD_CONST              17 ('return')
    
-    21         232 LOAD_NAME               37 (float)
+    21         232 LOAD_NAME               36 (float)
    
     15         234 BUILD_TUPLE             12
-               236 LOAD_CONST              17 (<code object token_distance, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py", line 15>)
+               236 LOAD_CONST              18 (<code object token_distance, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py", line 15>)
                238 MAKE_FUNCTION            4 (annotations)
-               240 STORE_NAME              38 (token_distance)
+               240 STORE_NAME              37 (token_distance)
    
-    43         242 LOAD_CONST              11 ('similarity')
+    45         242 LOAD_CONST              12 ('similarity')
    
-    44         244 LOAD_NAME               20 (Similarity)
+    46         244 LOAD_NAME               20 (Similarity)
    
-    43         246 LOAD_CONST              12 ('mean')
+    45         246 LOAD_CONST              13 ('mean')
    
-    45         248 LOAD_NAME               16 (Mean)
+    47         248 LOAD_NAME               16 (Mean)
    
-    43         250 LOAD_CONST              13 ('weight')
+    45         250 LOAD_CONST              14 ('weight')
    
-    46         252 LOAD_NAME               33 (Weight)
+    48         252 LOAD_NAME               32 (Weight)
    
-    43         254 LOAD_CONST              14 ('tokens')
+    45         254 LOAD_CONST              15 ('tokens')
    
-    47         256 LOAD_NAME                1 (Collection)
+    49         256 LOAD_NAME                1 (Collection)
                258 LOAD_NAME               27 (Token)
                260 BINARY_SUBSCR
    
-    43         270 LOAD_CONST              15 ('candidates')
+    45         270 LOAD_CONST              16 ('candidates')
    
-    48         272 LOAD_NAME                1 (Collection)
-               274 LOAD_NAME               36 (str)
+    50         272 LOAD_NAME                1 (Collection)
+               274 LOAD_NAME               35 (str)
                276 BINARY_SUBSCR
    
-    43         286 LOAD_CONST              16 ('return')
+    45         286 LOAD_CONST              17 ('return')
    
-    49         288 LOAD_NAME               37 (float)
+    51         288 LOAD_NAME               36 (float)
    
-    43         290 BUILD_TUPLE             12
-               292 LOAD_CONST              18 (<code object exclusive_token_distance, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py", line 43>)
+    45         290 BUILD_TUPLE             12
+               292 LOAD_CONST              19 (<code object exclusive_token_distance, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py", line 45>)
                294 MAKE_FUNCTION            4 (annotations)
-               296 STORE_NAME              39 (exclusive_token_distance)
+               296 STORE_NAME              38 (exclusive_token_distance)
    
-    82         298 LOAD_NAME                5 (dataclass)
+    71         298 LOAD_NAME                5 (dataclass)
    
-    83         300 PUSH_NULL
+    72         300 PUSH_NULL
                302 LOAD_BUILD_CLASS
-               304 LOAD_CONST              19 (<code object Config, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py", line 82>)
+               304 LOAD_CONST              20 (<code object Config, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py", line 71>)
                306 MAKE_FUNCTION            0
-               308 LOAD_CONST              20 ('Config')
+               308 LOAD_CONST              21 ('Config')
                310 PRECALL                  2
                314 CALL                     2
    
-    82         324 PRECALL                  0
+    71         324 PRECALL                  0
                328 CALL                     0
    
-    83         338 STORE_NAME              40 (Config)
+    72         338 STORE_NAME              39 (Config)
    
-   102         340 PUSH_NULL
-               342 LOAD_NAME               13 (TypeVar)
-               344 LOAD_CONST              21 ('_T')
+    91         340 PUSH_NULL
+               342 LOAD_NAME               11 (TypeVar)
+               344 LOAD_CONST              22 ('_T')
                346 PRECALL                  1
                350 CALL                     1
-               360 STORE_NAME              41 (_T)
+               360 STORE_NAME              40 (_T)
    
-   105         362 LOAD_CONST              22 ('get')
-               364 LOAD_NAME                2 (Callable)
-               366 LOAD_NAME               36 (str)
-               368 BUILD_LIST               1
-               370 LOAD_NAME               41 (_T)
-               372 BUILD_TUPLE              2
-               374 BINARY_SUBSCR
-               384 LOAD_CONST              23 ('value')
-               386 LOAD_NAME               41 (_T)
-               388 LOAD_NAME               36 (str)
-               390 BINARY_OP                7 (|)
-               394 LOAD_CONST              16 ('return')
-               396 LOAD_NAME               41 (_T)
-               398 BUILD_TUPLE              6
-               400 LOAD_CONST              24 (<code object _get_if_needed, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py", line 105>)
-               402 MAKE_FUNCTION            4 (annotations)
-               404 STORE_NAME              42 (_get_if_needed)
-   
-   120         406 PUSH_NULL
-               408 LOAD_BUILD_CLASS
-               410 LOAD_CONST              25 (<code object TokenDistanceAlgorithm, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py", line 120>)
-               412 MAKE_FUNCTION            0
-               414 LOAD_CONST              26 ('TokenDistanceAlgorithm')
-               416 LOAD_NAME               14 (Protocol)
-               418 PRECALL                  3
-               422 CALL                     3
-               432 STORE_NAME              43 (TokenDistanceAlgorithm)
-   
-   132         434 PUSH_NULL
-               436 LOAD_NAME               40 (Config)
-               438 PRECALL                  0
-               442 CALL                     0
-               452 BUILD_TUPLE              1
-               454 LOAD_CONST              27 ('config')
-               456 LOAD_NAME               40 (Config)
-               458 LOAD_CONST              16 ('return')
-               460 LOAD_NAME               43 (TokenDistanceAlgorithm)
-               462 BUILD_TUPLE              4
-               464 LOAD_CONST              28 (<code object from_config, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py", line 132>)
-               466 MAKE_FUNCTION            5 (defaults, annotations)
-               468 STORE_NAME              44 (from_config)
-               470 LOAD_CONST              29 (None)
-               472 RETURN_VALUE
+    97         362 PUSH_NULL
+               364 LOAD_BUILD_CLASS
+               366 LOAD_CONST              23 (<code object TokenDistanceAlgorithm, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py", line 97>)
+               368 MAKE_FUNCTION            0
+               370 LOAD_CONST              24 ('TokenDistanceAlgorithm')
+               372 LOAD_NAME               12 (Protocol)
+               374 PRECALL                  3
+               378 CALL                     3
+               388 STORE_NAME              41 (TokenDistanceAlgorithm)
+   
+   110         390 PUSH_NULL
+               392 LOAD_NAME               39 (Config)
+               394 PRECALL                  0
+               398 CALL                     0
+               408 BUILD_TUPLE              1
+               410 LOAD_CONST              25 ('config')
+               412 LOAD_NAME               39 (Config)
+               414 LOAD_CONST              17 ('return')
+               416 LOAD_NAME               41 (TokenDistanceAlgorithm)
+               418 BUILD_TUPLE              4
+               420 LOAD_CONST              26 (<code object from_config, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py", line 110>)
+               422 MAKE_FUNCTION            5 (defaults, annotations)
+               424 STORE_NAME              42 (from_config)
+               426 LOAD_CONST              27 (None)
+               428 RETURN_VALUE
    consts
       0
       ('Collection', 'Callable', 'Sequence')
       ('dataclass',)
       ('partial',)
-      ('attrgetter',)
       ('Pattern',)
       ('TypeVar', 'Protocol')
+      ('match_tokens',)
       ('Mean', 'average', 'get_mean_by_name')
-      ('Similarity', 'as_recording', 'RecordingSimilarity', 'jaro_winkler', 'get_similarity_by_name')
-      ('WeightedToken', 'Token', 'EvaluatedToken', 'RecordingToken', 'split_text_by', 'parse_token')
+      ('Similarity', 'jaro_winkler', 'get_similarity_by_name')
+      ('get_if_needed',)
+      ('WeightedToken', 'Token', 'EvaluatedToken', 'split_text_by', 'parse_token')
       ('Weight', 'even_weight', 'get_weight_by_name')
       'similarity'
       'mean'
       'weight'
       'tokens'
       'candidates'
       'return'
@@ -406,197 +389,96 @@
          cellvars   ('similarity', 'candidates')
          filename   '/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py'
          name       'token_distance'
          firstlineno 15
          lnotab 0x061416010a0202fe1204
       code
          argcount  : 5
-         nlocals   : 12
-         stacksize : 7
+         nlocals   : 5
+         stacksize : 9
          flags     : 3
          code
-            0x97007401000000000000000000007c04a6010000ab0100000000000000
-            007d057403000000000000000000007c00a6010000ab0100000000000000
-            007d0674050000000000000000000002007c027c03a6010000ab01000000
-            00000000007407000000000000000000006401a6010000ab010000000000
-            0000006402ac03a6030000ab0300000000000000007d0774010000000000
-            0000000000a6000000ab0000000000000000007d087c0744005d877d097c
-            0573207c08a004000000000000000000000000000000000000000002007c
-            007c096404a6020000ab020000000000000000a6010000ab010000000000
-            00000001008c24740b000000000000000000007c067c09a6020000ab0200
-            000000000000007d0a740d00000000000000000000740f00000000000000
-            0000007c0a7c05a6020000ab020000000000000000a6010000ab01000000
-            00000000007d0b7c08a00400000000000000000000000000000000000000
-            007c0ba6010000ab01000000000000000001007c0b6a0800000000000000
-            00811a7c05a00900000000000000000000000000000000000000007c0b6a
-            080000000000000000a6010000ab01000000000000000001008c8802007c
-            017c08a6010000ab0100000000000000005300
-          43           0 RESUME                   0
-         
-          66           2 LOAD_GLOBAL              1 (NULL + list)
-                      14 LOAD_FAST                4 (candidates)
-                      16 PRECALL                  1
-                      20 CALL                     1
-                      30 STORE_FAST               5 (remaining_candidates)
-         
-          67          32 LOAD_GLOBAL              3 (NULL + as_recording)
-                      44 LOAD_FAST                0 (similarity)
-                      46 PRECALL                  1
-                      50 CALL                     1
-                      60 STORE_FAST               6 (recording_sim)
-         
-          68          62 LOAD_GLOBAL              5 (NULL + sorted)
-                      74 PUSH_NULL
-                      76 LOAD_FAST                2 (weight)
-                      78 LOAD_FAST                3 (tokens)
-                      80 PRECALL                  1
-                      84 CALL                     1
-                      94 LOAD_GLOBAL              7 (NULL + attrgetter)
-                     106 LOAD_CONST               1 ('weight')
-                     108 PRECALL                  1
-                     112 CALL                     1
-                     122 LOAD_CONST               2 (True)
-                     124 KW_NAMES                 3
-                     126 PRECALL                  3
-                     130 CALL                     3
-                     140 STORE_FAST               7 (weighted_tokens)
-         
-          69         142 LOAD_GLOBAL              1 (NULL + list)
-                     154 PRECALL                  0
-                     158 CALL                     0
-                     168 STORE_FAST               8 (evaluated_tokens)
-         
-          70         170 LOAD_FAST                7 (weighted_tokens)
-                     172 GET_ITER
-                 >>  174 FOR_ITER               135 (to 446)
-                     176 STORE_FAST               9 (token)
-         
-          71         178 LOAD_FAST                5 (remaining_candidates)
-                     180 POP_JUMP_FORWARD_IF_TRUE    32 (to 246)
-         
-          72         182 LOAD_FAST                8 (evaluated_tokens)
-                     184 LOAD_METHOD              4 (append)
-                     206 PUSH_NULL
-                     208 LOAD_FAST                0 (similarity)
-                     210 LOAD_FAST                9 (token)
-                     212 LOAD_CONST               4 ('')
-                     214 PRECALL                  2
-                     218 CALL                     2
-                     228 PRECALL                  1
-                     232 CALL                     1
-                     242 POP_TOP
-                     244 JUMP_BACKWARD           36 (to 174)
-         
-          74     >>  246 LOAD_GLOBAL             11 (NULL + partial)
-                     258 LOAD_FAST                6 (recording_sim)
-                     260 LOAD_FAST                9 (token)
-                     262 PRECALL                  2
-                     266 CALL                     2
-                     276 STORE_FAST              10 (evaluate)
-         
-          75         278 LOAD_GLOBAL             13 (NULL + max)
-                     290 LOAD_GLOBAL             15 (NULL + map)
-                     302 LOAD_FAST               10 (evaluate)
-                     304 LOAD_FAST                5 (remaining_candidates)
-                     306 PRECALL                  2
-                     310 CALL                     2
-                     320 PRECALL                  1
-                     324 CALL                     1
-                     334 STORE_FAST              11 (best)
-         
-          76         336 LOAD_FAST                8 (evaluated_tokens)
-                     338 LOAD_METHOD              4 (append)
-                     360 LOAD_FAST               11 (best)
-                     362 PRECALL                  1
-                     366 CALL                     1
-                     376 POP_TOP
-         
-          77         378 LOAD_FAST               11 (best)
-                     380 LOAD_ATTR                8 (matched_with)
-                     390 POP_JUMP_FORWARD_IF_NONE    26 (to 444)
-         
-          78         392 LOAD_FAST                5 (remaining_candidates)
-                     394 LOAD_METHOD              9 (remove)
-                     416 LOAD_FAST               11 (best)
-                     418 LOAD_ATTR                8 (matched_with)
-                     428 PRECALL                  1
-                     432 CALL                     1
-                     442 POP_TOP
-                 >>  444 JUMP_BACKWARD          136 (to 174)
-         
-          79     >>  446 PUSH_NULL
-                     448 LOAD_FAST                1 (mean)
-                     450 LOAD_FAST                8 (evaluated_tokens)
-                     452 PRECALL                  1
-                     456 CALL                     1
-                     466 RETURN_VALUE
+            0x970002007c017401000000000000000000007c007c0264017c037c04a6
+            050000ab050000000000000000a6010000ab0100000000000000005300
+          45           0 RESUME                   0
+         
+          68           2 PUSH_NULL
+                       4 LOAD_FAST                1 (mean)
+                       6 LOAD_GLOBAL              1 (NULL + match_tokens)
+                      18 LOAD_FAST                0 (similarity)
+                      20 LOAD_FAST                2 (weight)
+                      22 LOAD_CONST               1 (True)
+                      24 LOAD_FAST                3 (tokens)
+                      26 LOAD_FAST                4 (candidates)
+                      28 PRECALL                  5
+                      32 CALL                     5
+                      42 PRECALL                  1
+                      46 CALL                     1
+                      56 RETURN_VALUE
          consts
             '\n    Calculate the token distance between a collection of tokens and a collection of candidates.\n    If a token gets matched to a candidate, this candidate will no longer be matchable for other tokens,\n    if not multiple instances of candidate exist in the text.\n\n    Args:\n        similarity: A Similarity instance used for calculating token similarity.\n        mean: A Mean instance used for calculating the mean of evaluated tokens.\n        weight: A Weight instance used for weighting tokens.\n        tokens: A collection of Token instances representing the tokens to be evaluated.\n        candidates: A collection of strings representing the candidate tokens to compare with.\n\n    Returns:\n        float: The result of applying the mean function to the evaluated tokens.\n\n    '
-            'weight'
             True
-            ('key', 'reverse')
-            ''
-         names      ('list', 'as_recording', 'sorted', 'attrgetter', 'append', 'partial', 'max', 'map', 'matched_with', 'remove')
-         varnames   ('similarity', 'mean', 'weight', 'tokens', 'candidates', 'remaining_candidates', 'recording_sim', 'weighted_tokens', 'evaluated_tokens', 'token', 'evaluate', 'best')
+         names      ('match_tokens',)
+         varnames   ('similarity', 'mean', 'weight', 'tokens', 'candidates')
          freevars   ()
          cellvars   ()
          filename   '/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py'
          name       'exclusive_token_distance'
-         firstlineno 43
-         lnotab 0x02171e011e0150011c0108010401400220013a012a010e013601
+         firstlineno 45
+         lnotab 0x0217
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 4
          flags     : 0
          code
             0x970065005a0164005a02550064015a0365045a05650665077a07000065
             0864023c00000065095a0a650b65077a070000650864033c000000650c5a
             0d650e65077a070000650864043c00000064055a0f651065076701651165
             071900000000000000000066021900000000000000000065127a07000065
             077a07000064057a070000650864063c00000064075a136514650864083c
             00000064055300
-          82           0 RESUME                   0
+          71           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('Config')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          84          12 LOAD_CONST               1 ("\n    Config represents the configuration options for token distance.\n\n    Attributes:\n        similarity (Similarity | str): The similarity metric to be used. Defaults to 'jaro_winkler'.\n        mean (Mean | str): The mean calculation method to be used. Defaults to 'average'.\n        weight (Weight | str): The weighting method to be used. Defaults to 'even_weight'.\n        tokenize (Callable[[str], Sequence[str]] | Pattern | str | None): The tokenization method to be used.\n            Defaults to None.\n        exclusive (bool): Whether exclusive matching should be used. Defaults to False.\n    ")
+          73          12 LOAD_CONST               1 ("\n    Config represents the configuration options for token distance.\n\n    Attributes:\n        similarity (Similarity | str): The similarity metric to be used. Defaults to 'jaro_winkler'.\n        mean (Mean | str): The mean calculation method to be used. Defaults to 'average'.\n        weight (Weight | str): The weighting method to be used. Defaults to 'even_weight'.\n        tokenize (Callable[[str], Sequence[str]] | Pattern | str | None): The tokenization method to be used.\n            Defaults to None.\n        exclusive (bool): Whether exclusive matching should be used. Defaults to False.\n    ")
                       14 STORE_NAME               3 (__doc__)
          
-          95          16 LOAD_NAME                4 (jaro_winkler)
+          84          16 LOAD_NAME                4 (jaro_winkler)
                       18 STORE_NAME               5 (similarity)
                       20 LOAD_NAME                6 (Similarity)
                       22 LOAD_NAME                7 (str)
                       24 BINARY_OP                7 (|)
                       28 LOAD_NAME                8 (__annotations__)
                       30 LOAD_CONST               2 ('similarity')
                       32 STORE_SUBSCR
          
-          96          36 LOAD_NAME                9 (average)
+          85          36 LOAD_NAME                9 (average)
                       38 STORE_NAME              10 (mean)
                       40 LOAD_NAME               11 (Mean)
                       42 LOAD_NAME                7 (str)
                       44 BINARY_OP                7 (|)
                       48 LOAD_NAME                8 (__annotations__)
                       50 LOAD_CONST               3 ('mean')
                       52 STORE_SUBSCR
          
-          97          56 LOAD_NAME               12 (even_weight)
+          86          56 LOAD_NAME               12 (even_weight)
                       58 STORE_NAME              13 (weight)
                       60 LOAD_NAME               14 (Weight)
                       62 LOAD_NAME                7 (str)
                       64 BINARY_OP                7 (|)
                       68 LOAD_NAME                8 (__annotations__)
                       70 LOAD_CONST               4 ('weight')
                       72 STORE_SUBSCR
          
-          98          76 LOAD_CONST               5 (None)
+          87          76 LOAD_CONST               5 (None)
                       78 STORE_NAME              15 (tokenize)
                       80 LOAD_NAME               16 (Callable)
                       82 LOAD_NAME                7 (str)
                       84 BUILD_LIST               1
                       86 LOAD_NAME               17 (Sequence)
                       88 LOAD_NAME                7 (str)
                       90 BINARY_SUBSCR
@@ -608,15 +490,15 @@
                      120 BINARY_OP                7 (|)
                      124 LOAD_CONST               5 (None)
                      126 BINARY_OP                7 (|)
                      130 LOAD_NAME                8 (__annotations__)
                      132 LOAD_CONST               6 ('tokenize')
                      134 STORE_SUBSCR
          
-          99         138 LOAD_CONST               7 (False)
+          88         138 LOAD_CONST               7 (False)
                      140 STORE_NAME              19 (exclusive)
                      142 LOAD_NAME               20 (bool)
                      144 LOAD_NAME                8 (__annotations__)
                      146 LOAD_CONST               8 ('exclusive')
                      148 STORE_SUBSCR
                      152 LOAD_CONST               5 (None)
                      154 RETURN_VALUE
@@ -632,80 +514,43 @@
             'exclusive'
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'jaro_winkler', 'similarity', 'Similarity', 'str', '__annotations__', 'average', 'mean', 'Mean', 'even_weight', 'weight', 'Weight', 'tokenize', 'Callable', 'Sequence', 'Pattern', 'exclusive', 'bool')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py'
          name       'Config'
-         firstlineno 82
+         firstlineno 71
          lnotab 0x0c02040b1401140114013e01
       'Config'
       '_T'
-      'get'
-      'value'
-      code
-         argcount  : 2
-         nlocals   : 2
-         stacksize : 4
-         flags     : 3
-         code
-            0x97007401000000000000000000007c01740200000000000000000000a6
-            020000ab02000000000000000073027c016e0a02007c007c01a6010000ab
-            0100000000000000005300
-         105           0 RESUME                   0
-         
-         117           2 LOAD_GLOBAL              1 (NULL + isinstance)
-                      14 LOAD_FAST                1 (value)
-                      16 LOAD_GLOBAL              2 (str)
-                      28 PRECALL                  2
-                      32 CALL                     2
-                      42 POP_JUMP_FORWARD_IF_TRUE     2 (to 48)
-                      44 LOAD_FAST                1 (value)
-                      46 JUMP_FORWARD            10 (to 68)
-                 >>   48 PUSH_NULL
-                      50 LOAD_FAST                0 (get)
-                      52 LOAD_FAST                1 (value)
-                      54 PRECALL                  1
-                      58 CALL                     1
-                 >>   68 RETURN_VALUE
-         consts
-            '\n    Args:\n        get: A callable function that takes a string as input and returns a value.\n        value: Either a value of type _T or a string. If it is a string, it will be passed to the "get" function to\n        retrieve the corresponding value.\n\n    Returns:\n        A value of type _T. If the "value" parameter is not a string, it is returned as is. If it is a string, the\n        "get" function is called with the string as input to retrieve the corresponding value, which is then returned.\n\n    '
-         names      ('isinstance', 'str')
-         varnames   ('get', 'value')
-         freevars   ()
-         cellvars   ()
-         filename   '/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py'
-         name       '_get_if_needed'
-         firstlineno 105
-         lnotab 0x020c
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 6
          flags     : 0
          code
             0x970065005a0164005a0264015a03640265046403650464046505660664
             0584045a0664065300
-         120           0 RESUME                   0
+          97           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('TokenDistanceAlgorithm')
                        8 STORE_NAME               2 (__qualname__)
          
-         121          10 LOAD_CONST               1 ('\n    This class represents a token distance algorithm.\n\n    Methods:\n    - __call__: Calculates the token distance between two strings.\n\n    ')
+          98          10 LOAD_CONST               1 ('\n    This class represents a token distance algorithm.\n\n    Methods:\n    - __call__: Calculates the token distance between two strings.\n\n    ')
                       12 STORE_NAME               3 (__doc__)
          
-         128          14 LOAD_CONST               2 ('left')
+         105          14 LOAD_CONST               2 ('left')
                       16 LOAD_NAME                4 (str)
                       18 LOAD_CONST               3 ('right')
                       20 LOAD_NAME                4 (str)
                       22 LOAD_CONST               4 ('return')
                       24 LOAD_NAME                5 (float)
                       26 BUILD_TUPLE              6
-                      28 LOAD_CONST               5 (<code object __call__, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py", line 128>)
+                      28 LOAD_CONST               5 (<code object __call__, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py", line 105>)
                       30 MAKE_FUNCTION            4 (annotations)
                       32 STORE_NAME               6 (__call__)
                       34 LOAD_CONST               6 (None)
                       36 RETURN_VALUE
          consts
             'TokenDistanceAlgorithm'
             '\n    This class represents a token distance algorithm.\n\n    Methods:\n    - __call__: Calculates the token distance between two strings.\n\n    '
@@ -714,36 +559,36 @@
             'return'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
                flags     : 3
                code 0x970064005300
-               128           0 RESUME                   0
+               105           0 RESUME                   0
                
-               129           2 LOAD_CONST               0 (None)
+               106           2 LOAD_CONST               0 (None)
                              4 RETURN_VALUE
                consts
                   None
                names      ()
                varnames   ('self', 'left', 'right')
                freevars   ()
                cellvars   ()
                filename   '/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py'
                name       '__call__'
-               firstlineno 128
+               firstlineno 105
                lnotab 0x0201
             None
          names      ('__name__', '__module__', '__qualname__', '__doc__', 'str', 'float', '__call__')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py'
          name       'TokenDistanceAlgorithm'
-         firstlineno 120
+         firstlineno 97
          lnotab 0x0a010407
       'TokenDistanceAlgorithm'
       'config'
       code
          argcount  : 1
          nlocals   : 3
          stacksize : 9
@@ -758,69 +603,69 @@
             0000000000000089006a0a0000000000000000a6020000ab020000000000
             000000a6040000ab0400000000000000008a036401741600000000000000
             000000640274160000000000000000000064037418000000000000000000
             0066068803880066026404840c7d027c025300
                        0 MAKE_CELL                0 (config)
                        2 MAKE_CELL                3 (algorithm)
          
-         132           4 RESUME                   0
+         110           4 RESUME                   0
          
-         145           6 LOAD_DEREF               0 (config)
+         123           6 LOAD_DEREF               0 (config)
                        8 LOAD_ATTR                0 (exclusive)
                       18 POP_JUMP_FORWARD_IF_FALSE     7 (to 34)
                       20 LOAD_GLOBAL              2 (exclusive_token_distance)
                       32 JUMP_FORWARD             6 (to 46)
                  >>   34 LOAD_GLOBAL              4 (token_distance)
          
-         142     >>   46 STORE_FAST               1 (base_algorithm)
+         120     >>   46 STORE_FAST               1 (base_algorithm)
          
-         147          48 LOAD_GLOBAL              7 (NULL + partial)
+         125          48 LOAD_GLOBAL              7 (NULL + partial)
          
-         148          60 LOAD_FAST                1 (base_algorithm)
+         126          60 LOAD_FAST                1 (base_algorithm)
          
-         149          62 LOAD_GLOBAL              9 (NULL + _get_if_needed)
+         127          62 LOAD_GLOBAL              9 (NULL + get_if_needed)
                       74 LOAD_GLOBAL             10 (get_similarity_by_name)
                       86 LOAD_DEREF               0 (config)
                       88 LOAD_ATTR                6 (similarity)
                       98 PRECALL                  2
                      102 CALL                     2
          
-         150         112 LOAD_GLOBAL              9 (NULL + _get_if_needed)
+         128         112 LOAD_GLOBAL              9 (NULL + get_if_needed)
                      124 LOAD_GLOBAL             14 (get_mean_by_name)
                      136 LOAD_DEREF               0 (config)
                      138 LOAD_ATTR                8 (mean)
                      148 PRECALL                  2
                      152 CALL                     2
          
-         151         162 LOAD_GLOBAL              9 (NULL + _get_if_needed)
+         129         162 LOAD_GLOBAL              9 (NULL + get_if_needed)
                      174 LOAD_GLOBAL             18 (get_weight_by_name)
                      186 LOAD_DEREF               0 (config)
                      188 LOAD_ATTR               10 (weight)
                      198 PRECALL                  2
                      202 CALL                     2
          
-         147         212 PRECALL                  4
+         125         212 PRECALL                  4
                      216 CALL                     4
                      226 STORE_DEREF              3 (algorithm)
          
-         154         228 LOAD_CONST               1 ('left')
+         132         228 LOAD_CONST               1 ('left')
                      230 LOAD_GLOBAL             22 (str)
                      242 LOAD_CONST               2 ('right')
                      244 LOAD_GLOBAL             22 (str)
                      256 LOAD_CONST               3 ('return')
                      258 LOAD_GLOBAL             24 (float)
                      270 BUILD_TUPLE              6
                      272 LOAD_CLOSURE             3 (algorithm)
                      274 LOAD_CLOSURE             0 (config)
                      276 BUILD_TUPLE              2
-                     278 LOAD_CONST               4 (<code object distance, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py", line 154>)
+                     278 LOAD_CONST               4 (<code object distance, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py", line 132>)
                      280 MAKE_FUNCTION           12 (annotations, closure)
                      282 STORE_FAST               2 (distance)
          
-         168         284 LOAD_FAST                2 (distance)
+         146         284 LOAD_FAST                2 (distance)
                      286 RETURN_VALUE
          consts
             '\n    Constructs a TokenDistanceAlgorithm function based on the provided configuration.\n\n    Args:\n        config: A Config object containing the algorithm configuration.\n\n    Returns:\n        A TokenDistanceAlgorithm function that calculates the distance between two strings.\n    '
             'left'
             'right'
             'return'
             code
@@ -833,67 +678,67 @@
                   0000007404000000000000000000007407000000000000000000007c0089
                   036a040000000000000000a6020000ab020000000000000000a6020000ab
                   020000000000000000a6010000ab01000000000000000074070000000000
                   00000000007c0189036a040000000000000000a6020000ab020000000000
                   000000a6020000ab0200000000000000005300
                              0 COPY_FREE_VARS           2
                
-               154           2 RESUME                   0
+               132           2 RESUME                   0
                
-               163           4 PUSH_NULL
+               141           4 PUSH_NULL
                              6 LOAD_DEREF               2 (algorithm)
                
-               164           8 LOAD_GLOBAL              1 (NULL + tuple)
+               142           8 LOAD_GLOBAL              1 (NULL + tuple)
                             20 LOAD_GLOBAL              3 (NULL + map)
                             32 LOAD_GLOBAL              4 (parse_token)
                             44 LOAD_GLOBAL              7 (NULL + split_text_by)
                             56 LOAD_FAST                0 (left)
                             58 LOAD_DEREF               3 (config)
                             60 LOAD_ATTR                4 (tokenize)
                             70 PRECALL                  2
                             74 CALL                     2
                             84 PRECALL                  2
                             88 CALL                     2
                             98 PRECALL                  1
                            102 CALL                     1
                
-               165         112 LOAD_GLOBAL              7 (NULL + split_text_by)
+               143         112 LOAD_GLOBAL              7 (NULL + split_text_by)
                            124 LOAD_FAST                1 (right)
                            126 LOAD_DEREF               3 (config)
                            128 LOAD_ATTR                4 (tokenize)
                            138 PRECALL                  2
                            142 CALL                     2
                
-               163         152 PRECALL                  2
+               141         152 PRECALL                  2
                            156 CALL                     2
                            166 RETURN_VALUE
                consts
                   '\n        Args:\n            left: A string representing the left text.\n            right: A string representing the right text.\n\n        Returns:\n            A float representing the token distance between the left and right texts.\n        '
                names      ('tuple', 'map', 'parse_token', 'split_text_by', 'tokenize')
                varnames   ('left', 'right')
                freevars   ('algorithm', 'config')
                cellvars   ()
                filename   '/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py'
                name       'distance'
-               firstlineno 154
+               firstlineno 132
                lnotab 0x04090401680128fe
-         names      ('exclusive', 'exclusive_token_distance', 'token_distance', 'partial', '_get_if_needed', 'get_similarity_by_name', 'similarity', 'get_mean_by_name', 'mean', 'get_weight_by_name', 'weight', 'str', 'float')
+         names      ('exclusive', 'exclusive_token_distance', 'token_distance', 'partial', 'get_if_needed', 'get_similarity_by_name', 'similarity', 'get_mean_by_name', 'mean', 'get_weight_by_name', 'weight', 'str', 'float')
          varnames   ('config', 'base_algorithm', 'distance')
          freevars   ()
          cellvars   ('config', 'algorithm')
          filename   '/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py'
          name       'from_config'
-         firstlineno 132
+         firstlineno 110
          lnotab 0x060d28fd02050c0102013201320132fc1007380e
       None
-   names      ('collections.abc', 'Collection', 'Callable', 'Sequence', 'dataclasses', 'dataclass', 'functools', 'partial', 'operator', 'attrgetter', 're', 'Pattern', 'typing', 'TypeVar', 'Protocol', 'token_distance.means', 'Mean', 'average', 'get_mean_by_name', 'token_distance.similarities', 'Similarity', 'as_recording', 'RecordingSimilarity', 'jaro_winkler', 'get_similarity_by_name', 'token_distance.types.token', 'WeightedToken', 'Token', 'EvaluatedToken', 'RecordingToken', 'split_text_by', 'parse_token', 'token_distance.weights', 'Weight', 'even_weight', 'get_weight_by_name', 'str', 'float', 'token_distance', 'exclusive_token_distance', 'Config', '_T', '_get_if_needed', 'TokenDistanceAlgorithm', 'from_config')
+   names      ('collections.abc', 'Collection', 'Callable', 'Sequence', 'dataclasses', 'dataclass', 'functools', 'partial', 're', 'Pattern', 'typing', 'TypeVar', 'Protocol', 'token_distance.algorithms.token_matching', 'match_tokens', 'token_distance.means', 'Mean', 'average', 'get_mean_by_name', 'token_distance.similarities', 'Similarity', 'jaro_winkler', 'get_similarity_by_name', 'token_distance.types.registry', 'get_if_needed', 'token_distance.types.token', 'WeightedToken', 'Token', 'EvaluatedToken', 'split_text_by', 'parse_token', 'token_distance.weights', 'Weight', 'even_weight', 'get_weight_by_name', 'str', 'float', 'token_distance', 'exclusive_token_distance', 'Config', '_T', 'TokenDistanceAlgorithm', 'from_config')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/voidpointercast/PycharmProjects/token-distance/token_distance/algorithms/token_distance.py'
    name       '<module>'
    firstlineno 1
    lnotab
-      0x00ff020114010c010c010c010c01100214011c0220011403020102ff02
-      0202fe020302fd02040efc02050efb020602fa081c020102ff020202fe02
-      0302fd02040efc02050efb020602fa0827020118ff0e01021316032c0f1c
-      0c
+      0x00ff020114010c010c010c0110020c01140114010c011c011403020102
+      ff020202fe020302fd02040efc02050efb020602fa081e020102ff020202
+      fe020302fd02040efc02050efb020602fa081a020118ff0e01021316061c
+      0d
```

### Comparing `token_distance-0.1.0/token_distance/algorithms/token_distance.py` & `token_distance-0.2.0/token_distance/algorithms/token_distance.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from collections.abc import Collection, Callable, Sequence
 from dataclasses import dataclass
 from functools import partial
-from operator import attrgetter
 from re import Pattern
 from typing import TypeVar, Protocol
 
+from token_distance.algorithms.token_matching import match_tokens
 from token_distance.means import Mean, average, get_mean_by_name
-from token_distance.similarities import Similarity, as_recording, RecordingSimilarity, jaro_winkler, \
-    get_similarity_by_name
-from token_distance.types.token import WeightedToken, Token, EvaluatedToken, RecordingToken, split_text_by, parse_token
+from token_distance.similarities import Similarity, jaro_winkler, get_similarity_by_name
+from token_distance.types.registry import get_if_needed
+from token_distance.types.token import WeightedToken, Token, EvaluatedToken, split_text_by, parse_token
 from token_distance.weights import Weight, even_weight, get_weight_by_name
 
 
 def token_distance(
     similarity: Similarity,
     mean: Mean,
     weight: Weight,
@@ -36,14 +36,16 @@
     evaluated_tokens: Collection[EvaluatedToken] = [
         max(similarity(token, candidate) for candidate in candidates)
         for token in weighted_tokens
     ]
     return mean(evaluated_tokens)
 
 
+
+
 def exclusive_token_distance(
     similarity: Similarity,
     mean: Mean,
     weight: Weight,
     tokens: Collection[Token],
     candidates: Collection[str]
 ) -> float:
@@ -59,28 +61,15 @@
         tokens: A collection of Token instances representing the tokens to be evaluated.
         candidates: A collection of strings representing the candidate tokens to compare with.
 
     Returns:
         float: The result of applying the mean function to the evaluated tokens.
 
     """
-    remaining_candidates: list[str] = list(candidates)
-    recording_sim: RecordingSimilarity = as_recording(similarity)
-    weighted_tokens: list[WeightedToken] = sorted(weight(tokens), key=attrgetter('weight'), reverse=True)
-    evaluated_tokens: list[EvaluatedToken] = list()
-    for token in weighted_tokens:
-        if not remaining_candidates:
-            evaluated_tokens.append(similarity(token, ''))
-        else:
-            evaluate: Callable[[str], RecordingToken] = partial(recording_sim, token)
-            best: RecordingToken = max(map(evaluate, remaining_candidates))
-            evaluated_tokens.append(best)
-            if best.matched_with is not None:
-                remaining_candidates.remove(best.matched_with)
-    return mean(evaluated_tokens)
+    return mean(match_tokens(similarity, weight, True, tokens, candidates))
 
 
 @dataclass
 class Config:
     """
     Config represents the configuration options for token distance.
 
@@ -98,41 +87,30 @@
     tokenize: Callable[[str], Sequence[str]] | Pattern | str | None = None
     exclusive: bool = False
 
 
 _T = TypeVar('_T')
 
 
-def _get_if_needed(get: Callable[[str], _T], value: _T | str) -> _T:
-    """
-    Args:
-        get: A callable function that takes a string as input and returns a value.
-        value: Either a value of type _T or a string. If it is a string, it will be passed to the "get" function to
-        retrieve the corresponding value.
 
-    Returns:
-        A value of type _T. If the "value" parameter is not a string, it is returned as is. If it is a string, the
-        "get" function is called with the string as input to retrieve the corresponding value, which is then returned.
-
-    """
-    return value if not isinstance(value, str) else get(value)
 
 
 class TokenDistanceAlgorithm(Protocol):
     """
     This class represents a token distance algorithm.
 
     Methods:
     - __call__: Calculates the token distance between two strings.
 
     """
     def __call__(self, left: str, right: str) -> float:
         ...
 
 
+
 def from_config(config: Config = Config()) -> TokenDistanceAlgorithm:
     """
     Constructs a TokenDistanceAlgorithm function based on the provided configuration.
 
     Args:
         config: A Config object containing the algorithm configuration.
 
@@ -142,17 +120,17 @@
     base_algorithm: Callable[
         [Similarity, Mean, Weight, Collection[Token], Collection[str]],
         float
     ] = exclusive_token_distance if config.exclusive else token_distance
 
     algorithm: Callable[[Collection[Token], Collection[str]], float] = partial(
         base_algorithm,
-        _get_if_needed(get_similarity_by_name, config.similarity),
-        _get_if_needed(get_mean_by_name, config.mean),
-        _get_if_needed(get_weight_by_name, config.weight),
+        get_if_needed(get_similarity_by_name, config.similarity),
+        get_if_needed(get_mean_by_name, config.mean),
+        get_if_needed(get_weight_by_name, config.weight),
     )
 
     def distance(left: str, right: str) -> float:
         """
         Args:
             left: A string representing the left text.
             right: A string representing the right text.
```

### Comparing `token_distance-0.1.0/token_distance/means/__init__.py` & `token_distance-0.2.0/token_distance/means/__init__.py`

 * *Files identical despite different names*

### Comparing `token_distance-0.1.0/token_distance/means/__pycache__/__init__.cpython-311.pyc` & `token_distance-0.2.0/token_distance/means/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `token_distance-0.1.0/token_distance/means/__pycache__/base.cpython-311.pyc` & `token_distance-0.2.0/token_distance/means/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `token_distance-0.1.0/token_distance/means/base.py` & `token_distance-0.2.0/token_distance/means/base.py`

 * *Files identical despite different names*

### Comparing `token_distance-0.1.0/token_distance/similarities/__init__.py` & `token_distance-0.2.0/token_distance/similarities/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 
 class RecordingSimilarity(Similarity, Protocol):
     """
     Module: RecordingSimilarity
 
     This module provides the class `RecordingSimilarity` which is responsible for calculating the similarity between a
-    `WeightedToken` and a `str` recording the match..
+    `WeightedToken` and a `str` recording the match.
     """
     def __call__(self, left: WeightedToken, right: str) -> RecordingToken:
         ...
 
 
 def as_recording(similarity: Similarity) -> RecordingSimilarity:
     """
```

### Comparing `token_distance-0.1.0/token_distance/similarities/__pycache__/__init__.cpython-311.pyc` & `token_distance-0.2.0/token_distance/similarities/__pycache__/__init__.cpython-311.pyc`

 * *Files 2% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x9ccd5866 (Thu May 30 19:03:56 2024 UTC)
-files sz: 1930
+moddate:  0xe5405b66 (Sat Jun  1 15:40:21 2024 UTC)
+files sz: 1929
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
       0x97005500640064016c006d015a016d025a020100640064026c036d045a
@@ -224,15 +224,15 @@
             0584045a0764065300
           23           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('RecordingSimilarity')
                        8 STORE_NAME               2 (__qualname__)
          
-          24          10 LOAD_CONST               1 ('\n    Module: RecordingSimilarity\n\n    This module provides the class `RecordingSimilarity` which is responsible for calculating the similarity between a\n    `WeightedToken` and a `str` recording the match..\n    ')
+          24          10 LOAD_CONST               1 ('\n    Module: RecordingSimilarity\n\n    This module provides the class `RecordingSimilarity` which is responsible for calculating the similarity between a\n    `WeightedToken` and a `str` recording the match.\n    ')
                       12 STORE_NAME               3 (__doc__)
          
           30          14 LOAD_CONST               2 ('left')
                       16 LOAD_NAME                4 (WeightedToken)
                       18 LOAD_CONST               3 ('right')
                       20 LOAD_NAME                5 (str)
                       22 LOAD_CONST               4 ('return')
@@ -241,15 +241,15 @@
                       28 LOAD_CONST               5 (<code object __call__, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/similarities/__init__.py", line 30>)
                       30 MAKE_FUNCTION            4 (annotations)
                       32 STORE_NAME               7 (__call__)
                       34 LOAD_CONST               6 (None)
                       36 RETURN_VALUE
          consts
             'RecordingSimilarity'
-            '\n    Module: RecordingSimilarity\n\n    This module provides the class `RecordingSimilarity` which is responsible for calculating the similarity between a\n    `WeightedToken` and a `str` recording the match..\n    '
+            '\n    Module: RecordingSimilarity\n\n    This module provides the class `RecordingSimilarity` which is responsible for calculating the similarity between a\n    `WeightedToken` and a `str` recording the match.\n    '
             'left'
             'right'
             'return'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 1
```

### Comparing `token_distance-0.1.0/token_distance/similarities/__pycache__/base.cpython-311.pyc` & `token_distance-0.2.0/token_distance/similarities/__pycache__/base.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `token_distance-0.1.0/token_distance/similarities/base.py` & `token_distance-0.2.0/token_distance/similarities/base.py`

 * *Files identical despite different names*

### Comparing `token_distance-0.1.0/token_distance/types/__pycache__/registry.cpython-311.pyc` & `token_distance-0.2.0/token_distance/types/__pycache__/registry.cpython-311.pyc`

 * *Files 22% similar despite different names*

#### Python bytecode

```diff
@@ -1,87 +1,108 @@
 magic:    0xa70d0d0a
-moddate:  0x9d365666 (Tue May 28 19:55:09 2024 UTC)
-files sz: 2017
+moddate:  0x9e455b66 (Sat Jun  1 16:00:30 2024 UTC)
+files sz: 2676
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 6
    flags     : 0
    code
-      0x9700640064016c006d015a010100640064026c026d035a036d045a046d
-      055a056d065a066d075a0701006506020047006403840064046507a60300
-      00ab030000000000000000a6000000ab0000000000000000005a08020065
-      0364056508ac06a6020000ab0200000000000000005a0902004700640784
-      0064086504650919000000000000000000a6030000ab0300000000000000
-      005a0a64095300
+      0x9700640064016c006d015a016d025a020100640064026c036d045a046d
+      055a056d065a066d075a076d085a08010065070200470064038400640465
+      08a6030000ab030000000000000000a6000000ab0000000000000000005a
+      090200650464056509ac06a6020000ab0200000000000000005a0a020047
+      006407840064086505650a19000000000000000000a6030000ab03000000
+      00000000005a0b64096502650c6701650a66021900000000000000000064
+      0a650a650c7a070000640b650a6606640c84045a0d640d5300
      0           0 RESUME                   0
    
      1           2 LOAD_CONST               0 (0)
-                 4 LOAD_CONST               1 (('Iterator',))
+                 4 LOAD_CONST               1 (('Iterator', 'Callable'))
                  6 IMPORT_NAME              0 (collections.abc)
                  8 IMPORT_FROM              1 (Iterator)
                 10 STORE_NAME               1 (Iterator)
-                12 POP_TOP
+                12 IMPORT_FROM              2 (Callable)
+                14 STORE_NAME               2 (Callable)
+                16 POP_TOP
    
-     2          14 LOAD_CONST               0 (0)
-                16 LOAD_CONST               2 (('TypeVar', 'Generic', 'Sequence', 'runtime_checkable', 'Protocol'))
-                18 IMPORT_NAME              2 (typing)
-                20 IMPORT_FROM              3 (TypeVar)
-                22 STORE_NAME               3 (TypeVar)
-                24 IMPORT_FROM              4 (Generic)
-                26 STORE_NAME               4 (Generic)
-                28 IMPORT_FROM              5 (Sequence)
-                30 STORE_NAME               5 (Sequence)
-                32 IMPORT_FROM              6 (runtime_checkable)
-                34 STORE_NAME               6 (runtime_checkable)
-                36 IMPORT_FROM              7 (Protocol)
-                38 STORE_NAME               7 (Protocol)
-                40 POP_TOP
+     2          18 LOAD_CONST               0 (0)
+                20 LOAD_CONST               2 (('TypeVar', 'Generic', 'Sequence', 'runtime_checkable', 'Protocol'))
+                22 IMPORT_NAME              3 (typing)
+                24 IMPORT_FROM              4 (TypeVar)
+                26 STORE_NAME               4 (TypeVar)
+                28 IMPORT_FROM              5 (Generic)
+                30 STORE_NAME               5 (Generic)
+                32 IMPORT_FROM              6 (Sequence)
+                34 STORE_NAME               6 (Sequence)
+                36 IMPORT_FROM              7 (runtime_checkable)
+                38 STORE_NAME               7 (runtime_checkable)
+                40 IMPORT_FROM              8 (Protocol)
+                42 STORE_NAME               8 (Protocol)
+                44 POP_TOP
    
-     5          42 LOAD_NAME                6 (runtime_checkable)
+     5          46 LOAD_NAME                7 (runtime_checkable)
    
-     6          44 PUSH_NULL
-                46 LOAD_BUILD_CLASS
-                48 LOAD_CONST               3 (<code object HasName, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/types/registry.py", line 5>)
-                50 MAKE_FUNCTION            0
-                52 LOAD_CONST               4 ('HasName')
-                54 LOAD_NAME                7 (Protocol)
-                56 PRECALL                  3
-                60 CALL                     3
+     6          48 PUSH_NULL
+                50 LOAD_BUILD_CLASS
+                52 LOAD_CONST               3 (<code object HasName, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/types/registry.py", line 5>)
+                54 MAKE_FUNCTION            0
+                56 LOAD_CONST               4 ('HasName')
+                58 LOAD_NAME                8 (Protocol)
+                60 PRECALL                  3
+                64 CALL                     3
    
-     5          70 PRECALL                  0
-                74 CALL                     0
+     5          74 PRECALL                  0
+                78 CALL                     0
    
-     6          84 STORE_NAME               8 (HasName)
+     6          88 STORE_NAME               9 (HasName)
    
-    10          86 PUSH_NULL
-                88 LOAD_NAME                3 (TypeVar)
-                90 LOAD_CONST               5 ('_T')
-                92 LOAD_NAME                8 (HasName)
-                94 KW_NAMES                 6
-                96 PRECALL                  2
-               100 CALL                     2
-               110 STORE_NAME               9 (_T)
+    10          90 PUSH_NULL
+                92 LOAD_NAME                4 (TypeVar)
+                94 LOAD_CONST               5 ('_T')
+                96 LOAD_NAME                9 (HasName)
+                98 KW_NAMES                 6
+               100 PRECALL                  2
+               104 CALL                     2
+               114 STORE_NAME              10 (_T)
    
-    13         112 PUSH_NULL
-               114 LOAD_BUILD_CLASS
-               116 LOAD_CONST               7 (<code object AlgorithmRegistry, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/types/registry.py", line 13>)
-               118 MAKE_FUNCTION            0
-               120 LOAD_CONST               8 ('AlgorithmRegistry')
-               122 LOAD_NAME                4 (Generic)
-               124 LOAD_NAME                9 (_T)
-               126 BINARY_SUBSCR
-               136 PRECALL                  3
-               140 CALL                     3
-               150 STORE_NAME              10 (AlgorithmRegistry)
-               152 LOAD_CONST               9 (None)
-               154 RETURN_VALUE
+    13         116 PUSH_NULL
+               118 LOAD_BUILD_CLASS
+               120 LOAD_CONST               7 (<code object AlgorithmRegistry, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/types/registry.py", line 13>)
+               122 MAKE_FUNCTION            0
+               124 LOAD_CONST               8 ('AlgorithmRegistry')
+               126 LOAD_NAME                5 (Generic)
+               128 LOAD_NAME               10 (_T)
+               130 BINARY_SUBSCR
+               140 PRECALL                  3
+               144 CALL                     3
+               154 STORE_NAME              11 (AlgorithmRegistry)
+   
+    64         156 LOAD_CONST               9 ('get')
+               158 LOAD_NAME                2 (Callable)
+               160 LOAD_NAME               12 (str)
+               162 BUILD_LIST               1
+               164 LOAD_NAME               10 (_T)
+               166 BUILD_TUPLE              2
+               168 BINARY_SUBSCR
+               178 LOAD_CONST              10 ('value')
+               180 LOAD_NAME               10 (_T)
+               182 LOAD_NAME               12 (str)
+               184 BINARY_OP                7 (|)
+               188 LOAD_CONST              11 ('return')
+               190 LOAD_NAME               10 (_T)
+               192 BUILD_TUPLE              6
+               194 LOAD_CONST              12 (<code object get_if_needed, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/types/registry.py", line 64>)
+               196 MAKE_FUNCTION            4 (annotations)
+               198 STORE_NAME              13 (get_if_needed)
+               200 LOAD_CONST              13 (None)
+               202 RETURN_VALUE
    consts
       0
-      ('Iterator',)
+      ('Iterator', 'Callable')
       ('TypeVar', 'Generic', 'Sequence', 'runtime_checkable', 'Protocol')
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 3
          flags     : 0
          code 0x970065005a0164005a0255006503650464013c00000064025300
@@ -376,16 +397,54 @@
          freevars   ()
          cellvars   ()
          filename   '/home/voidpointercast/PycharmProjects/token-distance/token_distance/types/registry.py'
          name       'AlgorithmRegistry'
          firstlineno 13
          lnotab 0x0a0104180c061803020116ff0e010209
       'AlgorithmRegistry'
+      'get'
+      'value'
+      'return'
+      code
+         argcount  : 2
+         nlocals   : 2
+         stacksize : 4
+         flags     : 3
+         code
+            0x97007401000000000000000000007c01740200000000000000000000a6
+            020000ab02000000000000000073027c016e0a02007c007c01a6010000ab
+            0100000000000000005300
+          64           0 RESUME                   0
+         
+          76           2 LOAD_GLOBAL              1 (NULL + isinstance)
+                      14 LOAD_FAST                1 (value)
+                      16 LOAD_GLOBAL              2 (str)
+                      28 PRECALL                  2
+                      32 CALL                     2
+                      42 POP_JUMP_FORWARD_IF_TRUE     2 (to 48)
+                      44 LOAD_FAST                1 (value)
+                      46 JUMP_FORWARD            10 (to 68)
+                 >>   48 PUSH_NULL
+                      50 LOAD_FAST                0 (get)
+                      52 LOAD_FAST                1 (value)
+                      54 PRECALL                  1
+                      58 CALL                     1
+                 >>   68 RETURN_VALUE
+         consts
+            '\n    Args:\n        get: A callable function that takes a string as input and returns a value.\n        value: Either a value of type _T or a string. If it is a string, it will be passed to the "get" function to\n        retrieve the corresponding value.\n\n    Returns:\n        A value of type _T. If the "value" parameter is not a string, it is returned as is. If it is a string, the\n        "get" function is called with the string as input to retrieve the corresponding value, which is then returned.\n\n    '
+         names      ('isinstance', 'str')
+         varnames   ('get', 'value')
+         freevars   ()
+         cellvars   ()
+         filename   '/home/voidpointercast/PycharmProjects/token-distance/token_distance/types/registry.py'
+         name       'get_if_needed'
+         firstlineno 64
+         lnotab 0x020c
       None
-   names      ('collections.abc', 'Iterator', 'typing', 'TypeVar', 'Generic', 'Sequence', 'runtime_checkable', 'Protocol', 'HasName', '_T', 'AlgorithmRegistry')
+   names      ('collections.abc', 'Iterator', 'Callable', 'typing', 'TypeVar', 'Generic', 'Sequence', 'runtime_checkable', 'Protocol', 'HasName', '_T', 'AlgorithmRegistry', 'str', 'get_if_needed')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/voidpointercast/PycharmProjects/token-distance/token_distance/types/registry.py'
    name       '<module>'
    firstlineno 1
-   lnotab 0x00ff02010c011c0302011aff0e0102041a03
+   lnotab 0x00ff020110011c0302011aff0e0102041a032833
```

### Comparing `token_distance-0.1.0/token_distance/types/__pycache__/token.cpython-311.pyc` & `token_distance-0.2.0/token_distance/types/__pycache__/token.cpython-311.pyc`

 * *Files 8% similar despite different names*

#### Python bytecode

```diff
@@ -1,10 +1,10 @@
 magic:    0xa70d0d0a
-moddate:  0x32a55866 (Thu May 30 16:11:30 2024 UTC)
-files sz: 4240
+moddate:  0x314e5b66 (Sat Jun  1 16:37:05 2024 UTC)
+files sz: 4699
 code
    argcount  : 0
    nlocals   : 0
    stacksize : 8
    flags     : 0
    code
       0x9700640064016c006d015a016d025a026d035a030100640064026c046d
@@ -129,46 +129,46 @@
                262 CALL                     3
    
     76         272 PRECALL                  0
                276 CALL                     0
    
     77         286 STORE_NAME              15 (RecordingToken)
    
-   103         288 NOP
+   110         288 NOP
    
-   101         290 LOAD_CONST              21 ((None,))
+   108         290 LOAD_CONST              21 ((None,))
                292 LOAD_CONST              18 ('text')
    
-   102         294 LOAD_NAME               10 (str)
+   109         294 LOAD_NAME               10 (str)
    
-   101         296 LOAD_CONST              19 ('by')
+   108         296 LOAD_CONST              19 ('by')
    
-   103         298 LOAD_NAME                1 (Callable)
+   110         298 LOAD_NAME                1 (Callable)
                300 LOAD_NAME               10 (str)
                302 BUILD_LIST               1
                304 LOAD_NAME                2 (Sequence)
                306 LOAD_NAME               10 (str)
                308 BINARY_SUBSCR
                318 BUILD_TUPLE              2
                320 BINARY_SUBSCR
                330 LOAD_NAME                7 (Pattern)
                332 BINARY_OP                7 (|)
                336 LOAD_NAME               10 (str)
                338 BINARY_OP                7 (|)
                342 LOAD_CONST              17 (None)
                344 BINARY_OP                7 (|)
    
-   101         348 LOAD_CONST               7 ('return')
+   108         348 LOAD_CONST               7 ('return')
    
-   104         350 LOAD_NAME                3 (Collection)
+   111         350 LOAD_NAME                3 (Collection)
                352 LOAD_NAME               10 (str)
                354 BINARY_SUBSCR
    
-   101         364 BUILD_TUPLE              6
-               366 LOAD_CONST              20 (<code object split_text_by, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/types/token.py", line 101>)
+   108         364 BUILD_TUPLE              6
+               366 LOAD_CONST              20 (<code object split_text_by, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/types/token.py", line 108>)
                368 MAKE_FUNCTION            5 (defaults, annotations)
                370 STORE_NAME              16 (split_text_by)
                372 LOAD_CONST              17 (None)
                374 RETURN_VALUE
    consts
       0
       ('Callable', 'Sequence', 'Collection')
@@ -512,75 +512,86 @@
       code
          argcount  : 0
          nlocals   : 0
          stacksize : 7
          flags     : 0
          code
             0x970065005a0164005a02550064015a0364025a04650564027a07000065
-            0664033c0000006507640465086405650564027a07000064066400660664
-            078404a6000000ab0000000000000000005a0964025300
+            0664033c00000064025a07650864027a070000650664043c000000650964
+            05650a6406650564027a07000064076400660664088404a6000000ab0000
+            000000000000005a0b64025300
           76           0 RESUME                   0
                        2 LOAD_NAME                0 (__name__)
                        4 STORE_NAME               1 (__module__)
                        6 LOAD_CONST               0 ('RecordingToken')
                        8 STORE_NAME               2 (__qualname__)
                       10 SETUP_ANNOTATIONS
          
-          78          12 LOAD_CONST               1 ('\n    Class representing a recording token.\n\n    Attributes:\n        matched_with (str | None): The string that the token was matched with, or None if no match.\n    ')
+          78          12 LOAD_CONST               1 ('\n    The `RecordingToken` class is a subclass of `EvaluatedToken` and represents a token that has been matched with a\n    specific value.\n\n    Attributes:\n        token (Token): The token object.\n        weight (float): The weight of the token.\n        similarity (float): The similarity value of the token.\n        is_distance (bool): Flag indicating whether the similarity represents a distance.\n        matched_with (str | None): The value the token has been matched with.\n        matched_token_position (int | None): The position of the matched token in the recording.\n    ')
                       14 STORE_NAME               3 (__doc__)
          
-          84          16 LOAD_CONST               2 (None)
+          90          16 LOAD_CONST               2 (None)
                       18 STORE_NAME               4 (matched_with)
                       20 LOAD_NAME                5 (str)
                       22 LOAD_CONST               2 (None)
                       24 BINARY_OP                7 (|)
                       28 LOAD_NAME                6 (__annotations__)
                       30 LOAD_CONST               3 ('matched_with')
                       32 STORE_SUBSCR
          
-          86          36 LOAD_NAME                7 (classmethod)
-         
-          87          38 LOAD_CONST               4 ('token')
-                      40 LOAD_NAME                8 (EvaluatedToken)
-                      42 LOAD_CONST               5 ('match')
-                      44 LOAD_NAME                5 (str)
-                      46 LOAD_CONST               2 (None)
-                      48 BINARY_OP                7 (|)
-                      52 LOAD_CONST               6 ('return')
-                      54 LOAD_CONST               0 ('RecordingToken')
-                      56 BUILD_TUPLE              6
-                      58 LOAD_CONST               7 (<code object matched_from, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/types/token.py", line 86>)
-                      60 MAKE_FUNCTION            4 (annotations)
-         
-          86          62 PRECALL                  0
-                      66 CALL                     0
-         
-          87          76 STORE_NAME               9 (matched_from)
-                      78 LOAD_CONST               2 (None)
-                      80 RETURN_VALUE
+          91          36 LOAD_CONST               2 (None)
+                      38 STORE_NAME               7 (matched_token_position)
+                      40 LOAD_NAME                8 (int)
+                      42 LOAD_CONST               2 (None)
+                      44 BINARY_OP                7 (|)
+                      48 LOAD_NAME                6 (__annotations__)
+                      50 LOAD_CONST               4 ('matched_token_position')
+                      52 STORE_SUBSCR
+         
+          93          56 LOAD_NAME                9 (classmethod)
+         
+          94          58 LOAD_CONST               5 ('token')
+                      60 LOAD_NAME               10 (EvaluatedToken)
+                      62 LOAD_CONST               6 ('match')
+                      64 LOAD_NAME                5 (str)
+                      66 LOAD_CONST               2 (None)
+                      68 BINARY_OP                7 (|)
+                      72 LOAD_CONST               7 ('return')
+                      74 LOAD_CONST               0 ('RecordingToken')
+                      76 BUILD_TUPLE              6
+                      78 LOAD_CONST               8 (<code object matched_from, file "/home/voidpointercast/PycharmProjects/token-distance/token_distance/types/token.py", line 93>)
+                      80 MAKE_FUNCTION            4 (annotations)
+         
+          93          82 PRECALL                  0
+                      86 CALL                     0
+         
+          94          96 STORE_NAME              11 (matched_from)
+                      98 LOAD_CONST               2 (None)
+                     100 RETURN_VALUE
          consts
             'RecordingToken'
-            '\n    Class representing a recording token.\n\n    Attributes:\n        matched_with (str | None): The string that the token was matched with, or None if no match.\n    '
+            '\n    The `RecordingToken` class is a subclass of `EvaluatedToken` and represents a token that has been matched with a\n    specific value.\n\n    Attributes:\n        token (Token): The token object.\n        weight (float): The weight of the token.\n        similarity (float): The similarity value of the token.\n        is_distance (bool): Flag indicating whether the similarity represents a distance.\n        matched_with (str | None): The value the token has been matched with.\n        matched_token_position (int | None): The position of the matched token in the recording.\n    '
             None
             'matched_with'
+            'matched_token_position'
             'token'
             'match'
             'return'
             code
                argcount  : 3
                nlocals   : 3
                stacksize : 7
                flags     : 3
                code
                   0x97007401000000000000000000007c016a0100000000000000007c016a
                   0200000000000000007c016a0300000000000000007c016a040000000000
                   0000007c02a6050000ab0500000000000000005300
-                86           0 RESUME                   0
+                93           0 RESUME                   0
                
-                97           2 LOAD_GLOBAL              1 (NULL + RecordingToken)
+               104           2 LOAD_GLOBAL              1 (NULL + RecordingToken)
                             14 LOAD_FAST                1 (token)
                             16 LOAD_ATTR                1 (token)
                             26 LOAD_FAST                1 (token)
                             28 LOAD_ATTR                2 (weight)
                             38 LOAD_FAST                1 (token)
                             40 LOAD_ATTR                3 (similarity)
                             50 LOAD_FAST                1 (token)
@@ -593,24 +604,24 @@
                   '\n        Args:\n            token: An instance of the EvaluatedToken class representing the token.\n            match: A string representing the match value.\n\n        Returns:\n            An instance of the RecordingToken class.\n\n        '
                names      ('RecordingToken', 'token', 'weight', 'similarity', 'is_distance')
                varnames   ('cls', 'token', 'match')
                freevars   ()
                cellvars   ()
                filename   '/home/voidpointercast/PycharmProjects/token-distance/token_distance/types/token.py'
                name       'matched_from'
-               firstlineno 86
+               firstlineno 93
                lnotab 0x020b
-         names      ('__name__', '__module__', '__qualname__', '__doc__', 'matched_with', 'str', '__annotations__', 'classmethod', 'EvaluatedToken', 'matched_from')
+         names      ('__name__', '__module__', '__qualname__', '__doc__', 'matched_with', 'str', '__annotations__', 'matched_token_position', 'int', 'classmethod', 'EvaluatedToken', 'matched_from')
          varnames   ()
          freevars   ()
          cellvars   ()
          filename   '/home/voidpointercast/PycharmProjects/token-distance/token_distance/types/token.py'
          name       'RecordingToken'
          firstlineno 76
-         lnotab 0x0c0204061402020118ff0e01
+         lnotab 0x0c02040c14011402020118ff0e01
       'RecordingToken'
       None
       'text'
       'by'
       code
          argcount  : 2
          nlocals   : 2
@@ -623,87 +634,87 @@
             01a00000000000000000000000000000000000000000007c00a6010000ab
             01000000000000000053007403000000000000000000007c017406000000
             00000000000000a6020000ab02000000000000000072157c00a000000000
             00000000000000000000000000000000007c01a6010000ab010000000000
             00000053007409000000000000000000007c01a6010000ab010000000000
             000000720b02007c017c00a6010000ab0100000000000000005300740b00
             0000000000000000006402a6010000ab0100000000000000008201
-         101           0 RESUME                   0
+         108           0 RESUME                   0
          
-         126           2 LOAD_FAST                1 (by)
+         133           2 LOAD_FAST                1 (by)
                        4 POP_JUMP_FORWARD_IF_NOT_NONE    20 (to 46)
          
-         127           6 LOAD_FAST                0 (text)
+         134           6 LOAD_FAST                0 (text)
                        8 LOAD_METHOD              0 (split)
                       30 PRECALL                  0
                       34 CALL                     0
                       44 RETURN_VALUE
          
-         128     >>   46 LOAD_GLOBAL              3 (NULL + isinstance)
+         135     >>   46 LOAD_GLOBAL              3 (NULL + isinstance)
                       58 LOAD_FAST                1 (by)
                       60 LOAD_GLOBAL              4 (Pattern)
                       72 PRECALL                  2
                       76 CALL                     2
                       86 POP_JUMP_FORWARD_IF_FALSE    21 (to 130)
          
-         129          88 LOAD_FAST                1 (by)
+         136          88 LOAD_FAST                1 (by)
                       90 LOAD_METHOD              0 (split)
                      112 LOAD_FAST                0 (text)
                      114 PRECALL                  1
                      118 CALL                     1
                      128 RETURN_VALUE
          
-         130     >>  130 LOAD_GLOBAL              3 (NULL + isinstance)
+         137     >>  130 LOAD_GLOBAL              3 (NULL + isinstance)
                      142 LOAD_FAST                1 (by)
                      144 LOAD_GLOBAL              6 (str)
                      156 PRECALL                  2
                      160 CALL                     2
                      170 POP_JUMP_FORWARD_IF_FALSE    21 (to 214)
          
-         131         172 LOAD_FAST                0 (text)
+         138         172 LOAD_FAST                0 (text)
                      174 LOAD_METHOD              0 (split)
                      196 LOAD_FAST                1 (by)
                      198 PRECALL                  1
                      202 CALL                     1
                      212 RETURN_VALUE
          
-         132     >>  214 LOAD_GLOBAL              9 (NULL + callable)
+         139     >>  214 LOAD_GLOBAL              9 (NULL + callable)
                      226 LOAD_FAST                1 (by)
                      228 PRECALL                  1
                      232 CALL                     1
                      242 POP_JUMP_FORWARD_IF_FALSE    11 (to 266)
          
-         133         244 PUSH_NULL
+         140         244 PUSH_NULL
                      246 LOAD_FAST                1 (by)
                      248 LOAD_FAST                0 (text)
                      250 PRECALL                  1
                      254 CALL                     1
                      264 RETURN_VALUE
          
-         135     >>  266 LOAD_GLOBAL             11 (NULL + ValueError)
+         142     >>  266 LOAD_GLOBAL             11 (NULL + ValueError)
                      278 LOAD_CONST               2 ("Invalid 'by' argument")
                      280 PRECALL                  1
                      284 CALL                     1
                      294 RAISE_VARARGS            1
          consts
             "\n    Splits the given text by a specific delimiter.\n\n    Args:\n        text: A string representing the text to be split.\n        by: A delimiter for splitting the text. It can be a callable function, a regular expression pattern,\n            a string, or None. If None is provided, the text is split using whitespace.\n\n    Returns:\n        A collection of strings obtained by splitting the text according to the specified delimiter.\n\n    Raises:\n        ValueError: If the 'by' argument is not a valid type.\n\n    Note:\n        The 'by' argument can be one of the following types:\n            - Callable: A function that takes a string as input and returns a sequence of strings.\n            - Pattern: A regular expression pattern object.\n            - str: A string representing the delimiter to split the text.\n            - None: If None is provided, the text is split using whitespace.\n    "
             None
             "Invalid 'by' argument"
          names      ('split', 'isinstance', 'Pattern', 'str', 'callable', 'ValueError')
          varnames   ('text', 'by')
          freevars   ()
          cellvars   ()
          filename   '/home/voidpointercast/PycharmProjects/token-distance/token_distance/types/token.py'
          name       'split_text_by'
-         firstlineno 101
+         firstlineno 108
          lnotab 0x0219040128012a012a012a012a011e011602
       (None,)
    names      ('collections.abc', 'Callable', 'Sequence', 'Collection', 'dataclasses', 'dataclass', 're', 'Pattern', 'typing', 'NewType', 'str', 'Token', 'parse_token', 'WeightedToken', 'EvaluatedToken', 'RecordingToken', 'split_text_by')
    varnames   ()
    freevars   ()
    cellvars   ()
    filename   '/home/voidpointercast/PycharmProjects/token-distance/token_distance/types/token.py'
    name       '<module>'
    firstlineno 1
    lnotab
       0x00ff020114010c010c010c0218031003160118ff0e01021a16011aff0e
-      01022416011aff0e01021a02fe040102ff020232fe02030efd
+      01022416011aff0e01022102fe040102ff020232fe02030efd
```

### Comparing `token_distance-0.1.0/token_distance/types/token.py` & `token_distance-0.2.0/token_distance/types/token.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,20 +72,27 @@
         """
         return cls(token.token, token.weight, similarity, is_distance)
 
 
 @dataclass(frozen=True)
 class RecordingToken(EvaluatedToken):
     """
-    Class representing a recording token.
+    The `RecordingToken` class is a subclass of `EvaluatedToken` and represents a token that has been matched with a
+    specific value.
 
     Attributes:
-        matched_with (str | None): The string that the token was matched with, or None if no match.
+        token (Token): The token object.
+        weight (float): The weight of the token.
+        similarity (float): The similarity value of the token.
+        is_distance (bool): Flag indicating whether the similarity represents a distance.
+        matched_with (str | None): The value the token has been matched with.
+        matched_token_position (int | None): The position of the matched token in the recording.
     """
     matched_with: str | None = None
+    matched_token_position: int | None = None
 
     @classmethod
     def matched_from(cls, token: EvaluatedToken, match: str | None) -> 'RecordingToken':
         """
         Args:
             token: An instance of the EvaluatedToken class representing the token.
             match: A string representing the match value.
```

### Comparing `token_distance-0.1.0/token_distance/ui/__pycache__/console.cpython-311.pyc` & `token_distance-0.2.0/token_distance/ui/__pycache__/console.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `token_distance-0.1.0/token_distance/ui/console.py` & `token_distance-0.2.0/token_distance/ui/console.py`

 * *Files identical despite different names*

### Comparing `token_distance-0.1.0/token_distance/weights/__init__.py` & `token_distance-0.2.0/token_distance/weights/__init__.py`

 * *Files identical despite different names*

### Comparing `token_distance-0.1.0/token_distance/weights/__pycache__/__init__.cpython-311.pyc` & `token_distance-0.2.0/token_distance/weights/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `token_distance-0.1.0/token_distance/weights/__pycache__/common.cpython-311.pyc` & `token_distance-0.2.0/token_distance/weights/__pycache__/common.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `token_distance-0.1.0/token_distance/weights/common.py` & `token_distance-0.2.0/token_distance/weights/common.py`

 * *Files identical despite different names*

### Comparing `token_distance-0.1.0/PKG-INFO` & `token_distance-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: token-distance
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python library designed to perform fuzzy token matching within text documents. Utilizing advanced algorithms, this tool allows developers and data scientists to search and compare tokens based on flexible criteria, beyond exact matches. The library supports tokenization through whitespace, regular expressions, or custom functions, and provides weighted comparisons for nuanced analysis.
 Home-page: https://gitlab.com/patrick.daniel.gress/token-distance
 License: BSD
 Keywords: fuzzy match,search
 Author: voidpointercast
 Author-email: voidpointercast@justmail.de
 Requires-Python: >=3.10,<4.0
@@ -37,16 +37,15 @@
 reflects its importance, which could depend on factors like token length or predefined criteria.
 
 For each search token, token-distance identifies the most similar token in the target text based on these weights. The
 core of the library's functionality lies in how it calculates similarity: it pairs each search token with the best
 matching token in the target text and computes a weighted average of these pairings to produce a final similarity score.
 
 The operations of token-distance are summarized in the chart below, which illustrates the step-by-step process from
-tokenization to the calculation of similarity scores. This visual aid helps users understand how inputs are transformed
-into meaningful outputs.
+tokenization to the calculation of similarity scores. 
 
 
 ![](source/_static/schema.png)
 
 
 ## Installation
 
@@ -92,8 +91,18 @@
 
 calculate_distance: Callable[[str, str], float] = from_config(Config(mean='geometric'))
 ````
 
 This configuration uses a geometric mean to compute the similarity score between tokens, which is useful for certain
 types of textual analysis.
 
+token-distance can also obtain information about the actual matching of the tokens, if those are of interest:
+
+````python
+from collections.abc import Callable, Collection
+from token_distance import match_from_config, MatchConfig, RecordingToken
+
+get_best_matches: Callable[[str, str], Collection[RecordingToken]] = match_from_config(MatchConfig())
+````
+
+
```

