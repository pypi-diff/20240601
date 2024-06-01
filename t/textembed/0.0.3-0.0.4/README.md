# Comparing `tmp/textembed-0.0.3.tar.gz` & `tmp/textembed-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textembed-0.0.3.tar", last modified: Wed May 29 17:33:39 2024, max compression
+gzip compressed data, was "textembed-0.0.4.tar", last modified: Sat Jun  1 19:46:15 2024, max compression
```

## Comparing `textembed-0.0.3.tar` & `textembed-0.0.4.tar`

### file list

```diff
@@ -1,46 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.445384 textembed-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-05-29 17:33:35.000000 textembed-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-29 17:33:35.000000 textembed-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-29 17:33:39.445384 textembed-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1840 2024-05-29 17:33:35.000000 textembed-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 17:33:35.000000 textembed-0.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-29 17:33:39.445384 textembed-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-05-29 17:33:35.000000 textembed-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.437384 textembed-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.441384 textembed-0.0.3/src/textembed/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.441384 textembed-0.0.3/src/textembed/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/api/docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/api/embed.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/api/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/api/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3664 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/api/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.445384 textembed-0.0.3/src/textembed/application/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/application/application.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.445384 textembed-0.0.3/src/textembed/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/batch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4283 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/batch/batch_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.445384 textembed-0.0.3/src/textembed/cache/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/cache/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.445384 textembed-0.0.3/src/textembed/engine/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/engine/args.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/engine/async_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.445384 textembed-0.0.3/src/textembed/executor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/executor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/executor/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.445384 textembed-0.0.3/src/textembed/executor/embedder/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/executor/embedder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4135 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/executor/embedder/sentence_transformer.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/executor/primitives.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-29 17:33:35.000000 textembed-0.0.3/src/textembed/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-29 17:33:39.445384 textembed-0.0.3/src/textembed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-05-29 17:33:39.000000 textembed-0.0.3/src/textembed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-29 17:33:39.000000 textembed-0.0.3/src/textembed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-29 17:33:39.000000 textembed-0.0.3/src/textembed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-05-29 17:33:39.000000 textembed-0.0.3/src/textembed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-29 17:33:39.000000 textembed-0.0.3/src/textembed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:46:15.114381 textembed-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11348 2024-06-01 19:46:10.000000 textembed-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-06-01 19:46:10.000000 textembed-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-06-01 19:46:15.114381 textembed-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-06-01 19:46:10.000000 textembed-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-06-01 19:46:10.000000 textembed-0.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-06-01 19:46:15.114381 textembed-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-06-01 19:46:10.000000 textembed-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:46:15.106381 textembed-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:46:15.110381 textembed-0.0.4/src/textembed/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:46:15.110381 textembed-0.0.4/src/textembed/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1480 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/api/docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3492 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/api/embed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/api/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/api/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/api/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:46:15.110381 textembed-0.0.4/src/textembed/application/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/application/application.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:46:15.114381 textembed-0.0.4/src/textembed/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/batch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/batch/batch_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:46:15.114381 textembed-0.0.4/src/textembed/engine/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1629 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/engine/args.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/engine/async_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:46:15.114381 textembed-0.0.4/src/textembed/executor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/executor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/executor/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:46:15.114381 textembed-0.0.4/src/textembed/executor/embedder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/executor/embedder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/executor/embedder/sentence_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      586 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/executor/primitives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-06-01 19:46:10.000000 textembed-0.0.4/src/textembed/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-06-01 19:46:15.114381 textembed-0.0.4/src/textembed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-06-01 19:46:15.000000 textembed-0.0.4/src/textembed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-06-01 19:46:15.000000 textembed-0.0.4/src/textembed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-06-01 19:46:15.000000 textembed-0.0.4/src/textembed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-06-01 19:46:15.000000 textembed-0.0.4/src/textembed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-06-01 19:46:15.000000 textembed-0.0.4/src/textembed.egg-info/top_level.txt
```

### Comparing `textembed-0.0.3/LICENSE` & `textembed-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `textembed-0.0.3/PKG-INFO` & `textembed-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: textembed
-Version: 0.0.3
+Version: 0.0.4
 Summary: TextEmbed provides a robust and scalable REST API for generating vector embeddings from text. Built for performance and flexibility, it supports various sentence-transformer models, allowing users to easily integrate state-of-the-art NLP techniques into their applications. Whether you need embeddings for search, recommendation, or other NLP tasks, TextEmbed delivers with high efficiency.
 Home-page: https://github.com/kevaldekivadiya2415/textembed
 Author: Keval Dekivadiya
 Author-email: kevaldekivadiya2415@gmail.com
 License: Apache License 2.0
 Keywords: Embedding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.11.0
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==4.3.0
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: click==8.1.7
@@ -57,15 +58,15 @@
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: regex==2024.5.15
 Requires-Dist: requests==2.31.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: safetensors==0.4.3
 Requires-Dist: scikit-learn==1.4.2
 Requires-Dist: scipy==1.13.0
-Requires-Dist: sentence-transformers==2.7.0
+Requires-Dist: sentence-transformers==3.0.0
 Requires-Dist: shellingham==1.5.4
 Requires-Dist: sniffio==1.3.1
 Requires-Dist: starlette==0.37.2
 Requires-Dist: sympy==1.12
 Requires-Dist: threadpoolctl==3.5.0
 Requires-Dist: tokenizers==0.19.1
 Requires-Dist: torch==2.3.0
@@ -98,15 +99,15 @@
 
 Ensure you have Python 3.11 or higher installed. You will also need to install the required dependencies.
 
 ### Installation
 
 1. Install the required dependencies:
     ```bash
