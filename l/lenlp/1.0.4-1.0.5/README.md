# Comparing `tmp/lenlp-1.0.4.tar.gz` & `tmp/lenlp-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenlp-1.0.4.tar", last modified: Fri May 31 13:13:56 2024, max compression
+gzip compressed data, was "lenlp-1.0.5.tar", last modified: Sat Jun  1 13:55:02 2024, max compression
```

## Comparing `lenlp-1.0.4.tar` & `lenlp-1.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-05-31 13:13:56.185446 lenlp-1.0.4/
--rw-rw-rw-   0        0        0      538 2024-05-31 13:13:16.000000 lenlp-1.0.4/Cargo.toml
--rw-rw-rw-   0        0        0       47 2024-05-31 13:13:16.000000 lenlp-1.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     7643 2024-05-31 13:13:56.185446 lenlp-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     7181 2024-05-31 13:13:16.000000 lenlp-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-31 13:13:56.185446 lenlp-1.0.4/lenlp/
--rw-rw-rw-   0        0        0       97 2024-05-31 13:13:16.000000 lenlp-1.0.4/lenlp/__init__.py
--rw-rw-rw-   0        0        0       66 2024-05-31 13:13:16.000000 lenlp-1.0.4/lenlp/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:13:56.185446 lenlp-1.0.4/lenlp/analyzer/
--rw-rw-rw-   0        0        0       64 2024-05-31 13:13:16.000000 lenlp-1.0.4/lenlp/analyzer/__init__.py
--rw-rw-rw-   0        0        0     1973 2024-05-31 13:13:16.000000 lenlp-1.0.4/lenlp/analyzer/analyze.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:13:56.185446 lenlp-1.0.4/lenlp/counter/
--rw-rw-rw-   0        0        0       49 2024-05-31 13:13:16.000000 lenlp-1.0.4/lenlp/counter/__init__.py
--rw-rw-rw-   0        0        0     3999 2024-05-31 13:13:16.000000 lenlp-1.0.4/lenlp/counter/count.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:13:56.185446 lenlp-1.0.4/lenlp/flash/
--rw-rw-rw-   0        0        0       62 2024-05-31 13:13:16.000000 lenlp-1.0.4/lenlp/flash/__init__.py
--rw-rw-rw-   0        0        0     1449 2024-05-31 13:13:16.000000 lenlp-1.0.4/lenlp/flash/flash_text.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:13:56.185446 lenlp-1.0.4/lenlp/normalizer/
--rw-rw-rw-   0        0        0       61 2024-05-31 13:13:16.000000 lenlp-1.0.4/lenlp/normalizer/__init__.py
--rw-rw-rw-   0        0        0      513 2024-05-31 13:13:16.000000 lenlp-1.0.4/lenlp/normalizer/normalize.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:13:56.185446 lenlp-1.0.4/lenlp/sparse/
--rw-rw-rw-   0        0        0      209 2024-05-31 13:13:16.000000 lenlp-1.0.4/lenlp/sparse/__init__.py
--rw-rw-rw-   0        0        0     3866 2024-05-31 13:13:16.000000 lenlp-1.0.4/lenlp/sparse/bm25_vectorizer.py
--rw-rw-rw-   0        0        0     3694 2024-05-31 13:13:16.000000 lenlp-1.0.4/lenlp/sparse/count_vectorizer.py
--rw-rw-rw-   0        0        0     3988 2024-05-31 13:13:16.000000 lenlp-1.0.4/lenlp/sparse/tfidf_vectorizer.py
-drwxrwxrwx   0        0        0        0 2024-05-31 13:13:56.185446 lenlp-1.0.4/lenlp.egg-info/
--rw-rw-rw-   0        0        0     7643 2024-05-31 13:13:56.000000 lenlp-1.0.4/lenlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      558 2024-05-31 13:13:56.000000 lenlp-1.0.4/lenlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-31 13:13:56.000000 lenlp-1.0.4/lenlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      135 2024-05-31 13:13:56.000000 lenlp-1.0.4/lenlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-31 13:13:56.000000 lenlp-1.0.4/lenlp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-31 13:13:56.185446 lenlp-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1197 2024-05-31 13:13:16.000000 lenlp-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:55:02.897760 lenlp-1.0.5/
+-rw-rw-rw-   0        0        0      538 2024-06-01 13:54:28.000000 lenlp-1.0.5/Cargo.toml
+-rw-rw-rw-   0        0        0       47 2024-06-01 13:54:28.000000 lenlp-1.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     7643 2024-06-01 13:55:02.897760 lenlp-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7181 2024-06-01 13:54:28.000000 lenlp-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2024-06-01 13:55:02.888508 lenlp-1.0.5/lenlp/
+-rw-rw-rw-   0        0        0       97 2024-06-01 13:54:28.000000 lenlp-1.0.5/lenlp/__init__.py
+-rw-rw-rw-   0        0        0       66 2024-06-01 13:54:28.000000 lenlp-1.0.5/lenlp/__version__.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:55:02.892304 lenlp-1.0.5/lenlp/analyzer/
+-rw-rw-rw-   0        0        0       64 2024-06-01 13:54:28.000000 lenlp-1.0.5/lenlp/analyzer/__init__.py
+-rw-rw-rw-   0        0        0     1973 2024-06-01 13:54:28.000000 lenlp-1.0.5/lenlp/analyzer/analyze.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:55:02.893385 lenlp-1.0.5/lenlp/counter/
+-rw-rw-rw-   0        0        0       49 2024-06-01 13:54:28.000000 lenlp-1.0.5/lenlp/counter/__init__.py
+-rw-rw-rw-   0        0        0     3999 2024-06-01 13:54:28.000000 lenlp-1.0.5/lenlp/counter/count.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:55:02.893903 lenlp-1.0.5/lenlp/flash/
+-rw-rw-rw-   0        0        0       62 2024-06-01 13:54:28.000000 lenlp-1.0.5/lenlp/flash/__init__.py
+-rw-rw-rw-   0        0        0     1449 2024-06-01 13:54:28.000000 lenlp-1.0.5/lenlp/flash/flash_text.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:55:02.893903 lenlp-1.0.5/lenlp/normalizer/
+-rw-rw-rw-   0        0        0       61 2024-06-01 13:54:28.000000 lenlp-1.0.5/lenlp/normalizer/__init__.py
+-rw-rw-rw-   0        0        0      513 2024-06-01 13:54:28.000000 lenlp-1.0.5/lenlp/normalizer/normalize.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:55:02.897188 lenlp-1.0.5/lenlp/sparse/
+-rw-rw-rw-   0        0        0      209 2024-06-01 13:54:28.000000 lenlp-1.0.5/lenlp/sparse/__init__.py
+-rw-rw-rw-   0        0        0     3866 2024-06-01 13:54:28.000000 lenlp-1.0.5/lenlp/sparse/bm25_vectorizer.py
+-rw-rw-rw-   0        0        0     3694 2024-06-01 13:54:28.000000 lenlp-1.0.5/lenlp/sparse/count_vectorizer.py
+-rw-rw-rw-   0        0        0     3988 2024-06-01 13:54:28.000000 lenlp-1.0.5/lenlp/sparse/tfidf_vectorizer.py
+drwxrwxrwx   0        0        0        0 2024-06-01 13:55:02.891702 lenlp-1.0.5/lenlp.egg-info/
+-rw-rw-rw-   0        0        0     7643 2024-06-01 13:55:02.000000 lenlp-1.0.5/lenlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      558 2024-06-01 13:55:02.000000 lenlp-1.0.5/lenlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-06-01 13:55:02.000000 lenlp-1.0.5/lenlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2024-06-01 13:55:02.000000 lenlp-1.0.5/lenlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-06-01 13:55:02.000000 lenlp-1.0.5/lenlp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-06-01 13:55:02.897760 lenlp-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1197 2024-06-01 13:54:28.000000 lenlp-1.0.5/setup.py
```

### Comparing `lenlp-1.0.4/Cargo.toml` & `lenlp-1.0.5/Cargo.toml`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.4/PKG-INFO` & `lenlp-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lenlp
-Version: 1.0.4
+Version: 1.0.5
 Home-page: https://github.com/raphaelsty/lenlp
 Download-URL: https://github.com/raphaelsty/lenlp/archive/v_01.tar.gz
 Author: Raphael Sourty
 Author-email: raphael.sourty@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lenlp Version: 1.0.4 Home-page: https://github.com/
+Metadata-Version: 2.1 Name: lenlp Version: 1.0.5 Home-page: https://github.com/
 raphaelsty/lenlp Download-URL: https://github.com/raphaelsty/lenlp/archive/
 v_01.tar.gz Author: Raphael Sourty Author-email: raphael.sourty@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Rust Classifier: Operating System :: OS Independent Requires-
 Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: dev
                               ************ LLeeNNLLPP ************
            Natural Language Processing toolbox for Python with Rust
```

