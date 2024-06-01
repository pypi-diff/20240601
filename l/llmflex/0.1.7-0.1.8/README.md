# Comparing `tmp/llmflex-0.1.7.tar.gz` & `tmp/llmflex-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmflex-0.1.7.tar", last modified: Wed May 22 20:09:35 2024, max compression
+gzip compressed data, was "llmflex-0.1.8.tar", last modified: Sat Jun  1 11:26:33 2024, max compression
```

## Comparing `llmflex-0.1.7.tar` & `llmflex-0.1.8.tar`

### file list

```diff
@@ -1,79 +1,76 @@
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.132888 llmflex-0.1.7/
--rw-r--r--   0 nathan95   (501) staff       (20)     1067 2024-01-22 01:35:14.000000 llmflex-0.1.7/LICENSE.md
--rw-r--r--   0 nathan95   (501) staff       (20)    10171 2024-05-22 20:09:35.132659 llmflex-0.1.7/PKG-INFO
--rw-r--r--   0 nathan95   (501) staff       (20)     8926 2024-05-21 17:59:14.000000 llmflex-0.1.7/README.md
--rw-r--r--   0 nathan95   (501) staff       (20)     1244 2024-05-21 17:59:14.000000 llmflex-0.1.7/pyproject.toml
--rw-r--r--   0 nathan95   (501) staff       (20)       38 2024-05-22 20:09:35.132941 llmflex-0.1.7/setup.cfg
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.121561 llmflex-0.1.7/src/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.123479 llmflex-0.1.7/src/llmflex/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.125162 llmflex-0.1.7/src/llmflex/Embeddings/
--rw-r--r--   0 nathan95   (501) staff       (20)      226 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Embeddings/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4555 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Embeddings/api_embeddings.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4608 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Embeddings/base_embeddings.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2275 2024-03-15 22:38:26.000000 llmflex-0.1.7/src/llmflex/Embeddings/hf_embeddings_server.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4147 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Embeddings/huggingface_embeddings.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.125620 llmflex-0.1.7/src/llmflex/Frontend/
--rw-r--r--   0 nathan95   (501) staff       (20)      102 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Frontend/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    29992 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Frontend/gradio_interface.py
--rw-r--r--   0 nathan95   (501) staff       (20)    37304 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Frontend/streamlit_interface.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.125927 llmflex-0.1.7/src/llmflex/KnowledgeBase/
--rw-r--r--   0 nathan95   (501) staff       (20)      108 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/KnowledgeBase/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    13135 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/KnowledgeBase/knowledge_base.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.126841 llmflex-0.1.7/src/llmflex/Memory/
--rw-r--r--   0 nathan95   (501) staff       (20)      287 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Memory/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     8298 2024-03-11 17:44:28.000000 llmflex-0.1.7/src/llmflex/Memory/assistant_long_term_memory.py
--rw-r--r--   0 nathan95   (501) staff       (20)    13190 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Memory/base_memory.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7727 2024-03-11 17:44:28.000000 llmflex-0.1.7/src/llmflex/Memory/long_short_memory.py
--rw-r--r--   0 nathan95   (501) staff       (20)    13523 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Memory/longshort_memory.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.127040 llmflex-0.1.7/src/llmflex/Models/
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.128324 llmflex-0.1.7/src/llmflex/Models/Cores/
--rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Models/Cores/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    15434 2024-05-22 20:08:53.000000 llmflex-0.1.7/src/llmflex/Models/Cores/base_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7915 2024-02-25 22:17:53.000000 llmflex-0.1.7/src/llmflex/Models/Cores/exllamav2_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     9365 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Models/Cores/huggingface_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     8223 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Models/Cores/llamacpp_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     9273 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Models/Cores/openai_core.py
--rw-r--r--   0 nathan95   (501) staff       (20)     7524 2024-05-22 20:08:53.000000 llmflex-0.1.7/src/llmflex/Models/Cores/utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.128585 llmflex-0.1.7/src/llmflex/Models/Factory/
--rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Models/Factory/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    10723 2024-04-14 12:29:06.000000 llmflex-0.1.7/src/llmflex/Models/Factory/llm_factory.py
--rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Models/__init__.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.128919 llmflex-0.1.7/src/llmflex/Prompts/
--rw-r--r--   0 nathan95   (501) staff       (20)       52 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Prompts/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    21647 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Prompts/prompt_template.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.129330 llmflex-0.1.7/src/llmflex/Rankers/
--rw-r--r--   0 nathan95   (501) staff       (20)       81 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Rankers/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1471 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Rankers/base_ranker.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2309 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Rankers/flashrank_ranker.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.129710 llmflex-0.1.7/src/llmflex/Schemas/
--rw-r--r--   0 nathan95   (501) staff       (20)       64 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Schemas/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1414 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Schemas/documents.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2429 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Schemas/tokenizer.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.130214 llmflex-0.1.7/src/llmflex/TextSplitters/
--rw-r--r--   0 nathan95   (501) staff       (20)      123 2024-03-11 17:44:28.000000 llmflex-0.1.7/src/llmflex/TextSplitters/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1526 2024-03-11 17:44:28.000000 llmflex-0.1.7/src/llmflex/TextSplitters/base_text_splitter.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2860 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/TextSplitters/sentence_token_text_splitter.py
--rw-r--r--   0 nathan95   (501) staff       (20)     1423 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/TextSplitters/token_text_splitter.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.131386 llmflex-0.1.7/src/llmflex/Tools/
--rw-r--r--   0 nathan95   (501) staff       (20)      115 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Tools/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    11795 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/Tools/base_tool.py
--rw-r--r--   0 nathan95   (501) staff       (20)     2983 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Tools/browser_tool.py
--rw-r--r--   0 nathan95   (501) staff       (20)       45 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Tools/tool_prompting.py
--rw-r--r--   0 nathan95   (501) staff       (20)     6603 2024-03-11 17:44:28.000000 llmflex-0.1.7/src/llmflex/Tools/tool_selection.py
--rw-r--r--   0 nathan95   (501) staff       (20)     9639 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Tools/tool_utils.py
--rw-r--r--   0 nathan95   (501) staff       (20)    11421 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/Tools/web_search_tool.py
--rw-r--r--   0 nathan95   (501) staff       (20)    15193 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/Tools/web_search_utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.131838 llmflex-0.1.7/src/llmflex/VectorDBs/
--rw-r--r--   0 nathan95   (501) staff       (20)       93 2024-03-11 17:44:28.000000 llmflex-0.1.7/src/llmflex/VectorDBs/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)    24488 2024-05-21 17:59:14.000000 llmflex-0.1.7/src/llmflex/VectorDBs/base_vectordb.py
--rw-r--r--   0 nathan95   (501) staff       (20)     5362 2024-04-21 17:42:51.000000 llmflex-0.1.7/src/llmflex/VectorDBs/faiss_vectordb.py
--rw-r--r--   0 nathan95   (501) staff       (20)      275 2024-05-22 20:08:53.000000 llmflex-0.1.7/src/llmflex/__init__.py
--rw-r--r--   0 nathan95   (501) staff       (20)     4381 2024-02-24 22:31:02.000000 llmflex-0.1.7/src/llmflex/cli.py
--rw-r--r--   0 nathan95   (501) staff       (20)     6178 2024-03-11 17:44:28.000000 llmflex-0.1.7/src/llmflex/utils.py
-drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-05-22 20:09:35.132036 llmflex-0.1.7/src/llmflex.egg-info/
--rw-r--r--   0 nathan95   (501) staff       (20)    10171 2024-05-22 20:09:35.000000 llmflex-0.1.7/src/llmflex.egg-info/PKG-INFO
--rw-r--r--   0 nathan95   (501) staff       (20)     2165 2024-05-22 20:09:35.000000 llmflex-0.1.7/src/llmflex.egg-info/SOURCES.txt
--rw-r--r--   0 nathan95   (501) staff       (20)        1 2024-05-22 20:09:35.000000 llmflex-0.1.7/src/llmflex.egg-info/dependency_links.txt
--rw-r--r--   0 nathan95   (501) staff       (20)       44 2024-05-22 20:09:35.000000 llmflex-0.1.7/src/llmflex.egg-info/entry_points.txt
--rw-r--r--   0 nathan95   (501) staff       (20)      357 2024-05-22 20:09:35.000000 llmflex-0.1.7/src/llmflex.egg-info/requires.txt
--rw-r--r--   0 nathan95   (501) staff       (20)        8 2024-05-22 20:09:35.000000 llmflex-0.1.7/src/llmflex.egg-info/top_level.txt
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.601190 llmflex-0.1.8/
+-rw-r--r--   0 nathan95   (501) staff       (20)     1067 2024-01-22 01:35:14.000000 llmflex-0.1.8/LICENSE.md
+-rw-r--r--   0 nathan95   (501) staff       (20)     8503 2024-06-01 11:26:33.600912 llmflex-0.1.8/PKG-INFO
+-rw-r--r--   0 nathan95   (501) staff       (20)     7177 2024-06-01 11:25:49.000000 llmflex-0.1.8/README.md
+-rw-r--r--   0 nathan95   (501) staff       (20)     1301 2024-06-01 11:25:49.000000 llmflex-0.1.8/pyproject.toml
+-rw-r--r--   0 nathan95   (501) staff       (20)       38 2024-06-01 11:26:33.601240 llmflex-0.1.8/setup.cfg
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.591616 llmflex-0.1.8/src/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.593323 llmflex-0.1.8/src/llmflex/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.594795 llmflex-0.1.8/src/llmflex/Embeddings/
+-rw-r--r--   0 nathan95   (501) staff       (20)      226 2024-02-24 22:31:02.000000 llmflex-0.1.8/src/llmflex/Embeddings/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4555 2024-04-21 17:42:51.000000 llmflex-0.1.8/src/llmflex/Embeddings/api_embeddings.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4608 2024-04-21 17:42:51.000000 llmflex-0.1.8/src/llmflex/Embeddings/base_embeddings.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2275 2024-03-15 22:38:26.000000 llmflex-0.1.8/src/llmflex/Embeddings/hf_embeddings_server.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4145 2024-06-01 11:25:49.000000 llmflex-0.1.8/src/llmflex/Embeddings/huggingface_embeddings.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.595203 llmflex-0.1.8/src/llmflex/Frontend/
+-rw-r--r--   0 nathan95   (501) staff       (20)      107 2024-06-01 11:25:49.000000 llmflex-0.1.8/src/llmflex/Frontend/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    12994 2024-06-01 11:25:49.000000 llmflex-0.1.8/src/llmflex/Frontend/app_resource.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    25909 2024-06-01 11:25:49.000000 llmflex-0.1.8/src/llmflex/Frontend/streamlit_interface.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.595474 llmflex-0.1.8/src/llmflex/KnowledgeBase/
+-rw-r--r--   0 nathan95   (501) staff       (20)      108 2024-05-21 17:59:14.000000 llmflex-0.1.8/src/llmflex/KnowledgeBase/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    13135 2024-05-21 17:59:14.000000 llmflex-0.1.8/src/llmflex/KnowledgeBase/knowledge_base.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.596029 llmflex-0.1.8/src/llmflex/Memory/
+-rw-r--r--   0 nathan95   (501) staff       (20)      245 2024-06-01 11:25:49.000000 llmflex-0.1.8/src/llmflex/Memory/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    12272 2024-06-01 11:25:49.000000 llmflex-0.1.8/src/llmflex/Memory/base_memory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     9660 2024-06-01 11:25:49.000000 llmflex-0.1.8/src/llmflex/Memory/long_short_memory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     4899 2024-06-01 11:25:49.000000 llmflex-0.1.8/src/llmflex/Memory/memory_utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.596172 llmflex-0.1.8/src/llmflex/Models/
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.597077 llmflex-0.1.8/src/llmflex/Models/Cores/
+-rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.8/src/llmflex/Models/Cores/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    15434 2024-05-22 20:08:53.000000 llmflex-0.1.8/src/llmflex/Models/Cores/base_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7915 2024-02-25 22:17:53.000000 llmflex-0.1.8/src/llmflex/Models/Cores/exllamav2_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     9365 2024-05-21 17:59:14.000000 llmflex-0.1.8/src/llmflex/Models/Cores/huggingface_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     8223 2024-05-21 17:59:14.000000 llmflex-0.1.8/src/llmflex/Models/Cores/llamacpp_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     9273 2024-05-21 17:59:14.000000 llmflex-0.1.8/src/llmflex/Models/Cores/openai_core.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     7524 2024-05-22 20:08:53.000000 llmflex-0.1.8/src/llmflex/Models/Cores/utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.597321 llmflex-0.1.8/src/llmflex/Models/Factory/
+-rw-r--r--   0 nathan95   (501) staff       (20)        0 2024-02-24 22:31:02.000000 llmflex-0.1.8/src/llmflex/Models/Factory/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    10723 2024-04-14 12:29:06.000000 llmflex-0.1.8/src/llmflex/Models/Factory/llm_factory.py
+-rw-r--r--   0 nathan95   (501) staff       (20)       43 2024-02-24 22:31:02.000000 llmflex-0.1.8/src/llmflex/Models/__init__.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.597610 llmflex-0.1.8/src/llmflex/Prompts/
+-rw-r--r--   0 nathan95   (501) staff       (20)       52 2024-02-24 22:31:02.000000 llmflex-0.1.8/src/llmflex/Prompts/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    21647 2024-05-21 17:59:14.000000 llmflex-0.1.8/src/llmflex/Prompts/prompt_template.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.597999 llmflex-0.1.8/src/llmflex/Rankers/
+-rw-r--r--   0 nathan95   (501) staff       (20)       81 2024-04-21 17:42:51.000000 llmflex-0.1.8/src/llmflex/Rankers/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1471 2024-04-21 17:42:51.000000 llmflex-0.1.8/src/llmflex/Rankers/base_ranker.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2309 2024-04-21 17:42:51.000000 llmflex-0.1.8/src/llmflex/Rankers/flashrank_ranker.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.598351 llmflex-0.1.8/src/llmflex/Schemas/
+-rw-r--r--   0 nathan95   (501) staff       (20)       64 2024-04-21 17:42:51.000000 llmflex-0.1.8/src/llmflex/Schemas/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1414 2024-04-21 17:42:51.000000 llmflex-0.1.8/src/llmflex/Schemas/documents.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2429 2024-04-21 17:42:51.000000 llmflex-0.1.8/src/llmflex/Schemas/tokenizer.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.598891 llmflex-0.1.8/src/llmflex/TextSplitters/
+-rw-r--r--   0 nathan95   (501) staff       (20)      172 2024-06-01 11:25:49.000000 llmflex-0.1.8/src/llmflex/TextSplitters/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1526 2024-03-11 17:44:28.000000 llmflex-0.1.8/src/llmflex/TextSplitters/base_text_splitter.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     2860 2024-05-21 17:59:14.000000 llmflex-0.1.8/src/llmflex/TextSplitters/sentence_token_text_splitter.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     1423 2024-04-21 17:42:51.000000 llmflex-0.1.8/src/llmflex/TextSplitters/token_text_splitter.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.599701 llmflex-0.1.8/src/llmflex/Tools/
+-rw-r--r--   0 nathan95   (501) staff       (20)      134 2024-06-01 11:25:49.000000 llmflex-0.1.8/src/llmflex/Tools/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    11795 2024-02-24 22:31:02.000000 llmflex-0.1.8/src/llmflex/Tools/base_tool.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     3460 2024-06-01 11:25:49.000000 llmflex-0.1.8/src/llmflex/Tools/browser_tool.py
+-rw-r--r--   0 nathan95   (501) staff       (20)      393 2024-06-01 11:25:49.000000 llmflex-0.1.8/src/llmflex/Tools/tool_classes.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    23839 2024-06-01 11:25:49.000000 llmflex-0.1.8/src/llmflex/Tools/tool_utils.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    15250 2024-06-01 11:25:49.000000 llmflex-0.1.8/src/llmflex/Tools/web_search_utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.600100 llmflex-0.1.8/src/llmflex/VectorDBs/
+-rw-r--r--   0 nathan95   (501) staff       (20)       93 2024-03-11 17:44:28.000000 llmflex-0.1.8/src/llmflex/VectorDBs/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)    24488 2024-05-21 17:59:14.000000 llmflex-0.1.8/src/llmflex/VectorDBs/base_vectordb.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     5362 2024-04-21 17:42:51.000000 llmflex-0.1.8/src/llmflex/VectorDBs/faiss_vectordb.py
+-rw-r--r--   0 nathan95   (501) staff       (20)      275 2024-06-01 11:25:49.000000 llmflex-0.1.8/src/llmflex/__init__.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     3567 2024-06-01 11:25:49.000000 llmflex-0.1.8/src/llmflex/cli.py
+-rw-r--r--   0 nathan95   (501) staff       (20)     6178 2024-03-11 17:44:28.000000 llmflex-0.1.8/src/llmflex/utils.py
+drwxr-xr-x   0 nathan95   (501) staff       (20)        0 2024-06-01 11:26:33.600286 llmflex-0.1.8/src/llmflex.egg-info/
+-rw-r--r--   0 nathan95   (501) staff       (20)     8503 2024-06-01 11:26:33.000000 llmflex-0.1.8/src/llmflex.egg-info/PKG-INFO
+-rw-r--r--   0 nathan95   (501) staff       (20)     2033 2024-06-01 11:26:33.000000 llmflex-0.1.8/src/llmflex.egg-info/SOURCES.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)        1 2024-06-01 11:26:33.000000 llmflex-0.1.8/src/llmflex.egg-info/dependency_links.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)       44 2024-06-01 11:26:33.000000 llmflex-0.1.8/src/llmflex.egg-info/entry_points.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)      393 2024-06-01 11:26:33.000000 llmflex-0.1.8/src/llmflex.egg-info/requires.txt
+-rw-r--r--   0 nathan95   (501) staff       (20)        8 2024-06-01 11:26:33.000000 llmflex-0.1.8/src/llmflex.egg-info/top_level.txt
```

### Comparing `llmflex-0.1.7/LICENSE.md` & `llmflex-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/PKG-INFO` & `llmflex-0.1.8/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflex
-Version: 0.1.7
+Version: 0.1.8
 Summary: A python package for developing AI applications with local LLMs.
 Author-email: Nathan Tam <nathan1295@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nath1295/LLMFlex
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -14,25 +14,28 @@
 Requires-Dist: transformers>=4.35.0
 Requires-Dist: accelerate>=0.25.0
 Requires-Dist: sentence-transformers
 Requires-Dist: langchain
 Requires-Dist: faiss-cpu
 Requires-Dist: optimum
 Requires-Dist: gradio>=4.2
