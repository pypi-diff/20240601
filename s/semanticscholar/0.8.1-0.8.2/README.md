# Comparing `tmp/semanticscholar-0.8.1.tar.gz` & `tmp/semanticscholar-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semanticscholar-0.8.1.tar", last modified: Fri May 17 15:50:33 2024, max compression
+gzip compressed data, was "semanticscholar-0.8.2.tar", last modified: Sat Jun  1 03:17:34 2024, max compression
```

## Comparing `semanticscholar-0.8.1.tar` & `semanticscholar-0.8.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:50:33.806467 semanticscholar-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-17 15:50:33.806467 semanticscholar-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13417 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:50:33.806467 semanticscholar-0.8.1/semanticscholar/
--rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/ApiRequester.py
--rw-r--r--   0 runner    (1001) docker     (127)    25987 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/AsyncSemanticScholar.py
--rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/Author.py
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/BaseReference.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/Citation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/Journal.py
--rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/PaginatedResults.py
--rw-r--r--   0 runner    (1001) docker     (127)    10827 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/Paper.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/PublicationVenue.py
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/Reference.py
--rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/SemanticScholar.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/SemanticScholarException.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/SemanticScholarObject.py
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/Tldr.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/semanticscholar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:50:33.806467 semanticscholar-0.8.1/semanticscholar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-05-17 15:50:33.000000 semanticscholar-0.8.1/semanticscholar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-05-17 15:50:33.000000 semanticscholar-0.8.1/semanticscholar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:50:33.000000 semanticscholar-0.8.1/semanticscholar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 15:50:33.000000 semanticscholar-0.8.1/semanticscholar.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-17 15:50:33.000000 semanticscholar-0.8.1/semanticscholar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-17 15:50:33.000000 semanticscholar-0.8.1/semanticscholar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 15:50:33.806467 semanticscholar-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-05-17 15:50:25.000000 semanticscholar-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 15:50:33.806467 semanticscholar-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    40321 2024-05-17 15:50:26.000000 semanticscholar-0.8.1/tests/test_semanticscholar.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:34.278720 semanticscholar-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-06-01 03:17:34.278720 semanticscholar-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13417 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:34.278720 semanticscholar-0.8.2/semanticscholar/
+-rw-r--r--   0 runner    (1001) docker     (127)     5333 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/semanticscholar/ApiRequester.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25987 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/semanticscholar/AsyncSemanticScholar.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3685 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/semanticscholar/Author.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/semanticscholar/BaseReference.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/semanticscholar/Citation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/semanticscholar/Journal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5172 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/semanticscholar/PaginatedResults.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10799 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/semanticscholar/Paper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/semanticscholar/PublicationVenue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/semanticscholar/Reference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19436 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/semanticscholar/SemanticScholar.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/semanticscholar/SemanticScholarException.py
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/semanticscholar/SemanticScholarObject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/semanticscholar/Tldr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/semanticscholar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:34.278720 semanticscholar-0.8.2/semanticscholar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14431 2024-06-01 03:17:34.000000 semanticscholar-0.8.2/semanticscholar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-06-01 03:17:34.000000 semanticscholar-0.8.2/semanticscholar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 03:17:34.000000 semanticscholar-0.8.2/semanticscholar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 03:17:34.000000 semanticscholar-0.8.2/semanticscholar.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-06-01 03:17:34.000000 semanticscholar-0.8.2/semanticscholar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-06-01 03:17:34.000000 semanticscholar-0.8.2/semanticscholar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 03:17:34.278720 semanticscholar-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 03:17:34.278720 semanticscholar-0.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    40321 2024-06-01 03:17:25.000000 semanticscholar-0.8.2/tests/test_semanticscholar.py
```

### Comparing `semanticscholar-0.8.1/LICENSE` & `semanticscholar-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.1/PKG-INFO` & `semanticscholar-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semanticscholar
-Version: 0.8.1
+Version: 0.8.2
 Summary: Unofficial Python client library for Semantic Scholar APIs.
 Home-page: http://danielnsilva.com/semanticscholar
 Author: Daniel Silva
 Author-email: danielnsilva@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `semanticscholar-0.8.1/README.md` & `semanticscholar-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.1/semanticscholar/ApiRequester.py` & `semanticscholar-0.8.2/semanticscholar/ApiRequester.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,16 +70,17 @@
                 self,
                 url: str,
                 method: str,
                 headers: dict,
                 payload: dict = None
             ) -> str:
         curl_cmd = f'curl -X {method}'
-        for key, value in headers.items():
-            curl_cmd += f' -H \'{key}: {value}\''
+        if headers:
+            for key, value in headers.items():
+                curl_cmd += f' -H \'{key}: {value}\''
         curl_cmd += f' -d \'{json.dumps(payload)}\'' if payload else ''
         curl_cmd += f' {url}'
         return curl_cmd
 
     def _print_debug(self, url, headers, payload, method) -> None:
         print('-' * 80)
         print(f'Method: {method}\n')
```

