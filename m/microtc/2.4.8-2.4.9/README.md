# Comparing `tmp/microtc-2.4.8.tar.gz` & `tmp/microtc-2.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microtc-2.4.8.tar", last modified: Fri Feb 17 11:19:47 2023, max compression
+gzip compressed data, was "microtc-2.4.9.tar", last modified: Mon Feb 20 21:14:39 2023, max compression
```

## Comparing `microtc-2.4.8.tar` & `microtc-2.4.9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:19:47.900035 microtc-2.4.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-17 11:18:44.000000 microtc-2.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-17 11:18:44.000000 microtc-2.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-02-17 11:19:47.900035 microtc-2.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-02-17 11:18:44.000000 microtc-2.4.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:19:47.896035 microtc-2.4.8/microtc/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18951 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/emoticons.py
--rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/params.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/regscorewrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:19:47.900035 microtc-2.4.8/microtc/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    56751 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/resources/emoticons.json
--rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/scorewrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:19:47.900035 microtc-2.4.8/microtc/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/tests/test_classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/tests/test_command_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/tests/test_emoticons.py
--rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/tests/test_textmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/tests/test_weighting.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/tests/text.json
--rw-r--r--   0 runner    (1001) docker     (123)    23590 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/textmodel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:19:47.900035 microtc-2.4.8/microtc/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/tools/microtc-ensemble
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/tools/microtc-kfolds
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/tools/microtc-params
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/tools/microtc-perf
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/tools/microtc-predict
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/tools/microtc-retrain
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/tools/microtc-textModel
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/tools/microtc-train
--rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10773 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/weighting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-02-17 11:18:44.000000 microtc-2.4.8/microtc/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 11:19:47.900035 microtc-2.4.8/microtc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-02-17 11:19:47.000000 microtc-2.4.8/microtc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-17 11:19:47.000000 microtc-2.4.8/microtc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 11:19:47.000000 microtc-2.4.8/microtc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 11:19:47.000000 microtc-2.4.8/microtc.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-17 11:19:47.000000 microtc-2.4.8/microtc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 11:19:47.900035 microtc-2.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-02-17 11:18:44.000000 microtc-2.4.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 21:14:39.009085 microtc-2.4.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-20 21:13:46.000000 microtc-2.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-20 21:13:46.000000 microtc-2.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-02-20 21:14:39.005085 microtc-2.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-02-20 21:13:46.000000 microtc-2.4.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 21:14:39.005085 microtc-2.4.9/microtc/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18951 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6091 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/emoticons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9306 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/regscorewrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 21:14:39.005085 microtc-2.4.9/microtc/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)    56751 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/resources/emoticons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6537 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/scorewrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 21:14:39.005085 microtc-2.4.9/microtc/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/tests/test_classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/tests/test_command_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/tests/test_emoticons.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11213 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/tests/test_textmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2990 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5853 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/tests/test_weighting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/tests/text.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23594 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/textmodel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 21:14:39.005085 microtc-2.4.9/microtc/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/tools/microtc-ensemble
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/tools/microtc-kfolds
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/tools/microtc-params
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/tools/microtc-perf
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/tools/microtc-predict
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/tools/microtc-retrain
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/tools/microtc-textModel
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/tools/microtc-train
+-rw-r--r--   0 runner    (1001) docker     (123)     6443 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10816 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/weighting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-02-20 21:13:46.000000 microtc-2.4.9/microtc/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 21:14:39.005085 microtc-2.4.9/microtc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-02-20 21:14:38.000000 microtc-2.4.9/microtc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-02-20 21:14:38.000000 microtc-2.4.9/microtc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 21:14:38.000000 microtc-2.4.9/microtc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 21:14:38.000000 microtc-2.4.9/microtc.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-02-20 21:14:38.000000 microtc-2.4.9/microtc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 21:14:39.009085 microtc-2.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1888 2023-02-20 21:13:46.000000 microtc-2.4.9/setup.py
```

### Comparing `microtc-2.4.8/LICENSE` & `microtc-2.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/PKG-INFO` & `microtc-2.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microtc
-Version: 2.4.8
+Version: 2.4.9
 Summary: A generic minimal text classifier
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `microtc-2.4.8/README.rst` & `microtc-2.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/__init__.py` & `microtc-2.4.9/microtc/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,10 +24,10 @@
 syntactic analysis, etc. Contrary to traditional approaches,
 :math:`\mu\text{TC}` is a minimalist and multi-propose text-classifier able to tackle
 tasks independently of domain and language.
 
 The starting point is :py:class:`microtc.textmodel.TextModel`
 
 """
-__version__ = "2.4.8"
+__version__ = "2.4.9"
 
 from microtc.textmodel import TextModel
```

