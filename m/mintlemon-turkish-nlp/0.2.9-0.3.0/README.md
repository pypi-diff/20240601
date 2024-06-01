# Comparing `tmp/mintlemon-turkish-nlp-0.2.9.tar.gz` & `tmp/mintlemon-turkish-nlp-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mintlemon-turkish-nlp-0.2.9.tar", last modified: Sat May 18 17:31:21 2024, max compression
+gzip compressed data, was "mintlemon-turkish-nlp-0.3.0.tar", last modified: Sat Jun  1 16:35:06 2024, max compression
```

## Comparing `mintlemon-turkish-nlp-0.2.9.tar` & `mintlemon-turkish-nlp-0.3.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:31:21.367021 mintlemon-turkish-nlp-0.2.9/
--rw-r--r--   0 koc        (501) staff       (20)      784 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.9/AUTHORS.rst
--rw-r--r--   0 koc        (501) staff       (20)    11357 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.9/LICENSE
--rw-r--r--   0 koc        (501) staff       (20)       75 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.9/MANIFEST.in
--rw-r--r--   0 koc        (501) staff       (20)     3887 2024-05-18 17:31:21.366505 mintlemon-turkish-nlp-0.2.9/PKG-INFO
--rw-r--r--   0 koc        (501) staff       (20)     1772 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.9/README.md
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:31:21.355809 mintlemon-turkish-nlp-0.2.9/mintlemon/
--rw-r--r--   0 koc        (501) staff       (20)      275 2024-02-19 23:15:49.000000 mintlemon-turkish-nlp-0.2.9/mintlemon/__init__.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:31:21.358619 mintlemon-turkish-nlp-0.2.9/mintlemon/data/
--rw-r--r--   0 koc        (501) staff       (20)     1565 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.9/mintlemon/data/TR_non_breaking_prefixes.txt
--rw-r--r--   0 koc        (501) staff       (20)   159044 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.9/mintlemon/data/ascii_to_str_dict.pickle
--rw-r--r--   0 koc        (501) staff       (20)     4260 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.9/mintlemon/data/stop_words.txt
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:31:21.360701 mintlemon-turkish-nlp-0.2.9/mintlemon/normalizer/
--rw-r--r--   0 koc        (501) staff       (20)      138 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.9/mintlemon/normalizer/__init__.py
--rw-r--r--   0 koc        (501) staff       (20)    15189 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.9/mintlemon/normalizer/_builtin.py
--rw-r--r--   0 koc        (501) staff       (20)    12341 2024-02-16 12:50:56.000000 mintlemon-turkish-nlp-0.2.9/mintlemon/normalizer/normalizer.py
--rw-r--r--   0 koc        (501) staff       (20)     3025 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.9/mintlemon/normalizer/text_to_root_dtm.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:31:21.361570 mintlemon-turkish-nlp-0.2.9/mintlemon/sentence_splitter/
--rw-r--r--   0 koc        (501) staff       (20)       80 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.9/mintlemon/sentence_splitter/__init__.py
--rw-r--r--   0 koc        (501) staff       (20)     1592 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.9/mintlemon/sentence_splitter/sentence_splitter.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:31:21.362331 mintlemon-turkish-nlp-0.2.9/mintlemon/turkish_spellcheck/
--rw-r--r--   0 koc        (501) staff       (20)       88 2024-02-19 23:14:58.000000 mintlemon-turkish-nlp-0.2.9/mintlemon/turkish_spellcheck/__init__.py
--rw-r--r--   0 koc        (501) staff       (20)     4263 2024-02-20 16:36:02.000000 mintlemon-turkish-nlp-0.2.9/mintlemon/turkish_spellcheck/turkish_spellchecker.py
-drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-05-18 17:31:21.365010 mintlemon-turkish-nlp-0.2.9/mintlemon_turkish_nlp.egg-info/
--rw-r--r--   0 koc        (501) staff       (20)     3887 2024-05-18 17:31:21.000000 mintlemon-turkish-nlp-0.2.9/mintlemon_turkish_nlp.egg-info/PKG-INFO
--rw-r--r--   0 koc        (501) staff       (20)      750 2024-05-18 17:31:21.000000 mintlemon-turkish-nlp-0.2.9/mintlemon_turkish_nlp.egg-info/SOURCES.txt
--rw-r--r--   0 koc        (501) staff       (20)        1 2024-05-18 17:31:21.000000 mintlemon-turkish-nlp-0.2.9/mintlemon_turkish_nlp.egg-info/dependency_links.txt
--rw-r--r--   0 koc        (501) staff       (20)      167 2024-05-18 17:31:21.000000 mintlemon-turkish-nlp-0.2.9/mintlemon_turkish_nlp.egg-info/requires.txt
--rw-r--r--   0 koc        (501) staff       (20)       10 2024-05-18 17:31:21.000000 mintlemon-turkish-nlp-0.2.9/mintlemon_turkish_nlp.egg-info/top_level.txt
--rw-r--r--   0 koc        (501) staff       (20)     1087 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.2.9/pyproject.toml
--rw-r--r--   0 koc        (501) staff       (20)       38 2024-05-18 17:31:21.367124 mintlemon-turkish-nlp-0.2.9/setup.cfg
--rw-r--r--   0 koc        (501) staff       (20)     2328 2024-05-18 17:30:40.000000 mintlemon-turkish-nlp-0.2.9/setup.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:35:06.348900 mintlemon-turkish-nlp-0.3.0/
+-rw-r--r--   0 koc        (501) staff       (20)      784 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/AUTHORS.rst
+-rw-r--r--   0 koc        (501) staff       (20)    11357 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/LICENSE
+-rw-r--r--   0 koc        (501) staff       (20)       75 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/MANIFEST.in
+-rw-r--r--   0 koc        (501) staff       (20)     3823 2024-06-01 16:35:06.348460 mintlemon-turkish-nlp-0.3.0/PKG-INFO
+-rw-r--r--   0 koc        (501) staff       (20)     1772 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/README.md
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:35:06.337212 mintlemon-turkish-nlp-0.3.0/mintlemon/
+-rw-r--r--   0 koc        (501) staff       (20)      275 2024-06-01 16:26:04.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/__init__.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:35:06.340141 mintlemon-turkish-nlp-0.3.0/mintlemon/data/
+-rw-r--r--   0 koc        (501) staff       (20)     1565 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/data/TR_non_breaking_prefixes.txt
+-rw-r--r--   0 koc        (501) staff       (20)   159044 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/data/ascii_to_str_dict.pickle
+-rw-r--r--   0 koc        (501) staff       (20)     4260 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/data/stop_words.txt
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:35:06.342774 mintlemon-turkish-nlp-0.3.0/mintlemon/normalizer/
+-rw-r--r--   0 koc        (501) staff       (20)      138 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/normalizer/__init__.py
+-rw-r--r--   0 koc        (501) staff       (20)    15189 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/normalizer/_builtin.py
+-rw-r--r--   0 koc        (501) staff       (20)    12341 2024-06-01 16:26:04.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/normalizer/normalizer.py
+-rw-r--r--   0 koc        (501) staff       (20)     3025 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/normalizer/text_to_root_dtm.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:35:06.343648 mintlemon-turkish-nlp-0.3.0/mintlemon/sentence_splitter/
+-rw-r--r--   0 koc        (501) staff       (20)       80 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/sentence_splitter/__init__.py
+-rw-r--r--   0 koc        (501) staff       (20)     1592 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/sentence_splitter/sentence_splitter.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:35:06.344680 mintlemon-turkish-nlp-0.3.0/mintlemon/turkish_spellcheck/
+-rw-r--r--   0 koc        (501) staff       (20)       88 2024-06-01 16:26:04.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/turkish_spellcheck/__init__.py
+-rw-r--r--   0 koc        (501) staff       (20)     4263 2024-06-01 16:26:04.000000 mintlemon-turkish-nlp-0.3.0/mintlemon/turkish_spellcheck/turkish_spellchecker.py
+drwxr-xr-x   0 koc        (501) staff       (20)        0 2024-06-01 16:35:06.347127 mintlemon-turkish-nlp-0.3.0/mintlemon_turkish_nlp.egg-info/
+-rw-r--r--   0 koc        (501) staff       (20)     3823 2024-06-01 16:35:06.000000 mintlemon-turkish-nlp-0.3.0/mintlemon_turkish_nlp.egg-info/PKG-INFO
+-rw-r--r--   0 koc        (501) staff       (20)      750 2024-06-01 16:35:06.000000 mintlemon-turkish-nlp-0.3.0/mintlemon_turkish_nlp.egg-info/SOURCES.txt
+-rw-r--r--   0 koc        (501) staff       (20)        1 2024-06-01 16:35:06.000000 mintlemon-turkish-nlp-0.3.0/mintlemon_turkish_nlp.egg-info/dependency_links.txt
+-rw-r--r--   0 koc        (501) staff       (20)      133 2024-06-01 16:35:06.000000 mintlemon-turkish-nlp-0.3.0/mintlemon_turkish_nlp.egg-info/requires.txt
+-rw-r--r--   0 koc        (501) staff       (20)       10 2024-06-01 16:35:06.000000 mintlemon-turkish-nlp-0.3.0/mintlemon_turkish_nlp.egg-info/top_level.txt
+-rw-r--r--   0 koc        (501) staff       (20)     1087 2024-02-16 12:29:01.000000 mintlemon-turkish-nlp-0.3.0/pyproject.toml
+-rw-r--r--   0 koc        (501) staff       (20)       38 2024-06-01 16:35:06.349012 mintlemon-turkish-nlp-0.3.0/setup.cfg
+-rw-r--r--   0 koc        (501) staff       (20)     2272 2024-06-01 16:33:52.000000 mintlemon-turkish-nlp-0.3.0/setup.py
```

### Comparing `mintlemon-turkish-nlp-0.2.9/AUTHORS.rst` & `mintlemon-turkish-nlp-0.3.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.9/LICENSE` & `mintlemon-turkish-nlp-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.9/PKG-INFO` & `mintlemon-turkish-nlp-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mintlemon-turkish-nlp
-Version: 0.2.9
+Version: 0.3.0
 Summary: Mint & Lemon Turkish NLP Library developed by Mint & Lemon Development Team.
 Home-page: https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp
 Author: Mint&Lemon
 License: Apache License, Version 2.0
 Project-URL: Tracker, https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp/issues
 Project-URL: Documentation, https://mintlemon-turkish-nlp.readthedocs.io
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -28,16 +28,14 @@
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: hunspell==0.5.5
-Requires-Dist: cyhunspell==2.0.2
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: regex>=2021.4.4
 Requires-Dist: zeyrek>=0.1.3
 Requires-Dist: nltk>=3.8.1
 Requires-Dist: pandas>=1.3.4
 Requires-Dist: scikit-learn>=1.2.0
 Provides-Extra: dev