-    pip install -r requirements.txt
+    pip install -U textembed
     ```
 
 2. Start the TextEmbed server with your desired model:
     ```bash
     python3 -m textembed.server --model <Model Name>
     ```
```

### Comparing `textembed-0.0.3/README.md` & `textembed-0.0.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 Ensure you have Python 3.11 or higher installed. You will also need to install the required dependencies.
 
 ### Installation
 
 1. Install the required dependencies:
     ```bash
-    pip install -r requirements.txt
+    pip install -U textembed
     ```
 
 2. Start the TextEmbed server with your desired model:
     ```bash
     python3 -m textembed.server --model <Model Name>
     ```
```

### Comparing `textembed-0.0.3/requirements.txt` & `textembed-0.0.4/requirements.txt`

 * *Files 11% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 PyYAML==6.0.1
 regex==2024.5.15
 requests==2.31.0
 rich==13.7.1
 safetensors==0.4.3
 scikit-learn==1.4.2
 scipy==1.13.0
-sentence-transformers==2.7.0
+sentence-transformers==3.0.0
 shellingham==1.5.4
 sniffio==1.3.1
 starlette==0.37.2
 sympy==1.12
 threadpoolctl==3.5.0
 tokenizers==0.19.1
 torch==2.3.0
```

### Comparing `textembed-0.0.3/setup.py` & `textembed-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,23 +64,24 @@
         long_description=open("README.md", "r", encoding="utf-8").read(),
         long_description_content_type="text/markdown",
         keywords=["Embedding"],
         license="Apache License 2.0",
         url="https://github.com/kevaldekivadiya2415/textembed",
         package_dir={"": "src"},
         packages=find_packages("src"),
-        python_requires=">=3.11.0",
+        python_requires=">=3.10.0",
         install_requires=get_requires(),
         classifiers=[
             "Development Status :: 4 - Beta",
             "Intended Audience :: Developers",
             "Intended Audience :: Education",
             "Intended Audience :: Science/Research",
             "License :: OSI Approved :: Apache Software License",
             "Operating System :: OS Independent",
+            "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: 3.11",
             "Programming Language :: Python :: 3.12",
             "Topic :: Scientific/Engineering :: Artificial Intelligence",
         ],
     )
```

### Comparing `textembed-0.0.3/src/textembed/api/docs.py` & `textembed-0.0.4/src/textembed/api/docs.py`

 * *Files identical despite different names*

### Comparing `textembed-0.0.3/src/textembed/api/embed.py` & `textembed-0.0.4/src/textembed/api/embed.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import asyncio
 import time
 from uuid import uuid4
 
 from fastapi import APIRouter, Request, status
 from fastapi.responses import ORJSONResponse
 