-Requires-Dist: duckduckgo-search>=5.2.2
+Requires-Dist: duckduckgo-search>=6.1.0
 Requires-Dist: fake-useragent
 Requires-Dist: openai>=1.0.0
 Requires-Dist: tiktoken
 Requires-Dist: protobuf
 Requires-Dist: beautifulsoup4
 Requires-Dist: streamlit
+Requires-Dist: streamlit-extras
 Requires-Dist: watchdog
+Requires-Dist: guidance
 Requires-Dist: spacy>=3.7.0
 Requires-Dist: flask
 Requires-Dist: PyMuPDF
+Requires-Dist: flashrank
 Requires-Dist: python-docx
 Provides-Extra: cu121
 Requires-Dist: auto-gptq>=0.6.0; extra == "cu121"
 Requires-Dist: autoawq; extra == "cu121"
 Requires-Dist: exllamav2; extra == "cu121"
 Provides-Extra: cu118
 Requires-Dist: auto-gptq; extra == "cu118"
@@ -90,18 +93,18 @@
 2. `LongShortTermChatMemory`  
 Memory class using an underlying `VectorDatabase` to maintain long term memory along with the most recent memory.
 
 ### 7. Prompt template
 A `PromptTemplate` class is implemented to format your prompt with different prompt formats for models from different sources. Some presets like `Llama2`, `ChatML`, `Vicuna`, and more are already implemented, but you can alway add your own prompt format template.
 
 ### 8. Custom tools
-A base class `BaseTool` for creating llm powered tools. A `WebSearchTool` powered by __DuckDuckGo__ is implemented as an example.
+A base class `BaseTool` for creating llm powered tools. A `BrowserTool` powered by __DuckDuckGo__ is implemented as an example.
 
 ### 9. Chatbot frontend interface
-If you simply want to play with a model, there's a gradio frontend chatbot that allows you to chat with a model with different generation configurations. You can switch between chat histories and prompt format, and you can set your system prompt and other model text generation sampling configurations in the gradio webapp.
+If you simply want to play with a model, there is a streamlit frontend chatbot that allows you to chat with a model with different generation configurations. You can switch between chat histories and prompt format, and you can set your system prompt and other model text generation sampling configurations in the webapp.
 
 ## Using LLMFlex
 
 ### 1. Create LLMs
 This is how you can start with any text generation model on HuggingFace with your machine.
 
 ```python
@@ -132,96 +135,54 @@
 To load an embedding model and use a vector database:
 
 ```python
 from llmflex.Embeddings import HuggingfaceEmbeddingsToolkit
 from llmflex.VectorDBs import FaissVectorDatabase
 
 # Loading the embedding model toolkit
-embeddings = HuggingfaceEmbeddingsToolkit(model_id="thenlper/gte-large")
+embeddings = HuggingfaceEmbeddingsToolkit(model_id="thenlper/gte-small")
 
 # Create a vector database
 food = ["Apple", "Banana", "Pork"]
-vectordb = FaissVectorDatabase.from_texts(index=food, embeddings=embeddings)
+vectordb = FaissVectorDatabase.from_texts(embeddings=embeddings, texts=food)
 
 # Do semantic search on the vector database
 print(vectordb.search("Beef"))
 ```
 
-### 3. Use memory and prompt template to create a chatbot
-Use the Memory classes and the `PromptTemplate` class to create a chatbot.
-```python
-from llmflex.Memory import LongShortTermChatMemory, create_long_short_prompt
-from llmflex.Prompts import PromptTemplate
-
-# Create the memory with the embeddings toolkit created earlier
-memory = LongShortTermChatMemory(title="My first conversation with OpenHermes", embeddings=embeddings, from_exist=False)
-
-# Get a prompt template
-prompt_template = PromptTemplate.from_preset("ChatML")
-
-# Create an llm from the model factory
-chat_llm = model(max_new_tokens=512, stop=prompt_template.stop + ["###"])
-
-# Create the prompt for the llm
-user_input = "What is the meaning of life?"
-prompt = create_long_short_prompt(
-    user_input=user_input,
-    prompt_template=prompt_template,
-    llm=chat_llm,
-    memory=memory
-)
-
-# Generating the response from the model
-output = ""
-for token in chat_llm.stream(prompt):
-    output += token
-    print(token, end="")
-
-# Save the interaction between you and the chatbot
-memory.save_interaction(user_input=user_input, assistant_output=output)
-```
-### 4. Use tools
+### 3. Use tools
 A `WebSearchTool` class is implemented as an example to build a tool with LLMFlex. The tool is using __DuckDuckGo__ by default. Here is how you can use it:
 ```python
-from llmflex.Tools import WebSearchTool
-
-# Create a web search tool with the embeddings toolkit created earlier
-tool = WebSearchTool(embeddings=embeddings, verbose=True)
+from llmflex.Tools import BrowserTool
 
-# Run the tool with the previsous chat memory for a more coherent response
-tool_input = "Can you give me some views of the meaning of life from some famous philosophers?"
-output_generator = tool.run(tool_input, 
-    llm=chat_llm, 
-    history=memory.get_recent_memory(last_k=2), 
-    prompt_template=prompt_template,
-    stream=True)
-
-tool_output = ""
-for token in output_generator:
-    tool_output += token
-    print(token, end="")
+# Create a broswer tool with the embeddings toolkit created earlier
+tool = BrowserTool(embeddings=embeddings)
 
-# And save the response to the memory
-memory = memory.save_interaction(user_input=tool_input, assistant_output=tool_output)
+# Run the tool
+tool(search_query='Install python')
 ```
 
-### 5. Chat with the model in a Streamlit web app
+### 4. Chat with the model in a Streamlit web app
 If you just want a GUI to start chatting with your LLM model with both long term and short term memory, type this command in the terminal:
 ```bash
-llmflex interface --model_id TheBloke/OpenHermes-2.5-Mistral-7B-GGUF --embeddings thenlper/gte-small
+llmflex interface
+```
+If you want to configure the llm model, embedding model, text splitter, and reranker, create a config file and modify it first:
+```bash
+# Create a config file for the webapp
+llmflex create-app-config
 ```
-If you want to chat with the web search tool:
+after modifying the file, run the following:
 ```bash
-# Use a model with longer context for web search
-llmflex interface --model_id TheBloke/OpenHermes-2.5-Mistral-7B-16k-GGUF --embeddings thenlper/gte-small --web_search --extras "model_file='openhermes-2.5-mistral-7b-16k.Q6_K.gguf', context_length=16384"
+llmflex interface --config_dir chatbot_config.yaml
 ```
 You will see a streamlit frontend, use it to chat with the LLM model.  
-![Streamlit GUI](imgs/chat_gui_streamlit.png)
+![Streamlit GUI](imgs/webapp.png)
 
-### 6. Serve an OpenAI API with a GGUF model
+### 5. Serve an OpenAI API with a GGUF model
 To serve a GGUF model with OpenAI API:
 ```bash
 llmflex serve --model_id TheBloke/OpenHermes-2.5-Mistral-7B-GGUF --model_file openhermes-2.5-mistral-7b.Q6_K.gguf --context_size 4096
 ```
 
 ## Documentations
 Python documentation for all the classes, methods, and functions is provided in the `./docs` directory in this repository.
```

### Comparing `llmflex-0.1.7/README.md` & `llmflex-0.1.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -49,18 +49,18 @@
 2. `LongShortTermChatMemory`  
 Memory class using an underlying `VectorDatabase` to maintain long term memory along with the most recent memory.
 
 ### 7. Prompt template
 A `PromptTemplate` class is implemented to format your prompt with different prompt formats for models from different sources. Some presets like `Llama2`, `ChatML`, `Vicuna`, and more are already implemented, but you can alway add your own prompt format template.
 
 ### 8. Custom tools
-A base class `BaseTool` for creating llm powered tools. A `WebSearchTool` powered by __DuckDuckGo__ is implemented as an example.
+A base class `BaseTool` for creating llm powered tools. A `BrowserTool` powered by __DuckDuckGo__ is implemented as an example.
 
 ### 9. Chatbot frontend interface
-If you simply want to play with a model, there's a gradio frontend chatbot that allows you to chat with a model with different generation configurations. You can switch between chat histories and prompt format, and you can set your system prompt and other model text generation sampling configurations in the gradio webapp.
+If you simply want to play with a model, there is a streamlit frontend chatbot that allows you to chat with a model with different generation configurations. You can switch between chat histories and prompt format, and you can set your system prompt and other model text generation sampling configurations in the webapp.
 
 ## Using LLMFlex
 
 ### 1. Create LLMs
 This is how you can start with any text generation model on HuggingFace with your machine.
 
 ```python
@@ -91,96 +91,54 @@
 To load an embedding model and use a vector database:
 
 ```python
 from llmflex.Embeddings import HuggingfaceEmbeddingsToolkit
 from llmflex.VectorDBs import FaissVectorDatabase
 
 # Loading the embedding model toolkit
-embeddings = HuggingfaceEmbeddingsToolkit(model_id="thenlper/gte-large")
+embeddings = HuggingfaceEmbeddingsToolkit(model_id="thenlper/gte-small")
 
 # Create a vector database
 food = ["Apple", "Banana", "Pork"]
-vectordb = FaissVectorDatabase.from_texts(index=food, embeddings=embeddings)
+vectordb = FaissVectorDatabase.from_texts(embeddings=embeddings, texts=food)
 
 # Do semantic search on the vector database
 print(vectordb.search("Beef"))
 ```
 
-### 3. Use memory and prompt template to create a chatbot
-Use the Memory classes and the `PromptTemplate` class to create a chatbot.
-```python
-from llmflex.Memory import LongShortTermChatMemory, create_long_short_prompt
-from llmflex.Prompts import PromptTemplate
-
-# Create the memory with the embeddings toolkit created earlier
-memory = LongShortTermChatMemory(title="My first conversation with OpenHermes", embeddings=embeddings, from_exist=False)
-
-# Get a prompt template
-prompt_template = PromptTemplate.from_preset("ChatML")
-
-# Create an llm from the model factory
-chat_llm = model(max_new_tokens=512, stop=prompt_template.stop + ["###"])
-
-# Create the prompt for the llm
-user_input = "What is the meaning of life?"
-prompt = create_long_short_prompt(
-    user_input=user_input,
-    prompt_template=prompt_template,
-    llm=chat_llm,
-    memory=memory
-)
-
-# Generating the response from the model
-output = ""
-for token in chat_llm.stream(prompt):
-    output += token
-    print(token, end="")
-
-# Save the interaction between you and the chatbot
-memory.save_interaction(user_input=user_input, assistant_output=output)
-```
-### 4. Use tools
+### 3. Use tools
 A `WebSearchTool` class is implemented as an example to build a tool with LLMFlex. The tool is using __DuckDuckGo__ by default. Here is how you can use it:
 ```python
-from llmflex.Tools import WebSearchTool
-
-# Create a web search tool with the embeddings toolkit created earlier
-tool = WebSearchTool(embeddings=embeddings, verbose=True)
+from llmflex.Tools import BrowserTool
 
-# Run the tool with the previsous chat memory for a more coherent response
-tool_input = "Can you give me some views of the meaning of life from some famous philosophers?"
-output_generator = tool.run(tool_input, 
-    llm=chat_llm, 
-    history=memory.get_recent_memory(last_k=2), 
-    prompt_template=prompt_template,
-    stream=True)
-
-tool_output = ""
-for token in output_generator:
-    tool_output += token
-    print(token, end="")
+# Create a broswer tool with the embeddings toolkit created earlier
+tool = BrowserTool(embeddings=embeddings)
 
-# And save the response to the memory
-memory = memory.save_interaction(user_input=tool_input, assistant_output=tool_output)
+# Run the tool
+tool(search_query='Install python')
 ```
 
-### 5. Chat with the model in a Streamlit web app
+### 4. Chat with the model in a Streamlit web app
 If you just want a GUI to start chatting with your LLM model with both long term and short term memory, type this command in the terminal:
 ```bash
-llmflex interface --model_id TheBloke/OpenHermes-2.5-Mistral-7B-GGUF --embeddings thenlper/gte-small
+llmflex interface
+```
+If you want to configure the llm model, embedding model, text splitter, and reranker, create a config file and modify it first:
+```bash
+# Create a config file for the webapp
+llmflex create-app-config
 ```
-If you want to chat with the web search tool:
+after modifying the file, run the following:
 ```bash
-# Use a model with longer context for web search
-llmflex interface --model_id TheBloke/OpenHermes-2.5-Mistral-7B-16k-GGUF --embeddings thenlper/gte-small --web_search --extras "model_file='openhermes-2.5-mistral-7b-16k.Q6_K.gguf', context_length=16384"
+llmflex interface --config_dir chatbot_config.yaml
 ```
 You will see a streamlit frontend, use it to chat with the LLM model.  
-![Streamlit GUI](imgs/chat_gui_streamlit.png)
+![Streamlit GUI](imgs/webapp.png)
 
-### 6. Serve an OpenAI API with a GGUF model
+### 5. Serve an OpenAI API with a GGUF model
 To serve a GGUF model with OpenAI API:
 ```bash
 llmflex serve --model_id TheBloke/OpenHermes-2.5-Mistral-7B-GGUF --model_file openhermes-2.5-mistral-7b.Q6_K.gguf --context_size 4096
 ```
 
 ## Documentations
 Python documentation for all the classes, methods, and functions is provided in the `./docs` directory in this repository.
```