```

### Comparing `mintlemon-turkish-nlp-0.2.9/README.md` & `mintlemon-turkish-nlp-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.9/mintlemon/data/TR_non_breaking_prefixes.txt` & `mintlemon-turkish-nlp-0.3.0/mintlemon/data/TR_non_breaking_prefixes.txt`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.9/mintlemon/data/ascii_to_str_dict.pickle` & `mintlemon-turkish-nlp-0.3.0/mintlemon/data/ascii_to_str_dict.pickle`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.9/mintlemon/data/stop_words.txt` & `mintlemon-turkish-nlp-0.3.0/mintlemon/data/stop_words.txt`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.9/mintlemon/normalizer/_builtin.py` & `mintlemon-turkish-nlp-0.3.0/mintlemon/normalizer/_builtin.py`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.9/mintlemon/normalizer/normalizer.py` & `mintlemon-turkish-nlp-0.3.0/mintlemon/normalizer/normalizer.py`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.9/mintlemon/normalizer/text_to_root_dtm.py` & `mintlemon-turkish-nlp-0.3.0/mintlemon/normalizer/text_to_root_dtm.py`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.9/mintlemon/sentence_splitter/sentence_splitter.py` & `mintlemon-turkish-nlp-0.3.0/mintlemon/sentence_splitter/sentence_splitter.py`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.9/mintlemon/turkish_spellcheck/turkish_spellchecker.py` & `mintlemon-turkish-nlp-0.3.0/mintlemon/turkish_spellcheck/turkish_spellchecker.py`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.9/mintlemon_turkish_nlp.egg-info/PKG-INFO` & `mintlemon-turkish-nlp-0.3.0/mintlemon_turkish_nlp.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mintlemon-turkish-nlp
-Version: 0.2.9
+Version: 0.3.0
 Summary: Mint & Lemon Turkish NLP Library developed by Mint & Lemon Development Team.
 Home-page: https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp
 Author: Mint&Lemon
 License: Apache License, Version 2.0
 Project-URL: Tracker, https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp/issues
 Project-URL: Documentation, https://mintlemon-turkish-nlp.readthedocs.io
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -28,16 +28,14 @@
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: AUTHORS.rst
-Requires-Dist: hunspell==0.5.5
-Requires-Dist: cyhunspell==2.0.2
 Requires-Dist: numpy>=1.20.0
 Requires-Dist: regex>=2021.4.4
 Requires-Dist: zeyrek>=0.1.3
 Requires-Dist: nltk>=3.8.1
 Requires-Dist: pandas>=1.3.4
 Requires-Dist: scikit-learn>=1.2.0
 Provides-Extra: dev