### Comparing `semanticscholar-0.8.1/semanticscholar/AsyncSemanticScholar.py` & `semanticscholar-0.8.2/semanticscholar/AsyncSemanticScholar.py`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.1/semanticscholar/Author.py` & `semanticscholar-0.8.2/semanticscholar/Author.py`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.1/semanticscholar/BaseReference.py` & `semanticscholar-0.8.2/semanticscholar/BaseReference.py`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.1/semanticscholar/Journal.py` & `semanticscholar-0.8.2/semanticscholar/Journal.py`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.1/semanticscholar/PaginatedResults.py` & `semanticscholar-0.8.2/semanticscholar/PaginatedResults.py`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.1/semanticscholar/Paper.py` & `semanticscholar-0.8.2/semanticscholar/Paper.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     This class abstracts a paper.
     '''
 
     FIELDS = [
         'abstract',
         'authors',
         'authors.affiliations',
-        'authors.aliases',
         'authors.authorId',
         'authors.citationCount',
         'authors.externalIds',
         'authors.hIndex',
         'authors.homepage',
         'authors.name',
         'authors.paperCount',
```

### Comparing `semanticscholar-0.8.1/semanticscholar/PublicationVenue.py` & `semanticscholar-0.8.2/semanticscholar/PublicationVenue.py`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.1/semanticscholar/SemanticScholar.py` & `semanticscholar-0.8.2/semanticscholar/SemanticScholar.py`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.1/semanticscholar/SemanticScholarObject.py` & `semanticscholar-0.8.2/semanticscholar/SemanticScholarObject.py`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.1/semanticscholar/Tldr.py` & `semanticscholar-0.8.2/semanticscholar/Tldr.py`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.1/semanticscholar.egg-info/PKG-INFO` & `semanticscholar-0.8.2/semanticscholar.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semanticscholar
-Version: 0.8.1
+Version: 0.8.2
 Summary: Unofficial Python client library for Semantic Scholar APIs.
 Home-page: http://danielnsilva.com/semanticscholar
 Author: Daniel Silva
 Author-email: danielnsilva@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `semanticscholar-0.8.1/semanticscholar.egg-info/SOURCES.txt` & `semanticscholar-0.8.2/semanticscholar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `semanticscholar-0.8.1/setup.py` & `semanticscholar-0.8.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 
 setup(
     name='semanticscholar',
-    version='0.8.1',
+    version='0.8.2',
     description='Unofficial Python client library for Semantic Scholar APIs.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='http://danielnsilva.com/semanticscholar',
     author='Daniel Silva',
     author_email='danielnsilva@gmail.com',
     license='MIT',
```

### Comparing `semanticscholar-0.8.1/tests/test_semanticscholar.py` & `semanticscholar-0.8.2/tests/test_semanticscholar.py`

 * *Files identical despite different names*