+from textembed.api.errors import ModelNotFoundException
 from textembed.api.schemas import (
     EmbeddingData,
     EmbeddingRequest,
     EmbeddingResponse,
     ModelDetails,
     ModelList,
     Usage,
@@ -34,15 +35,22 @@
     Args:
         request (Request): The user request.
 
     Returns:
         ModelList: A list of available embedding models.
     """
     engine_args: AsyncEngineArgs = request.app.state.async_engine.engine_args
-    return ModelList(data=[ModelDetails(id=engine_args.model)])
+    return ModelList(
+        data=[
+            ModelDetails(
+                id=engine_args.model,
+                served_model_name=engine_args.served_model_name,  # type: ignore
+            )
+        ]
+    )
 
 
 @embed_router.post(
     "/embedding",
     response_class=ORJSONResponse,
     response_model=EmbeddingResponse,
     status_code=status.HTTP_200_OK,
@@ -57,14 +65,23 @@
         embed_request (EmbeddingRequest): The request containing input text
                                         and optional model and user information.
 
     Returns:
         EmbeddingResponse: The response containing embedding data.
     """
     async_engine: AsyncEngine = request.app.state.async_engine
+    async_engine_args = async_engine.engine_args
+
+    # Check model
+    if embed_request.model != async_engine_args.served_model_name:
+        raise ModelNotFoundException(
+            message=f"The requested model `{embed_request.model}` was not found. "
+            f"Please ensure that you have specified the correct model name. "
+            f"Currently served model is `{async_engine_args.served_model_name}`."
+        )
 
     # Ensure input
     if isinstance(embed_request.input, str):
         embed_request.input = [embed_request.input]
 
     start_time = time.perf_counter()
```

### Comparing `textembed-0.0.3/src/textembed/api/monitor.py` & `textembed-0.0.4/src/textembed/api/monitor.py`

 * *Files identical despite different names*

### Comparing `textembed-0.0.3/src/textembed/api/schemas.py` & `textembed-0.0.4/src/textembed/api/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,21 +35,23 @@
     code: Optional[int] = None
 
 
 class ModelDetails(BaseModel):
     """Details of a model.
 
     Attributes:
-        id (str): Unique identifier for the model.
+        id (str): Model name or id.
+        served_model_name (str): Served model name, default is "".
         object (str): Type of the object, default is "model".
         owned_by (str): Owner of the model, default is "textembed".
         created (int): Timestamp when the model details were created.
     """
 
     id: str
+    served_model_name: str = None # type: ignore
     object: str = "model"
     owned_by: str = "textembed"
     created: int = Field(default_factory=lambda: int(time.time()))
 
 
 class ModelList(BaseModel):
     """List of model details objects.
```

### Comparing `textembed-0.0.3/src/textembed/application/application.py` & `textembed-0.0.4/src/textembed/application/application.py`

 * *Files identical despite different names*

### Comparing `textembed-0.0.3/src/textembed/batch/batch_processor.py` & `textembed-0.0.4/src/textembed/batch/batch_processor.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,14 +41,20 @@
         self.workers = workers
         self.batch_size = batch_size
         self.request_queue: Queue = Queue()
         self.loop = asyncio.get_running_loop()
         self.worker_tasks = [
             self.loop.create_task(self.batch_processor(i)) for i in range(workers)
         ]
+        # Wait until all worker tasks are started
+        self.loop.create_task(self._log_workers_started())
+
+    async def _log_workers_started(self):
+        await asyncio.sleep(0)  # Yield control to ensure workers have started
+        logger.info("All %d workers started.", self.workers)
 
     async def batch_processor(self, worker_id: int):
         """Worker task that processes requests from the queue in batches.
 
         Args:
             worker_id (int): The identifier for the worker task.
         """
```

### Comparing `textembed-0.0.3/src/textembed/engine/args.py` & `textembed-0.0.4/src/textembed/engine/args.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @dataclass
 class AsyncEngineArgs:
     """A dataclass representing the arguments required to initialize an asynchronous engine.
 
     Attributes:
         model (str): The path or identifier of the model to be used by the engine.
         served_model_name (Optional[str]): An optional name to be used for serving the model.
-                                           If not provided, it is derived from the last two segments of the model path.
+                                            Default is `model` name
         trust_remote_code (bool): Whether to trust remote code.
         workers (int): The number of worker tasks to process requests. Defaults to the number of CPU cores.
         batch_size (int): The maximum number of requests to process in a single batch.
                           Must be greater than or equal to 1.
         embedding_dtype(str): Embedding data type for final generate embedding.
     """
 
@@ -26,20 +26,15 @@
     workers: int = multiprocessing.cpu_count()
     batch_size: int = 32
     embedding_dtype: str = "float32"
 
     def __post_init__(self):
         # If served_model_name is not provided, derive it from the model path
         if self.served_model_name is None:
-            # Split the model path and take the last two segments to form the served_model_name
-            segments = self.model.split("/")
-            if len(segments) >= 2:
-                self.served_model_name = "/".join(segments[-2:])
-            else:
-                self.served_model_name = segments[-1] if segments else "default_model"
+            self.served_model_name = self.model
 
         # Ensure the batch size is valid
         if self.batch_size < 1:
             raise ValueError("Batch size must be greater than or equal to 1.")
 
         # Ensure the number of workers is valid
         if self.workers < 1:
```

### Comparing `textembed-0.0.3/src/textembed/engine/async_engine.py` & `textembed-0.0.4/src/textembed/engine/async_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -61,14 +61,17 @@
             model=self.model,
             workers=self._engine_args.workers,
             batch_size=self._engine_args.batch_size,
         )
         self.running = True
         logger.info("Engine started.")
 
+        # Warm-up the model
+        await self.model.warm_up()
+
     async def stop(self):
         """Stop the engine.
 
         This method sets the running flag to False, indicating that the engine
         is no longer active and will not process requests.
 
         Raises:
```

### Comparing `textembed-0.0.3/src/textembed/executor/base.py` & `textembed-0.0.4/src/textembed/executor/base.py`

 * *Files identical despite different names*

### Comparing `textembed-0.0.3/src/textembed/executor/embedder/sentence_transformer.py` & `textembed-0.0.4/src/textembed/executor/embedder/sentence_transformer.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,20 @@
             model_name_or_path=engine_args.model,
             device="cpu",
             trust_remote_code=engine_args.trust_remote_code,
         )
         self.embedding_dtype = engine_args.embedding_dtype
         self.eval()
 