### Comparing `lenlp-1.0.4/README.md` & `lenlp-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.4/lenlp/analyzer/analyze.py` & `lenlp-1.0.5/lenlp/analyzer/analyze.py`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.4/lenlp/counter/count.py` & `lenlp-1.0.5/lenlp/counter/count.py`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.4/lenlp/flash/flash_text.py` & `lenlp-1.0.5/lenlp/flash/flash_text.py`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.4/lenlp/normalizer/normalize.py` & `lenlp-1.0.5/lenlp/normalizer/normalize.py`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.4/lenlp/sparse/bm25_vectorizer.py` & `lenlp-1.0.5/lenlp/sparse/bm25_vectorizer.py`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.4/lenlp/sparse/count_vectorizer.py` & `lenlp-1.0.5/lenlp/sparse/count_vectorizer.py`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.4/lenlp/sparse/tfidf_vectorizer.py` & `lenlp-1.0.5/lenlp/sparse/tfidf_vectorizer.py`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.4/lenlp.egg-info/PKG-INFO` & `lenlp-1.0.5/lenlp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lenlp
-Version: 1.0.4
+Version: 1.0.5
 Home-page: https://github.com/raphaelsty/lenlp
 Download-URL: https://github.com/raphaelsty/lenlp/archive/v_01.tar.gz
 Author: Raphael Sourty
 Author-email: raphael.sourty@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Rust
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: lenlp Version: 1.0.4 Home-page: https://github.com/
+Metadata-Version: 2.1 Name: lenlp Version: 1.0.5 Home-page: https://github.com/
 raphaelsty/lenlp Download-URL: https://github.com/raphaelsty/lenlp/archive/
 v_01.tar.gz Author: Raphael Sourty Author-email: raphael.sourty@gmail.com
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Rust Classifier: Operating System :: OS Independent Requires-
 Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: dev
                               ************ LLeeNNLLPP ************
            Natural Language Processing toolbox for Python with Rust
```

### Comparing `lenlp-1.0.4/lenlp.egg-info/SOURCES.txt` & `lenlp-1.0.5/lenlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lenlp-1.0.4/setup.py` & `lenlp-1.0.5/setup.py`

 * *Files identical despite different names*

