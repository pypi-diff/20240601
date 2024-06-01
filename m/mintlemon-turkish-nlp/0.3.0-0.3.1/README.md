# Comparing `tmp/mintlemon-turkish-nlp-0.3.0.tar.gz` & `tmp/mintlemon-turkish-nlp-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mintlemon-turkish-nlp-0.3.0.tar", last modified: Sat Jun  1 16:35:06 2024, max compression
+gzip compressed data, was "mintlemon-turkish-nlp-0.3.1.tar", last modified: Sat Jun  1 16:46:46 2024, max compression
```

## Comparing `mintlemon-turkish-nlp-0.3.0.tar` & `mintlemon-turkish-nlp-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,29 @@
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:35:06.348900 mintlemon-turkish-nlp-0.3.0/
--rw-r--r--   0 koc        (501) staff       (20)      784 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/AUTHORS.rst
--rw-r--r--   0 koc        (501) staff       (20)    11357 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/LICENSE
--rw-r--r--   0 koc        (501) staff       (20)       75 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/MANIFEST.in
--rw-r--r--   0 koc        (501) staff       (20)     3823 2024-06-01 16:35:06.348460 mintlemon-turkish-nlp-0.3.0/PKG-INFO
--rw-r--r--   0 koc        (501) staff       (20)     1772 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/README.md
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:35:06.337212 mintlemon-turkish-nlp-0.3.0/mintlemon/
--rw-r--r--   0 koc        (501) staff       (20)      275 2024-06-01 16:26:04.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/__init__.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:35:06.340141 mintlemon-turkish-nlp-0.3.0/mintlemon/data/
--rw-r--r--   0 koc        (501) staff       (20)     1565 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/data/TR_non_breaking_prefixes.txt
--rw-r--r--   0 koc        (501) staff       (20)   159044 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/data/ascii_to_str_dict.pickle
--rw-r--r--   0 koc        (501) staff       (20)     4260 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/data/stop_words.txt
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:35:06.342774 mintlemon-turkish-nlp-0.3.0/mintlemon/normalizer/
--rw-r--r--   0 koc        (501) staff       (20)      138 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/normalizer/__init__.py
--rw-r--r--   0 koc        (501) staff       (20)    15189 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/normalizer/_builtin.py
--rw-r--r--   0 koc        (501) staff       (20)    12341 2024-06-01 16:26:04.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/normalizer/normalizer.py
--rw-r--r--   0 koc        (501) staff       (20)     3025 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/normalizer/text_to_root_dtm.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:35:06.343648 mintlemon-turkish-nlp-0.3.0/mintlemon/sentence_splitter/
--rw-r--r--   0 koc        (501) staff       (20)       80 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/sentence_splitter/__init__.py
--rw-r--r--   0 koc        (501) staff       (20)     1592 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/sentence_splitter/sentence_splitter.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:35:06.344680 mintlemon-turkish-nlp-0.3.0/mintlemon/turkish_spellcheck/
--rw-r--r--   0 koc        (501) staff       (20)       88 2024-06-01 16:26:04.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/turkish_spellcheck/__init__.py
--rw-r--r--   0 koc        (501) staff       (20)     4263 2024-06-01 16:26:04.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/turkish_spellcheck/turkish_spellchecker.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:35:06.347127 mintlemon-turkish-nlp-0.3.0/mintlemon_turkish_nlp.egg-info/
--rw-r--r--   0 koc        (501) staff       (20)     3823 2024-06-01 16:35:06.000000 mintlemon-turkish-nlp-0.3.0/mintlemon_turkish_nlp.egg-info/PKG-INFO
--rw-r--r--   0 koc        (501) staff       (20)      750 2024-06-01 16:35:06.000000 mintlemon-turkish-nlp-0.3.0/mintlemon_turkish_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 koc        (501) staff       (20)        1 2024-06-01 16:35:06.000000 mintlemon-turkish-nlp-0.3.0/mintlemon_turkish_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 koc        (501) staff       (20)      133 2024-06-01 16:35:06.000000 mintlemon-turkish-nlp-0.3.0/mintlemon_turkish_nlp.egg-info/requires.txt
--rw-r--r--   0 koc        (501) staff       (20)       10 2024-06-01 16:35:06.000000 mintlemon-turkish-nlp-0.3.0/mintlemon_turkish_nlp.egg-info/top_level.txt
--rw-r--r--   0 koc        (501) staff       (20)     1087 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/pyproject.toml
--rw-r--r--   0 koc        (501) staff       (20)       38 2024-06-01 16:35:06.349012 mintlemon-turkish-nlp-0.3.0/setup.cfg
--rw-r--r--   0 koc        (501) staff       (20)     2272 2024-06-01 16:33:52.000000 mintlemon-turkish-nlp-0.3.0/setup.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:46:46.105255 mintlemon-turkish-nlp-0.3.1/
+-rw-r--r--   0 koc        (501) staff       (20)      784 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.1/AUTHORS.rst
+-rw-r--r--   0 koc        (501) staff       (20)    11357 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.1/LICENSE
+-rw-r--r--   0 koc        (501) staff       (20)       75 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.1/MANIFEST.in
+-rw-r--r--   0 koc        (501) staff       (20)     3823 2024-06-01 16:46:46.104860 mintlemon-turkish-nlp-0.3.1/PKG-INFO
+-rw-r--r--   0 koc        (501) staff       (20)     1772 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.1/README.md
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:46:46.095433 mintlemon-turkish-nlp-0.3.1/mintlemon/
+-rw-r--r--   0 koc        (501) staff       (20)      252 2024-06-01 16:44:35.000000 mintlemon-turkish-nlp-0.3.1/mintlemon/__init__.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:46:46.098125 mintlemon-turkish-nlp-0.3.1/mintlemon/data/
+-rw-r--r--   0 koc        (501) staff       (20)     1565 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.1/mintlemon/data/TR_non_breaking_prefixes.txt
+-rw-r--r--   0 koc        (501) staff       (20)   159044 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.1/mintlemon/data/ascii_to_str_dict.pickle
+-rw-r--r--   0 koc        (501) staff       (20)     4260 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.1/mintlemon/data/stop_words.txt
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:46:46.100071 mintlemon-turkish-nlp-0.3.1/mintlemon/normalizer/
+-rw-r--r--   0 koc        (501) staff       (20)      138 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.1/mintlemon/normalizer/__init__.py
+-rw-r--r--   0 koc        (501) staff       (20)    15189 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.1/mintlemon/normalizer/_builtin.py
+-rw-r--r--   0 koc        (501) staff       (20)    12341 2024-06-01 16:26:04.000000 mintlemon-turkish-nlp-0.3.1/mintlemon/normalizer/normalizer.py
+-rw-r--r--   0 koc        (501) staff       (20)     3025 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.1/mintlemon/normalizer/text_to_root_dtm.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:46:46.100945 mintlemon-turkish-nlp-0.3.1/mintlemon/sentence_splitter/
+-rw-r--r--   0 koc        (501) staff       (20)       80 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.1/mintlemon/sentence_splitter/__init__.py
+-rw-r--r--   0 koc        (501) staff       (20)     1592 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.1/mintlemon/sentence_splitter/sentence_splitter.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:46:46.103435 mintlemon-turkish-nlp-0.3.1/mintlemon_turkish_nlp.egg-info/
+-rw-r--r--   0 koc        (501) staff       (20)     3823 2024-06-01 16:46:45.000000 mintlemon-turkish-nlp-0.3.1/mintlemon_turkish_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 koc        (501) staff       (20)      656 2024-06-01 16:46:46.000000 mintlemon-turkish-nlp-0.3.1/mintlemon_turkish_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 koc        (501) staff       (20)        1 2024-06-01 16:46:45.000000 mintlemon-turkish-nlp-0.3.1/mintlemon_turkish_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 koc        (501) staff       (20)      133 2024-06-01 16:46:45.000000 mintlemon-turkish-nlp-0.3.1/mintlemon_turkish_nlp.egg-info/requires.txt
+-rw-r--r--   0 koc        (501) staff       (20)       10 2024-06-01 16:46:45.000000 mintlemon-turkish-nlp-0.3.1/mintlemon_turkish_nlp.egg-info/top_level.txt
+-rw-r--r--   0 koc        (501) staff       (20)     1087 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.1/pyproject.toml
+-rw-r--r--   0 koc        (501) staff       (20)       38 2024-06-01 16:46:46.105333 mintlemon-turkish-nlp-0.3.1/setup.cfg
+-rw-r--r--   0 koc        (501) staff       (20)     2272 2024-06-01 16:44:48.000000 mintlemon-turkish-nlp-0.3.1/setup.py
```

### Comparing `mintlemon-turkish-nlp-0.3.0/AUTHORS.rst` & `mintlemon-turkish-nlp-0.3.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.3.0/LICENSE` & `mintlemon-turkish-nlp-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.3.0/PKG-INFO` & `mintlemon-turkish-nlp-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mintlemon-turkish-nlp
-Version: 0.3.0
+Version: 0.3.1
 Summary: Mint & Lemon Turkish NLP Library developed by Mint & Lemon Development Team.
 Home-page: https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp
 Author: Mint&Lemon
 License: Apache License, Version 2.0
 Project-URL: Tracker, https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp/issues
 Project-URL: Documentation, https://mintlemon-turkish-nlp.readthedocs.io
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `mintlemon-turkish-nlp-0.3.0/README.md` & `mintlemon-turkish-nlp-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.3.0/mintlemon/data/TR_non_breaking_prefixes.txt` & `mintlemon-turkish-nlp-0.3.1/mintlemon/data/TR_non_breaking_prefixes.txt`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.3.0/mintlemon/data/ascii_to_str_dict.pickle` & `mintlemon-turkish-nlp-0.3.1/mintlemon/data/ascii_to_str_dict.pickle`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.3.0/mintlemon/data/stop_words.txt` & `mintlemon-turkish-nlp-0.3.1/mintlemon/data/stop_words.txt`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.3.0/mintlemon/normalizer/_builtin.py` & `mintlemon-turkish-nlp-0.3.1/mintlemon/normalizer/_builtin.py`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.3.0/mintlemon/normalizer/normalizer.py` & `mintlemon-turkish-nlp-0.3.1/mintlemon/normalizer/normalizer.py`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.3.0/mintlemon/normalizer/text_to_root_dtm.py` & `mintlemon-turkish-nlp-0.3.1/mintlemon/normalizer/text_to_root_dtm.py`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.3.0/mintlemon/sentence_splitter/sentence_splitter.py` & `mintlemon-turkish-nlp-0.3.1/mintlemon/sentence_splitter/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.3.0/mintlemon_turkish_nlp.egg-info/PKG-INFO` & `mintlemon-turkish-nlp-0.3.1/mintlemon_turkish_nlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mintlemon-turkish-nlp
-Version: 0.3.0
+Version: 0.3.1
 Summary: Mint & Lemon Turkish NLP Library developed by Mint & Lemon Development Team.
 Home-page: https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp
 Author: Mint&Lemon
 License: Apache License, Version 2.0
 Project-URL: Tracker, https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp/issues
 Project-URL: Documentation, https://mintlemon-turkish-nlp.readthedocs.io
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `mintlemon-turkish-nlp-0.3.0/mintlemon_turkish_nlp.egg-info/SOURCES.txt` & `mintlemon-turkish-nlp-0.3.1/mintlemon_turkish_nlp.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -10,14 +10,12 @@
 mintlemon/data/stop_words.txt
 mintlemon/normalizer/__init__.py
 mintlemon/normalizer/_builtin.py
 mintlemon/normalizer/normalizer.py
 mintlemon/normalizer/text_to_root_dtm.py
 mintlemon/sentence_splitter/__init__.py
 mintlemon/sentence_splitter/sentence_splitter.py
-mintlemon/turkish_spellcheck/__init__.py
-mintlemon/turkish_spellcheck/turkish_spellchecker.py
 mintlemon_turkish_nlp.egg-info/PKG-INFO
 mintlemon_turkish_nlp.egg-info/SOURCES.txt
 mintlemon_turkish_nlp.egg-info/dependency_links.txt
 mintlemon_turkish_nlp.egg-info/requires.txt
 mintlemon_turkish_nlp.egg-info/top_level.txt
```

### Comparing `mintlemon-turkish-nlp-0.3.0/pyproject.toml` & `mintlemon-turkish-nlp-0.3.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.3.0/setup.py` & `mintlemon-turkish-nlp-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def get_long_description():
     with open("README.md", "r", encoding="utf-8") as f:
         return f.read()
 
 setup(
     name="mintlemon-turkish-nlp",
-    version = "0.3.0",
+    version = "0.3.1",
     description="Mint & Lemon Turkish NLP Library developed by Mint & Lemon Development Team.",
     author="Mint&Lemon",
     license="Apache License, Version 2.0",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp",
     project_urls={
```

