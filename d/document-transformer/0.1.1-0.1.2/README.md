# Comparing `tmp/document_transformer-0.1.1.tar.gz` & `tmp/document_transformer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "document_transformer-0.1.1.tar", max compression
+gzip compressed data, was "document_transformer-0.1.2.tar", max compression
```

## Comparing `document_transformer-0.1.1.tar` & `document_transformer-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-06-01 16:24:26.013275 document_transformer-0.1.1/LICENSE
--rw-r--r--   0        0        0     3009 2024-06-01 19:14:07.363210 document_transformer-0.1.1/README.md
--rw-r--r--   0        0        0     2375 2024-05-29 19:09:05.795246 document_transformer-0.1.1/document_transformer/Document.py
--rw-r--r--   0        0        0     2108 2024-06-01 17:19:36.963254 document_transformer-0.1.1/document_transformer/Pipeline.py
--rw-r--r--   0        0        0     2759 2024-06-01 17:06:40.133259 document_transformer-0.1.1/document_transformer/Transformer.py
--rw-r--r--   0        0        0      106 2024-06-01 16:56:15.523263 document_transformer-0.1.1/document_transformer/__init__.py
--rw-r--r--   0        0        0      366 2024-06-01 17:21:45.423253 document_transformer-0.1.1/document_transformer/utils.py
--rw-r--r--   0        0        0      324 2024-06-01 19:15:48.043209 document_transformer-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3548 1970-01-01 00:00:00.000000 document_transformer-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-06-01 16:24:26.013275 document_transformer-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3009 2024-06-01 19:14:07.363210 document_transformer-0.1.2/README.md
+-rw-r--r--   0        0        0     2375 2024-05-29 19:09:05.795246 document_transformer-0.1.2/document_transformer/Document.py
+-rw-r--r--   0        0        0     2108 2024-06-01 17:19:36.963254 document_transformer-0.1.2/document_transformer/Pipeline.py
+-rw-r--r--   0        0        0     2759 2024-06-01 17:06:40.133259 document_transformer-0.1.2/document_transformer/Transformer.py
+-rw-r--r--   0        0        0      106 2024-06-01 16:56:15.523263 document_transformer-0.1.2/document_transformer/__init__.py
+-rw-r--r--   0        0        0      366 2024-06-01 17:21:45.423253 document_transformer-0.1.2/document_transformer/utils.py
+-rw-r--r--   0        0        0      674 2024-06-01 19:25:10.213205 document_transformer-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3997 1970-01-01 00:00:00.000000 document_transformer-0.1.2/PKG-INFO
```

### Comparing `document_transformer-0.1.1/LICENSE` & `document_transformer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `document_transformer-0.1.1/README.md` & `document_transformer-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `document_transformer-0.1.1/document_transformer/Document.py` & `document_transformer-0.1.2/document_transformer/Document.py`

 * *Files identical despite different names*

### Comparing `document_transformer-0.1.1/document_transformer/Pipeline.py` & `document_transformer-0.1.2/document_transformer/Pipeline.py`

 * *Files identical despite different names*

### Comparing `document_transformer-0.1.1/document_transformer/Transformer.py` & `document_transformer-0.1.2/document_transformer/Transformer.py`

 * *Files identical despite different names*

### Comparing `document_transformer-0.1.1/PKG-INFO` & `document_transformer-0.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,26 @@
 Metadata-Version: 2.1
 Name: document-transformer
-Version: 0.1.1
-Summary: 
+Version: 0.1.2
+Summary: Organize your document transformation pipeline. Define your components, this tool ensure traceability and organization. Reuse your work easily in other projects
+Home-page: https://github.com/johngonzalez/document-transformer
+License: MIT
+Keywords: document,transformer,pipeline,components,reuse,traceability,organization
 Author: John Gonzalez
 Author-email: johngonzalezv@gmail.com
 Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: graphviz (>=0.20.3,<0.21.0)
 Requires-Dist: pydantic (>=2.7.2,<3.0.0)
+Project-URL: Repository, https://github.com/johngonzalez/document-transformer
 Description-Content-Type: text/markdown
 
 # Document Transformer
 
 Document Transformer allows users to define and apply transformations to documents in a flexible and robust manner, ensuring traceability of each change made to the documents.
 
 ## Table of Contents
```