### Comparing `llmflex-0.1.7/pyproject.toml` & `llmflex-0.1.8/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -16,25 +16,28 @@
     "transformers>=4.35.0",
     "accelerate>=0.25.0",
     "sentence-transformers",
     "langchain",
     "faiss-cpu",
     "optimum",
     "gradio>=4.2",
-    "duckduckgo-search>=5.2.2",
+    "duckduckgo-search>=6.1.0",
     "fake-useragent",
     "openai>=1.0.0",
     "tiktoken",
     "protobuf",
     "beautifulsoup4",
     "streamlit",
+    "streamlit-extras",
     "watchdog",
+    "guidance",
     "spacy>=3.7.0",
     "flask",
     "PyMuPDF",
+    "flashrank",
     "python-docx"
 ]
 
 [project.urls]
 Homepage = "https://github.com/nath1295/LLMFlex"
 
 [project.scripts]
```

### Comparing `llmflex-0.1.7/src/llmflex/Embeddings/api_embeddings.py` & `llmflex-0.1.8/src/llmflex/Embeddings/api_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Embeddings/base_embeddings.py` & `llmflex-0.1.8/src/llmflex/Embeddings/base_embeddings.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Embeddings/hf_embeddings_server.py` & `llmflex-0.1.8/src/llmflex/Embeddings/hf_embeddings_server.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Embeddings/huggingface_embeddings.py` & `llmflex-0.1.8/src/llmflex/Embeddings/huggingface_embeddings.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             chunk_size (Optional[int], optional): Chunk size for the text splitter. If not provided, the min of the model max_seq_length or 512 will be used. Defaults to None.
             chunk_overlap_perc (float, optional): Number of tokens percentage overlap during text splitting. Defaults to 0.1.
             model_kwargs (Optional[Dict[str, Any]], optional): Keyword arguments for loading the model. Defaults to None.
             encode_kwargs (Optional[Dict[str, Any]], optional): Keyword arguments for encoding text. If None is given, the default is normalize_embeddings=True, batch_size=128. Defaults to None.
         """
         from ..TextSplitters.token_text_splitter import TokenCountTextSplitter
         from ..Schemas.tokenizer import Tokenizer
-        embedding_model = HuggingFaceEmbeddings(model_name=model_id, model_kwargs=model_kwargs, encode_kwargs=encode_kwargs)
+        embedding_model = HuggingFaceEmbeddings(model_id=model_id, model_kwargs=model_kwargs, encode_kwargs=encode_kwargs)
         name = model_id
         type = 'huggingface_embeddings'
         chunk_size = min(embedding_model._max_seq_length, 512) if not isinstance(chunk_size, int) else chunk_size
         encode_fn = lambda x: embedding_model._tokenizer.encode(x, add_special_tokens=False)
         decode_fn = lambda x: embedding_model._tokenizer.decode(x, skip_special_tokens=True)
         tokenizer = Tokenizer(tokenize_fn=encode_fn, detokenize_fn=decode_fn)
         text_splitter = TokenCountTextSplitter(encode_fn=encode_fn, decode_fn=decode_fn, chunk_overlap=int(chunk_size * chunk_overlap_perc), chunk_size=chunk_size)
```

### Comparing `llmflex-0.1.7/src/llmflex/Frontend/gradio_interface.py` & `llmflex-0.1.8/src/llmflex/Frontend/streamlit_interface.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,575 +1,552 @@
-import os
-from ..Models.Factory.llm_factory import LlmFactory
-from ..Embeddings.base_embeddings import BaseEmbeddingsToolkit
-from typing import Dict, Any, Union, List, Tuple, Type, Iterator
-
-
-class GradioInterface:
-
-    def __init__(self, model: LlmFactory, embeddings: Type[BaseEmbeddingsToolkit]) -> None:
-        from ..Memory.long_short_memory import LongShortTermChatMemory
-        from ..Prompts.prompt_template import DEFAULT_SYSTEM_MESSAGE, PromptTemplate
-        self.model = model
-        self.embeddings = embeddings
-        self.memory = LongShortTermChatMemory(title='Untitled 0', embeddings=self.embeddings, from_exist=False)
-        self.system = DEFAULT_SYSTEM_MESSAGE
-        self.template = self.model.prompt_template
-        self.llm = self.model(stop=self.template.stop + ['###'])
-        self.short_limit = 600
-        self.long_limit = 500
-        self.score_threshold = 0.5
-        self.mobile = False
-        self.bot = dict()
-        self.state = dict(generate=False)
+import streamlit as st
+from streamlit_extras.bottom_container import bottom
+from streamlit_extras.row import row
+from ..Frontend.app_resource import AppBackend
+from ..Memory.base_memory import list_chat_ids, get_title_from_id
+from ..Memory.memory_utils import create_prompt_with_history
+from ..Prompts.prompt_template import presets
+from ..Tools.tool_utils import gen_string
+from ..utils import PACKAGE_DISPLAY_NAME
+from typing import Dict, Any, Literal, Optional, Tuple
+import yaml
+
+DEFAULT_CONFIG = dict(
+    model = dict(
+        model_id = 'NousResearch/Hermes-2-Theta-Llama-3-8B-GGUF',
+        model_type = 'gguf',
+        model_file = 'Hermes-2-Pro-Llama-3-Instruct-Merged-DPO-Q4_K_M.gguf',
+        context_length = 8192
+    ),
+    embeddings = dict(
+        class_name = 'HuggingfaceEmbeddingsToolkit',
+        model_id = 'thenlper/gte-small'
+    ),
+    ranker = dict(
+        class_name = 'FlashrankRanker'
+    ),
+    text_splitter = dict(
+        class_name = 'SentenceTokenTextSplitter',
+        count_token_fn = 'default'
+    ),
+    tools = [
+        dict(
+            class_name = 'BrowserTool',
+            llm = 'default',
+            embeddings = 'default',
+            ranker = 'default'
+        ),
+        dict(
+            class_name = 'math_tool'
+        )
+    ],
+    credentials = None
+)
+
+def create_streamlit_script() -> str:
+    """Create the main script to run the app.
+
+    Returns:
+        str: Script directory.
+    """
+    script = ['from llmflex.Frontend.streamlit_interface import AppInterface']
+    script.append('if __name__ == "__main__":')
+    script.append('\tapp = AppInterface()\n\tapp.run()')
+    script = '\n'.join(script)
+    import os
+    from ..utils import get_config
+    script_dir = os.path.join(get_config()['package_home'], '.streamlit_scripts', 'webapp.py')
+    os.makedirs(os.path.dirname(script_dir), exist_ok=True)
+    with open(script_dir, 'w') as f:
+        f.write(script)
+    return script_dir
+
+@st.cache_resource
+def get_backend() -> AppBackend:
+    """Get the backend object for the webapp.
+
+    Returns:
+        AppBackend: Backend object for the webapp.
+    """
+    from ..utils import get_config
+    import os
+    with open(os.path.join(get_config()['package_home'], '.streamlit_scripts', 'chatbot_config.yaml'), 'r') as f:
+        config = yaml.safe_load(f)
+    return AppBackend(config=config)
+
+class AppInterface:
+
+    def __init__(self) -> None:
+        from ..utils import get_config
+        import os
+        st.set_page_config(layout='wide')
+        self.log_dir = os.path.join(get_config()['package_home'], '.streamlit_scripts', 'logs')
+        os.makedirs(self.log_dir, exist_ok=True)
 
     @property
-    def titles(self) -> List[str]:
-        """All existing chat titles.
+    def credentials(self) -> Optional[Tuple[str, str]]:
+        """Login credentials if provided.
 
         Returns:
-            List[str]: All existing chat titles.
+            Optional[Tuple[str, str]]: Login credentials if provided.
         """
-        from ..Memory.base_memory import list_titles
-        return list_titles()
-    
+        return self.backend.config.get('credentials')
+
     @property
-    def current_title(self) -> str:
-        """Current memory chat title.
+    def is_login(self) -> bool:
+        """Whether it is logged in or not.
 
         Returns:
-            str: Current memory chat title.
+            bool: Whether it is logged in or not.
         """
-        return self.memory.title
-      
+        if not hasattr(st.session_state, 'is_login'):
+            st.session_state.is_login = False if self.credentials is not None else True
+        return st.session_state.is_login
+
     @property
-    def history(self) -> List[List[str]]:
-        """Current conversation history.
+    def backend(self) -> AppBackend:
+        """Backend resources.
 
         Returns:
-            List[List[str]]: Current conversation history.
+            AppBackend: Backend resources.
         """
-        return self.memory.history
-       
+        return get_backend()
+    
     @property
-    def presets(self) -> List[str]:
-        """List of prompt templates presets.
+    def generating(self) -> bool:
+        """Whether text generation in progress.
 
         Returns:
-            List[str]: List of prompt templates presets.
+            bool: Whether text generation in progress.
         """
-        from ..Prompts.prompt_template import presets
-        return list(presets.keys())
-
-    @property
-    def config_dict(self) -> Dict[str, Any]:
-        from ..Prompts.prompt_template import DEFAULT_SYSTEM_MESSAGE
-        config = dict(
-            # conversation list
-            new = dict(obj='textbox', args=dict(value = '', interactive=True, show_label=False, placeholder='New chat title here...', scale=4, container=False)),
-            add = dict(obj='btn', args=dict(value='Add', min_width=15, variant='primary', size='sm', scale=1, interactive=True)),
-            convos = dict(obj='dropdown', args=dict(choices=self.titles, label='Conversations', value=None, container=True)),
-            select = dict(obj='btn', args=dict(value='Select', min_width=25, variant='primary', size='sm', interactive=True)),
-            remove = dict(obj='btn', args=dict(value='Remove', min_width=25, variant='secondary', size='sm', interactive=True)),
-
-            # main console
-            bot = dict(obj='chatbot', args=dict(label=self.current_title, height=600, value=self.history, show_copy_button=True)),
-            user = dict(obj='textbox', args=dict(value = '', interactive=True, show_label=False, placeholder='Type your message here...', max_lines=40, scale=7, container=False)),
-            send = dict(obj='btn', args=dict(value='Send', min_width=35, variant='primary', size='sm', scale=2, interactive=True)),
-            cont = dict(obj='btn', args=dict(value='Continue', min_width=15, size='sm', scale=1, interactive=True)),
-            start = dict(obj='textbox', args=dict(value = '', interactive=True, show_label=False, placeholder='Type the start of the chatbot message...', max_lines=40, scale=7, container=False)),
-            regen = dict(obj='btn', args=dict(value='Retry', min_width=15, size='sm', scale=2, interactive=True)),
-            rmlast = dict(obj='btn', args=dict(value='Undo', min_width=15, size='sm', scale=2, interactive=True)),
-
-            # settings
-            # system settings 
-            system = dict(obj='textbox', args=dict(value=DEFAULT_SYSTEM_MESSAGE, show_label=False, placeholder='System message here...', lines=8, max_lines=40, scale=4, interactive=True)),
-            long_limit = dict(obj='slider', args=dict(value=self.long_limit, minimum=0, maximum=4000, step=1, label='Long term memory tokens limit')),
-            short_limit = dict(obj='slider', args=dict(value=self.short_limit, minimum=0, maximum=6000, step=1, label='Short term memory tokens limit')),
-            sim_score = dict(obj='slider', args=dict(value=self.score_threshold, minimum=0, maximum=1, step=0.01, label='Long term memory relevance score threshold')),
-            sys_save = dict(obj='btn', args=dict(value='Save', min_width=20, variant='secondary', size='sm', scale=2, interactive=True)),
-            sys_log = dict(obj='text', args=dict(show_label=False, value=self.get_memory_settings(), lines=5, container=False)),
-
-            # format settings
-            templates = dict(obj='dropdown', args=dict(choices=self.presets, value=self.template.template_name, show_label=False, interactive=True, container=False)),
-            format_save = dict(obj='btn', args=dict(value='Save', min_width=20, variant='secondary', size='sm', scale=2, interactive=True)),
-            format_log = dict(obj='text', args=dict(show_label=False, value=self.get_prompt_settings(), lines=2, container=False)),
-
-            # LLM settings
-            temperature = dict(obj='slider', args=dict(value=self.llm.generation_config['temperature'], minimum=0, maximum=2, step=0.01, label='Temperature')),
-            tokens = dict(obj='slider', args=dict(value=self.llm.generation_config['max_new_tokens'], minimum=0, maximum=4096, step=1, label='Maximum number of new tokens')),
-            repeat = dict(obj='slider', args=dict(value=self.llm.generation_config['repetition_penalty'], minimum=0, maximum=2, step=0.01, label='Repetition penalty')),
-            topp = dict(obj='slider', args=dict(value=self.llm.generation_config['top_p'], minimum=0, maximum=1, step=0.001, label='Top P')),
-            topk = dict(obj='slider', args=dict(value=self.llm.generation_config['top_k'], minimum=0, maximum=500, step=1, label='Top K')),
-            llm_save = dict(obj='btn', args=dict(value='Save', min_width=20, variant='secondary', size='sm', scale=2, interactive=True)),
-            llm_log = dict(obj='text', args=dict(show_label=False, value=self.get_llm_settings(), lines=6, container=False)),
-        )
-        return config
+        if not hasattr(st.session_state, 'generating'):
+            st.session_state.generating = False
+        return st.session_state.generating
     
     @property
-    def mobile_config_dict(self) -> Dict[str, Any]:
-        from copy import deepcopy
-        config = deepcopy(self.config_dict)
-        changes = dict(
-            bot = dict(height=450, show_copy_button=False),
-            start = dict(scale=4, placeholder='Start of bot message...'),
-            send = dict(scale=1),
-            cont = dict(scale=2)
-        )
-        for k, v in changes.items():
-            for a, i in v.items():
-                config[k]['args'][a] = i
-        return config
-    
-    @property
-    def buttons(self) -> List[str]:
-        """List of buttons except send.
+    def chat_delete_button(self) -> bool:
+        """Whether to show chat deletion buttons.
 
         Returns:
-            List[str]: List of buttons except send.
+            bool: Whether to show chat deletion buttons.
         """
-        btns = []
-        for k, v in self.config_dict.items():
-            if ((v['obj'] == 'btn') & (k != 'send')):
-                btns.append(k)
-        return btns
-
-    def get_memory_settings(self) -> str:
-        settings = [
-            'Current memory settings:',
-            f'System message size: {self.llm.get_num_tokens(self.system)} tokens',
-            f'Long term memory tokens limit: {self.long_limit}',
-            f'Short term memory tokens limit: {self.short_limit}',
-            f'Long term memory relevance score threshold: {self.score_threshold}'
-        ]
-        return '\n'.join(settings)
+        if not hasattr(st.session_state, 'chat_delete_button'):
+            st.session_state.chat_delete_button = False
+        return st.session_state.chat_delete_button
     
-    def get_prompt_settings(self) -> str:
-        settings = [
-            'Current prompt settings:',
-            f'Preset: {self.template.template_name}'
-        ]
-        return '\n'.join(settings)
-    
-    def get_llm_settings(self) -> str:
-        settings = [
-            'Current LLM settings:',
-            f'Temperature: {self.llm.generation_config["temperature"]}',
-            f'Maximum number of new tokens: {self.llm.generation_config["max_new_tokens"]}',
-            f'Repetition penalty: {self.llm.generation_config["repetition_penalty"]}',
-            f'Top P: {self.llm.generation_config["top_p"]}',
-            f'Top K: {self.llm.generation_config["top_k"]}'
-        ]
-        return '\n'.join(settings)
-
-    def get_prompt(self, user_input: str, ai_start: str = '') -> str:
-        from ..Memory.long_short_memory import create_long_short_prompt
-        prompt = create_long_short_prompt(
-            user=user_input,
-            prompt_template=self.template,
-            llm=self.llm,
-            memory=self.memory,
-            system=self.system,
-            short_token_limit=self.short_limit,
-            long_token_limit=self.long_limit,
-            score_threshold=self.score_threshold
-        ) + ai_start.lstrip(' \r\n\t')
-        return prompt
-
-    def change_prompt_format(self, template: str) -> str:
-        """Changing the prompt format.
+    @property
+    def mobile(self) -> bool:
+        """Whether on mobile device.
 