+    async def warm_up(self) -> None:
+        """Warm up the model by performing a dummy inference."""
+        sample_sentences = ["This is a sample sentence."] * 10
+        # Perform inference
+        await self.process_batch(sample_sentences)
+
     async def preprocess(
         self, sentences: List[str]
     ) -> Tuple[Dict[str, Tensor], List[int]]:
         """Tokenizes the input sentences.
 
         Args:
             sentences (List[str]): List of sentences to be tokenized.
```

### Comparing `textembed-0.0.3/src/textembed/executor/primitives.py` & `textembed-0.0.4/src/textembed/executor/primitives.py`

 * *Files identical despite different names*

### Comparing `textembed-0.0.3/src/textembed/log.py` & `textembed-0.0.4/src/textembed/log.py`

 * *Files identical despite different names*

### Comparing `textembed-0.0.3/src/textembed/server.py` & `textembed-0.0.4/src/textembed/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import multiprocessing
 import warnings
 
 import typer
 import uvicorn
 from typing_extensions import Annotated
 
-from textembed.api.errors import EmbeddingException, embedding_exception_handler
+from textembed.api.errors import HandleExceptions
 from textembed.application.application import create_application
 from textembed.engine.args import AsyncEngineArgs
 
 # Filter out all warnings
 warnings.filterwarnings("ignore")
 
 app_typer = typer.Typer()
@@ -78,14 +78,14 @@
 
     app = create_application(
         engine_args=engine_args,
         doc_extra={"host": host, "port": port},
     )
 
     # Handle Errors
-    app.add_exception_handler(EmbeddingException, embedding_exception_handler)  # type: ignore
+    HandleExceptions(app=app)
 
     uvicorn.run(app, host=host, port=port, log_level="error")
 
 
 if __name__ == "__main__":
     app_typer()
```

### Comparing `textembed-0.0.3/src/textembed.egg-info/PKG-INFO` & `textembed-0.0.4/src/textembed.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: textembed
-Version: 0.0.3
+Version: 0.0.4
 Summary: TextEmbed provides a robust and scalable REST API for generating vector embeddings from text. Built for performance and flexibility, it supports various sentence-transformer models, allowing users to easily integrate state-of-the-art NLP techniques into their applications. Whether you need embeddings for search, recommendation, or other NLP tasks, TextEmbed delivers with high efficiency.
 Home-page: https://github.com/kevaldekivadiya2415/textembed
 Author: Keval Dekivadiya
 Author-email: kevaldekivadiya2415@gmail.com
 License: Apache License 2.0
 Keywords: Embedding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Requires-Python: >=3.11.0
+Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: annotated-types==0.6.0
 Requires-Dist: anyio==4.3.0
 Requires-Dist: certifi==2024.2.2
 Requires-Dist: charset-normalizer==3.3.2
 Requires-Dist: click==8.1.7
@@ -57,15 +58,15 @@
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: regex==2024.5.15
 Requires-Dist: requests==2.31.0
 Requires-Dist: rich==13.7.1
 Requires-Dist: safetensors==0.4.3
 Requires-Dist: scikit-learn==1.4.2
 Requires-Dist: scipy==1.13.0
-Requires-Dist: sentence-transformers==2.7.0
+Requires-Dist: sentence-transformers==3.0.0
 Requires-Dist: shellingham==1.5.4
 Requires-Dist: sniffio==1.3.1
 Requires-Dist: starlette==0.37.2
 Requires-Dist: sympy==1.12
 Requires-Dist: threadpoolctl==3.5.0
 Requires-Dist: tokenizers==0.19.1
 Requires-Dist: torch==2.3.0
@@ -98,15 +99,15 @@
 
 Ensure you have Python 3.11 or higher installed. You will also need to install the required dependencies.
 
 ### Installation
 
 1. Install the required dependencies:
     ```bash
-    pip install -r requirements.txt
+    pip install -U textembed
     ```
 
 2. Start the TextEmbed server with your desired model:
     ```bash
     python3 -m textembed.server --model <Model Name>
     ```
```

### Comparing `textembed-0.0.3/src/textembed.egg-info/SOURCES.txt` & `textembed-0.0.4/src/textembed.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -17,16 +17,14 @@
 src/textembed/api/errors.py
 src/textembed/api/monitor.py
 src/textembed/api/schemas.py
 src/textembed/application/__init__.py
 src/textembed/application/application.py
 src/textembed/batch/__init__.py
 src/textembed/batch/batch_processor.py
-src/textembed/cache/__init__.py
-src/textembed/cache/cache.py
 src/textembed/engine/__init__.py
 src/textembed/engine/args.py
 src/textembed/engine/async_engine.py
 src/textembed/executor/__init__.py
 src/textembed/executor/base.py
 src/textembed/executor/primitives.py
 src/textembed/executor/embedder/__init__.py
```

### Comparing `textembed-0.0.3/src/textembed.egg-info/requires.txt` & `textembed-0.0.4/src/textembed.egg-info/requires.txt`

 * *Files 11% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 PyYAML==6.0.1
 regex==2024.5.15
 requests==2.31.0
 rich==13.7.1
 safetensors==0.4.3
 scikit-learn==1.4.2
 scipy==1.13.0
-sentence-transformers==2.7.0
+sentence-transformers==3.0.0
 shellingham==1.5.4
 sniffio==1.3.1
 starlette==0.37.2
 sympy==1.12
 threadpoolctl==3.5.0
 tokenizers==0.19.1
 torch==2.3.0
```