### Comparing `microtc-2.4.8/microtc/command_line.py` & `microtc-2.4.9/microtc/command_line.py`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/emoticons.py` & `microtc-2.4.9/microtc/emoticons.py`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/params.py` & `microtc-2.4.9/microtc/params.py`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/regscorewrapper.py` & `microtc-2.4.9/microtc/regscorewrapper.py`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/resources/emoticons.json` & `microtc-2.4.9/microtc/resources/emoticons.json`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/scorewrapper.py` & `microtc-2.4.9/microtc/scorewrapper.py`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/tests/test_classifier.py` & `microtc-2.4.9/microtc/tests/test_classifier.py`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/tests/test_command_line.py` & `microtc-2.4.9/microtc/tests/test_command_line.py`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/tests/test_emoticons.py` & `microtc-2.4.9/microtc/tests/test_emoticons.py`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/tests/test_textmodel.py` & `microtc-2.4.9/microtc/tests/test_textmodel.py`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/tests/test_utils.py` & `microtc-2.4.9/microtc/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/tests/test_weighting.py` & `microtc-2.4.9/microtc/tests/test_weighting.py`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/textmodel.py` & `microtc-2.4.9/microtc/textmodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -747,15 +747,15 @@
         Token identifier to token
 
         >>> from microtc.textmodel import TextModel
         >>> corpus = ['buenos dias', 'catedras de conacyt', 'categorizacion de texto ingeotec']
         >>> textmodel = TextModel().fit(corpus)
         >>> _ = textmodel.transform(corpus)
         >>> textmodel.id2token[0]
-        'de'
+        'buenos'
         """
         try:
             return self._id2token
         except AttributeError:
             self._id2token = {v:k for k, v in self.token2id.items()}
             return self._id2token
 
@@ -765,12 +765,12 @@
         Token to token identifier
 
         >>> from microtc.textmodel import TextModel
         >>> corpus = ['buenos dias', 'catedras de conacyt', 'categorizacion de texto ingeotec']
         >>> textmodel = TextModel().fit(corpus)
         >>> _ = textmodel.transform(corpus)
         >>> textmodel.token2id['de']
-        0
+        4
         """
         return self.model.word2id
```

### Comparing `microtc-2.4.8/microtc/tools/microtc-ensemble` & `microtc-2.4.9/microtc/tools/microtc-ensemble`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/tools/microtc-kfolds` & `microtc-2.4.9/microtc/tools/microtc-kfolds`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/tools/microtc-params` & `microtc-2.4.9/microtc/tools/microtc-params`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/tools/microtc-perf` & `microtc-2.4.9/microtc/tools/microtc-perf`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/tools/microtc-predict` & `microtc-2.4.9/microtc/tools/microtc-predict`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/tools/microtc-retrain` & `microtc-2.4.9/microtc/tools/microtc-retrain`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/tools/microtc-textModel` & `microtc-2.4.9/microtc/tools/microtc-textModel`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/tools/microtc-train` & `microtc-2.4.9/microtc/tools/microtc-train`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/utils.py` & `microtc-2.4.9/microtc/utils.py`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc/weighting.py` & `microtc-2.4.9/microtc/weighting.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,17 @@
                         token_max_filter=self.token_max_filter)
         self.word2id, self.wordWeight = self.counter2weight(counter)
         return self
 
     def counter2weight(self, counter):
         weight = dict()
         w2id = dict()
-        for i, (k, v) in enumerate(counter.most_common()):
+        keys = sorted(counter.keys())
+        for i, k in enumerate(keys):
+            v = counter[k]
             weight[i] = v
             w2id[k] = i
         return w2id, weight
 
     @property
     def N(self):
         return self._ndocs
```

### Comparing `microtc-2.4.8/microtc/wrappers.py` & `microtc-2.4.9/microtc/wrappers.py`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/microtc.egg-info/PKG-INFO` & `microtc-2.4.9/microtc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microtc
-Version: 2.4.8
+Version: 2.4.9
 Summary: A generic minimal text classifier
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS :: MacOS X
```

### Comparing `microtc-2.4.8/microtc.egg-info/SOURCES.txt` & `microtc-2.4.9/microtc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microtc-2.4.8/setup.py` & `microtc-2.4.9/setup.py`

 * *Files identical despite different names*