-        Args:
-            template (str): Preset name from the dropdown menu.
+        Returns:
+            bool: Whether on mobile device.
         """
-        from ..Prompts.prompt_template import PromptTemplate
-        self.template = PromptTemplate.from_preset(template)
-        return self.get_prompt_settings()
-
-    def change_memory_setting(self, system: str, long_limit: int, short_limit: int, sim_score: float) -> str:
-        """Changing the system message and memory settings.
-
-        Args:
-            system (str): System textbox.
-            long_limit (int): Long term memory slider.
-            short_limit (int): Short term memory slider.
-            sim_score (float): Similarity score threshold slider.
-        """
-        self.system = system.strip(' \n\r\t')
-        self.memory.vectordb._info['system'] = self.system
-        self.memory.save()
-        self.long_limit = long_limit
-        self.short_limit = short_limit
-        self.score_threshold = sim_score
-        return self.get_memory_settings()
-
-    def change_llm_setting(self, temperature: float, max_tokens: int, repeat_penalty: float, top_p: float, top_k: int) -> str:
-        """Change llm generation settings.
-
-        Args:
-            temperature (float): Temperature of the llm.
-            max_tokens (int): Maximum number of tokens to generate.
-            repeat_penalty (float): Repetition penalty.
-            top_p (float): Top P.
-            top_k (int): Top K.
-        """
-        self.llm = self.model(
-            temperature=temperature,
-            repetition_penalty=repeat_penalty,
-            max_new_tokens=max_tokens,
-            top_p=top_p,
-            top_k=top_k,
-            stop=self.template.stop + ['###']
-            )
-        return self.get_llm_settings()
-
-    def change_memory(self, btn: str, title: str) -> Tuple[Any]:
-        """Handling memory changing settings.
-
-        Args:
-            btn (str): Button that triggered this function.
-            title (str): Title used for this trigger.
+        if not hasattr(st.session_state, 'mobile'):
+            st.session_state.mobile = False
+        return st.session_state.mobile
+    
+    @property
+    def enable_begin_text(self) -> bool:
+        """Whether on mobile device.
 
         Returns:
-            Tuple[Any]: New title textbox, Chats dropdown menu, the Chatbot box, and the system textbox.
+            bool: Whether on mobile device.
         """
-        import gradio as gr
-        from ..Memory.long_short_memory import LongShortTermChatMemory
-        from ..Prompts.prompt_template import DEFAULT_SYSTEM_MESSAGE
-        title = title.strip(' \r\n\t')
-        if ((btn == 'Add') & (title != '') & (title not in self.titles)):
-            self.memory = LongShortTermChatMemory(title=title, embeddings=self.embeddings, from_exist=True)
-        elif ((btn == 'Select') & (title != '') & (title is not None)):
-            from_exist = title != 'Untitled 0'
-            self.memory = LongShortTermChatMemory(title=title, embeddings=self.embeddings, from_exist=from_exist)
-        elif ((btn == 'Remove') & (title != '') & (title is not None)):
-            import shutil
-            if title ==self.current_title:
-                shutil.rmtree(self.memory.chat_dir)
-                self.memory =  LongShortTermChatMemory(title='Untitled 0', embeddings=self.embeddings, from_exist=False)
-            else:
-                mem = LongShortTermChatMemory(title=title, embeddings=self.embeddings, from_exist=False)
-                shutil.rmtree(mem.chat_dir)
-        system = self.memory.info.get('system', DEFAULT_SYSTEM_MESSAGE)
-        self.system = system
-        # Things to return: new, title dropdown, chatbot, system
-        return gr.Textbox(value=''), gr.Dropdown(choices=self.titles, value=None), gr.Chatbot(value=self.history, label=self.current_title), gr.Textbox(value=system, interactive=True), self.get_memory_settings()
-
-    def remove_last(self) -> List[List[str]]:
-        """Removing the last interaction of the conversation.
+        if not hasattr(st.session_state, 'enable_begin_text'):
+            st.session_state.enable_begin_text = False
+        return st.session_state.enable_begin_text
+    
+    @property
+    def begin_text_cache(self) -> str:
+        """Begin text cache.
 
         Returns:
-            List[List[str]]: Conversation history after removing the last interaction.
+            str: Begin text cache.
         """
-        if len(self.history) != 0:
-            self.memory.remove_last_interaction()
-        return self.history
-
-    def input_handler(self, btn: str, user: str, start: str, bot: List[List[str]]) -> Tuple[Any]:
-        """Handling GUI and class attributes before text generation.
+        if not hasattr(st.session_state, 'begin_text_cache'):
+            st.session_state.begin_text_cache = ''
+        return st.session_state.begin_text_cache
 
-        Args:
-            btn (str): Button used to trigger the function.
-            user (str): User input.
-            start (str): Start of the chatbot output, should be an empty string by default.
-            bot (List[List[str]]): Chatbot conversation history.
+    @property
+    def input_config(self) -> Optional[Dict[str, Any]]:
+        """Configuration for text generation if available.
 
         Returns:
-            Tuple[Any]: send button, user input box, conversation box, and all other buttons.
+            Optional[Dict[str, Any]]: Configuration for text generation if available.
         """
-        import gradio as gr
-        user_input = user.strip(' \n\r\t')
-        freeze = True
-        if ((btn == 'Send') & (user != '')):
-            self.state['generate'] = True
-            self.state['prompt'] = self.get_prompt(user_input=user_input, ai_start=start)
-            self.state['start'] = start
-            user = ''
-            bot = self.history + [[user_input, None]]
-        elif((btn == 'Retry') & (len(self.history) != 0)):
-            user_input = self.history[-1][0]
-            self.memory.remove_last_interaction()
-            self.state['generate'] = True
-            self.state['prompt'] = self.get_prompt(user_input=user_input, ai_start=start)
-            self.state['start'] = start
-            bot = self.history + [[user_input, None]]
-        elif((btn == 'Continue') & (len(self.history) != 0)):
-            user_input = self.history[-1][0]
-            ai_start = self.history[-1][1]
-            self.memory.remove_last_interaction()
-            self.state['generate'] = True
-            self.state['prompt'] = self.get_prompt(user_input=user_input, ai_start=ai_start)
-            self.state['start'] = ai_start
-            bot = self.history + [[user_input, None]]
-        elif btn == 'Stop':
-            self.state = dict(generate=False)
-            bot = bot
-        else:
-            freeze = False
-
-        if freeze:
-            returns = [
-                gr.Button(value='Stop', variant='stop'),
-                user,
-                bot,
-            ] + [gr.Button(interactive=False)] * len(self.buttons)
-        else:
-            returns = [
-                gr.Button(value='Send'),
-                user,
-                self.history,
-            ] + [gr.Button(interactive=True)] * len(self.buttons)
-        return tuple(returns)
+        if hasattr(st.session_state, 'input_config'):
+            return st.session_state.input_config
 
-    def generation(self, bot: List[List[str]]) -> Iterator[List[List[str]]]:
-        """Text generation.
+    # Login page
+    def login(self) -> None:
+        """Creating login page.
+        """
+        login_form = st.form(key='login')
+        with login_form:
+            user = st.text_input(label='Username:', placeholder='Your username...')
+            password = st.text_input(label='Password', placeholder='Your password...', type='password')
+            if st.form_submit_button(label='Login'):
+                if ((user == self.credentials[0]) & (password == self.credentials[1])):
+                    st.session_state.is_login = True
+                    st.rerun()
+                else:
+                    st.warning('Incorrect credentials. Please try again.')
 
-        Args:
-            bot (List[List[str]]): Chatbot conversation history.
+    # Sidebar frontend
+    def chats(self) -> None:
+        """Listing all conversations.
+        """
+        st.button(label=':heavy_plus_sign: Start a new conversation', key=f'new_chat', use_container_width=True, on_click=self.backend.create_memory, disabled=self.generating)
+
+        active_chat_id = self.backend.memory.chat_id
+        ids = list_chat_ids()
+
+        def toggle_delete_chats():
+            st.session_state.chat_delete_button = not st.session_state.chat_delete_button
+
+        if self.chat_delete_button:
+            convs = dict()
+            for id in ids:
+                btn_type = 'primary' if id == active_chat_id else 'secondary'
+                real_title = get_title_from_id(id)
+                title = real_title.replace('_', ' ').title()
+                if len(title) > 20:
+                    title = title[:20] + '...'
+                convs[id] = row(spec=[0.8, 0.2])
+                convs[id].button(label=title, key=id, type=btn_type, use_container_width=True, 
+                                 on_click=self.backend.switch_memory, kwargs=dict(chat_id=id), disabled=self.generating, help=real_title)
+                convs[id].button(label=':heavy_minus_sign:', key=f'del_{id}', use_container_width=True, 
+                                 on_click=self.backend.drop_memory, kwargs=dict(chat_id=id), disabled=self.generating)
+        else:
+            for id in ids:
+                btn_type = 'primary' if id == active_chat_id else 'secondary'
+                real_title = get_title_from_id(id)
+                title = real_title.replace('_', ' ').title()
+                if len(title) > 25:
+                    title = title[:25] + '...'
+                st.button(label=title, key=id, type=btn_type, use_container_width=True, 
+                          on_click=self.backend.switch_memory, kwargs=dict(chat_id=id), disabled=self.generating, help=real_title)
+        st.toggle(label=':wastebasket:', key=f'conv_delete', disabled=self.generating, 
+                value=self.chat_delete_button, on_change=toggle_delete_chats, help='Select conversations to remove.')
+
+    def settings(self) -> None:
+        """Creating the settings.
+        """
+        page_dict = {
+            'Prompt Format Settings': self.prompt_format_settings, 
+            'System Message Settings': self.system_message_setttings, 
+            'Memory Settings': self.memory_settings, 
+            'Model Settings': self.model_settings
+            }
+        if self.backend.has_tools:
+            page_dict['Tool Settings'] = self.tool_settings
+        self.mobile_settings()
+        self.begin_text_settings()
+        setting_dropdown = st.selectbox(
+            label = 'Setting dropdown',
+            label_visibility='collapsed',
+            options= list(page_dict.keys())
+        )
+        st.markdown(setting_dropdown + ':')
+        page_dict[setting_dropdown]()
 
-        Returns:
-            List[List[str]]: The updated conversation.
+    def mobile_settings(self) -> None:
+        """Create toggle button for mobile mode.
         """
-        if self.state['generate']:
-            output = self.state['start']
-            prompt = self.state['prompt']
-            print(f'Input tokens: {self.llm.get_num_tokens(prompt)}')
-            for i in self.llm.stream(prompt):
-                if self.state['generate']:
-                    output += i
-                    bot[-1][1] = output.strip(' \r\n\t')
-                    yield bot
-                else:
-                    yield bot
-                    break
-            if bot[-1][1] is None:
-                bot[-1][1] = ''
-            self.memory.save_interaction(bot[-1][0], bot[-1][1])
-            self.state = dict(generate=False)
-            yield bot
-        else:
-            yield bot
+        def toggle_mobile() -> None:
+            st.session_state.mobile = not st.session_state.mobile
+        st.toggle(label='Mobile', value=self.mobile, help='Toggle mobile mode.', on_change=toggle_mobile, disabled=self.generating) 
 
-    def postgen_handler(self) -> List[Any]:
-        """Reactivate all the buttons.
+    def begin_text_settings(self) -> None:
+        """Create toggle button for response starting text.
+        """
+        def toggle_begin_text() -> None:
+            st.session_state.enable_begin_text = not st.session_state.enable_begin_text
+        st.toggle(label='Response Edit', value=self.enable_begin_text, help='Toggle mobile mode.', on_change=toggle_begin_text, disabled=self.generating) 
 
-        Returns:
-            List[Any]: All buttons.
+    def prompt_format_settings(self) -> None:
+        """Prompt format settings.
         """