```

### Comparing `mintlemon-turkish-nlp-0.2.9/mintlemon_turkish_nlp.egg-info/SOURCES.txt` & `mintlemon-turkish-nlp-0.3.0/mintlemon_turkish_nlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.9/pyproject.toml` & `mintlemon-turkish-nlp-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mintlemon-turkish-nlp-0.2.9/setup.py` & `mintlemon-turkish-nlp-0.3.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 def get_long_description():
     with open("README.md", "r", encoding="utf-8") as f:
         return f.read()
 
 setup(
     name="mintlemon-turkish-nlp",
-    version = "0.2.9",
+    version = "0.3.0",
     description="Mint & Lemon Turkish NLP Library developed by Mint & Lemon Development Team.",
     author="Mint&Lemon",
     license="Apache License, Version 2.0",
     long_description=get_long_description(),
     long_description_content_type="text/markdown",
     url="https://github.com/Teknofest-Nane-Limon/mintlemon-turkish-nlp",
     project_urls={
@@ -41,16 +41,14 @@
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.7",
     packages=find_packages(),
     package_data={"mintlemon": ["data/*"]},
     include_package_data=True,
     install_requires=[
-        "hunspell==0.5.5",
-        "cyhunspell==2.0.2",
         "numpy>=1.20.0",    
         "regex>=2021.4.4",    
         "zeyrek>=0.1.3",    
         "nltk>=3.8.1",    
         "pandas>=1.3.4",    
         "scikit-learn>=1.2.0",
     ],
```