-        import gradio as gr
-        return [gr.Button(value='Send', variant='primary', interactive=True)] + ([gr.Button(interactive=True)] * len(self.buttons))
+        def set_prompt_template() -> None:
+            if st.session_state.prompt_format in presets.keys():
+                self.backend.set_prompt_template(st.session_state.prompt_format)
+            else:
+                self.backend._prompt_template = self.backend.factory.prompt_template
+        options = list(presets.keys())
+        if self.backend.prompt_template.template_name not in options:
+            options.append(self.backend.prompt_template.template_name)
+        option_index_dict = dict(zip(options, range(len(options))))
+        current_index = option_index_dict.get(self.backend.prompt_template.template_name)
+        prompt_format = st.selectbox(
+            label='prompt_formats', 
+            label_visibility='collapsed',
+            key='prompt_format',
+            options=options, 
+            disabled=self.generating, 
+            index=current_index,
+            on_change=set_prompt_template
+        )
+        if not self.backend.prompt_template.allow_custom_role:
+            st.warning('Current prompt format does not support function calling.')
+        
+    def system_message_setttings(self) -> None:
+        """Create settings for system message.
+        """
+        self.system_text = st.text_area(label='System message', height=250, key='system_msg',label_visibility='collapsed', value=self.backend.memory.system, disabled=self.generating)
+        st.markdown(f'System message token count: {self.backend.llm.get_num_tokens(self.backend.memory.system)}')
+        st.button(label=':floppy_disk:', key='system_save', disabled=self.generating, use_container_width=True, on_click=self.backend.set_system_message, kwargs=dict(system=self.system_text))
+
+    def memory_settings(self) -> None:
+        """Create settings for memory.
+        """
+        self.short_limit_slidder = st.slider('Short term memory token limit', min_value=0, max_value=10000, step=1, 
+                value=self.backend.memory_config['recent_token_limit'], disabled=self.generating)
+        self.long_limit_slidder = st.slider('Long term memory token limit', min_value=0, max_value=6000, step=1, 
+                value=self.backend.memory_config['relevant_token_limit'], disabled=self.generating)
+        self.rel_score_threshold_slidder = st.slider('Relevance score threshold for long term memory', min_value=0.0, max_value=1.0, step=0.01,
+                value=self.backend.memory_config['relevance_score_threshold'], disabled=self.generating)
+        self.sim_score_threshold_slidder = st.slider('Similarity score threshold for long term memory', min_value=0.0, max_value=1.0, step=0.01,
+                value=self.backend.memory_config['similarity_score_threshold'], disabled=self.generating)
+        summary = [
+            'Current settings:',
+            f"Short term memory token limit: {self.backend.memory_config['recent_token_limit']}",
+            f"Long term memory token limit: {self.backend.memory_config['relevant_token_limit']}",
+            f"Relevance score threshold: {self.backend.memory_config['relevance_score_threshold']}",
+            f"Similarity score threshold: {self.backend.memory_config['similarity_score_threshold']}"
 
-    def vars(self, var_name: str, **kwargs: Dict[str, Any]) -> Any:
-        """Generate the gradio component in the config dictionary given the key in the config dict.
+        ]
+        st.markdown('  \n'.join(summary))
+        st.button(label=':floppy_disk:', key='memory_token_save', disabled=self.generating, 
+                  use_container_width=True,
+                  on_click=self.backend.set_memory_config,
+                  kwargs=dict(recent_token_limit=self.short_limit_slidder,
+                              relevant_token_limit=self.long_limit_slidder,
+                              relevance_score_threshold=self.rel_score_threshold_slidder,
+                              similarity_score_threshold=self.sim_score_threshold_slidder))
+
+    def model_settings(self) -> None:
+        """Create settings for text generation.
+        """
+        self.temperature_slidder = st.slider('Temparature', min_value=0.0, max_value=2.0, step=0.01, value=self.backend.generation_config['temperature'], disabled=self.generating)
+        self.max_new_token_slidder = st.slider('Maximum number of new tokens', min_value=0, max_value=4096, step=1, value=self.backend.generation_config['max_new_tokens'], disabled=self.generating)
+        self.repetition_slidder = st.slider('Repetition penalty', min_value=1.0, max_value=2.0, step=0.01, value=self.backend.generation_config['repetition_penalty'], disabled=self.generating)
+        self.topp_slidder = st.slider('Top P', min_value=0.0, max_value=1.0, step=0.01, value=self.backend.generation_config['top_p'], disabled=self.generating)
+        self.topk_slidder = st.slider('Top K', min_value=0, max_value=30000, step=1, value=self.backend.generation_config['top_k'], disabled=self.generating)
+        summary = [
+            'Current settings:',
+            f"Temperature: {self.backend.generation_config['temperature']}",
+            f"Max new tokens: {self.backend.generation_config['max_new_tokens']}",
+            f"Repetition penalty: {self.backend.generation_config['repetition_penalty']}",
+            f"Top P: {self.backend.generation_config['top_p']}",
+            f"Top K: {self.backend.generation_config['top_k']}",
+        ]
+        st.markdown('  \n'.join(summary))
+        st.button(label=':floppy_disk:', 
+                  key='llm_config_save', 
+                  disabled=self.generating, 
+                  use_container_width=True,
+                  on_click=self.backend.set_generation_config,
+                  kwargs=dict(temperature=self.temperature_slidder,
+                              max_new_tokens=self.max_new_token_slidder,
+                              repetition_penalty=self.repetition_slidder,
+                              top_p=self.topp_slidder,
+                              top_k=self.topk_slidder))
+
+    def tool_settings(self) -> None:
+        """Create settings for tools.
+        """
+        for k, v in self.backend.tool_status.items():
+            pretty_name = k.replace('_', ' ').strip().title()
+            st.toggle(label=f'{pretty_name}', value=v, on_change=self.backend.toggle_tool, kwargs=dict(tool_name=k),
+                        disabled=self.generating)
+
+    def sidebar(self) -> None:
+        """Creating the sidebar.
+        """
+        with st.sidebar:
+            app_summary = ['Powered by:', 
+                        f'* LLM: {self.backend.factory.model_id}', 
+                        f'* Embedding model: {self.backend.embeddings.name}', 
+                        '', 
+                        'Current conversation:', 
+                        f'* {self.backend.memory.title}',
+                        '',
+                        'Current prompt format:',
+                        f'* {self.backend.prompt_template.template_name}']
+            st.header(PACKAGE_DISPLAY_NAME.upper(), help='  \n'.join(app_summary), divider="grey")
+            with st.expander(label=':left_speech_bubble: Conversations', expanded=True):
+                self.chats()
+
+            with st.expander(label=':gear: Settings', expanded=False):
+                self.settings()
+
+    # Chatbot frontend
+    def create_input_config(self, user_input: str, begin_text: str, generation_mode: Literal['new', 'retry', 'continue']) -> None:
+        """Create everything needed for the next generation.
 
         Args:
-            var_name (str): Key in the config dict.
+            user_input (str): User request.
+            begin_text (str): Starting text of the response.
+            generation_mode (Literal[&#39;new&#39;, &#39;retry&#39;, &#39;continue&#39;]): Mode of generation.
+        """
+        new_input = user_input.strip()
+        ai_start = begin_text.lstrip()
+        if generation_mode != 'new':
+            last_record = self.backend.memory.history[-1]
+            new_input = last_record[0]
+            if generation_mode == 'continue':
+                ai_start = last_record[1]
+            self.backend.memory.remove_last_interaction()
+        prompt_args = dict(
+            llm=self.backend.llm,
+            memory=self.backend.memory,
+            user_input=new_input,
+            prompt_template=self.backend.prompt_template,
+            system=self.backend.memory.system,
+            recent_token_limit=self.backend.memory_config['recent_token_limit'],
+            relevant_token_limit=self.backend.memory_config['relevant_token_limit'],
+            relevance_score_threshold=self.backend.memory_config['relevance_score_threshold'],
+            similarity_score_threshold=self.backend.memory_config['similarity_score_threshold']
+        )
+        if ai_start.strip() != '':
+            prompt = create_prompt_with_history(**prompt_args) + ai_start
+            st.session_state.begin_text_cache = ai_start
+        elif ((not self.backend.tool_selector.is_empty) & (self.backend.prompt_template.allow_custom_role)):
+            prompt_args['tool_selector'] = self.backend.tool_selector
+            prompt = create_prompt_with_history(**prompt_args)
+        else:
+            prompt = create_prompt_with_history(**prompt_args)
+        
+        st.session_state.input_config = dict(
+            prompt=prompt,
+            user_input=new_input,
+            begin_text=ai_start,
+            mode=generation_mode
+        )
 
-        Returns:
-            Any: The gradio component.
+    def generation_message(self) -> None:
+        """Create streaming message.
         """
-        from copy import deepcopy
-        import gradio as gr
-        keys = ['btn', 'text', 'textbox', 'dropdown', 'chatbot', 'slider']
-        values = [gr.Button, gr.Text, gr.Textbox, gr.Dropdown, gr.Chatbot, gr.Slider]
-        type_map = dict(zip(keys, values))
-        vars = deepcopy(self.mobile_config_dict if self.mobile else self.config_dict)
-
-        output = vars[var_name].copy()
-        for k, v in kwargs.items():
-            output['args'][k] = v
-        output = type_map[output['obj']](**output['args'])
-        return output
-    
-    def output_map(self, keys: Union[str, List[str]]) -> List[Any]:
-        if type(keys) == str:
-            keys = [keys]
-        return list(map(lambda x: self.bot[x], keys))
-    
-    def _init_pc_frame(self) -> None:
-        import gradio as gr
-        with gr.Blocks() as self.frame:
-            with gr.Tab(label='Chat'):
-                with gr.Row():
-                    with gr.Column(): # Conversations
-                        with gr.Group():
-                            with gr.Row(variant='compact'):
-                                self.bot['new'] = self.vars('new')
-                                self.bot['add'] = self.vars('add')
-                            self.bot['convos'] = self.vars('convos')
-                            with gr.Row(variant='compact'):
-                                self.bot['select'] = self.vars('select')
-                                self.bot['remove'] = self.vars('remove')
-                        with gr.Accordion(label='Prompt format settings', open=True):
-                            self.bot['templates'] = self.vars('templates')
-                            self.bot['format_save'] = self.vars('format_save')
-                            self.bot['format_log'] = self.vars('format_log')
-
-                    with gr.Column(scale=4): # Main console
-                        self.bot['bot'] = self.vars('bot')
-                        with gr.Row(variant='compact'):
-                            self.bot['user'] = self.vars('user')
-                            self.bot['send'] = self.vars('send')
-                            self.bot['cont'] = self.vars('cont')
-                        with gr.Row(variant='compact'):
-                            self.bot['start'] = self.vars('start')
-                            self.bot['regen'] = self.vars('regen')
-                            self.bot['rmlast'] = self.vars('rmlast')
-
-            with gr.Tab(label='Settings'): # Settings
-                with gr.Row():
-                    with gr.Column(scale=1):
-                        self.bot['system'] = self.vars('system')
-                        self.bot['long_limit'] = self.vars('long_limit')
-                        self.bot['short_limit'] = self.vars('short_limit')
-                        self.bot['sim_score'] = self.vars('sim_score')
-                        self.bot['sys_save'] = self.vars('sys_save')
-                        self.bot['sys_log'] = self.vars('sys_log')
-                    with gr.Column(scale=1):
-                        self.bot['temperature'] = self.vars('temperature')
-                        self.bot['tokens'] = self.vars('tokens')
-                        self.bot['repeat'] = self.vars('repeat')
-                        self.bot['topp'] = self.vars('topp')
-                        self.bot['topk'] = self.vars('topk')
-                        self.bot['llm_save'] = self.vars('llm_save')
-                        self.bot['llm_log'] = self.vars('llm_log')
-
-
-            # functions
-            self.bot['add'].click(fn=self.change_memory, inputs=self.output_map(['add', 'new']), outputs=self.output_map(['new', 'convos', 'bot', 'system', 'sys_log']))
-            self.bot['select'].click(fn=self.change_memory, inputs=self.output_map(['select', 'convos']), outputs=self.output_map(['new', 'convos', 'bot', 'system', 'sys_log']))
-            self.bot['remove'].click(fn=self.change_memory, inputs=self.output_map(['remove', 'convos']), outputs=self.output_map(['new', 'convos', 'bot', 'system', 'sys_log']))
-
-            self.bot['format_save'].click(fn=self.change_prompt_format, inputs=self.output_map(['templates']), outputs=self.output_map(['format_log']))
-            self.bot['sys_save'].click(fn=self.change_memory_setting, inputs=self.output_map(['system', 'long_limit', 'short_limit', 'sim_score']), outputs=self.output_map(['sys_log']))
-            self.bot['llm_save'].click(fn=self.change_llm_setting, inputs=self.output_map(['temperature', 'tokens', 'repeat', 'topp', 'topk']), outputs=self.output_map(['llm_log']))
-            self.bot['rmlast'].click(fn=self.remove_last, outputs=self.output_map('bot'))
-
-            self.bot['send'].click(fn=self.input_handler, 
-                                   inputs=self.output_map([ 'send', 'user', 'start', 'bot']), 
-                                   outputs=self.output_map(['send', 'user', 'bot'] + self.buttons),
-                                   queue=False).then(
-                                       fn=self.generation, inputs=self.output_map('bot'), outputs=self.output_map('bot')
-                                   ).then(
-                                       fn=self.postgen_handler, outputs=self.output_map(['send'] + self.buttons)
-                                   )
-            self.bot['user'].submit(fn=self.input_handler, 
-                                   inputs=self.output_map([ 'send', 'user', 'start', 'bot']), 
-                                   outputs=self.output_map(['send', 'user', 'bot'] + self.buttons),
-                                   queue=False).then(
-                                       fn=self.generation, inputs=self.output_map('bot'), outputs=self.output_map('bot')
-                                   ).then(
-                                       fn=self.postgen_handler, outputs=self.output_map(['send'] + self.buttons)
-                                   )
-            self.bot['cont'].click(fn=self.input_handler, 
-                                   inputs=self.output_map([ 'cont', 'user', 'start', 'bot']), 
-                                   outputs=self.output_map(['send', 'user', 'bot'] + self.buttons),
-                                   queue=False).then(
-                                       fn=self.generation, inputs=self.output_map('bot'), outputs=self.output_map('bot')
-                                   ).then(
-                                       fn=self.postgen_handler, outputs=self.output_map(['send'] + self.buttons)
-                                   )
-            self.bot['regen'].click(fn=self.input_handler, 
-                                   inputs=self.output_map([ 'regen', 'user', 'start', 'bot']), 
-                                   outputs=self.output_map(['send', 'user', 'bot'] + self.buttons),
-                                   queue=False).then(
-                                       fn=self.generation, inputs=self.output_map('bot'), outputs=self.output_map('bot')
-                                   ).then(
-                                       fn=self.postgen_handler, outputs=self.output_map(['send'] + self.buttons)
-                                   )
-
-    def _init_mobile_frame(self) -> None:
-        import gradio as gr
-        with gr.Blocks() as self.frame:
-            with gr.Tab(label='Chat'):
-                self.bot['bot'] = self.vars('bot')
-                self.bot['user'] = self.vars('user')
-                with gr.Row('compact'):
-                    self.bot['start'] = self.vars('start')
-                    self.bot['send'] = self.vars('send')
-                with gr.Row(variant='compact'):
-                    self.bot['cont'] = self.vars('cont')
-                    self.bot['regen'] = self.vars('regen')
-                    self.bot['rmlast'] = self.vars('rmlast')
-
-            with gr.Tab(label='Conversations'):
-                with gr.Group():
-                    with gr.Row(variant='compact'):
-                        self.bot['new'] = self.vars('new')
-                        self.bot['add'] = self.vars('add')
-                    self.bot['convos'] = self.vars('convos')
-                    with gr.Row(variant='compact'):
-                        self.bot['select'] = self.vars('select')
-                        self.bot['remove'] = self.vars('remove')
-                with gr.Accordion(label='Prompt format settings', open=True):
-                    self.bot['templates'] = self.vars('templates')
-                    self.bot['format_save'] = self.vars('format_save')
-                    self.bot['format_log'] = self.vars('format_log')
-
-
-            with gr.Tab(label='Settings'): # Settings
-                with gr.Accordion('System and memory settings', open=True):
-                    self.bot['system'] = self.vars('system')
-                    self.bot['long_limit'] = self.vars('long_limit')
-                    self.bot['short_limit'] = self.vars('short_limit')
-                    self.bot['sim_score'] = self.vars('sim_score')
-                    self.bot['sys_save'] = self.vars('sys_save')
-                    self.bot['sys_log'] = self.vars('sys_log')
-                with gr.Accordion('LLM settings', open=True):
-                    self.bot['temperature'] = self.vars('temperature')
-                    self.bot['tokens'] = self.vars('tokens')
-                    self.bot['repeat'] = self.vars('repeat')
-                    self.bot['topp'] = self.vars('topp')
-                    self.bot['topk'] = self.vars('topk')
-                    self.bot['llm_save'] = self.vars('llm_save')
-                    self.bot['llm_log'] = self.vars('llm_log')
-
-
-            # functions
-            self.bot['add'].click(fn=self.change_memory, inputs=self.output_map(['add', 'new']), outputs=self.output_map(['new', 'convos', 'bot', 'system', 'sys_log']))
-            self.bot['select'].click(fn=self.change_memory, inputs=self.output_map(['select', 'convos']), outputs=self.output_map(['new', 'convos', 'bot', 'system', 'sys_log']))
-            self.bot['remove'].click(fn=self.change_memory, inputs=self.output_map(['remove', 'convos']), outputs=self.output_map(['new', 'convos', 'bot', 'system', 'sys_log']))
-
-            self.bot['format_save'].click(fn=self.change_prompt_format, inputs=self.output_map(['templates']), outputs=self.output_map(['format_log']))
-            self.bot['sys_save'].click(fn=self.change_memory_setting, inputs=self.output_map(['system', 'long_limit', 'short_limit', 'sim_score']), outputs=self.output_map(['sys_log']))
-            self.bot['llm_save'].click(fn=self.change_llm_setting, inputs=self.output_map(['temperature', 'tokens', 'repeat', 'topp', 'topk']), outputs=self.output_map(['llm_log']))
-            self.bot['rmlast'].click(fn=self.remove_last, outputs=self.output_map('bot'))
-
-            self.bot['send'].click(fn=self.input_handler, 
-                                   inputs=self.output_map([ 'send', 'user', 'start', 'bot']), 
-                                   outputs=self.output_map(['send', 'user', 'bot'] + self.buttons),
-                                   queue=False).then(
-                                       fn=self.generation, inputs=self.output_map('bot'), outputs=self.output_map('bot')
-                                   ).then(
-                                       fn=self.postgen_handler, outputs=self.output_map(['send'] + self.buttons)
-                                   )
-            self.bot['cont'].click(fn=self.input_handler, 
-                                   inputs=self.output_map([ 'cont', 'user', 'start', 'bot']), 
-                                   outputs=self.output_map(['send', 'user', 'bot'] + self.buttons),
-                                   queue=False).then(
-                                       fn=self.generation, inputs=self.output_map('bot'), outputs=self.output_map('bot')
-                                   ).then(
-                                       fn=self.postgen_handler, outputs=self.output_map(['send'] + self.buttons)
-                                   )
-            self.bot['regen'].click(fn=self.input_handler, 
-                                   inputs=self.output_map([ 'regen', 'user', 'start', 'bot']), 
-                                   outputs=self.output_map(['send', 'user', 'bot'] + self.buttons),
-                                   queue=False).then(
-                                       fn=self.generation, inputs=self.output_map('bot'), outputs=self.output_map('bot')
-                                   ).then(
-                                       fn=self.postgen_handler, outputs=self.output_map(['send'] + self.buttons)
-                                   )
-
-
-
-    def launch(self, mobile: bool = False, **kwargs) -> None:
-        if mobile:
-            self.mobile = True
-            default_config = dict(inbrowser=False, share=False, auth=None)
-            default_config.update(kwargs)
-            self._init_mobile_frame()
-        else:
-            default_config = dict(inbrowser=True, share=False, auth=None)
-            default_config.update(kwargs)
-            self._init_pc_frame()
-        self.frame.launch(**default_config)
+        import json
+        if self.input_config is not None:
+            import os
+            from ..utils import current_time, save_json
+            logfilename = os.path.join(self.log_dir, f'{self.backend.memory.chat_id}_{current_time()}.json')
+            save_json(content=self.input_config, file_dir=logfilename)
+            with st.chat_message(name='user'):
+                st.markdown(self.input_config['user_input'])
+            with st.chat_message(name='assistant'):
+                with st.spinner('Thinking....'):
+                    prompt = self.input_config['prompt']
+                    begin_text = self.input_config['begin_text']
+                    save_args = dict()
+                    if not isinstance(prompt, str):
+                        tool_input = self.backend.tool_selector.tool_call_input(llm=self.backend.llm, messages=prompt, prompt_template=self.backend.prompt_template, **self.backend.generation_config)
+                        if tool_input['name'] == 'direct_response':
+                            prompt = self.backend.prompt_template.create_custom_prompt(messages=prompt) + begin_text
+                        else:
+                            toolholder = st.empty()
+                            tool_name = tool_input['name'].replace('_', ' ').title().strip()
+                            with toolholder.status(label=f":hammer_and_pick: Running __{tool_name}__...", state='running'):
+                                st.text(json.dumps(tool_input, indent=4))
+                                tool_output = self.backend.tool_selector.tool_call_output(tool_input=tool_input, return_error=True)
+                                save_args['function_call'] = tool_output
+                            with toolholder.status(label=f":hammer_and_pick: __{tool_name}__", state='complete'):
+                                st.text(json.dumps(tool_output, indent=4))
+                            prompt.append(dict(role='function_call', content=str(tool_output)))
+                            prompt = self.backend.prompt_template.create_custom_prompt(messages=prompt) + begin_text
+                    placeholder = st.empty()
+                    streamer = self.backend.llm.stream(prompt, stop=self.backend.prompt_template.stop, **self.backend.generation_config)
+                    output = begin_text
+                    placeholder.markdown(output.strip(' \r\n\t'))
+                    for i in streamer:
+                        output += i
+                        placeholder.markdown(output.strip(' \r\n\t'))
+                    self.backend.memory.save_interaction(user_input=self.input_config['user_input'], assistant_output=output, **save_args)
+
+                    # Change title if the title is New Chat
+                    if self.backend.memory.title == 'New Chat':
+                        pref = '\n\nNote: This is the short title of this conversation: {"title": '
+                        title = gen_string(self.backend.llm, prompt=prompt + output + pref, max_new_tokens=30)
+                        if title != 'New Chat':
+                            self.backend.memory.update_title(title)
+                    st.session_state.input_config = None
+                    st.session_state.generating = False
+                    st.rerun()
+
+    def historical_conversation(self) -> None:
+        """Creating the historical conversation.
+        """
+        import json
+        history = self.backend.memory.history_dict
+        for message in history:
+            with st.chat_message(name=message['role']):
+                fn_call = message.get('function_call')
+                content = message['content']
+                if fn_call is not None:
+                    fn_name = fn_call['name'].replace('_', ' ').strip().title()
+                    with st.status(label=f":hammer_and_pick: __{fn_name}__", state='complete'):
+                        st.code(json.dumps(fn_call, indent=4), language='plaintext')
+                    if fn_call.get('output', dict()).get('footnote') is not None:
+                        footnote = fn_call.get('output', dict()).get('footnote')
+                        if isinstance(footnote, list):
+                            footnote = '  \n'.join(footnote)
+                        else:
+                            footnote = str(footnote)
+                        content += '\n\n---\n' + footnote
+                st.markdown(content, help=f'Number of tokens: {self.backend.llm.get_num_tokens(message["content"])}')
+        self.generation_message()
+
+    def util_buttons(self) -> None:
+        """Create utility buttons for text generation.
+        """
+        def retry_response(mode):
+            if self.backend.memory.interaction_count != 0:
+                self.create_input_config(user_input='sample', begin_text=self.begin_text, generation_mode=mode)
+                st.session_state.generating = True
+
+        btns = row([1, 1, 1])
+        btns.button(':arrows_counterclockwise:', use_container_width=True, help='Re-generate response', disabled=self.generating, 
+                      on_click=retry_response, kwargs=dict(mode='retry'))
+
+        btns.button(':fast_forward:', use_container_width=True, help='Continue generating response', disabled=self.generating,
+                      on_click=retry_response, kwargs=dict(mode='retry'))
+
+        btns.button(':wastebasket:', use_container_width=True, help='Remove the latest question and response', disabled=self.generating, 
+                       on_click=self.backend.memory.remove_last_interaction)
+
+    def input_box(self) -> None:
+        """Creating the input box.
+        """
+        with bottom():
+            self.user_input = st.chat_input(placeholder='Your message...', disabled=self.generating)
+            if self.enable_begin_text:
+                self.begin_text = st.text_area(label='response_start', placeholder='Starting text of the response here...', value=self.begin_text_cache, label_visibility='collapsed')
+            else:
+                self.begin_text = ''
 
+            if self.user_input:
+                if self.user_input.strip() != '':
+                    self.create_input_config(user_input=self.user_input, begin_text=self.begin_text, generation_mode='new')
+                    st.session_state.generating = True
+                    st.rerun()
+
+            if self.mobile:
+                with st.expander(':gear: Extra options'):
+                    self.util_buttons()
+            else:
+                self.util_buttons()
+            
+    def chatbot(self) -> None:
+        """Creating the chatbot interface.
+        """
+        self.historical_conversation()
+        self.input_box()
+
+    def run(self) -> None:
+        """Run the app.
+        """
+        if self.is_login:
+            self.sidebar()
+            self.chatbot()
+        else:
+            self.login()
```

### Comparing `llmflex-0.1.7/src/llmflex/KnowledgeBase/knowledge_base.py` & `llmflex-0.1.8/src/llmflex/KnowledgeBase/knowledge_base.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Memory/base_memory.py` & `llmflex-0.1.8/src/llmflex/Frontend/app_resource.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,324 +1,334 @@
-import os
-from ..utils import get_config
+from ..Models.Factory.llm_factory import LlmFactory
 from ..Models.Cores.base_core import BaseLLM
-from ..Prompts.prompt_template import DEFAULT_SYSTEM_MESSAGE, PromptTemplate
-from ..KnowledgeBase.knowledge_base import KnowledgeBase
-from typing import List, Dict, Any, Type, Tuple, Optional
+from ..Embeddings.base_embeddings import BaseEmbeddingsToolkit
+from ..TextSplitters.base_text_splitter import BaseTextSplitter
+from ..Rankers.base_ranker import BaseRanker
+from ..Tools.tool_utils import BaseTool, ToolSelector, normalise_tool_name
+from ..Prompts.prompt_template import presets, PromptTemplate
+from ..Memory.long_short_memory import LongShortTermChatMemory
+from ..Memory.base_memory import list_titles, list_chat_ids, get_new_chat_id, get_title_from_id, get_dir_from_id
+from typing import List, Type, Dict, Any, Union, Optional
 
-
-def chat_memory_home() -> str:
-    """Return the default directory for saving chat memories.
-
-    Returns:
-        str: The default directory for saving chat memories.
-    """
-    history_dir = os.path.join(get_config()['package_home'], 'chat_memories')
-    os.makedirs(history_dir, exist_ok=True)
-    return history_dir
-
-def list_chat_dirs() -> List[str]:
-    """List the directories of all chat memories.
-
-    Returns:
-        List[str]: List of directories of all chat memories.
+class AppBackend:
+    """Resources for the App to share.
     """
-    chats_dir = chat_memory_home()
-    dirs = list(map(lambda x: os.path.join(chats_dir, x), os.listdir(chats_dir)))
-    dirs = list(filter(lambda x: os.path.basename(x).startswith('chat_'), dirs))
-    dirs = list(filter(lambda x: ((os.path.isdir(x)) & ('info.json' in os.listdir(x))), dirs))
-    return dirs
-
-def title_dir_map() -> Dict[str, str]:
-    """Return a dictionary with chat titles as keys and their respective directories as values.
-
-    Returns:
-        Dict[str, str]: A dictionary with chat titles as keys and their respective directories as values.
-    """
-    from ..utils import read_json
-    dirs = list_chat_dirs()
-    titles = list(map(lambda x: read_json(os.path.join(x, 'info.json'))['title'], dirs))
-    return dict(zip(titles, dirs))
+    def __init__(self, config: Dict[str, Any]) -> None:
+        """Initialise the backend resourses.
+        Args:
+            config (Dict[str, Any]): Configuration of all the resources.
+        """
+        self._config = config
+        self._init_llm_factory()
+        self._init_ranker()
+        self._init_text_splitter()
+        self._init_embeddings()
+        self._init_tools()
+        
+    @property
+    def config(self) -> Dict[str, Any]:
+        """Configuration of all the resources.ry_
 
-def list_titles() -> List[str]:
-    """Return a list of chat titles.
+        Returns:
+            Dict[str, Any]: Configuration of all the resources.
+        """
+        return self._config
+    
+    @property
+    def factory(self) -> LlmFactory:
+        """LLM factory.
 
-    Returns:
-        List[str]: List of chat titles, sorted by last update descendingly.
-    """
-    from ..utils import read_json
-    mapper = list(title_dir_map().items())
-    mapper = list(map(lambda x: (x[0], read_json(os.path.join(x[1], 'info.json'))['last_update']), mapper))
-    mapper.sort(key=lambda x: x[1], reverse=True)
-    return list(map(lambda x: x[0], mapper))   
+        Returns:
+            LlmFactory: LLM factory.
+        """
+        return self._factory
+    
+    @property
+    def llm(self) -> BaseLLM:
+        """LLM.
 
-class BaseChatMemory:
-    """Base class for chat memory.
-    """
-    def __init__(self, title: str, from_exist: bool = True, system: Optional[str] = None) -> None:
-        """Initialising the memory class.
+        Returns:
+            BaseLLM: LLM.
+        """
+        if not hasattr(self, '_llm'):
+            self._llm = self.factory()
+        return self._llm
+    
+    @property
+    def ranker(self) -> BaseRanker:
+        """Reranker.
 
-        Args:
-            title (str): Title of the chat.
-            from_exist (bool, optional): Initialising the chat memory from existing files if the title exists. Defaults to True.
-            system (Optional[str], optional): System message for the chat. If None is given, the default system message or the stored system message will be used. Defaults to None.
+        Returns:
+            BaseRanker: Reranker.
         """
-        title = title.strip(' \n\r\t')
-        if title == '':
-            raise ValueError('Chat title cannot be an empty string.')
-        self._title = title
-        self._init_memory(from_exist=from_exist)
-        self.info['system'] = system.strip() if system is not None else self.info.get('system', DEFAULT_SYSTEM_MESSAGE)
-        self.save()
+        return self._ranker
+    
+    @property
+    def text_splitter(self) -> BaseTextSplitter:
+        """Text splitter.
 
+        Returns:
+            BaseTextSplitter: Text splitter.
+        """
+        return self._text_splitter
+    
     @property
-    def title(self) -> str:
-        """Chat title.
+    def embeddings(self) -> BaseEmbeddingsToolkit:
+        """Embeddings toolkit.
 
         Returns:
-            str: Chat title.
+            BaseEmbeddingsToolkit: Embeddings toolkit.
         """
-        return self._title
+        return self._embeddings
     
     @property
-    def chat_dir(self) -> str:
-        """Directory of the chat.
+    def tool_selector(self) -> ToolSelector:
+        """Tool selector.
 
         Returns:
-            str: Directory of the chat.
+            ToolSelector: Tool selector.
         """
-        mapper = title_dir_map()
-        if hasattr(self, '_chat_dir'):
-            return self._chat_dir
-        elif self.title in list(mapper.keys()):
-            self._chat_dir = mapper[self.title]
-            return self._chat_dir
-        elif len(list(mapper.keys())) == 0:
-            self._chat_dir = os.path.join(chat_memory_home(), 'chat_0')
-            os.makedirs(self._chat_dir, exist_ok=True)
-            return self._chat_dir
-        else:
-            dirs = list(mapper.values())
-            new = max(list(map(lambda x: int(os.path.basename(x).removeprefix('chat_')), dirs))) + 1
-            self._chat_dir = os.path.join(chat_memory_home(), f'chat_{new}')
-            os.makedirs(self._chat_dir, exist_ok=True)
-            return self._chat_dir
+        return self._tool_selector
     
     @property
-    def info(self) -> Dict[str, Any]:
-        """Information of the chat.
+    def prompt_template(self) -> PromptTemplate:
+        """Prompt template.
 
         Returns:
-            Dict[str, Any]: Information of the chat.
+            PromptTemplate: Prompt template.
         """
-        if hasattr(self, '_info'):
-            return self._info
-        elif 'info.json' in os.listdir(self.chat_dir):
-            from ..utils import read_json
-            self._info = read_json(os.path.join(self.chat_dir, 'info.json'))
-            return self._info
-        else:
-            from ..utils import save_json, current_time
-            self._info = dict(title=self.title, last_update=current_time())
-            save_json(self._info, os.path.join(self.chat_dir, 'info.json'))
-            return self._info
+        if not hasattr(self, '_prompt_template'):
+            self._prompt_template = self.factory.prompt_template
+        return self._prompt_template
 
     @property
-    def system(self) -> str:
-        """Default system message of the memory.
+    def memory(self) -> LongShortTermChatMemory:
+        """Current chat memory.
 
         Returns:
-            str: Default system message of the memory.
+            LongShortTermChatMemory: Current chat memory.
         """
-        return self.info.get('system', DEFAULT_SYSTEM_MESSAGE)
-
-    @property    
-    def history(self) -> List[Tuple[str, str]]:
-        """Entire chat history.
+        if not hasattr(self, '_memory'):
+            self.create_memory()
+        return self._memory
+    
+    @property
+    def generation_config(self) -> Dict[str, float]:
+        """Text generation config.
 
         Returns:
-            List[Tuple[str, str]]: Entire chat history.
+            Dict[str, float]: Text generation config.
         """
-        history = list(map(lambda x: [x.metadata['user'], x.metadata['assistant'], x.metadata['order']], self._data.values()))
-        if len(history) == 0:
-            return []
-        count = max(list(map(lambda x: x[2], history))) + 1
-        history = list(map(lambda x: list(filter(lambda y: y[2] == x, history))[0], range(count)))
-        history.sort(key=lambda x: x[2], reverse=False)
-        return list(map(lambda x: tuple(x[:2]), history))
+        if not hasattr(self, '_generation_config'):
+            self._generation_config = dict(
+            temperature = 0.8,
+            max_new_tokens = 1024,
+            top_p  = 0.95,
+            top_k = 40,
+            repetition_penalty = 1.1
+        )
+        return self._generation_config
+
+    @property
+    def memory_config(self) -> Dict[str, float]:
+        if not hasattr(self, '_memory_config'):
+            self._memory_config = dict(
+                recent_token_limit = 600, 
+                relevant_token_limit= 500,
+                relevance_score_threshold = 0.8, 
+                similarity_score_threshold = 0.5
+            )
+        return self._memory_config
 
     @property
-    def interaction_count(self) -> int:
-        """Number of interactions.
+    def tool_status(self) -> Dict[str, bool]:
+        """Whether each tool is on or off.
 
         Returns:
-            int: Number of interactions.
+            Dict[str, bool]: Whether each tool is on or off.
         """
-        return len(self.history)
+        from copy import deepcopy
+        import gc
+        status = deepcopy(self.tool_selector._enabled)
+        status.pop('direct_response')
+        gc.collect()
+        return status
 
-    def _init_memory(self, from_exist: bool = True) -> None:
-        """Method to initialise the components in the memory.
+    @property
+    def has_tools(self) -> bool:
+        """Whether any tools exist in the tool selector.
 
-        Args:
-            from_exist (bool, optional): Whether to initialise from existing files. Defaults to True.
+        Returns:
+            bool: Whether any tools exist in the tool selector.
         """
-        if ((from_exist) & (self.title in list_titles())):
-            import pickle
-            with open(os.path.join(self.chat_dir, 'data.pkl'), 'rb') as f:
-                self._data = pickle.load(f)
-
-        else:
-            self._data = dict()
-            self.save()
-
-    def save(self) -> None:
-        """Save the current state of the memory.
-        """
-        from ..utils import save_json, current_time
-        import pickle
-        self.info
-        self._info['last_update'] = current_time()
-        save_json(self._info, os.path.join(self.chat_dir, 'info.json'))
-        with open(os.path.join(self.chat_dir, 'data.pkl'), 'wb') as f:
-            pickle.dump(self._data, f)
-
-    def update_system_message(self, system: str) -> None:
-        """Update the default system message for the memory.
+        if not hasattr(self, '_has_tools'):
+            self._has_tools = len(self.tool_status) > 0
+        return self._has_tools
 
-        Args:
-            system (str): New system message.
+    def _init_llm_factory(self) -> None:
+        """Initialising the llm factory.
         """
-        self.info['system'] = system.strip()
-        self.save()
+        self._factory = LlmFactory(**self.config['model'])
 
-    def save_interaction(self, user_input: str, assistant_output: str, **kwargs) -> None:
-        """Saving an interaction to the memory.
+    def _init_ranker(self) -> None:
+        """Initialise the reranker.
+        """
+        from .. import Rankers
+        from copy import deepcopy
+        config = deepcopy(self.config.get('ranker', dict(class_name='FlashrankRanker')))
+        class_name = config.pop('class_name', 'FlashrankRanker')
+        rclass = Rankers.__dict__[class_name]
+        self._ranker = rclass(**config)
 
-        Args:
-            user_input (str): User input.
-            assistant_output (str): Chatbot output.
+    def _init_text_splitter(self) -> None:
+        """Initialise the text splitter.
         """
-        from ..Schemas.documents import Document
+        from .. import TextSplitters
         from copy import deepcopy
-        user_input = user_input.strip(' \n\r\t')
-        assistant_output = assistant_output.strip(' \n\r\t')
-        metadata = dict(user=user_input, assistant=assistant_output, order=self.interaction_count)
-        for k, v in kwargs.items():
-            if k not in ['user', 'assistant', 'order', 'role']:
-                metadata[k] = v
-        new_key = max(list(self._data.keys())) + 1 if len(self._data) != 0 else 0
-        meta_user = deepcopy(metadata)
-        meta_user['role'] = 'user'
-        meta_assistant = deepcopy(metadata)
-        meta_assistant['role'] = 'assistant'
-        self._data[new_key] = Document(
-            index=user_input,
-            metadata=meta_user
-        )
-        self._data[new_key + 1] = Document(
-            index=assistant_output,
-            metadata=meta_assistant
-        )
-        self.save()
+        config = deepcopy(self.config.get('text_splitter', dict(class_name='SentenceTokenTextSplitter', count_token_fn='default')))
+        class_name = config.pop('class_name', 'SentenceTokenTextSplitter')
+        if config.get('count_token_fn') == 'default':
+            config['count_token_fn'] = self.llm.get_num_tokens
+        rclass = TextSplitters.__dict__[class_name]
+        self._text_splitter = rclass(**config)      
 
-    def remove_last_interaction(self) -> None:
-        """Remove the latest interaction.
+    def _init_embeddings(self) -> None:
+        """Initialising the embeddings toolkit.
         """
-        if len(self._data) != 0:
-            order = self.interaction_count
-            data = list(filter(lambda x: x.metadata['order'] != order, list(self._data.values())))
-            self._data = dict(zip(range(len(data)), data))
-            self.save()
+        from .. import Embeddings
+        from copy import deepcopy
+        config = deepcopy(self.config.get('embeddings', dict(class_name='HuggingfaceEmbeddingsToolkit', model_id='')))
+        class_name = config.pop('class_name', 'HuggingfaceEmbeddingsToolkit')
+        if ((class_name == 'HuggingfaceEmbeddingsToolkit') & ('model_id' not in config.keys())):
+            config['model_id'] = ''
+        eclass = Embeddings.__dict__[class_name]
+        self._embeddings= eclass(**config)
 
-    def clear(self) -> None:
-        """Empty the whole chat history.
+    def _init_tools(self) -> None:
+        """Initialising tool selector.
         """
-        self._init_memory(from_exist=False)
+        from ..Tools import tool_classes
+        from copy import deepcopy
+        from inspect import isclass
+        config = deepcopy(self.config.get('tools', []))
+        tool_classes =  list(map(lambda x: tool_classes.__dict__.get(x['class_name']), config))
+        tool_names = []
+        tool_instances = []
+        for i, cf in enumerate(config):
+            tclass = tool_classes[i]
+            tool_name = normalise_tool_name(cf.pop('class_name'))
+            if isclass(tclass):
+                if issubclass(tclass, BaseTool):
+                    if cf.get('llm') == 'default':
+                        cf['llm'] = self.llm
+                    if cf.get('embeddings') == 'default':
+                        cf['embeddings'] = self.embeddings
+                    if cf.get('ranker') == 'default':
+                        cf['ranker'] = self.ranker
+                    if cf.get('text_splitter') == 'default':
+                        cf['text_splitter'] = self.text_splitter
+                    if cf.get('count_token_fn') == 'default':
+                        cf['count_token_fn'] = self.llm.get_num_tokens
+                    tool = tclass(**cf)
+                    if tool.name not in tool_names:
+                        tool_instances.append(tool)
+                        tool_names.append(tool.name)
+            elif tool_name not in tool_names:
+                tool_instances.append(tclass)
+                tool_names.append(tool_name)
+        self._tool_selector = ToolSelector(tools=tool_instances)
+        self.tool_selector.turn_off_tools(self.tool_selector.enabled_tools)
 
-    def get_recent_memory(self, k: int = 3) -> List[Tuple[str, str]]:
-        """Get the last k interactions as a list.
+    def switch_memory(self, chat_id: str) -> None:
+        """Switch to the memory given the chat ID.
 
         Args:
-            k (int, optional): Maximum number of latest interactions. Defaults to 3.
-
-        Returns:
-            List[Tuple[str, str]]: List of interactions.
+            chat_id (str): Chat ID.
         """
-        from copy import deepcopy
-        history = self.history
-        results = history if len(history) <= k else history[-k:]
-        return deepcopy(results)
+        if chat_id in list_chat_ids():
+            self._memory = LongShortTermChatMemory(chat_id=chat_id, 
+                    embeddings=self.embeddings, 
+                    llm=self.llm, 
+                    ranker=self.ranker, 
+                    text_splitter=self.text_splitter,
+                    from_exist=True)
+            
+    def create_memory(self) -> None:
+        """Create a new chat memory.
+        """
+        self._memory = LongShortTermChatMemory(chat_id=get_new_chat_id(), 
+                embeddings=self.embeddings, 
+                llm=self.llm, 
+                ranker=self.ranker, 
+                text_splitter=self.text_splitter)
 
-    def get_token_memory(self, llm: Type[BaseLLM], token_limit: int = 400) -> List[str]:
-        """Get the latest conversation limited by number of tokens.
+    def drop_memory(self, chat_id: str) -> None:
+        """Delete the chat memory give the chat ID.
 
         Args:
-            llm (Type[BaseLLM]): LLM to count tokens.
-            token_limit (int, optional): Maximum number of tokens allowed. Defaults to 400.
-
-        Returns:
-            List[str]: List of most recent messages.
+            chat_id (str): Chat ID.
         """
-        if len(self.history) == 0:
-            return []
-        tk_count = 0
-        history = sum(list(map(list, self.history)), [])
-        history = list(reversed(history))
-        results = list()
-        for m in history:
-            msg_count = llm.get_num_tokens(m)
-            if (((msg_count + tk_count) <= token_limit) | (len(results) < 2)):
-                results = [m] + results
-                tk_count += msg_count
-            else:
-                break
-        return results
-    
-    def create_prompt_with_memory(self, user: str, prompt_template: PromptTemplate, llm: Type[BaseLLM],
-            system: Optional[str] = None, recent_token_limit: int = 200, 
-            knowledge_base: Optional[KnowledgeBase] = None, relevance_token_limit: int = 200, relevance_score_threshold: float = 0.8, **kwargs) -> str:
-        """Wrapper function to create full chat prompts using the prompt template given, with long term memory included in the prompt. 
+        import shutil
+        if chat_id in list_chat_ids():
+            if chat_id == self.memory.chat_id:
+                self.create_memory()
+            chat_dir = get_dir_from_id(chat_id=chat_id)
+            shutil.rmtree(chat_dir)
+
+    def set_generation_config(self, temperature: Optional[float] = None, max_new_tokens: Optional[int] = None, 
+                top_p: Optional[float] = None, top_k: Optional[int] = None, repetition_penalty: Optional[float] = None) -> None:
+        """Update the LLM generation config. If None is given to any arguments, the argument will not change.
 
         Args:
-            user (str): User newest message.
-            prompt_template (PromptTemplate): Prompt template to use.
-            llm (Type[BaseLLM]): LLM for counting tokens.
-            system (Optional[str], optional): System message to override the default system message for the memory. Defaults to None.
-            recent_token_limit (int, optional): Maximum number of tokens for recent term memory. Defaults to 200.
-            knowledge_base (Optional[KnowledgeBase]): Knowledge base that helps the assistant to answer questions. Defaults to None.
-            relevance_token_limit (int, optional): Maximum number of tokens for search results from the knowledge base if a knowledge base is given. Defaults to 200.
-            relevance_score_threshold (float, optional): Reranking score threshold for knowledge base search if a knowledge base is given. Defaults to 0.8.
+            temperature (Optional[float], optional): Set how "creative" the model is, the smaller it is, the more static of the output. Defaults to None.
+            max_new_tokens (Optional[int], optional): Maximum number of tokens to generate by the llm. Defaults to None.
+            top_p (Optional[float], optional): While sampling the next token, only consider the tokens above this p value. Defaults to None.
+            top_k (Optional[int], optional): While sampling the next token, only consider the top "top_k" tokens. Defaults to None.
+            repetition_penalty (Optional[float], optional): The value to penalise the model for generating repetitive text. Defaults to None.
+        """
+        args = [temperature, max_new_tokens, top_p, top_k, repetition_penalty]
+        arg_names = ['temperature', 'max_new_tokens', 'top_p', 'top_k', 'repetition_penalty']
+        for i, arg in enumerate(args):
+            if arg is not None:
+                self._generation_config[arg_names[i]] = arg
+
+    def set_memory_config(self, recent_token_limit: Optional[int] = None, relevant_token_limit: Optional[int] = None, 
+                relevance_score_threshold: Optional[float] = None, similarity_score_threshold: Optional[float] = None) -> None:
+        """Update the memory config. If None is given to any arguments, the argument will not change.
 
+        Args:
+        recent_token_limit (Optional[int], optional): Token limit for the most recent conversation history. Defaults to None.
+        relevant_token_limit (Optional[int], optional): Token limit for the relevant contents from older conversation history. Defaults to None.
+        relevance_score_threshold (Optional[float], optional): Score threshold for the reranker for relevant conversation history content extraction. Defaults to None.
+        similarity_score_threshold (Optional[float], optional): Score threshold for the vector database search for relevant conversation history content extraction. Defaults to None.
+        """
+        args = [recent_token_limit, relevant_token_limit, relevance_score_threshold, similarity_score_threshold]
+        arg_names = ['recent_token_limit', 'relevant_token_limit', 'relevance_score_threshold', 'similarity_score_threshold']
+        for i, arg in enumerate(args):
+            if arg is not None:
+                self._memory_config[arg_names[i]] = arg
 
-        Returns:
-            str: The full chat prompt.
-        """
-        user = user.strip()
-        short = self.get_token_memory(llm=llm, token_limit=recent_token_limit)
-        system = self.system if not isinstance(system, str) else system
-        messages: list = [dict(role='system', content=self.system)] + prompt_template.format_history(short, return_list=True)
-        if knowledge_base is not None:
-            res = knowledge_base.search(query=user, token_limit=relevance_token_limit, fetch_k=50, count_fn=llm.get_num_tokens, relevance_score_threshold=relevance_score_threshold)
-            if len(res) != 0:
-                import json
-                res = list(map(lambda x: x.index, res))
-                if prompt_template.allow_custom_role:
-                    res = json.dumps({'Information from knowledge base': res}, indent=4)
-                    messages.extend([dict(role='user', content=user), dict(role='extra information', content=res)])
-                    prompt = prompt_template.create_custom_prompt(messages=messages, add_generation_prompt=True) 
-                else:
-                    messages.append(dict(role='user', content=user))
-                    prompt = prompt_template.create_custom_prompt(messages=messages, add_generation_prompt=True)
-                    res = json.dumps({'Information from knowledge base': res}, indent=4)
-                    prompt += f'{res}\n\nResponse: '
-            else:
-                messages.append(dict(role='user', content=user))
-                prompt = prompt_template.create_custom_prompt(messages=messages, add_generation_prompt=True)    
-        else:
-            messages.append(dict(role='user', content=user))
-            prompt = prompt_template.create_custom_prompt(messages=messages, add_generation_prompt=True)
-        return prompt
+    def set_system_message(self, system: str) -> None:
+        """Update the system message of the current conversation.
 
+        Args:
+            system (str): Update the system message of the current conversation.
+        """
+        self.memory.update_system_message(system=system)
 
+    def set_prompt_template(self, preset: str) -> None:
+        """Updating prompt template.
 
+        Args:
+            preset (str): Preset name of the prompt template.
+        """
+        if preset in presets.keys():
+            self._prompt_template = PromptTemplate.from_preset(style=preset)
 
+    def toggle_tool(self, tool_name: str) -> None:
+        """Toggle the on/off status of the given tool.
 
+        Args:
+            tool_name (str): Tool to toggle.
+        """
+        if tool_name in self.tool_status.keys():
+            self.tool_selector._enabled[tool_name] = not self.tool_selector._enabled[tool_name]
```

### Comparing `llmflex-0.1.7/src/llmflex/Models/Cores/base_core.py` & `llmflex-0.1.8/src/llmflex/Models/Cores/base_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Models/Cores/exllamav2_core.py` & `llmflex-0.1.8/src/llmflex/Models/Cores/exllamav2_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Models/Cores/huggingface_core.py` & `llmflex-0.1.8/src/llmflex/Models/Cores/huggingface_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Models/Cores/llamacpp_core.py` & `llmflex-0.1.8/src/llmflex/Models/Cores/llamacpp_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Models/Cores/openai_core.py` & `llmflex-0.1.8/src/llmflex/Models/Cores/openai_core.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Models/Cores/utils.py` & `llmflex-0.1.8/src/llmflex/Models/Cores/utils.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Models/Factory/llm_factory.py` & `llmflex-0.1.8/src/llmflex/Models/Factory/llm_factory.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Prompts/prompt_template.py` & `llmflex-0.1.8/src/llmflex/Prompts/prompt_template.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Rankers/base_ranker.py` & `llmflex-0.1.8/src/llmflex/Rankers/base_ranker.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Rankers/flashrank_ranker.py` & `llmflex-0.1.8/src/llmflex/Rankers/flashrank_ranker.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Schemas/documents.py` & `llmflex-0.1.8/src/llmflex/Schemas/documents.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Schemas/tokenizer.py` & `llmflex-0.1.8/src/llmflex/Schemas/tokenizer.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/TextSplitters/base_text_splitter.py` & `llmflex-0.1.8/src/llmflex/TextSplitters/base_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/TextSplitters/sentence_token_text_splitter.py` & `llmflex-0.1.8/src/llmflex/TextSplitters/sentence_token_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/TextSplitters/token_text_splitter.py` & `llmflex-0.1.8/src/llmflex/TextSplitters/token_text_splitter.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Tools/base_tool.py` & `llmflex-0.1.8/src/llmflex/Tools/base_tool.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/Tools/browser_tool.py` & `llmflex-0.1.8/src/llmflex/Tools/browser_tool.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,28 +4,37 @@
 from ..Rankers.base_ranker import BaseRanker
 from typing import Optional, Dict, Any, List
 
 class BrowserTool(BaseTool):
     """Tool for browsing contents via the DuckDuckGo search engine given any search query. The output will be the most relevant chunks of content found from the search engine according to the search query.
     """
     def __init__(self, embeddings: BaseEmbeddingsToolkit, llm: Optional[BaseLLM] = None, ranker: Optional[BaseRanker] = None) -> None:
+        """Initialising the tool.
+
+        Args:
+            embeddings (BaseEmbeddingsToolkit): Embeddings toolkit for the vector database.
+            llm (Optional[BaseLLM], optional): LLM to count number of tokens for each chunk. Defaults to None.
+            ranker (Optional[BaseRanker], optional): Reranker to rerank results. If none is given, results will not be reranked after the search on the vector database. Defaults to None.
+        """
         from ..VectorDBs.faiss_vectordb import FaissVectorDatabase
         self.embeddings = embeddings
         self.vdb = FaissVectorDatabase.from_documents(embeddings=self.embeddings, docs=[])
         self.llm = llm
         self.ranker = ranker
+        super().__init__()
 
-    def __call__(self, search_query: str) -> List[Dict[str, str]]:
+    def __call__(self, search_query: str, max_num_results: int = 3) -> Dict[str, List[str]]:
         """Entry point of the tool.
 
         Args:
             search_query (str): Search query to browse on DuckDuckGo.
+            max_num_results (int, optional): Maximum number of relevant chunks of contents from the search results. Defaults to 3.
 
         Returns:
-            List[Dict[str, str]]: The most relevant chunks on contents along with their resepctive URLs.
+            Dict[str, List[str]]: The most relevant chunks on contents along with their resepctive URLs.
         """
         import gc
         from .web_search_utils import ddg_search, get_markdown, create_content_chunks
         from ..Schemas.documents import Document
         results = ddg_search(query=search_query, urls_only=False)
         contents = list(map(lambda x: get_markdown(x['href'], as_list=True), results))
         count_fn = self.llm.get_num_tokens if self.llm is not None else self.embeddings.tokenizer.get_num_tokens
@@ -33,34 +42,25 @@
         for i, c in enumerate(contents):
             if c is not None:
                 doc = create_content_chunks(contents=c, token_count_fn=count_fn)
                 doc = list(map(lambda x: Document(index=x, metadata=results[i]), doc))
                 docs.extend(doc)
         self.vdb.add_documents(docs, split_text=False)
         if self.ranker:
-            chunks = self.vdb.search(query=search_query, top_k=15, index_only=False)
+            chunks = self.vdb.search(query=search_query, top_k=max(int(max_num_results * 2), 15), index_only=False)
             self.vdb.clear()
-            res = self.ranker.rerank(query=search_query, elements=chunks, top_k=3)
-            res = map(lambda x: x.to_dict(), res)
-            chunks = list(map(self._create_chunk, res))
+            res = self.ranker.rerank(query=search_query, elements=chunks, top_k=max_num_results)
+            res = list(map(lambda x: x.to_dict(), res))
+            chunks = list(map(lambda x: x['index'], res))
+            sources = list(set(map(lambda x: x['metadata']['href'], res)))
         else:
-            chunks = self.vdb.search(query=search_query, top_k=3, index_only=False)
+            chunks = self.vdb.search(query=search_query, top_k=max_num_results, index_only=False)
             self.vdb.clear()
             res = chunks.copy()
-            chunks = list(map(self._create_chunk, res))
+            chunks = list(map(lambda x: x['index'], res))
+            sources = list(set(map(lambda x: x['metadata']['href'], res)))
         gc.collect()
-        return chunks
+        output = dict(relevant_contents=chunks, footnote=sources)
+        return output
     
-    def _create_chunk(self, result: Dict[str, Any]) -> Dict[str, str]:
-        """Formatting a content chunk into a dictionary.
 
-        Args:
-            result (Dict[str, Any]): Dictionary of the original search result.
-
-        Returns:
-            Dict[str, str]: Formatted dictionary of the search result.
-        """
-        return dict(
-            chunk_content=result['index'], 
-            source=result['metadata']['href']
-        )
```

### Comparing `llmflex-0.1.7/src/llmflex/Tools/web_search_utils.py` & `llmflex-0.1.8/src/llmflex/Tools/web_search_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,14 +363,15 @@
             continue
         elif len(o) < 3: # Remove random elements with less than 3 characters.
             continue
         else:
             final.append(o)
     if len(final) == 0:
         return None
+    final = list(filter(lambda x: x is not None, final))
     if as_list:
         return final
     else:
         final = list(map(lambda x: x + end, final))
         return sep.join(final)
     
 def create_content_chunks(contents: Optional[List[str]], token_count_fn: Callable[[str], int], chunk_size: int = 400) -> List[str]:
```

### Comparing `llmflex-0.1.7/src/llmflex/VectorDBs/base_vectordb.py` & `llmflex-0.1.8/src/llmflex/VectorDBs/base_vectordb.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/VectorDBs/faiss_vectordb.py` & `llmflex-0.1.8/src/llmflex/VectorDBs/faiss_vectordb.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex/utils.py` & `llmflex-0.1.8/src/llmflex/utils.py`

 * *Files identical despite different names*

### Comparing `llmflex-0.1.7/src/llmflex.egg-info/PKG-INFO` & `llmflex-0.1.8/src/llmflex.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmflex
-Version: 0.1.7
+Version: 0.1.8
 Summary: A python package for developing AI applications with local LLMs.
 Author-email: Nathan Tam <nathan1295@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/nath1295/LLMFlex
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -14,25 +14,28 @@
 Requires-Dist: transformers>=4.35.0
 Requires-Dist: accelerate>=0.25.0
 Requires-Dist: sentence-transformers
 Requires-Dist: langchain
 Requires-Dist: faiss-cpu
 Requires-Dist: optimum
 Requires-Dist: gradio>=4.2
-Requires-Dist: duckduckgo-search>=5.2.2
+Requires-Dist: duckduckgo-search>=6.1.0
 Requires-Dist: fake-useragent
 Requires-Dist: openai>=1.0.0
 Requires-Dist: tiktoken
 Requires-Dist: protobuf
 Requires-Dist: beautifulsoup4
 Requires-Dist: streamlit
+Requires-Dist: streamlit-extras
 Requires-Dist: watchdog
+Requires-Dist: guidance
 Requires-Dist: spacy>=3.7.0
 Requires-Dist: flask
 Requires-Dist: PyMuPDF
+Requires-Dist: flashrank
 Requires-Dist: python-docx
 Provides-Extra: cu121
 Requires-Dist: auto-gptq>=0.6.0; extra == "cu121"
 Requires-Dist: autoawq; extra == "cu121"
 Requires-Dist: exllamav2; extra == "cu121"
 Provides-Extra: cu118
 Requires-Dist: auto-gptq; extra == "cu118"
@@ -90,18 +93,18 @@
 2. `LongShortTermChatMemory`  
 Memory class using an underlying `VectorDatabase` to maintain long term memory along with the most recent memory.
 
 ### 7. Prompt template
 A `PromptTemplate` class is implemented to format your prompt with different prompt formats for models from different sources. Some presets like `Llama2`, `ChatML`, `Vicuna`, and more are already implemented, but you can alway add your own prompt format template.
 
 ### 8. Custom tools
-A base class `BaseTool` for creating llm powered tools. A `WebSearchTool` powered by __DuckDuckGo__ is implemented as an example.
+A base class `BaseTool` for creating llm powered tools. A `BrowserTool` powered by __DuckDuckGo__ is implemented as an example.
 
 ### 9. Chatbot frontend interface
-If you simply want to play with a model, there's a gradio frontend chatbot that allows you to chat with a model with different generation configurations. You can switch between chat histories and prompt format, and you can set your system prompt and other model text generation sampling configurations in the gradio webapp.
+If you simply want to play with a model, there is a streamlit frontend chatbot that allows you to chat with a model with different generation configurations. You can switch between chat histories and prompt format, and you can set your system prompt and other model text generation sampling configurations in the webapp.
 
 ## Using LLMFlex
 
 ### 1. Create LLMs
 This is how you can start with any text generation model on HuggingFace with your machine.
 
 ```python
@@ -132,96 +135,54 @@
 To load an embedding model and use a vector database:
 
 ```python
 from llmflex.Embeddings import HuggingfaceEmbeddingsToolkit
 from llmflex.VectorDBs import FaissVectorDatabase
 
 # Loading the embedding model toolkit
-embeddings = HuggingfaceEmbeddingsToolkit(model_id="thenlper/gte-large")
+embeddings = HuggingfaceEmbeddingsToolkit(model_id="thenlper/gte-small")
 
 # Create a vector database
 food = ["Apple", "Banana", "Pork"]
-vectordb = FaissVectorDatabase.from_texts(index=food, embeddings=embeddings)
+vectordb = FaissVectorDatabase.from_texts(embeddings=embeddings, texts=food)
 
 # Do semantic search on the vector database
 print(vectordb.search("Beef"))
 ```
 
-### 3. Use memory and prompt template to create a chatbot
-Use the Memory classes and the `PromptTemplate` class to create a chatbot.
-```python
-from llmflex.Memory import LongShortTermChatMemory, create_long_short_prompt
-from llmflex.Prompts import PromptTemplate
-
-# Create the memory with the embeddings toolkit created earlier
-memory = LongShortTermChatMemory(title="My first conversation with OpenHermes", embeddings=embeddings, from_exist=False)
-
-# Get a prompt template
-prompt_template = PromptTemplate.from_preset("ChatML")
-
-# Create an llm from the model factory
-chat_llm = model(max_new_tokens=512, stop=prompt_template.stop + ["###"])
-
-# Create the prompt for the llm
-user_input = "What is the meaning of life?"
-prompt = create_long_short_prompt(
-    user_input=user_input,
-    prompt_template=prompt_template,
-    llm=chat_llm,
-    memory=memory
-)
-
-# Generating the response from the model
-output = ""
-for token in chat_llm.stream(prompt):
-    output += token
-    print(token, end="")
-
-# Save the interaction between you and the chatbot
-memory.save_interaction(user_input=user_input, assistant_output=output)
-```
-### 4. Use tools
+### 3. Use tools
 A `WebSearchTool` class is implemented as an example to build a tool with LLMFlex. The tool is using __DuckDuckGo__ by default. Here is how you can use it:
 ```python
-from llmflex.Tools import WebSearchTool
-
-# Create a web search tool with the embeddings toolkit created earlier
-tool = WebSearchTool(embeddings=embeddings, verbose=True)
+from llmflex.Tools import BrowserTool
 
-# Run the tool with the previsous chat memory for a more coherent response
-tool_input = "Can you give me some views of the meaning of life from some famous philosophers?"
-output_generator = tool.run(tool_input, 
-    llm=chat_llm, 
-    history=memory.get_recent_memory(last_k=2), 
-    prompt_template=prompt_template,
-    stream=True)
-
-tool_output = ""
-for token in output_generator:
-    tool_output += token
-    print(token, end="")
+# Create a broswer tool with the embeddings toolkit created earlier
+tool = BrowserTool(embeddings=embeddings)
 
-# And save the response to the memory
-memory = memory.save_interaction(user_input=tool_input, assistant_output=tool_output)
+# Run the tool
+tool(search_query='Install python')
 ```
 
-### 5. Chat with the model in a Streamlit web app
+### 4. Chat with the model in a Streamlit web app
 If you just want a GUI to start chatting with your LLM model with both long term and short term memory, type this command in the terminal:
 ```bash
-llmflex interface --model_id TheBloke/OpenHermes-2.5-Mistral-7B-GGUF --embeddings thenlper/gte-small
+llmflex interface
+```
+If you want to configure the llm model, embedding model, text splitter, and reranker, create a config file and modify it first:
+```bash
+# Create a config file for the webapp
+llmflex create-app-config
 ```
-If you want to chat with the web search tool:
+after modifying the file, run the following:
 ```bash
-# Use a model with longer context for web search
-llmflex interface --model_id TheBloke/OpenHermes-2.5-Mistral-7B-16k-GGUF --embeddings thenlper/gte-small --web_search --extras "model_file='openhermes-2.5-mistral-7b-16k.Q6_K.gguf', context_length=16384"
+llmflex interface --config_dir chatbot_config.yaml
 ```
 You will see a streamlit frontend, use it to chat with the LLM model.  
-![Streamlit GUI](imgs/chat_gui_streamlit.png)
+![Streamlit GUI](imgs/webapp.png)
 
-### 6. Serve an OpenAI API with a GGUF model
+### 5. Serve an OpenAI API with a GGUF model
 To serve a GGUF model with OpenAI API:
 ```bash
 llmflex serve --model_id TheBloke/OpenHermes-2.5-Mistral-7B-GGUF --model_file openhermes-2.5-mistral-7b.Q6_K.gguf --context_size 4096
 ```
 
 ## Documentations
 Python documentation for all the classes, methods, and functions is provided in the `./docs` directory in this repository.
```

### Comparing `llmflex-0.1.7/src/llmflex.egg-info/SOURCES.txt` & `llmflex-0.1.8/src/llmflex.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,23 +12,22 @@
 src/llmflex.egg-info/top_level.txt
 src/llmflex/Embeddings/__init__.py
 src/llmflex/Embeddings/api_embeddings.py
 src/llmflex/Embeddings/base_embeddings.py
 src/llmflex/Embeddings/hf_embeddings_server.py
 src/llmflex/Embeddings/huggingface_embeddings.py
 src/llmflex/Frontend/__init__.py
-src/llmflex/Frontend/gradio_interface.py
+src/llmflex/Frontend/app_resource.py
 src/llmflex/Frontend/streamlit_interface.py
 src/llmflex/KnowledgeBase/__init__.py
 src/llmflex/KnowledgeBase/knowledge_base.py
 src/llmflex/Memory/__init__.py
-src/llmflex/Memory/assistant_long_term_memory.py
 src/llmflex/Memory/base_memory.py
 src/llmflex/Memory/long_short_memory.py
-src/llmflex/Memory/longshort_memory.py
+src/llmflex/Memory/memory_utils.py
 src/llmflex/Models/__init__.py
 src/llmflex/Models/Cores/__init__.py
 src/llmflex/Models/Cores/base_core.py
 src/llmflex/Models/Cores/exllamav2_core.py
 src/llmflex/Models/Cores/huggingface_core.py
 src/llmflex/Models/Cores/llamacpp_core.py
 src/llmflex/Models/Cores/openai_core.py
@@ -46,15 +45,13 @@
 src/llmflex/TextSplitters/__init__.py
 src/llmflex/TextSplitters/base_text_splitter.py
 src/llmflex/TextSplitters/sentence_token_text_splitter.py
 src/llmflex/TextSplitters/token_text_splitter.py
 src/llmflex/Tools/__init__.py
 src/llmflex/Tools/base_tool.py
 src/llmflex/Tools/browser_tool.py
-src/llmflex/Tools/tool_prompting.py
-src/llmflex/Tools/tool_selection.py
+src/llmflex/Tools/tool_classes.py
 src/llmflex/Tools/tool_utils.py
-src/llmflex/Tools/web_search_tool.py
 src/llmflex/Tools/web_search_utils.py
 src/llmflex/VectorDBs/__init__.py
 src/llmflex/VectorDBs/base_vectordb.py
 src/llmflex/VectorDBs/faiss_vectordb.py
```

