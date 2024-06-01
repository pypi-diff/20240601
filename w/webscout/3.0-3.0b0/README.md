# Comparing `tmp/webscout-3.0.tar.gz` & `tmp/webscout-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webscout-3.0.tar", last modified: Sat Jun  1 14:23:40 2024, max compression
+gzip compressed data, was "webscout-3.0b0.tar", last modified: Thu May 30 06:49:41 2024, max compression
```

## Comparing `webscout-3.0.tar` & `webscout-3.0b0.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxrwxrwx   0        0        0        0 2024-06-01 14:23:40.848595 webscout-3.0/
-drwxrwxrwx   0        0        0        0 2024-06-01 14:23:39.587900 webscout-3.0/DeepWEBS/
--rw-rw-rw-   0        0        0        0 2024-06-01 14:19:28.000000 webscout-3.0/DeepWEBS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-06-01 14:23:39.601900 webscout-3.0/DeepWEBS/documents/
--rw-rw-rw-   0        0        0        0 2024-06-01 14:19:28.000000 webscout-3.0/DeepWEBS/documents/__init__.py
--rw-rw-rw-   0        0        0     4049 2024-06-01 14:19:28.000000 webscout-3.0/DeepWEBS/documents/query_results_extractor.py
--rw-rw-rw-   0        0        0     5272 2024-06-01 14:19:28.000000 webscout-3.0/DeepWEBS/documents/webpage_content_extractor.py
-drwxrwxrwx   0        0        0        0 2024-06-01 14:23:39.629909 webscout-3.0/DeepWEBS/networks/
--rw-rw-rw-   0        0        0        0 2024-06-01 14:19:28.000000 webscout-3.0/DeepWEBS/networks/__init__.py
--rw-rw-rw-   0        0        0     3183 2024-06-01 14:19:28.000000 webscout-3.0/DeepWEBS/networks/filepath_converter.py
--rw-rw-rw-   0        0        0     1966 2024-06-01 14:19:28.000000 webscout-3.0/DeepWEBS/networks/google_searcher.py
--rw-rw-rw-   0        0        0      726 2024-06-01 14:19:28.000000 webscout-3.0/DeepWEBS/networks/network_configs.py
--rw-rw-rw-   0        0        0     3590 2024-06-01 14:19:28.000000 webscout-3.0/DeepWEBS/networks/webpage_fetcher.py
-drwxrwxrwx   0        0        0        0 2024-06-01 14:23:39.656231 webscout-3.0/DeepWEBS/utilsdw/
--rw-rw-rw-   0        0        0        0 2024-06-01 14:19:28.000000 webscout-3.0/DeepWEBS/utilsdw/__init__.py
--rw-rw-rw-   0        0        0     2472 2024-06-01 14:19:28.000000 webscout-3.0/DeepWEBS/utilsdw/enver.py
--rw-rw-rw-   0        0        0     8174 2024-06-01 14:19:28.000000 webscout-3.0/DeepWEBS/utilsdw/logger.py
--rw-rw-rw-   0        0        0     3150 2024-06-01 14:19:28.000000 webscout-3.0/LICENSE.md
--rw-rw-rw-   0        0        0    61994 2024-06-01 14:23:40.841599 webscout-3.0/PKG-INFO
--rw-rw-rw-   0        0        0    59422 2024-06-01 14:19:28.000000 webscout-3.0/README.md
--rw-rw-rw-   0        0        0       42 2024-06-01 14:23:40.848595 webscout-3.0/setup.cfg
--rw-rw-rw-   0        0        0     2816 2024-06-01 14:19:28.000000 webscout-3.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-06-01 14:23:40.036502 webscout-3.0/webscout/
--rw-rw-rw-   0        0        0    18246 2024-06-01 14:19:28.000000 webscout-3.0/webscout/AIauto.py
--rw-rw-rw-   0        0        0     4710 2024-06-01 14:19:28.000000 webscout-3.0/webscout/AIbase.py
--rw-rw-rw-   0        0        0    33272 2024-06-01 14:19:28.000000 webscout-3.0/webscout/AIutel.py
--rw-rw-rw-   0        0        0     7332 2024-06-01 14:19:28.000000 webscout-3.0/webscout/DWEBS.py
--rw-rw-rw-   0        0        0     4184 2024-06-01 14:19:28.000000 webscout-3.0/webscout/LLM.py
-drwxrwxrwx   0        0        0        0 2024-06-01 14:23:40.288980 webscout-3.0/webscout/Local/
--rw-rw-rw-   0        0        0      217 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Local/__init__.py
--rw-rw-rw-   0        0        0       83 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Local/_version.py
--rw-rw-rw-   0        0        0    18994 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Local/formats.py
--rw-rw-rw-   0        0        0    30710 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Local/model.py
--rw-rw-rw-   0        0        0     4372 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Local/samplers.py
--rw-rw-rw-   0        0        0    27408 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Local/thread.py
--rw-rw-rw-   0        0        0     6197 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Local/utils.py
-drwxrwxrwx   0        0        0        0 2024-06-01 14:23:40.798867 webscout-3.0/webscout/Provider/
--rw-rw-rw-   0        0        0     8416 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/BasedGPT.py
--rw-rw-rw-   0        0        0     8552 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/Berlin4h.py
--rw-rw-rw-   0        0        0    17182 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/Blackboxai.py
--rw-rw-rw-   0        0        0     8570 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/ChatGPTUK.py
--rw-rw-rw-   0        0        0     8711 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/Cohere.py
--rw-rw-rw-   0        0        0     8451 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/Gemini.py
--rw-rw-rw-   0        0        0    21094 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/Groq.py
--rw-rw-rw-   0        0        0    15806 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/Koboldai.py
--rw-rw-rw-   0        0        0    19987 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/Leo.py
--rw-rw-rw-   0        0        0    17525 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/Llama2.py
--rw-rw-rw-   0        0        0    18890 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/OpenGPT.py
--rw-rw-rw-   0        0        0    20617 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/Openai.py
--rw-rw-rw-   0        0        0     8826 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/Perplexity.py
--rw-rw-rw-   0        0        0    19907 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/Phind.py
--rw-rw-rw-   0        0        0     7510 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/Poe.py
--rw-rw-rw-   0        0        0     8917 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/Reka.py
--rw-rw-rw-   0        0        0    11616 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/ThinkAnyAI.py
--rw-rw-rw-   0        0        0     9039 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/Xjai.py
--rw-rw-rw-   0        0        0    19875 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/Yepchat.py
--rw-rw-rw-   0        0        0     7976 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/Youchat.py
--rw-rw-rw-   0        0        0     1457 2024-06-01 14:19:28.000000 webscout-3.0/webscout/Provider/__init__.py
--rw-rw-rw-   0        0        0     1856 2024-06-01 14:19:28.000000 webscout-3.0/webscout/__init__.py
--rw-rw-rw-   0        0        0      126 2024-06-01 14:19:28.000000 webscout-3.0/webscout/__main__.py
--rw-rw-rw-   0        0        0      684 2024-06-01 14:19:28.000000 webscout-3.0/webscout/async_providers.py
--rw-rw-rw-   0        0        0    18743 2024-06-01 14:19:28.000000 webscout-3.0/webscout/cli.py
--rw-rw-rw-   0        0        0      498 2024-06-01 14:19:28.000000 webscout-3.0/webscout/exceptions.py
--rw-rw-rw-   0        0        0    24487 2024-06-01 14:19:28.000000 webscout-3.0/webscout/g4f.py
--rw-rw-rw-   0        0        0      692 2024-06-01 14:19:28.000000 webscout-3.0/webscout/models.py
--rw-rw-rw-   0        0        0     5896 2024-06-01 14:19:28.000000 webscout-3.0/webscout/tempid.py
--rw-rw-rw-   0        0        0    20622 2024-06-01 14:19:28.000000 webscout-3.0/webscout/transcriber.py
--rw-rw-rw-   0        0        0     2603 2024-06-01 14:19:28.000000 webscout-3.0/webscout/utils.py
--rw-rw-rw-   0        0        0       23 2024-06-01 14:19:28.000000 webscout-3.0/webscout/version.py
--rw-rw-rw-   0        0        0      967 2024-06-01 14:19:28.000000 webscout-3.0/webscout/voice.py
--rw-rw-rw-   0        0        0    85324 2024-06-01 14:19:28.000000 webscout-3.0/webscout/webai.py
--rw-rw-rw-   0        0        0    42650 2024-06-01 14:19:28.000000 webscout-3.0/webscout/webscout_search.py
--rw-rw-rw-   0        0        0    14471 2024-06-01 14:19:28.000000 webscout-3.0/webscout/webscout_search_async.py
-drwxrwxrwx   0        0        0        0 2024-06-01 14:23:40.829597 webscout-3.0/webscout.egg-info/
--rw-rw-rw-   0        0        0    61994 2024-06-01 14:23:38.000000 webscout-3.0/webscout.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1827 2024-06-01 14:23:39.000000 webscout-3.0/webscout.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-06-01 14:23:38.000000 webscout-3.0/webscout.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       73 2024-06-01 14:23:38.000000 webscout-3.0/webscout.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      433 2024-06-01 14:23:38.000000 webscout-3.0/webscout.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2024-06-01 14:23:38.000000 webscout-3.0/webscout.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:41.265169 webscout-3.0b0/
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:39.148168 webscout-3.0b0/DeepWEBS/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:39.182165 webscout-3.0b0/DeepWEBS/documents/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/documents/__init__.py
+-rw-rw-rw-   0        0        0     4049 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/documents/query_results_extractor.py
+-rw-rw-rw-   0        0        0     5272 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/documents/webpage_content_extractor.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:39.231167 webscout-3.0b0/DeepWEBS/networks/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/networks/__init__.py
+-rw-rw-rw-   0        0        0     3183 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/networks/filepath_converter.py
+-rw-rw-rw-   0        0        0     1966 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/networks/google_searcher.py
+-rw-rw-rw-   0        0        0      726 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/networks/network_configs.py
+-rw-rw-rw-   0        0        0     3590 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/networks/webpage_fetcher.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:39.283155 webscout-3.0b0/DeepWEBS/utilsdw/
+-rw-rw-rw-   0        0        0        0 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/utilsdw/__init__.py
+-rw-rw-rw-   0        0        0     2472 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/utilsdw/enver.py
+-rw-rw-rw-   0        0        0     8174 2024-05-08 15:52:48.000000 webscout-3.0b0/DeepWEBS/utilsdw/logger.py
+-rw-rw-rw-   0        0        0     3150 2024-05-08 15:52:48.000000 webscout-3.0b0/LICENSE.md
+-rw-rw-rw-   0        0        0    47777 2024-05-30 06:49:41.259353 webscout-3.0b0/PKG-INFO
+-rw-rw-rw-   0        0        0    45203 2024-05-19 15:11:59.000000 webscout-3.0b0/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-30 06:49:41.265169 webscout-3.0b0/setup.cfg
+-rw-rw-rw-   0        0        0     2821 2024-05-30 06:44:43.000000 webscout-3.0b0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:40.102566 webscout-3.0b0/webscout/
+-rw-rw-rw-   0        0        0    18246 2024-05-12 12:54:03.000000 webscout-3.0b0/webscout/AIauto.py
+-rw-rw-rw-   0        0        0     4710 2024-05-08 15:52:48.000000 webscout-3.0b0/webscout/AIbase.py
+-rw-rw-rw-   0        0        0    33272 2024-05-27 06:28:40.000000 webscout-3.0b0/webscout/AIutel.py
+-rw-rw-rw-   0        0        0     7332 2024-05-08 15:52:48.000000 webscout-3.0b0/webscout/DWEBS.py
+-rw-rw-rw-   0        0        0     4184 2024-05-19 17:29:05.000000 webscout-3.0b0/webscout/LLM.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:40.643324 webscout-3.0b0/webscout/Local/
+-rw-rw-rw-   0        0        0      217 2024-05-14 07:50:22.000000 webscout-3.0b0/webscout/Local/__init__.py
+-rw-rw-rw-   0        0        0       83 2024-05-26 12:42:35.000000 webscout-3.0b0/webscout/Local/_version.py
+-rw-rw-rw-   0        0        0    18994 2024-05-30 06:36:15.000000 webscout-3.0b0/webscout/Local/formats.py
+-rw-rw-rw-   0        0        0    30463 2024-05-30 06:26:30.000000 webscout-3.0b0/webscout/Local/model.py
+-rw-rw-rw-   0        0        0     4372 2024-05-13 10:22:16.000000 webscout-3.0b0/webscout/Local/samplers.py
+-rw-rw-rw-   0        0        0    27453 2024-05-30 06:39:51.000000 webscout-3.0b0/webscout/Local/thread.py
+-rw-rw-rw-   0        0        0     6197 2024-05-26 12:41:46.000000 webscout-3.0b0/webscout/Local/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:41.247290 webscout-3.0b0/webscout/Provider/
+-rw-rw-rw-   0        0        0     8191 2024-05-16 04:06:55.000000 webscout-3.0b0/webscout/Provider/BasedGPT.py
+-rw-rw-rw-   0        0        0     8342 2024-05-12 04:47:12.000000 webscout-3.0b0/webscout/Provider/Berlin4h.py
+-rw-rw-rw-   0        0        0    16743 2024-05-11 08:19:16.000000 webscout-3.0b0/webscout/Provider/Blackboxai.py
+-rw-rw-rw-   0        0        0     8357 2024-05-12 05:14:27.000000 webscout-3.0b0/webscout/Provider/ChatGPTUK.py
+-rw-rw-rw-   0        0        0     8489 2024-05-11 08:19:31.000000 webscout-3.0b0/webscout/Provider/Cohere.py
+-rw-rw-rw-   0        0        0     8235 2024-05-11 08:19:44.000000 webscout-3.0b0/webscout/Provider/Gemini.py
+-rw-rw-rw-   0        0        0    20583 2024-05-11 08:19:52.000000 webscout-3.0b0/webscout/Provider/Groq.py
+-rw-rw-rw-   0        0        0    15405 2024-05-11 08:20:01.000000 webscout-3.0b0/webscout/Provider/Koboldai.py
+-rw-rw-rw-   0        0        0    19519 2024-05-11 08:20:16.000000 webscout-3.0b0/webscout/Provider/Leo.py
+-rw-rw-rw-   0        0        0    17089 2024-05-11 08:20:22.000000 webscout-3.0b0/webscout/Provider/Llama2.py
+-rw-rw-rw-   0        0        0    18404 2024-05-11 08:20:30.000000 webscout-3.0b0/webscout/Provider/OpenGPT.py
+-rw-rw-rw-   0        0        0    20107 2024-05-11 08:20:26.000000 webscout-3.0b0/webscout/Provider/Openai.py
+-rw-rw-rw-   0        0        0     8597 2024-05-11 08:20:36.000000 webscout-3.0b0/webscout/Provider/Perplexity.py
+-rw-rw-rw-   0        0        0    19390 2024-05-11 08:20:42.000000 webscout-3.0b0/webscout/Provider/Phind.py
+-rw-rw-rw-   0        0        0     7303 2024-05-14 14:08:46.000000 webscout-3.0b0/webscout/Provider/Poe.py
+-rw-rw-rw-   0        0        0     8692 2024-05-11 08:20:50.000000 webscout-3.0b0/webscout/Provider/Reka.py
+-rw-rw-rw-   0        0        0    11616 2024-05-11 08:20:56.000000 webscout-3.0b0/webscout/Provider/ThinkAnyAI.py
+-rw-rw-rw-   0        0        0     8809 2024-05-11 08:21:00.000000 webscout-3.0b0/webscout/Provider/Xjai.py
+-rw-rw-rw-   0        0        0    19398 2024-05-11 08:21:06.000000 webscout-3.0b0/webscout/Provider/Yepchat.py
+-rw-rw-rw-   0        0        0     7756 2024-05-21 13:54:46.000000 webscout-3.0b0/webscout/Provider/Youchat.py
+-rw-rw-rw-   0        0        0     1396 2024-05-27 06:27:55.000000 webscout-3.0b0/webscout/Provider/__init__.py
+-rw-rw-rw-   0        0        0     1856 2024-05-27 06:28:13.000000 webscout-3.0b0/webscout/__init__.py
+-rw-rw-rw-   0        0        0      126 2024-05-08 15:52:48.000000 webscout-3.0b0/webscout/__main__.py
+-rw-rw-rw-   0        0        0      684 2024-05-12 11:18:43.000000 webscout-3.0b0/webscout/async_providers.py
+-rw-rw-rw-   0        0        0    18743 2024-05-19 12:59:44.000000 webscout-3.0b0/webscout/cli.py
+-rw-rw-rw-   0        0        0      498 2024-05-10 14:34:10.000000 webscout-3.0b0/webscout/exceptions.py
+-rw-rw-rw-   0        0        0    24487 2024-05-12 13:39:37.000000 webscout-3.0b0/webscout/g4f.py
+-rw-rw-rw-   0        0        0      692 2024-05-08 15:52:48.000000 webscout-3.0b0/webscout/models.py
+-rw-rw-rw-   0        0        0     5896 2024-05-08 15:52:48.000000 webscout-3.0b0/webscout/tempid.py
+-rw-rw-rw-   0        0        0    20622 2024-05-08 15:52:48.000000 webscout-3.0b0/webscout/transcriber.py
+-rw-rw-rw-   0        0        0     2603 2024-05-09 03:33:11.000000 webscout-3.0b0/webscout/utils.py
+-rw-rw-rw-   0        0        0       23 2024-05-26 12:42:41.000000 webscout-3.0b0/webscout/version.py
+-rw-rw-rw-   0        0        0      967 2024-05-08 15:52:48.000000 webscout-3.0b0/webscout/voice.py
+-rw-rw-rw-   0        0        0    85324 2024-05-14 14:12:32.000000 webscout-3.0b0/webscout/webai.py
+-rw-rw-rw-   0        0        0    42650 2024-05-19 13:03:19.000000 webscout-3.0b0/webscout/webscout_search.py
+-rw-rw-rw-   0        0        0    14471 2024-05-19 13:04:35.000000 webscout-3.0b0/webscout/webscout_search_async.py
+drwxrwxrwx   0        0        0        0 2024-05-30 06:49:41.251897 webscout-3.0b0/webscout.egg-info/
+-rw-rw-rw-   0        0        0    47777 2024-05-30 06:49:37.000000 webscout-3.0b0/webscout.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1827 2024-05-30 06:49:38.000000 webscout-3.0b0/webscout.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-30 06:49:37.000000 webscout-3.0b0/webscout.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       73 2024-05-30 06:49:37.000000 webscout-3.0b0/webscout.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      433 2024-05-30 06:49:37.000000 webscout-3.0b0/webscout.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2024-05-30 06:49:37.000000 webscout-3.0b0/webscout.egg-info/top_level.txt
```

### Comparing `webscout-3.0/DeepWEBS/documents/query_results_extractor.py` & `webscout-3.0b0/DeepWEBS/documents/query_results_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/DeepWEBS/documents/webpage_content_extractor.py` & `webscout-3.0b0/DeepWEBS/documents/webpage_content_extractor.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/DeepWEBS/networks/filepath_converter.py` & `webscout-3.0b0/DeepWEBS/networks/filepath_converter.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/DeepWEBS/networks/google_searcher.py` & `webscout-3.0b0/DeepWEBS/networks/google_searcher.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/DeepWEBS/networks/network_configs.py` & `webscout-3.0b0/DeepWEBS/networks/network_configs.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/DeepWEBS/networks/webpage_fetcher.py` & `webscout-3.0b0/DeepWEBS/networks/webpage_fetcher.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/DeepWEBS/utilsdw/enver.py` & `webscout-3.0b0/DeepWEBS/utilsdw/enver.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/DeepWEBS/utilsdw/logger.py` & `webscout-3.0b0/DeepWEBS/utilsdw/logger.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/LICENSE.md` & `webscout-3.0b0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `webscout-3.0/PKG-INFO` & `webscout-3.0b0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webscout
-Version: 3.0
+Version: 3.0b0
 Summary: Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
 Author: OEvortex
 Author-email: helpingai5@gmail.com
 License: HelpingAI Simplified Universal License
 Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
 Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
 Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
@@ -138,15 +138,14 @@
     - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35)
     - [13. `ThinkAny` - AI search engine](#13-thinkany---ai-search-engine)
     - [14. `chatgptuk` - Chat with gemini-pro](#14-chatgptuk---chat-with-gemini-pro)
     - [15. `poe`- chat with poe](#15-poe--chat-with-poe)
     - [16. `BasedGPT` - chat with GPT](#16-basedgpt---chat-with-gpt)
     - [`LLM`](#llm)
     - [`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-gguf-models)
-    - [`Function-calling-local-llm`](#function-calling-local-llm)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
 pip install -U webscout
@@ -1260,86 +1259,14 @@
 
 # 3. Create a Thread for conversation
 thread = Thread(model, formats.phi3)
 
 # 4. Start interacting with the model
 thread.interact()
 ```
-### `Function-calling-local-llm`
-```python
-from webscout.Local import Model, Thread, formats
-from webscout import DeepWEBS
-from webscout.Local.utils import download_model
-from webscout.Local.model import Model
-from webscout.Local.thread import Thread
-from webscout.Local import formats
-from webscout.Local.samplers import SamplerSettings
-def deepwebs_search(query, max_results=5):
-    """Performs a web search using DeepWEBS and returns results as JSON."""
-    deepwebs = DeepWEBS()
-    search_config = DeepWEBS.DeepSearch(
-        queries=[query],
-        max_results=max_results,
-        extract_webpage=False,
-        safe=False,
-        types=["web"],
-        overwrite_query_html=True,
-        overwrite_webpage_html=True,
-    )
-    search_results = deepwebs.queries_to_search_results(search_config)
-    formatted_results = []
-    for result in search_results[0]:  # Assuming only one query
-        formatted_results.append(f"Title: {result['title']}\nURL: {result['url']}\n")
-    return "\n".join(formatted_results)
-
-# Load your model
-repo_id = "OEvortex/HelpingAI-9B" 
-filename = "helpingai-9b.Q4_0.gguf"
-model_path = download_model(repo_id, filename, token='')
-
-# 2. Load the model 
-model = Model(model_path, n_gpu_layers=10)
-
-# Create a Thread
-system_prompt = "You are a helpful AI assistant. Respond to user queries concisely. If a user asks for information that requires a web search, use the `deepwebs_search` tool. Do not call the tool if it is not necessary."
-sampler = SamplerSettings(temp=0.7, top_p=0.9)  # Adjust these values as needed
-# 4. Create a custom chatml format with your system prompt
-custom_chatml = formats.chatml.copy()
-custom_chatml['system_content'] = system_prompt
-thread = Thread(model, custom_chatml, sampler=sampler)
-# Add the deepwebs_search tool
-thread.add_tool({
-    "type": "function",
-    "function": {
-        "name": "deepwebs_search",
-        "description": "Performs a web search using DeepWEBS and returns the title and URLs of the results.",
-        "execute": deepwebs_search,
-        "parameters": {
-            "type": "object",
-            "properties": {
-                "query": {
-                    "type": "string",
-                    "description": "The query to search on the web",
-                },
-                "max_results": {
-                    "type": "integer",
-                    "description": "Maximum number of search results (default: 5)",
-                },
-            },
-            "required": ["query"],
-        },
-    },
-})
-
-# Start interacting with the model
-while True:
-    user_input = input("You: ")
-    response = thread.send(user_input)
-    print("Bot: ", response) 
-```
 ### `LLM` with internet
 ```python
 from __future__ import annotations
 from typing import List, Optional
 
 from webscout.LLM import LLM
 from webscout import WEBS
@@ -1496,324 +1423,49 @@
             print("AI:", response)
         else:
             print("No response")
 ```
 ## `Webai` - terminal gpt and a open interpeter
 
 ```python
-import time
-import uuid
-from typing import Dict, Any, Optional, AsyncGenerator
-from rich.console import Console
-from rich.markdown import Markdown
-from rich.panel import Panel
-from rich.style import Style
-import webscout
-import webscout.AIutel
-import g4f
-from webscout.g4f import *
-from webscout.async_providers import mapper as async_provider_map
+from webscout.webai import Main
 
-class TaskExecutor:
+def use_rawdog_with_webai(prompt):
     """
-    Manages an interactive chat session, handling user input, AI responses, 
-    and optional features like web search, code execution, and text-to-speech.
+    Wrap the webscout default method in a try-except block to catch any unhandled
+    exceptions and print a helpful message.
     """
-
-    def __init__(self) -> None:
-        """Initializes the conversational assistant with default settings."""
-        self._console: Console = Console()
-
-        # Session configuration
-        self._selected_provider: str = "phind"
-        self._selected_model: str = "Phind Model"
-        self._conversation_enabled: bool = True
-        self._max_tokens: int = 600
-        self._temperature: float = 0.2
-        self._top_k: int = -1
-        self._top_p: float = 0.999
-        self._timeout: int = 30
-        self._auth_token: str = None  # API key, if required
-        self._chat_completion_enabled: bool = True  # g4fauto
-        self._ignore_working: bool = False  # Ignore working status of providers
-        self._proxy_path: str = None  # Path to proxy configuration
-
-        # History Management
-        self._history_filepath: str = None
-        self._update_history_file: bool = True
-        self._history_offset: int = 10250
-
-        # Prompt Engineering
-        self._initial_prompt: str = None
-        self._awesome_prompt_content: str = None 
-
-        # Optional Features
-        self._web_search_enabled: bool = False  # Enable web search
-        self._rawdog_enabled: bool = True
-        self._internal_script_execution_enabled: bool = False
-        self._script_confirmation_required: bool = False
-        self._selected_interpreter: str = "python"
-        self._selected_optimizer: str = "code"
-        self._suppress_output: bool = False  # Suppress verbose output
-
-        # AI provider mapping
-        self._ai_provider_mapping: Dict[str, Any] = {
-            "phind": webscout.PhindSearch,
-            "opengpt": webscout.OPENGPT,
-            "koboldai": webscout.KOBOLDAI,
-            "blackboxai": webscout.BLACKBOXAI,
-            "llama2": webscout.LLAMA2,
-            "yepchat": webscout.YEPCHAT,
-            "leo": webscout.LEO,
-            "groq": webscout.GROQ,
-            "openai": webscout.OPENAI,
-            "perplexity": webscout.PERPLEXITY,
-            "you": webscout.YouChat,
-            "xjai": webscout.Xjai,
-            "cohere": webscout.Cohere,
-            "reka": webscout.REKA,
-            "thinkany": webscout.ThinkAnyAI,
-            "gemini": webscout.GEMINI, 
-            "berlin4h": webscout.Berlin4h,
-            "chatgptuk": webscout.ChatGPTUK,
-            "poe": webscout.POE,
-            "basedgpt": webscout.BasedGPT,
-        }
-
-        # Initialize Rawdog if enabled
-        if self._rawdog_enabled:
-            self._rawdog_instance: webscout.AIutel.RawDog = webscout.AIutel.RawDog(
-                quiet=self._suppress_output,
-                internal_exec=self._internal_script_execution_enabled,
-                confirm_script=self._script_confirmation_required,
-                interpreter=self._selected_interpreter,
-            )
-
-            self._initial_prompt = self._rawdog_instance.intro_prompt
-
-        # Initialize the selected AI model 
-        self._ai_model = self._get_ai_model()
-
-    def _get_ai_model(self):
-        """
-        Determines the appropriate AI model based on the selected provider, 
-        including automatic provider selection and g4fauto support.
-        """
-        if self._selected_provider == "g4fauto":
-            # Automatically select the best provider from g4f
-            test = TestProviders(quiet=self._suppress_output, timeout=self._timeout)
-            g4fauto = test.best if not self._ignore_working else test.auto
-            if isinstance(g4fauto, str):
-                self._selected_provider = "g4fauto+" + g4fauto
-                self._ai_model = self._create_g4f_model(g4fauto)
-            else:
-                raise Exception(
-                    "No working g4f provider found. "
-                    "Consider running 'webscout.webai gpt4free test -y' first"
-                )
-        else:
-            # Use the specified provider
-            self._ai_model = self._ai_provider_mapping[self._selected_provider](
-                is_conversation=self._conversation_enabled,
-                max_tokens=self._max_tokens,
-                timeout=self._timeout,
-                intro=self._initial_prompt,
-                filepath=self._history_filepath,
-                update_file=self._update_history_file,
-                proxies={},  # Load proxies from config if needed
-                history_offset=self._history_offset,
-                act=self._awesome_prompt_content, 
-                model=self._selected_model,
-                quiet=self._suppress_output,
-                # auth=self._auth_token,  # Pass API key if required
-            )
-        return self._ai_model
-
-    def _create_g4f_model(self, provider: str):
-        """
-        Creates a g4f model instance using the provided provider and webscout.WEBS for web search.
-        """
-        return webscout.g4f.GPT4FREE(
-            provider=provider,
-            auth=self._auth_token,
-            max_tokens=self._max_tokens,
-            chat_completion=self._chat_completion_enabled,
-            ignore_working=self._ignore_working,
-            timeout=self._timeout,
-            intro=self._initial_prompt,
-            filepath=self._history_filepath,
-            update_file=self._update_history_file,
-            proxies={},  # Load proxies from config if needed
-            history_offset=self._history_offset,
-            act=self._awesome_prompt_content, 
+    try:
+        webai_bot = Main(
+            max_tokens=500, 
+            provider="cohere",
+            temperature=0.7,  
+            top_k=40,          
+            top_p=0.95,        
+            model="command-r-plus",  # Replace with your desired model
+            auth=None,     # Replace with your auth key/value (if needed)
+            timeout=30,
+            disable_conversation=True,
+            filepath=None,
+            update_file=True,
+            intro=None,
+            rawdog=True,
+            history_offset=10250,
+            awesome_prompt=None,
+            proxy_path=None,
+            quiet=True
         )
+        webai_response = webai_bot.default(prompt) 
+    except Exception as e:
+        print("Unexpected error:", e)
 
-    def process_query(self, query: str) -> None:
-        """
-        Processes a user query, potentially enhancing it with web search results, 
-        passing it to the AI model, and handling the response.
-
-        Args:
-            query: The user's text input.
-
-        Returns:
-            None
-        """
-        if self._web_search_enabled:
-            query = self._augment_query_with_web_search(query)
-
-        # Apply code optimization if configured
-        if self._selected_optimizer == "code":
-            query = webscout.AIutel.Optimizers.code(query)
-
-        try:
-            response: str = self._ai_model.chat(query)
-        except webscout.exceptions.FailedToGenerateResponseError as e:
-            self._console.print(Markdown(f"LLM: [red]{e}[/red]"))
-            return
-
-        # Handle Rawdog responses if enabled
-        if self._rawdog_enabled:
-            self._handle_rawdog_response(response)
-        else:
-            self._console.print(Markdown(f"LLM: {response}"))
-
-    def _augment_query_with_web_search(self, query: str) -> str:
-        """Performs a web search and appends the results to the query.
-
-        Args:
-            query: The user's text input.
-
-        Returns:
-            str: The augmented query with web search results.
-        """
-        web_search_results = webscout.WEBS().text(query, max_results=3)
-        if web_search_results:
-            formatted_results = "\n".join(
-                f"{i+1}. {result['title']} - {result['href']}\n\nBody: {result['body']}"
-                for i, result in enumerate(web_search_results)
-            )
-            query += f"\n\n## Web Search Results are:\n\n{formatted_results}"
-        return query
-
-    def _handle_rawdog_response(self, response: str) -> None:
-        """Handles AI responses, potentially executing them as code with Rawdog.
-
-        Args:
-            response: The AI model's response.
-
-        Returns:
-            None
-        """
-        try:
-            is_feedback = self._rawdog_instance.main(response)
-        except Exception as e:
-            self._console.print(Markdown(f"LLM: [red]Error: {e}[/red]"))
-            return
-        if is_feedback:
-            self._console.print(Markdown(f"LLM: {is_feedback}"))
-        else:
-            self._console.print(Markdown("LLM: (Script executed successfully)"))
-
-    async def process_async_query(self, query: str) -> None:
-        """
-        Asynchronously processes a user query, potentially enhancing it with web search results, 
-        passing it to the AI model, and handling the response.
-
-        Args:
-            query: The user's text input.
-
-        Returns:
-            None
-        """
-        if self._web_search_enabled:
-            query = self._augment_query_with_web_search(query)
-
-        # Apply code optimization if configured
-        if self._selected_optimizer == "code":
-            query = webscout.AIutel.Optimizers.code(query)
-
-        async_model = self._get_async_ai_model()
-
-        try:
-            async for response in async_model.chat(query, stream=True):
-                self._console.print(Markdown(f"LLM: {response}"), end="")
-        except webscout.exceptions.FailedToGenerateResponseError as e:
-            self._console.print(Markdown(f"LLM: [red]{e}[/red]"))
-            return
-
-        # Handle Rawdog responses if enabled
-        if self._rawdog_enabled:
-            self._handle_rawdog_response(response)
-        else:
-            self._console.print(Markdown(f"LLM: {response}"))
-
-    def _get_async_ai_model(self):
-        """
-        Determines the appropriate asynchronous AI model based on the selected provider.
-        """
-        if self._selected_provider == "g4fauto":
-            # Automatically select the best provider from g4f
-            test = TestProviders(quiet=self._suppress_output, timeout=self._timeout)
-            g4fauto = test.best if not self._ignore_working else test.auto
-            if isinstance(g4fauto, str):
-                self._selected_provider = "g4fauto+" + g4fauto
-                self._ai_model = self._create_async_g4f_model(g4fauto)
-            else:
-                raise Exception(
-                    "No working g4f provider found. "
-                    "Consider running 'webscout gpt4free test -y' first"
-                )
-        else:
-            # Use the specified provider
-            if self._selected_provider in async_provider_map:
-                self._ai_model = async_provider_map[self._selected_provider](
-                    is_conversation=self._conversation_enabled,
-                    max_tokens=self._max_tokens,
-                    timeout=self._timeout,
-                    intro=self._initial_prompt,
-                    filepath=self._history_filepath,
-                    update_file=self._update_history_file,
-                    proxies={},  # Load proxies from config if needed
-                    history_offset=self._history_offset,
-                    act=self._awesome_prompt_content, 
-                    model=self._selected_model,
-                    quiet=self._suppress_output,
-                    auth=self._auth_token,  # Pass API key if required
-                )
-            else:
-                raise Exception(
-                    f"Asynchronous provider '{self._selected_provider}' is not yet supported"
-                )
-        return self._ai_model
-
-    def _create_async_g4f_model(self, provider: str):
-        """
-        Creates an asynchronous g4f model instance using the provided provider and webscout.WEBS for web search.
-        """
-        return webscout.g4f.AsyncGPT4FREE(
-            provider=provider,
-            auth=self._auth_token,
-            max_tokens=self._max_tokens,
-            chat_completion=self._chat_completion_enabled,
-            ignore_working=self._ignore_working,
-            timeout=self._timeout,
-            intro=self._initial_prompt,
-            filepath=self._history_filepath,
-            update_file=self._update_history_file,
-            proxies={},  # Load proxies from config if needed
-            history_offset=self._history_offset,
-            act=self._awesome_prompt_content,
-        )
 
 if __name__ == "__main__":
-    assistant = TaskExecutor()
-    while True:
-        input_query = input("Enter your query: ")
-        assistant.process_query(input_query)
+    user_prompt = input("Enter your prompt: ")
+    use_rawdog_with_webai(user_prompt)
 
 ```
 ```shell
 python -m webscout.webai webai --provider "phind" --rawdog
 ```
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 2.1 Name: webscout Version: 3.0 Summary: Search for anything
-using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt
-videos, temporary email and phone number generation, has TTS support, webai
-(terminal gpt and open interpreter) and offline LLMs Author: OEvortex Author-
-email: helpingai5@gmail.com License: HelpingAI Simplified Universal License
-Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
-Project-URL: Source, https://github.com/OE-LUCIFER/Webscout Project-URL:
-Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-URL: YouTube,
-https://youtube.com/@OEvortex Classifier: Development Status :: 5 - Production/
-Stable Classifier: Intended Audience :: Developers Classifier: License ::
-Other/Proprietary License Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: Implementation :: CPython
-Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search Classifier: Topic
-:: Software Development :: Libraries :: Python Modules Description-Content-
-Type: text/markdown License-File: LICENSE.md Requires-Dist:
+Metadata-Version: 2.1 Name: webscout Version: 3.0b0 Summary: Search for
+anything using Google, DuckDuckGo, phind.com, Contains AI models, can
+transcribe yt videos, temporary email and phone number generation, has TTS
+support, webai (terminal gpt and open interpreter) and offline LLMs Author:
+OEvortex Author-email: helpingai5@gmail.com License: HelpingAI Simplified
+Universal License Project-URL: Documentation, https://github.com/OE-LUCIFER/
+Webscout/wiki Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
+Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-
+URL: YouTube, https://youtube.com/@OEvortex Classifier: Development Status :: 5
+- Production/Stable Classifier: Intended Audience :: Developers Classifier:
+License :: Other/Proprietary License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
 docstring_inheritance Requires-Dist: click Requires-Dist: curl_cffi Requires-
 Dist: lxml Requires-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist:
 tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
 Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
 Dist: beautifulsoup4 Requires-Dist: markdownify Requires-Dist: pydantic
 Requires-Dist: requests Requires-Dist: sse_starlette Requires-Dist: termcolor
 Requires-Dist: tiktoken Requires-Dist: tldextract Requires-Dist: orjson
@@ -75,86 +75,86 @@
 chat with reka](#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere]
  (#11-cohere---chat-with-cohere) - [12. `Xjai` - chat with free gpt 3.5](#12-
    xjai---chat-with-free-gpt-35) - [13. `ThinkAny` - AI search engine](#13-
  thinkany---ai-search-engine) - [14. `chatgptuk` - Chat with gemini-pro](#14-
  chatgptuk---chat-with-gemini-pro) - [15. `poe`- chat with poe](#15-poe--chat-
  with-poe) - [16. `BasedGPT` - chat with GPT](#16-basedgpt---chat-with-gpt) -
   [`LLM`](#llm) - [`Local-LLM` webscout can now run GGUF models](#local-llm-
- webscout-can-now-run-gguf-models) - [`Function-calling-local-llm`](#function-
-  calling-local-llm) - [`LLM` with internet](#llm-with-internet) - [LLM with
-deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter]
-(#webai---terminal-gpt-and-a-open-interpeter) ## Install ```python pip install
-   -U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
+webscout-can-now-run-gguf-models) - [`LLM` with internet](#llm-with-internet) -
+ [LLM with deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt and a open
+ interpeter](#webai---terminal-gpt-and-a-open-interpeter) ## Install ```python
+pip install -U webscout ``` ## CLI version ```python3 python -m webscout --help
+``` | Command | Description | |-------------------------------------------|----
 -------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | [Go To TOP](#TOP)
- ## Regions expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina
-au-en for Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium
-(nl) br-pt for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr)
-ct-ca for Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for
-Croatia cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for
-  Finland fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong
-Kong hu-hu for Hungary in-en for India id-id for Indonesia id-en for Indonesia
- (en) ie-en for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr
- for Korea lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms
-for Malaysia my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-
-en for New Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl
-for Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-
-ru for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia
-za-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland
- (de) ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan
-th-th for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom
-us-en for United States ue-es for United States (es) ve-es for Venezuela vn-vi
-  for Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp
-number ### Temp number ```python from rich.console import Console from webscout
-             import tempid def main(): console = Console() phone =
-    tempid.TemporaryPhoneNumber() try: # Get a temporary phone number for a
-   specific country (or random) number = phone.get_number(country="Finland")
-console.print(f"Your temporary phone number: [bold cyan]{number}[/bold cyan]")
-# Pause execution briefly (replace with your actual logic) # import time module
- import time time.sleep(30) # Adjust the waiting time as needed # Retrieve and
-  print messages messages = phone.get_messages(number) if messages: # Access
-   individual messages using indexing: console.print(f"[bold green]{messages
- [0].frm}:[/] {messages[0].content}") # (Add more lines if you expect multiple
- messages) else: console.print("No messages received.") except Exception as e:
- console.print(f"[bold red]An error occurred: {e}") if __name__ == "__main__":
-   main() ``` ### Tempmail ```python import asyncio from rich.console import
- Console from rich.table import Table from rich.text import Text from webscout
-     import tempid async def main() -> None: console = Console() client =
-   tempid.Client() try: domains = await client.get_domains() if not domains:
-console.print("[bold red]No domains available. Please try again later.") return
-email = await client.create_email(domain=domains[0].name) console.print(f"Your
- temporary email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token
-  for accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
-  messages = await client.get_messages(email.email) if messages is not None:
-break if messages: table = Table(show_header=True, header_style="bold magenta")
-    table.add_column("From", style="bold cyan") table.add_column("Subject",
- style="bold yellow") table.add_column("Body", style="bold green") for message
- in messages: body_preview = Text(message.body_text if message.body_text else
- "No body") table.add_row(message.email_from or "Unknown", message.subject or
-   "No Subject", body_preview) console.print(table) else: console.print("No
-  messages found.") except Exception as e: console.print(f"[bold red]An error
-   occurred: {e}") finally: await client.close() if __name__ == '__main__':
-asyncio.run(main()) ``` ## Transcriber The transcriber function in webscout is
-     a handy tool that transcribes YouTube videos. Here's an example code
-demonstrating its usage: ```python import sys from webscout import transcriber
-  def extract_transcript(video_id): """Extracts the transcript from a YouTube
-  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
-transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
+ --------------------| | python -m webscout answers -k Text | CLI function to
+perform an answers search using Webscout. | | python -m webscout images -k Text
+    | CLI function to perform an images search using Webscout. | | python -
+m webscout maps -k Text | CLI function to perform a maps search using Webscout.
+  | | python -m webscout news -k Text | CLI function to perform a news search
+ using Webscout. | | python -m webscout suggestions -k Text | CLI function to
+  perform a suggestions search using Webscout. | | python -m webscout text -
+  k Text | CLI function to perform a text search using Webscout. | | python -
+    m webscout translate -k Text | CLI function to perform translate using
+  Webscout. | | python -m webscout version | A command-line interface command
+  that prints and returns the version of the program. | | python -m webscout
+videos -k Text | CLI function to perform a videos search using DuckDuckGo API.
+ | [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for Arabia (en)
+ ar-es for Argentina au-en for Australia at-de for Austria be-fr for Belgium
+   (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en for
+Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for China
+co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for Denmark
+ ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany gr-el
+  for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id for
+Indonesia id-en for Indonesia (en) ie-en for Ireland il-he for Israel it-it for
+Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania xl-
+   es for Latin America my-ms for Malaysia my-en for Malaysia (en) mx-es for
+ Mexico nl-nl for Netherlands nz-en for New Zealand no-no for Norway pe-es for
+ Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
+ for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
+Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
+  for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
+ Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
+ for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
+ States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
+   To TOP](#TOP) ## Tempmail and Temp number ### Temp number ```python from
+ rich.console import Console from webscout import tempid def main(): console =
+ Console() phone = tempid.TemporaryPhoneNumber() try: # Get a temporary phone
+      number for a specific country (or random) number = phone.get_number
+ (country="Finland") console.print(f"Your temporary phone number: [bold cyan]
+  {number}[/bold cyan]") # Pause execution briefly (replace with your actual
+  logic) # import time module import time time.sleep(30) # Adjust the waiting
+  time as needed # Retrieve and print messages messages = phone.get_messages
+      (number) if messages: # Access individual messages using indexing:
+ console.print(f"[bold green]{messages[0].frm}:[/] {messages[0].content}") #
+   (Add more lines if you expect multiple messages) else: console.print("No
+messages received.") except Exception as e: console.print(f"[bold red]An error
+ occurred: {e}") if __name__ == "__main__": main() ``` ### Tempmail ```python
+ import asyncio from rich.console import Console from rich.table import Table
+   from rich.text import Text from webscout import tempid async def main() -
+   > None: console = Console() client = tempid.Client() try: domains = await
+   client.get_domains() if not domains: console.print("[bold red]No domains
+ available. Please try again later.") return email = await client.create_email
+  (domain=domains[0].name) console.print(f"Your temporary email: [bold cyan]
+  {email.email}[/bold cyan]") console.print(f"Token for accessing the email:
+      [bold cyan]{email.token}[/bold cyan]") while True: messages = await
+ client.get_messages(email.email) if messages is not None: break if messages:
+ table = Table(show_header=True, header_style="bold magenta") table.add_column
+ ("From", style="bold cyan") table.add_column("Subject", style="bold yellow")
+     table.add_column("Body", style="bold green") for message in messages:
+  body_preview = Text(message.body_text if message.body_text else "No body")
+table.add_row(message.email_from or "Unknown", message.subject or "No Subject",
+ body_preview) console.print(table) else: console.print("No messages found.")
+   except Exception as e: console.print(f"[bold red]An error occurred: {e}")
+ finally: await client.close() if __name__ == '__main__': asyncio.run(main())
+ ``` ## Transcriber The transcriber function in webscout is a handy tool that
+  transcribes YouTube videos. Here's an example code demonstrating its usage:
+ ```python import sys from webscout import transcriber def extract_transcript
+     (video_id): """Extracts the transcript from a YouTube video.""" try:
+  transcript_list = transcriber.list_transcripts(video_id) for transcript in
+       transcript_list: transcript_data_list = transcript.fetch() lang =
  transcript.language transcript_text = "" if transcript.language_code == 'en':
     for line in transcript_data_list: start_time = line['start'] end_time =
      start_time + line['duration'] formatted_line = f"{start_time:.2f} -
   {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
   transcript_text elif transcript.is_translatable: english_transcript_list =
     transcript.translate('en').fetch() for line in english_transcript_list:
       start_time = line['start'] end_time = start_time + line['duration']
@@ -430,66 +430,35 @@
 webscout.Local.model import Model from webscout.Local.thread import Thread from
 webscout.Local import formats # 1. Download the model repo_id = "microsoft/Phi-
 3-mini-4k-instruct-gguf" # Replace with the desired Hugging Face repo filename
     = "Phi-3-mini-4k-instruct-q4.gguf" # Replace with the correct filename
   model_path = download_model(repo_id, filename) # 2. Load the model model =
 Model(model_path, n_gpu_layers=4) # 3. Create a Thread for conversation thread
       = Thread(model, formats.phi3) # 4. Start interacting with the model
-     thread.interact() ``` ### `Function-calling-local-llm` ```python from
-webscout.Local import Model, Thread, formats from webscout import DeepWEBS from
-  webscout.Local.utils import download_model from webscout.Local.model import
-   Model from webscout.Local.thread import Thread from webscout.Local import
-formats from webscout.Local.samplers import SamplerSettings def deepwebs_search
-  (query, max_results=5): """Performs a web search using DeepWEBS and returns
- results as JSON.""" deepwebs = DeepWEBS() search_config = DeepWEBS.DeepSearch
-( queries=[query], max_results=max_results, extract_webpage=False, safe=False,
-   types=["web"], overwrite_query_html=True, overwrite_webpage_html=True, )
-      search_results = deepwebs.queries_to_search_results(search_config)
-  formatted_results = [] for result in search_results[0]: # Assuming only one
-    query formatted_results.append(f"Title: {result['title']}\nURL: {result
- ['url']}\n") return "\n".join(formatted_results) # Load your model repo_id =
-   "OEvortex/HelpingAI-9B" filename = "helpingai-9b.Q4_0.gguf" model_path =
- download_model(repo_id, filename, token='') # 2. Load the model model = Model
-  (model_path, n_gpu_layers=10) # Create a Thread system_prompt = "You are a
-  helpful AI assistant. Respond to user queries concisely. If a user asks for
-information that requires a web search, use the `deepwebs_search` tool. Do not
-  call the tool if it is not necessary." sampler = SamplerSettings(temp=0.7,
- top_p=0.9) # Adjust these values as needed # 4. Create a custom chatml format
-  with your system prompt custom_chatml = formats.chatml.copy() custom_chatml
-   ['system_content'] = system_prompt thread = Thread(model, custom_chatml,
-   sampler=sampler) # Add the deepwebs_search tool thread.add_tool({ "type":
-"function", "function": { "name": "deepwebs_search", "description": "Performs a
-  web search using DeepWEBS and returns the title and URLs of the results.",
- "execute": deepwebs_search, "parameters": { "type": "object", "properties":
-{ "query": { "type": "string", "description": "The query to search on the web",
-}, "max_results": { "type": "integer", "description": "Maximum number of search
-     results (default: 5)", }, }, "required": ["query"], }, }, }) # Start
- interacting with the model while True: user_input = input("You: ") response =
- thread.send(user_input) print("Bot: ", response) ``` ### `LLM` with internet
-```python from __future__ import annotations from typing import List, Optional
-    from webscout.LLM import LLM from webscout import WEBS import warnings
-system_message: str = ( "As an AI assistant, I have been designed with advanced
- capabilities, including real-time access to online resources. This enables me
-    to enrich our conversations and provide you with informed and accurate
-responses, drawing from a vast array of information. With each interaction, my
- goal is to create a seamless and meaningful connection, offering insights and
-sharing relevant content." "My directives emphasize the importance of respect,
-    impartiality, and intellectual integrity. I am here to provide unbiased
-  responses, ensuring an ethical and respectful exchange. I will respect your
-privacy and refrain from sharing any personal information that may be obtained
-  during our conversations or through web searches, only utilizing web search
-   functionality when necessary to provide the most accurate and up-to-date
- information." "Together, let's explore a diverse range of topics, creating an
-    enjoyable and informative experience, all while maintaining the highest
-     standards of privacy and respect" ) # Ignore the specific UserWarning
- warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffio",
-     lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1",
-     system_message=system_message) def chat( user_input: str, webs: WEBS,
- max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
-  search based on the user input and generate a response using the LLM model.
+thread.interact() ``` ### `LLM` with internet ```python from __future__ import
+annotations from typing import List, Optional from webscout.LLM import LLM from
+    webscout import WEBS import warnings system_message: str = ( "As an AI
+assistant, I have been designed with advanced capabilities, including real-time
+  access to online resources. This enables me to enrich our conversations and
+provide you with informed and accurate responses, drawing from a vast array of
+    information. With each interaction, my goal is to create a seamless and
+  meaningful connection, offering insights and sharing relevant content." "My
+directives emphasize the importance of respect, impartiality, and intellectual
+  integrity. I am here to provide unbiased responses, ensuring an ethical and
+ respectful exchange. I will respect your privacy and refrain from sharing any
+ personal information that may be obtained during our conversations or through
+web searches, only utilizing web search functionality when necessary to provide
+   the most accurate and up-to-date information." "Together, let's explore a
+diverse range of topics, creating an enjoyable and informative experience, all
+while maintaining the highest standards of privacy and respect" ) # Ignore the
+ specific UserWarning warnings.filterwarnings("ignore", category=UserWarning,
+  module="curl_cffio", lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-
+Instruct-v0.1", system_message=system_message) def chat( user_input: str, webs:
+WEBS, max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a
+web search based on the user input and generate a response using the LLM model.
  Parameters ---------- user_input : str The user input to be used for the web
   search webs : WEBS The web search instance to be used to perform the search
 max_results : int, optional The maximum number of search results to include in
     the response, by default 10 Returns ------- Optional[str] The response
 generated by the LLM model, or None if there is no response """ # Perform a web
     search based on the user input search_results: List[str] = [] for r in
     webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
@@ -541,144 +510,23 @@
   including the user input, search results, and system message messages = [
    {"role": "user", "content": f"User question is:\n{user_input}\nwebsearch
     results are:\n{formatted_results}"}, ] # Use the chat method to get the
      response response = LLM.chat(messages) return response if __name__ ==
   "__main__": while True: # Get the user input user_input = input("User: ") #
   Perform a web search based on the user input response = chat(user_input) #
     Print the response if response: print("AI:", response) else: print("No
-response") ``` ## `Webai` - terminal gpt and a open interpeter ```python import
- time import uuid from typing import Dict, Any, Optional, AsyncGenerator from
-rich.console import Console from rich.markdown import Markdown from rich.panel
-       import Panel from rich.style import Style import webscout import
-          webscout.AIutel import g4f from webscout.g4f import * from
-      webscout.async_providers import mapper as async_provider_map class
-TaskExecutor: """ Manages an interactive chat session, handling user input, AI
-responses, and optional features like web search, code execution, and text-to-
-   speech. """ def __init__(self) -> None: """Initializes the conversational
-   assistant with default settings.""" self._console: Console = Console() #
-         Session configuration self._selected_provider: str = "phind"
- self._selected_model: str = "Phind Model" self._conversation_enabled: bool =
- True self._max_tokens: int = 600 self._temperature: float = 0.2 self._top_k:
- int = -1 self._top_p: float = 0.999 self._timeout: int = 30 self._auth_token:
-str = None # API key, if required self._chat_completion_enabled: bool = True #
-g4fauto self._ignore_working: bool = False # Ignore working status of providers
-self._proxy_path: str = None # Path to proxy configuration # History Management
-   self._history_filepath: str = None self._update_history_file: bool = True
- self._history_offset: int = 10250 # Prompt Engineering self._initial_prompt:
-    str = None self._awesome_prompt_content: str = None # Optional Features
-          self._web_search_enabled: bool = False # Enable web search
-self._rawdog_enabled: bool = True self._internal_script_execution_enabled: bool
-           = False self._script_confirmation_required: bool = False
-  self._selected_interpreter: str = "python" self._selected_optimizer: str =
-   "code" self._suppress_output: bool = False # Suppress verbose output # AI
-    provider mapping self._ai_provider_mapping: Dict[str, Any] = { "phind":
-        webscout.PhindSearch, "opengpt": webscout.OPENGPT, "koboldai":
-        webscout.KOBOLDAI, "blackboxai": webscout.BLACKBOXAI, "llama2":
-  webscout.LLAMA2, "yepchat": webscout.YEPCHAT, "leo": webscout.LEO, "groq":
- webscout.GROQ, "openai": webscout.OPENAI, "perplexity": webscout.PERPLEXITY,
-  "you": webscout.YouChat, "xjai": webscout.Xjai, "cohere": webscout.Cohere,
-       "reka": webscout.REKA, "thinkany": webscout.ThinkAnyAI, "gemini":
-         webscout.GEMINI, "berlin4h": webscout.Berlin4h, "chatgptuk":
-  webscout.ChatGPTUK, "poe": webscout.POE, "basedgpt": webscout.BasedGPT, } #
- Initialize Rawdog if enabled if self._rawdog_enabled: self._rawdog_instance:
- webscout.AIutel.RawDog = webscout.AIutel.RawDog( quiet=self._suppress_output,
-            internal_exec=self._internal_script_execution_enabled,
-              confirm_script=self._script_confirmation_required,
-       interpreter=self._selected_interpreter, ) self._initial_prompt =
-     self._rawdog_instance.intro_prompt # Initialize the selected AI model
- self._ai_model = self._get_ai_model() def _get_ai_model(self): """ Determines
- the appropriate AI model based on the selected provider, including automatic
-   provider selection and g4fauto support. """ if self._selected_provider ==
-      "g4fauto": # Automatically select the best provider from g4f test =
-  TestProviders(quiet=self._suppress_output, timeout=self._timeout) g4fauto =
-  test.best if not self._ignore_working else test.auto if isinstance(g4fauto,
-     str): self._selected_provider = "g4fauto+" + g4fauto self._ai_model =
-self._create_g4f_model(g4fauto) else: raise Exception( "No working g4f provider
- found. " "Consider running 'webscout.webai gpt4free test -y' first" ) else: #
-     Use the specified provider self._ai_model = self._ai_provider_mapping
-    [self._selected_provider]( is_conversation=self._conversation_enabled,
-max_tokens=self._max_tokens, timeout=self._timeout, intro=self._initial_prompt,
-    filepath=self._history_filepath, update_file=self._update_history_file,
-               proxies={}, # Load proxies from config if needed
-    history_offset=self._history_offset, act=self._awesome_prompt_content,
-          model=self._selected_model, quiet=self._suppress_output, #
- auth=self._auth_token, # Pass API key if required ) return self._ai_model def
-_create_g4f_model(self, provider: str): """ Creates a g4f model instance using
-      the provided provider and webscout.WEBS for web search. """ return
-       webscout.g4f.GPT4FREE( provider=provider, auth=self._auth_token,
-  max_tokens=self._max_tokens, chat_completion=self._chat_completion_enabled,
-          ignore_working=self._ignore_working, timeout=self._timeout,
-         intro=self._initial_prompt, filepath=self._history_filepath,
- update_file=self._update_history_file, proxies={}, # Load proxies from config
-                if needed history_offset=self._history_offset,
-   act=self._awesome_prompt_content, ) def process_query(self, query: str) -
- > None: """ Processes a user query, potentially enhancing it with web search
- results, passing it to the AI model, and handling the response. Args: query:
- The user's text input. Returns: None """ if self._web_search_enabled: query =
-    self._augment_query_with_web_search(query) # Apply code optimization if
-           configured if self._selected_optimizer == "code": query =
-webscout.AIutel.Optimizers.code(query) try: response: str = self._ai_model.chat
-    (query) except webscout.exceptions.FailedToGenerateResponseError as e:
- self._console.print(Markdown(f"LLM: [red]{e}[/red]")) return # Handle Rawdog
-  responses if enabled if self._rawdog_enabled: self._handle_rawdog_response
-    (response) else: self._console.print(Markdown(f"LLM: {response}")) def
-  _augment_query_with_web_search(self, query: str) -> str: """Performs a web
-   search and appends the results to the query. Args: query: The user's text
-     input. Returns: str: The augmented query with web search results. """
-      web_search_results = webscout.WEBS().text(query, max_results=3) if
-web_search_results: formatted_results = "\n".join( f"{i+1}. {result['title']} -
-    {result['href']}\n\nBody: {result['body']}" for i, result in enumerate
-     (web_search_results) ) query += f"\n\n## Web Search Results are:\n\n
- {formatted_results}" return query def _handle_rawdog_response(self, response:
-str) -> None: """Handles AI responses, potentially executing them as code with
-    Rawdog. Args: response: The AI model's response. Returns: None """ try:
-   is_feedback = self._rawdog_instance.main(response) except Exception as e:
-    self._console.print(Markdown(f"LLM: [red]Error: {e}[/red]")) return if
-    is_feedback: self._console.print(Markdown(f"LLM: {is_feedback}")) else:
-self._console.print(Markdown("LLM: (Script executed successfully)")) async def
- process_async_query(self, query: str) -> None: """ Asynchronously processes a
-user query, potentially enhancing it with web search results, passing it to the
-   AI model, and handling the response. Args: query: The user's text input.
-            Returns: None """ if self._web_search_enabled: query =
-    self._augment_query_with_web_search(query) # Apply code optimization if
-           configured if self._selected_optimizer == "code": query =
-webscout.AIutel.Optimizers.code(query) async_model = self._get_async_ai_model()
-       try: async for response in async_model.chat(query, stream=True):
-       self._console.print(Markdown(f"LLM: {response}"), end="") except
-  webscout.exceptions.FailedToGenerateResponseError as e: self._console.print
-(Markdown(f"LLM: [red]{e}[/red]")) return # Handle Rawdog responses if enabled
-     if self._rawdog_enabled: self._handle_rawdog_response(response) else:
-   self._console.print(Markdown(f"LLM: {response}")) def _get_async_ai_model
-   (self): """ Determines the appropriate asynchronous AI model based on the
-selected provider. """ if self._selected_provider == "g4fauto": # Automatically
-            select the best provider from g4f test = TestProviders
-(quiet=self._suppress_output, timeout=self._timeout) g4fauto = test.best if not
-       self._ignore_working else test.auto if isinstance(g4fauto, str):
-        self._selected_provider = "g4fauto+" + g4fauto self._ai_model =
- self._create_async_g4f_model(g4fauto) else: raise Exception( "No working g4f
-provider found. " "Consider running 'webscout gpt4free test -y' first" ) else:
-# Use the specified provider if self._selected_provider in async_provider_map:
-         self._ai_model = async_provider_map[self._selected_provider]
-  ( is_conversation=self._conversation_enabled, max_tokens=self._max_tokens,
-              timeout=self._timeout, intro=self._initial_prompt,
-    filepath=self._history_filepath, update_file=self._update_history_file,
-               proxies={}, # Load proxies from config if needed
-    history_offset=self._history_offset, act=self._awesome_prompt_content,
-model=self._selected_model, quiet=self._suppress_output, auth=self._auth_token,
- # Pass API key if required ) else: raise Exception( f"Asynchronous provider '
- {self._selected_provider}' is not yet supported" ) return self._ai_model def
- _create_async_g4f_model(self, provider: str): """ Creates an asynchronous g4f
- model instance using the provided provider and webscout.WEBS for web search.
-           """ return webscout.g4f.AsyncGPT4FREE( provider=provider,
-              auth=self._auth_token, max_tokens=self._max_tokens,
-                chat_completion=self._chat_completion_enabled,
-          ignore_working=self._ignore_working, timeout=self._timeout,
-         intro=self._initial_prompt, filepath=self._history_filepath,
- update_file=self._update_history_file, proxies={}, # Load proxies from config
-                if needed history_offset=self._history_offset,
-  act=self._awesome_prompt_content, ) if __name__ == "__main__": assistant =
-     TaskExecutor() while True: input_query = input("Enter your query: ")
-  assistant.process_query(input_query) ``` ```shell python -m webscout.webai
-                     webai --provider "phind" --rawdog ```
+ response") ``` ## `Webai` - terminal gpt and a open interpeter ```python from
+  webscout.webai import Main def use_rawdog_with_webai(prompt): """ Wrap the
+webscout default method in a try-except block to catch any unhandled exceptions
+    and print a helpful message. """ try: webai_bot = Main( max_tokens=500,
+  provider="cohere", temperature=0.7, top_k=40, top_p=0.95, model="command-r-
+ plus", # Replace with your desired model auth=None, # Replace with your auth
+  key/value (if needed) timeout=30, disable_conversation=True, filepath=None,
+       update_file=True, intro=None, rawdog=True, history_offset=10250,
+      awesome_prompt=None, proxy_path=None, quiet=True ) webai_response =
+webai_bot.default(prompt) except Exception as e: print("Unexpected error:", e)
+     if __name__ == "__main__": user_prompt = input("Enter your prompt: ")
+use_rawdog_with_webai(user_prompt) ``` ```shell python -m webscout.webai webai
+                        --provider "phind" --rawdog ```
                _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
                           _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
                        _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
```

### Comparing `webscout-3.0/README.md` & `webscout-3.0b0/webscout.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,72 @@
+Metadata-Version: 2.1
+Name: webscout
+Version: 3.0b0
+Summary: Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs
+Author: OEvortex
+Author-email: helpingai5@gmail.com
+License: HelpingAI Simplified Universal License
+Project-URL: Documentation, https://github.com/OE-LUCIFER/Webscout/wiki
+Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
+Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues
+Project-URL: YouTube, https://youtube.com/@OEvortex
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: Other/Proprietary License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: docstring_inheritance
+Requires-Dist: click
+Requires-Dist: curl_cffi
+Requires-Dist: lxml
+Requires-Dist: nest-asyncio
+Requires-Dist: selenium
+Requires-Dist: tqdm
+Requires-Dist: webdriver-manager
+Requires-Dist: halo>=0.0.31
+Requires-Dist: g4f>=0.2.2.3
+Requires-Dist: rich
+Requires-Dist: python-dotenv
+Requires-Dist: beautifulsoup4
+Requires-Dist: markdownify
+Requires-Dist: pydantic
+Requires-Dist: requests
+Requires-Dist: sse_starlette
+Requires-Dist: termcolor
+Requires-Dist: tiktoken
+Requires-Dist: tldextract
+Requires-Dist: orjson
+Requires-Dist: PyYAML
+Requires-Dist: appdirs
+Requires-Dist: GoogleBard1>=2.1.4
+Requires-Dist: tls_client
+Requires-Dist: clipman
+Requires-Dist: Helpingai-T2
+Requires-Dist: playsound
+Requires-Dist: poe_api_wrapper
+Requires-Dist: pyreqwest_impersonate
+Provides-Extra: dev
+Requires-Dist: ruff>=0.1.6; extra == "dev"
+Requires-Dist: pytest>=7.4.2; extra == "dev"
+Provides-Extra: local
+Requires-Dist: llama-cpp-python; extra == "local"
+Requires-Dist: colorama; extra == "local"
+Requires-Dist: numpy; extra == "local"
+Requires-Dist: huggingface_hub; extra == "local"
+
 <div align="center">
   <!-- Replace `#` with your actual links -->
   <a href="https://t.me/devsdocode"><img alt="Telegram" src="https://img.shields.io/badge/Telegram-2CA5E0?style=for-the-badge&logo=telegram&logoColor=white"></a>
   <a href="https://www.instagram.com/sree.shades_/"><img alt="Instagram" src="https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white"></a>
   <a href="https://www.linkedin.com/in/developer-sreejan/"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white"></a>
   <a href="https://buymeacoffee.com/oevortex"><img alt="Buy Me A Coffee" src="https://img.shields.io/badge/Buy%20Me%20A%20Coffee-FFDD00?style=for-the-badge&logo=buymeacoffee&logoColor=black"></a>
 </div>
@@ -73,15 +138,14 @@
     - [12. `Xjai` - chat with free gpt 3.5](#12-xjai---chat-with-free-gpt-35)
     - [13. `ThinkAny` - AI search engine](#13-thinkany---ai-search-engine)
     - [14. `chatgptuk` - Chat with gemini-pro](#14-chatgptuk---chat-with-gemini-pro)
     - [15. `poe`- chat with poe](#15-poe--chat-with-poe)
     - [16. `BasedGPT` - chat with GPT](#16-basedgpt---chat-with-gpt)
     - [`LLM`](#llm)
     - [`Local-LLM` webscout can now run GGUF models](#local-llm-webscout-can-now-run-gguf-models)
-    - [`Function-calling-local-llm`](#function-calling-local-llm)
     - [`LLM` with internet](#llm-with-internet)
     - [LLM with deepwebs](#llm-with-deepwebs)
   - [`Webai` - terminal gpt and a open interpeter](#webai---terminal-gpt-and-a-open-interpeter)
 
 ## Install
 ```python
 pip install -U webscout
@@ -1195,86 +1259,14 @@
 
 # 3. Create a Thread for conversation
 thread = Thread(model, formats.phi3)
 
 # 4. Start interacting with the model
 thread.interact()
 ```
-### `Function-calling-local-llm`
-```python
-from webscout.Local import Model, Thread, formats
-from webscout import DeepWEBS
-from webscout.Local.utils import download_model
-from webscout.Local.model import Model
-from webscout.Local.thread import Thread
-from webscout.Local import formats
-from webscout.Local.samplers import SamplerSettings
-def deepwebs_search(query, max_results=5):
-    """Performs a web search using DeepWEBS and returns results as JSON."""
-    deepwebs = DeepWEBS()
-    search_config = DeepWEBS.DeepSearch(
-        queries=[query],
-        max_results=max_results,
-        extract_webpage=False,
-        safe=False,
-        types=["web"],
-        overwrite_query_html=True,
-        overwrite_webpage_html=True,
-    )
-    search_results = deepwebs.queries_to_search_results(search_config)
-    formatted_results = []
-    for result in search_results[0]:  # Assuming only one query
-        formatted_results.append(f"Title: {result['title']}\nURL: {result['url']}\n")
-    return "\n".join(formatted_results)
-
-# Load your model
-repo_id = "OEvortex/HelpingAI-9B" 
-filename = "helpingai-9b.Q4_0.gguf"
-model_path = download_model(repo_id, filename, token='')
-
-# 2. Load the model 
-model = Model(model_path, n_gpu_layers=10)
-
-# Create a Thread
-system_prompt = "You are a helpful AI assistant. Respond to user queries concisely. If a user asks for information that requires a web search, use the `deepwebs_search` tool. Do not call the tool if it is not necessary."
-sampler = SamplerSettings(temp=0.7, top_p=0.9)  # Adjust these values as needed
-# 4. Create a custom chatml format with your system prompt
-custom_chatml = formats.chatml.copy()
-custom_chatml['system_content'] = system_prompt
-thread = Thread(model, custom_chatml, sampler=sampler)
-# Add the deepwebs_search tool
-thread.add_tool({
-    "type": "function",
-    "function": {
-        "name": "deepwebs_search",
-        "description": "Performs a web search using DeepWEBS and returns the title and URLs of the results.",
-        "execute": deepwebs_search,
-        "parameters": {
-            "type": "object",
-            "properties": {
-                "query": {
-                    "type": "string",
-                    "description": "The query to search on the web",
-                },
-                "max_results": {
-                    "type": "integer",
-                    "description": "Maximum number of search results (default: 5)",
-                },
-            },
-            "required": ["query"],
-        },
-    },
-})
-
-# Start interacting with the model
-while True:
-    user_input = input("You: ")
-    response = thread.send(user_input)
-    print("Bot: ", response) 
-```
 ### `LLM` with internet
 ```python
 from __future__ import annotations
 from typing import List, Optional
 
 from webscout.LLM import LLM
 from webscout import WEBS
@@ -1431,324 +1423,49 @@
             print("AI:", response)
         else:
             print("No response")
 ```
 ## `Webai` - terminal gpt and a open interpeter
 
 ```python
-import time
-import uuid
-from typing import Dict, Any, Optional, AsyncGenerator
-from rich.console import Console
-from rich.markdown import Markdown
-from rich.panel import Panel
-from rich.style import Style
-import webscout
-import webscout.AIutel
-import g4f
-from webscout.g4f import *
-from webscout.async_providers import mapper as async_provider_map
+from webscout.webai import Main
 
-class TaskExecutor:
+def use_rawdog_with_webai(prompt):
     """
-    Manages an interactive chat session, handling user input, AI responses, 
-    and optional features like web search, code execution, and text-to-speech.
+    Wrap the webscout default method in a try-except block to catch any unhandled
+    exceptions and print a helpful message.
     """
-
-    def __init__(self) -> None:
-        """Initializes the conversational assistant with default settings."""
-        self._console: Console = Console()
-
-        # Session configuration
-        self._selected_provider: str = "phind"
-        self._selected_model: str = "Phind Model"
-        self._conversation_enabled: bool = True
-        self._max_tokens: int = 600
-        self._temperature: float = 0.2
-        self._top_k: int = -1
-        self._top_p: float = 0.999
-        self._timeout: int = 30
-        self._auth_token: str = None  # API key, if required
-        self._chat_completion_enabled: bool = True  # g4fauto
-        self._ignore_working: bool = False  # Ignore working status of providers
-        self._proxy_path: str = None  # Path to proxy configuration
-
-        # History Management
-        self._history_filepath: str = None
-        self._update_history_file: bool = True
-        self._history_offset: int = 10250
-
-        # Prompt Engineering
-        self._initial_prompt: str = None
-        self._awesome_prompt_content: str = None 
-
-        # Optional Features
-        self._web_search_enabled: bool = False  # Enable web search
-        self._rawdog_enabled: bool = True
-        self._internal_script_execution_enabled: bool = False
-        self._script_confirmation_required: bool = False
-        self._selected_interpreter: str = "python"
-        self._selected_optimizer: str = "code"
-        self._suppress_output: bool = False  # Suppress verbose output
-
-        # AI provider mapping
-        self._ai_provider_mapping: Dict[str, Any] = {
-            "phind": webscout.PhindSearch,
-            "opengpt": webscout.OPENGPT,
-            "koboldai": webscout.KOBOLDAI,
-            "blackboxai": webscout.BLACKBOXAI,
-            "llama2": webscout.LLAMA2,
-            "yepchat": webscout.YEPCHAT,
-            "leo": webscout.LEO,
-            "groq": webscout.GROQ,
-            "openai": webscout.OPENAI,
-            "perplexity": webscout.PERPLEXITY,
-            "you": webscout.YouChat,
-            "xjai": webscout.Xjai,
-            "cohere": webscout.Cohere,
-            "reka": webscout.REKA,
-            "thinkany": webscout.ThinkAnyAI,
-            "gemini": webscout.GEMINI, 
-            "berlin4h": webscout.Berlin4h,
-            "chatgptuk": webscout.ChatGPTUK,
-            "poe": webscout.POE,
-            "basedgpt": webscout.BasedGPT,
-        }
-
-        # Initialize Rawdog if enabled
-        if self._rawdog_enabled:
-            self._rawdog_instance: webscout.AIutel.RawDog = webscout.AIutel.RawDog(
-                quiet=self._suppress_output,
-                internal_exec=self._internal_script_execution_enabled,
-                confirm_script=self._script_confirmation_required,
-                interpreter=self._selected_interpreter,
-            )
-
-            self._initial_prompt = self._rawdog_instance.intro_prompt
-
-        # Initialize the selected AI model 
-        self._ai_model = self._get_ai_model()
-
-    def _get_ai_model(self):
-        """
-        Determines the appropriate AI model based on the selected provider, 
-        including automatic provider selection and g4fauto support.
-        """
-        if self._selected_provider == "g4fauto":
-            # Automatically select the best provider from g4f
-            test = TestProviders(quiet=self._suppress_output, timeout=self._timeout)
-            g4fauto = test.best if not self._ignore_working else test.auto
-            if isinstance(g4fauto, str):
-                self._selected_provider = "g4fauto+" + g4fauto
-                self._ai_model = self._create_g4f_model(g4fauto)
-            else:
-                raise Exception(
-                    "No working g4f provider found. "
-                    "Consider running 'webscout.webai gpt4free test -y' first"
-                )
-        else:
-            # Use the specified provider
-            self._ai_model = self._ai_provider_mapping[self._selected_provider](
-                is_conversation=self._conversation_enabled,
-                max_tokens=self._max_tokens,
-                timeout=self._timeout,
-                intro=self._initial_prompt,
-                filepath=self._history_filepath,
-                update_file=self._update_history_file,
-                proxies={},  # Load proxies from config if needed
-                history_offset=self._history_offset,
-                act=self._awesome_prompt_content, 
-                model=self._selected_model,
-                quiet=self._suppress_output,
-                # auth=self._auth_token,  # Pass API key if required
-            )
-        return self._ai_model
-
-    def _create_g4f_model(self, provider: str):
-        """
-        Creates a g4f model instance using the provided provider and webscout.WEBS for web search.
-        """
-        return webscout.g4f.GPT4FREE(
-            provider=provider,
-            auth=self._auth_token,
-            max_tokens=self._max_tokens,
-            chat_completion=self._chat_completion_enabled,
-            ignore_working=self._ignore_working,
-            timeout=self._timeout,
-            intro=self._initial_prompt,
-            filepath=self._history_filepath,
-            update_file=self._update_history_file,
-            proxies={},  # Load proxies from config if needed
-            history_offset=self._history_offset,
-            act=self._awesome_prompt_content, 
+    try:
+        webai_bot = Main(
+            max_tokens=500, 
+            provider="cohere",
+            temperature=0.7,  
+            top_k=40,          
+            top_p=0.95,        
+            model="command-r-plus",  # Replace with your desired model
+            auth=None,     # Replace with your auth key/value (if needed)
+            timeout=30,
+            disable_conversation=True,
+            filepath=None,
+            update_file=True,
+            intro=None,
+            rawdog=True,
+            history_offset=10250,
+            awesome_prompt=None,
+            proxy_path=None,
+            quiet=True
         )
+        webai_response = webai_bot.default(prompt) 
+    except Exception as e:
+        print("Unexpected error:", e)
 
-    def process_query(self, query: str) -> None:
-        """
-        Processes a user query, potentially enhancing it with web search results, 
-        passing it to the AI model, and handling the response.
-
-        Args:
-            query: The user's text input.
-
-        Returns:
-            None
-        """
-        if self._web_search_enabled:
-            query = self._augment_query_with_web_search(query)
-
-        # Apply code optimization if configured
-        if self._selected_optimizer == "code":
-            query = webscout.AIutel.Optimizers.code(query)
-
-        try:
-            response: str = self._ai_model.chat(query)
-        except webscout.exceptions.FailedToGenerateResponseError as e:
-            self._console.print(Markdown(f"LLM: [red]{e}[/red]"))
-            return
-
-        # Handle Rawdog responses if enabled
-        if self._rawdog_enabled:
-            self._handle_rawdog_response(response)
-        else:
-            self._console.print(Markdown(f"LLM: {response}"))
-
-    def _augment_query_with_web_search(self, query: str) -> str:
-        """Performs a web search and appends the results to the query.
-
-        Args:
-            query: The user's text input.
-
-        Returns:
-            str: The augmented query with web search results.
-        """
-        web_search_results = webscout.WEBS().text(query, max_results=3)
-        if web_search_results:
-            formatted_results = "\n".join(
-                f"{i+1}. {result['title']} - {result['href']}\n\nBody: {result['body']}"
-                for i, result in enumerate(web_search_results)
-            )
-            query += f"\n\n## Web Search Results are:\n\n{formatted_results}"
-        return query
-
-    def _handle_rawdog_response(self, response: str) -> None:
-        """Handles AI responses, potentially executing them as code with Rawdog.
-
-        Args:
-            response: The AI model's response.
-
-        Returns:
-            None
-        """
-        try:
-            is_feedback = self._rawdog_instance.main(response)
-        except Exception as e:
-            self._console.print(Markdown(f"LLM: [red]Error: {e}[/red]"))
-            return
-        if is_feedback:
-            self._console.print(Markdown(f"LLM: {is_feedback}"))
-        else:
-            self._console.print(Markdown("LLM: (Script executed successfully)"))
-
-    async def process_async_query(self, query: str) -> None:
-        """
-        Asynchronously processes a user query, potentially enhancing it with web search results, 
-        passing it to the AI model, and handling the response.
-
-        Args:
-            query: The user's text input.
-
-        Returns:
-            None
-        """
-        if self._web_search_enabled:
-            query = self._augment_query_with_web_search(query)
-
-        # Apply code optimization if configured
-        if self._selected_optimizer == "code":
-            query = webscout.AIutel.Optimizers.code(query)
-
-        async_model = self._get_async_ai_model()
-
-        try:
-            async for response in async_model.chat(query, stream=True):
-                self._console.print(Markdown(f"LLM: {response}"), end="")
-        except webscout.exceptions.FailedToGenerateResponseError as e:
-            self._console.print(Markdown(f"LLM: [red]{e}[/red]"))
-            return
-
-        # Handle Rawdog responses if enabled
-        if self._rawdog_enabled:
-            self._handle_rawdog_response(response)
-        else:
-            self._console.print(Markdown(f"LLM: {response}"))
-
-    def _get_async_ai_model(self):
-        """
-        Determines the appropriate asynchronous AI model based on the selected provider.
-        """
-        if self._selected_provider == "g4fauto":
-            # Automatically select the best provider from g4f
-            test = TestProviders(quiet=self._suppress_output, timeout=self._timeout)
-            g4fauto = test.best if not self._ignore_working else test.auto
-            if isinstance(g4fauto, str):
-                self._selected_provider = "g4fauto+" + g4fauto
-                self._ai_model = self._create_async_g4f_model(g4fauto)
-            else:
-                raise Exception(
-                    "No working g4f provider found. "
-                    "Consider running 'webscout gpt4free test -y' first"
-                )
-        else:
-            # Use the specified provider
-            if self._selected_provider in async_provider_map:
-                self._ai_model = async_provider_map[self._selected_provider](
-                    is_conversation=self._conversation_enabled,
-                    max_tokens=self._max_tokens,
-                    timeout=self._timeout,
-                    intro=self._initial_prompt,
-                    filepath=self._history_filepath,
-                    update_file=self._update_history_file,
-                    proxies={},  # Load proxies from config if needed
-                    history_offset=self._history_offset,
-                    act=self._awesome_prompt_content, 
-                    model=self._selected_model,
-                    quiet=self._suppress_output,
-                    auth=self._auth_token,  # Pass API key if required
-                )
-            else:
-                raise Exception(
-                    f"Asynchronous provider '{self._selected_provider}' is not yet supported"
-                )
-        return self._ai_model
-
-    def _create_async_g4f_model(self, provider: str):
-        """
-        Creates an asynchronous g4f model instance using the provided provider and webscout.WEBS for web search.
-        """
-        return webscout.g4f.AsyncGPT4FREE(
-            provider=provider,
-            auth=self._auth_token,
-            max_tokens=self._max_tokens,
-            chat_completion=self._chat_completion_enabled,
-            ignore_working=self._ignore_working,
-            timeout=self._timeout,
-            intro=self._initial_prompt,
-            filepath=self._history_filepath,
-            update_file=self._update_history_file,
-            proxies={},  # Load proxies from config if needed
-            history_offset=self._history_offset,
-            act=self._awesome_prompt_content,
-        )
 
 if __name__ == "__main__":
-    assistant = TaskExecutor()
-    while True:
-        input_query = input("Enter your query: ")
-        assistant.process_query(input_query)
+    user_prompt = input("Enter your prompt: ")
+    use_rawdog_with_webai(user_prompt)
 
 ```
 ```shell
 python -m webscout.webai webai --provider "phind" --rawdog
 ```
 
 <div align="center">
```

#### html2text {}

```diff
@@ -1,7 +1,41 @@
+Metadata-Version: 2.1 Name: webscout Version: 3.0b0 Summary: Search for
+anything using Google, DuckDuckGo, phind.com, Contains AI models, can
+transcribe yt videos, temporary email and phone number generation, has TTS
+support, webai (terminal gpt and open interpreter) and offline LLMs Author:
+OEvortex Author-email: helpingai5@gmail.com License: HelpingAI Simplified
+Universal License Project-URL: Documentation, https://github.com/OE-LUCIFER/
+Webscout/wiki Project-URL: Source, https://github.com/OE-LUCIFER/Webscout
+Project-URL: Tracker, https://github.com/OE-LUCIFER/Webscout/issues Project-
+URL: YouTube, https://youtube.com/@OEvortex Classifier: Development Status :: 5
+- Production/Stable Classifier: Intended Audience :: Developers Classifier:
+License :: Other/Proprietary License Classifier: Operating System :: OS
+Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Classifier: Programming Language ::
+Python :: 3.12 Classifier: Programming Language :: Python :: Implementation ::
+CPython Classifier: Topic :: Internet :: WWW/HTTP :: Indexing/Search
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Description-Content-Type: text/markdown License-File: LICENSE.md Requires-Dist:
+docstring_inheritance Requires-Dist: click Requires-Dist: curl_cffi Requires-
+Dist: lxml Requires-Dist: nest-asyncio Requires-Dist: selenium Requires-Dist:
+tqdm Requires-Dist: webdriver-manager Requires-Dist: halo>=0.0.31 Requires-
+Dist: g4f>=0.2.2.3 Requires-Dist: rich Requires-Dist: python-dotenv Requires-
+Dist: beautifulsoup4 Requires-Dist: markdownify Requires-Dist: pydantic
+Requires-Dist: requests Requires-Dist: sse_starlette Requires-Dist: termcolor
+Requires-Dist: tiktoken Requires-Dist: tldextract Requires-Dist: orjson
+Requires-Dist: PyYAML Requires-Dist: appdirs Requires-Dist: GoogleBard1>=2.1.4
+Requires-Dist: tls_client Requires-Dist: clipman Requires-Dist: Helpingai-T2
+Requires-Dist: playsound Requires-Dist: poe_api_wrapper Requires-Dist:
+pyreqwest_impersonate Provides-Extra: dev Requires-Dist: ruff>=0.1.6; extra ==
+"dev" Requires-Dist: pytest>=7.4.2; extra == "dev" Provides-Extra: local
+Requires-Dist: llama-cpp-python; extra == "local" Requires-Dist: colorama;
+extra == "local" Requires-Dist: numpy; extra == "local" Requires-Dist:
+huggingface_hub; extra == "local"
                _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
                           _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
                        _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
 # WEBSCOUT
                              [WebScout API Badge]
    _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]Search for anything using Google, DuckDuckGo,
  phind.com, Contains AI models, can transcribe yt videos, temporary email and
@@ -41,86 +75,86 @@
 chat with reka](#10-reka---chat-with-reka) - [11. `Cohere` - chat with cohere]
  (#11-cohere---chat-with-cohere) - [12. `Xjai` - chat with free gpt 3.5](#12-
    xjai---chat-with-free-gpt-35) - [13. `ThinkAny` - AI search engine](#13-
  thinkany---ai-search-engine) - [14. `chatgptuk` - Chat with gemini-pro](#14-
  chatgptuk---chat-with-gemini-pro) - [15. `poe`- chat with poe](#15-poe--chat-
  with-poe) - [16. `BasedGPT` - chat with GPT](#16-basedgpt---chat-with-gpt) -
   [`LLM`](#llm) - [`Local-LLM` webscout can now run GGUF models](#local-llm-
- webscout-can-now-run-gguf-models) - [`Function-calling-local-llm`](#function-
-  calling-local-llm) - [`LLM` with internet](#llm-with-internet) - [LLM with
-deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt and a open interpeter]
-(#webai---terminal-gpt-and-a-open-interpeter) ## Install ```python pip install
-   -U webscout ``` ## CLI version ```python3 python -m webscout --help ``` |
-Command | Description | |-------------------------------------------|----------
+webscout-can-now-run-gguf-models) - [`LLM` with internet](#llm-with-internet) -
+ [LLM with deepwebs](#llm-with-deepwebs) - [`Webai` - terminal gpt and a open
+ interpeter](#webai---terminal-gpt-and-a-open-interpeter) ## Install ```python
+pip install -U webscout ``` ## CLI version ```python3 python -m webscout --help
+``` | Command | Description | |-------------------------------------------|----
 -------------------------------------------------------------------------------
---------------| | python -m webscout answers -k Text | CLI function to perform
- an answers search using Webscout. | | python -m webscout images -k Text | CLI
-  function to perform an images search using Webscout. | | python -m webscout
-maps -k Text | CLI function to perform a maps search using Webscout. | | python
-    -m webscout news -k Text | CLI function to perform a news search using
-Webscout. | | python -m webscout suggestions -k Text | CLI function to perform
-a suggestions search using Webscout. | | python -m webscout text -k Text | CLI
-   function to perform a text search using Webscout. | | python -m webscout
-   translate -k Text | CLI function to perform translate using Webscout. | |
- python -m webscout version | A command-line interface command that prints and
-returns the version of the program. | | python -m webscout videos -k Text | CLI
- function to perform a videos search using DuckDuckGo API. | [Go To TOP](#TOP)
- ## Regions expand xa-ar for Arabia xa-en for Arabia (en) ar-es for Argentina
-au-en for Australia at-de for Austria be-fr for Belgium (fr) be-nl for Belgium
-(nl) br-pt for Brazil bg-bg for Bulgaria ca-en for Canada ca-fr for Canada (fr)
-ct-ca for Catalan cl-es for Chile cn-zh for China co-es for Colombia hr-hr for
-Croatia cz-cs for Czech Republic dk-da for Denmark ee-et for Estonia fi-fi for
-  Finland fr-fr for France de-de for Germany gr-el for Greece hk-tzh for Hong
-Kong hu-hu for Hungary in-en for India id-id for Indonesia id-en for Indonesia
- (en) ie-en for Ireland il-he for Israel it-it for Italy jp-jp for Japan kr-kr
- for Korea lv-lv for Latvia lt-lt for Lithuania xl-es for Latin America my-ms
-for Malaysia my-en for Malaysia (en) mx-es for Mexico nl-nl for Netherlands nz-
-en for New Zealand no-no for Norway pe-es for Peru ph-en for Philippines ph-tl
-for Philippines (tl) pl-pl for Poland pt-pt for Portugal ro-ro for Romania ru-
-ru for Russia sg-en for Singapore sk-sk for Slovak Republic sl-sl for Slovenia
-za-en for South Africa es-es for Spain se-sv for Sweden ch-de for Switzerland
- (de) ch-fr for Switzerland (fr) ch-it for Switzerland (it) tw-tzh for Taiwan
-th-th for Thailand tr-tr for Turkey ua-uk for Ukraine uk-en for United Kingdom
-us-en for United States ue-es for United States (es) ve-es for Venezuela vn-vi
-  for Vietnam wt-wt for No region ___ [Go To TOP](#TOP) ## Tempmail and Temp
-number ### Temp number ```python from rich.console import Console from webscout
-             import tempid def main(): console = Console() phone =
-    tempid.TemporaryPhoneNumber() try: # Get a temporary phone number for a
-   specific country (or random) number = phone.get_number(country="Finland")
-console.print(f"Your temporary phone number: [bold cyan]{number}[/bold cyan]")
-# Pause execution briefly (replace with your actual logic) # import time module
- import time time.sleep(30) # Adjust the waiting time as needed # Retrieve and
-  print messages messages = phone.get_messages(number) if messages: # Access
-   individual messages using indexing: console.print(f"[bold green]{messages
- [0].frm}:[/] {messages[0].content}") # (Add more lines if you expect multiple
- messages) else: console.print("No messages received.") except Exception as e:
- console.print(f"[bold red]An error occurred: {e}") if __name__ == "__main__":
-   main() ``` ### Tempmail ```python import asyncio from rich.console import
- Console from rich.table import Table from rich.text import Text from webscout
-     import tempid async def main() -> None: console = Console() client =
-   tempid.Client() try: domains = await client.get_domains() if not domains:
-console.print("[bold red]No domains available. Please try again later.") return
-email = await client.create_email(domain=domains[0].name) console.print(f"Your
- temporary email: [bold cyan]{email.email}[/bold cyan]") console.print(f"Token
-  for accessing the email: [bold cyan]{email.token}[/bold cyan]") while True:
-  messages = await client.get_messages(email.email) if messages is not None:
-break if messages: table = Table(show_header=True, header_style="bold magenta")
-    table.add_column("From", style="bold cyan") table.add_column("Subject",
- style="bold yellow") table.add_column("Body", style="bold green") for message
- in messages: body_preview = Text(message.body_text if message.body_text else
- "No body") table.add_row(message.email_from or "Unknown", message.subject or
-   "No Subject", body_preview) console.print(table) else: console.print("No
-  messages found.") except Exception as e: console.print(f"[bold red]An error
-   occurred: {e}") finally: await client.close() if __name__ == '__main__':
-asyncio.run(main()) ``` ## Transcriber The transcriber function in webscout is
-     a handy tool that transcribes YouTube videos. Here's an example code
-demonstrating its usage: ```python import sys from webscout import transcriber
-  def extract_transcript(video_id): """Extracts the transcript from a YouTube
-  video.""" try: transcript_list = transcriber.list_transcripts(video_id) for
-transcript in transcript_list: transcript_data_list = transcript.fetch() lang =
+ --------------------| | python -m webscout answers -k Text | CLI function to
+perform an answers search using Webscout. | | python -m webscout images -k Text
+    | CLI function to perform an images search using Webscout. | | python -
+m webscout maps -k Text | CLI function to perform a maps search using Webscout.
+  | | python -m webscout news -k Text | CLI function to perform a news search
+ using Webscout. | | python -m webscout suggestions -k Text | CLI function to
+  perform a suggestions search using Webscout. | | python -m webscout text -
+  k Text | CLI function to perform a text search using Webscout. | | python -
+    m webscout translate -k Text | CLI function to perform translate using
+  Webscout. | | python -m webscout version | A command-line interface command
+  that prints and returns the version of the program. | | python -m webscout
+videos -k Text | CLI function to perform a videos search using DuckDuckGo API.
+ | [Go To TOP](#TOP) ## Regions expand xa-ar for Arabia xa-en for Arabia (en)
+ ar-es for Argentina au-en for Australia at-de for Austria be-fr for Belgium
+   (fr) be-nl for Belgium (nl) br-pt for Brazil bg-bg for Bulgaria ca-en for
+Canada ca-fr for Canada (fr) ct-ca for Catalan cl-es for Chile cn-zh for China
+co-es for Colombia hr-hr for Croatia cz-cs for Czech Republic dk-da for Denmark
+ ee-et for Estonia fi-fi for Finland fr-fr for France de-de for Germany gr-el
+  for Greece hk-tzh for Hong Kong hu-hu for Hungary in-en for India id-id for
+Indonesia id-en for Indonesia (en) ie-en for Ireland il-he for Israel it-it for
+Italy jp-jp for Japan kr-kr for Korea lv-lv for Latvia lt-lt for Lithuania xl-
+   es for Latin America my-ms for Malaysia my-en for Malaysia (en) mx-es for
+ Mexico nl-nl for Netherlands nz-en for New Zealand no-no for Norway pe-es for
+ Peru ph-en for Philippines ph-tl for Philippines (tl) pl-pl for Poland pt-pt
+ for Portugal ro-ro for Romania ru-ru for Russia sg-en for Singapore sk-sk for
+Slovak Republic sl-sl for Slovenia za-en for South Africa es-es for Spain se-sv
+  for Sweden ch-de for Switzerland (de) ch-fr for Switzerland (fr) ch-it for
+ Switzerland (it) tw-tzh for Taiwan th-th for Thailand tr-tr for Turkey ua-uk
+ for Ukraine uk-en for United Kingdom us-en for United States ue-es for United
+ States (es) ve-es for Venezuela vn-vi for Vietnam wt-wt for No region ___ [Go
+   To TOP](#TOP) ## Tempmail and Temp number ### Temp number ```python from
+ rich.console import Console from webscout import tempid def main(): console =
+ Console() phone = tempid.TemporaryPhoneNumber() try: # Get a temporary phone
+      number for a specific country (or random) number = phone.get_number
+ (country="Finland") console.print(f"Your temporary phone number: [bold cyan]
+  {number}[/bold cyan]") # Pause execution briefly (replace with your actual
+  logic) # import time module import time time.sleep(30) # Adjust the waiting
+  time as needed # Retrieve and print messages messages = phone.get_messages
+      (number) if messages: # Access individual messages using indexing:
+ console.print(f"[bold green]{messages[0].frm}:[/] {messages[0].content}") #
+   (Add more lines if you expect multiple messages) else: console.print("No
+messages received.") except Exception as e: console.print(f"[bold red]An error
+ occurred: {e}") if __name__ == "__main__": main() ``` ### Tempmail ```python
+ import asyncio from rich.console import Console from rich.table import Table
+   from rich.text import Text from webscout import tempid async def main() -
+   > None: console = Console() client = tempid.Client() try: domains = await
+   client.get_domains() if not domains: console.print("[bold red]No domains
+ available. Please try again later.") return email = await client.create_email
+  (domain=domains[0].name) console.print(f"Your temporary email: [bold cyan]
+  {email.email}[/bold cyan]") console.print(f"Token for accessing the email:
+      [bold cyan]{email.token}[/bold cyan]") while True: messages = await
+ client.get_messages(email.email) if messages is not None: break if messages:
+ table = Table(show_header=True, header_style="bold magenta") table.add_column
+ ("From", style="bold cyan") table.add_column("Subject", style="bold yellow")
+     table.add_column("Body", style="bold green") for message in messages:
+  body_preview = Text(message.body_text if message.body_text else "No body")
+table.add_row(message.email_from or "Unknown", message.subject or "No Subject",
+ body_preview) console.print(table) else: console.print("No messages found.")
+   except Exception as e: console.print(f"[bold red]An error occurred: {e}")
+ finally: await client.close() if __name__ == '__main__': asyncio.run(main())
+ ``` ## Transcriber The transcriber function in webscout is a handy tool that
+  transcribes YouTube videos. Here's an example code demonstrating its usage:
+ ```python import sys from webscout import transcriber def extract_transcript
+     (video_id): """Extracts the transcript from a YouTube video.""" try:
+  transcript_list = transcriber.list_transcripts(video_id) for transcript in
+       transcript_list: transcript_data_list = transcript.fetch() lang =
  transcript.language transcript_text = "" if transcript.language_code == 'en':
     for line in transcript_data_list: start_time = line['start'] end_time =
      start_time + line['duration'] formatted_line = f"{start_time:.2f} -
   {end_time:.2f}: {line['text']}\n" transcript_text += formatted_line return
   transcript_text elif transcript.is_translatable: english_transcript_list =
     transcript.translate('en').fetch() for line in english_transcript_list:
       start_time = line['start'] end_time = start_time + line['duration']
@@ -396,66 +430,35 @@
 webscout.Local.model import Model from webscout.Local.thread import Thread from
 webscout.Local import formats # 1. Download the model repo_id = "microsoft/Phi-
 3-mini-4k-instruct-gguf" # Replace with the desired Hugging Face repo filename
     = "Phi-3-mini-4k-instruct-q4.gguf" # Replace with the correct filename
   model_path = download_model(repo_id, filename) # 2. Load the model model =
 Model(model_path, n_gpu_layers=4) # 3. Create a Thread for conversation thread
       = Thread(model, formats.phi3) # 4. Start interacting with the model
-     thread.interact() ``` ### `Function-calling-local-llm` ```python from
-webscout.Local import Model, Thread, formats from webscout import DeepWEBS from
-  webscout.Local.utils import download_model from webscout.Local.model import
-   Model from webscout.Local.thread import Thread from webscout.Local import
-formats from webscout.Local.samplers import SamplerSettings def deepwebs_search
-  (query, max_results=5): """Performs a web search using DeepWEBS and returns
- results as JSON.""" deepwebs = DeepWEBS() search_config = DeepWEBS.DeepSearch
-( queries=[query], max_results=max_results, extract_webpage=False, safe=False,
-   types=["web"], overwrite_query_html=True, overwrite_webpage_html=True, )
-      search_results = deepwebs.queries_to_search_results(search_config)
-  formatted_results = [] for result in search_results[0]: # Assuming only one
-    query formatted_results.append(f"Title: {result['title']}\nURL: {result
- ['url']}\n") return "\n".join(formatted_results) # Load your model repo_id =
-   "OEvortex/HelpingAI-9B" filename = "helpingai-9b.Q4_0.gguf" model_path =
- download_model(repo_id, filename, token='') # 2. Load the model model = Model
-  (model_path, n_gpu_layers=10) # Create a Thread system_prompt = "You are a
-  helpful AI assistant. Respond to user queries concisely. If a user asks for
-information that requires a web search, use the `deepwebs_search` tool. Do not
-  call the tool if it is not necessary." sampler = SamplerSettings(temp=0.7,
- top_p=0.9) # Adjust these values as needed # 4. Create a custom chatml format
-  with your system prompt custom_chatml = formats.chatml.copy() custom_chatml
-   ['system_content'] = system_prompt thread = Thread(model, custom_chatml,
-   sampler=sampler) # Add the deepwebs_search tool thread.add_tool({ "type":
-"function", "function": { "name": "deepwebs_search", "description": "Performs a
-  web search using DeepWEBS and returns the title and URLs of the results.",
- "execute": deepwebs_search, "parameters": { "type": "object", "properties":
-{ "query": { "type": "string", "description": "The query to search on the web",
-}, "max_results": { "type": "integer", "description": "Maximum number of search
-     results (default: 5)", }, }, "required": ["query"], }, }, }) # Start
- interacting with the model while True: user_input = input("You: ") response =
- thread.send(user_input) print("Bot: ", response) ``` ### `LLM` with internet
-```python from __future__ import annotations from typing import List, Optional
-    from webscout.LLM import LLM from webscout import WEBS import warnings
-system_message: str = ( "As an AI assistant, I have been designed with advanced
- capabilities, including real-time access to online resources. This enables me
-    to enrich our conversations and provide you with informed and accurate
-responses, drawing from a vast array of information. With each interaction, my
- goal is to create a seamless and meaningful connection, offering insights and
-sharing relevant content." "My directives emphasize the importance of respect,
-    impartiality, and intellectual integrity. I am here to provide unbiased
-  responses, ensuring an ethical and respectful exchange. I will respect your
-privacy and refrain from sharing any personal information that may be obtained
-  during our conversations or through web searches, only utilizing web search
-   functionality when necessary to provide the most accurate and up-to-date
- information." "Together, let's explore a diverse range of topics, creating an
-    enjoyable and informative experience, all while maintaining the highest
-     standards of privacy and respect" ) # Ignore the specific UserWarning
- warnings.filterwarnings("ignore", category=UserWarning, module="curl_cffio",
-     lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-Instruct-v0.1",
-     system_message=system_message) def chat( user_input: str, webs: WEBS,
- max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a web
-  search based on the user input and generate a response using the LLM model.
+thread.interact() ``` ### `LLM` with internet ```python from __future__ import
+annotations from typing import List, Optional from webscout.LLM import LLM from
+    webscout import WEBS import warnings system_message: str = ( "As an AI
+assistant, I have been designed with advanced capabilities, including real-time
+  access to online resources. This enables me to enrich our conversations and
+provide you with informed and accurate responses, drawing from a vast array of
+    information. With each interaction, my goal is to create a seamless and
+  meaningful connection, offering insights and sharing relevant content." "My
+directives emphasize the importance of respect, impartiality, and intellectual
+  integrity. I am here to provide unbiased responses, ensuring an ethical and
+ respectful exchange. I will respect your privacy and refrain from sharing any
+ personal information that may be obtained during our conversations or through
+web searches, only utilizing web search functionality when necessary to provide
+   the most accurate and up-to-date information." "Together, let's explore a
+diverse range of topics, creating an enjoyable and informative experience, all
+while maintaining the highest standards of privacy and respect" ) # Ignore the
+ specific UserWarning warnings.filterwarnings("ignore", category=UserWarning,
+  module="curl_cffio", lineno=205) LLM = LLM(model="mistralai/Mixtral-8x22B-
+Instruct-v0.1", system_message=system_message) def chat( user_input: str, webs:
+WEBS, max_results: int = 10 ) -> Optional[str]: """ Chat function to perform a
+web search based on the user input and generate a response using the LLM model.
  Parameters ---------- user_input : str The user input to be used for the web
   search webs : WEBS The web search instance to be used to perform the search
 max_results : int, optional The maximum number of search results to include in
     the response, by default 10 Returns ------- Optional[str] The response
 generated by the LLM model, or None if there is no response """ # Perform a web
     search based on the user input search_results: List[str] = [] for r in
     webs.text( user_input, region="wt-wt", safesearch="off", timelimit="y",
@@ -507,144 +510,23 @@
   including the user input, search results, and system message messages = [
    {"role": "user", "content": f"User question is:\n{user_input}\nwebsearch
     results are:\n{formatted_results}"}, ] # Use the chat method to get the
      response response = LLM.chat(messages) return response if __name__ ==
   "__main__": while True: # Get the user input user_input = input("User: ") #
   Perform a web search based on the user input response = chat(user_input) #
     Print the response if response: print("AI:", response) else: print("No
-response") ``` ## `Webai` - terminal gpt and a open interpeter ```python import
- time import uuid from typing import Dict, Any, Optional, AsyncGenerator from
-rich.console import Console from rich.markdown import Markdown from rich.panel
-       import Panel from rich.style import Style import webscout import
-          webscout.AIutel import g4f from webscout.g4f import * from
-      webscout.async_providers import mapper as async_provider_map class
-TaskExecutor: """ Manages an interactive chat session, handling user input, AI
-responses, and optional features like web search, code execution, and text-to-
-   speech. """ def __init__(self) -> None: """Initializes the conversational
-   assistant with default settings.""" self._console: Console = Console() #
-         Session configuration self._selected_provider: str = "phind"
- self._selected_model: str = "Phind Model" self._conversation_enabled: bool =
- True self._max_tokens: int = 600 self._temperature: float = 0.2 self._top_k:
- int = -1 self._top_p: float = 0.999 self._timeout: int = 30 self._auth_token:
-str = None # API key, if required self._chat_completion_enabled: bool = True #
-g4fauto self._ignore_working: bool = False # Ignore working status of providers
-self._proxy_path: str = None # Path to proxy configuration # History Management
-   self._history_filepath: str = None self._update_history_file: bool = True
- self._history_offset: int = 10250 # Prompt Engineering self._initial_prompt:
-    str = None self._awesome_prompt_content: str = None # Optional Features
-          self._web_search_enabled: bool = False # Enable web search
-self._rawdog_enabled: bool = True self._internal_script_execution_enabled: bool
-           = False self._script_confirmation_required: bool = False
-  self._selected_interpreter: str = "python" self._selected_optimizer: str =
-   "code" self._suppress_output: bool = False # Suppress verbose output # AI
-    provider mapping self._ai_provider_mapping: Dict[str, Any] = { "phind":
-        webscout.PhindSearch, "opengpt": webscout.OPENGPT, "koboldai":
-        webscout.KOBOLDAI, "blackboxai": webscout.BLACKBOXAI, "llama2":
-  webscout.LLAMA2, "yepchat": webscout.YEPCHAT, "leo": webscout.LEO, "groq":
- webscout.GROQ, "openai": webscout.OPENAI, "perplexity": webscout.PERPLEXITY,
-  "you": webscout.YouChat, "xjai": webscout.Xjai, "cohere": webscout.Cohere,
-       "reka": webscout.REKA, "thinkany": webscout.ThinkAnyAI, "gemini":
-         webscout.GEMINI, "berlin4h": webscout.Berlin4h, "chatgptuk":
-  webscout.ChatGPTUK, "poe": webscout.POE, "basedgpt": webscout.BasedGPT, } #
- Initialize Rawdog if enabled if self._rawdog_enabled: self._rawdog_instance:
- webscout.AIutel.RawDog = webscout.AIutel.RawDog( quiet=self._suppress_output,
-            internal_exec=self._internal_script_execution_enabled,
-              confirm_script=self._script_confirmation_required,
-       interpreter=self._selected_interpreter, ) self._initial_prompt =
-     self._rawdog_instance.intro_prompt # Initialize the selected AI model
- self._ai_model = self._get_ai_model() def _get_ai_model(self): """ Determines
- the appropriate AI model based on the selected provider, including automatic
-   provider selection and g4fauto support. """ if self._selected_provider ==
-      "g4fauto": # Automatically select the best provider from g4f test =
-  TestProviders(quiet=self._suppress_output, timeout=self._timeout) g4fauto =
-  test.best if not self._ignore_working else test.auto if isinstance(g4fauto,
-     str): self._selected_provider = "g4fauto+" + g4fauto self._ai_model =
-self._create_g4f_model(g4fauto) else: raise Exception( "No working g4f provider
- found. " "Consider running 'webscout.webai gpt4free test -y' first" ) else: #
-     Use the specified provider self._ai_model = self._ai_provider_mapping
-    [self._selected_provider]( is_conversation=self._conversation_enabled,
-max_tokens=self._max_tokens, timeout=self._timeout, intro=self._initial_prompt,
-    filepath=self._history_filepath, update_file=self._update_history_file,
-               proxies={}, # Load proxies from config if needed
-    history_offset=self._history_offset, act=self._awesome_prompt_content,
-          model=self._selected_model, quiet=self._suppress_output, #
- auth=self._auth_token, # Pass API key if required ) return self._ai_model def
-_create_g4f_model(self, provider: str): """ Creates a g4f model instance using
-      the provided provider and webscout.WEBS for web search. """ return
-       webscout.g4f.GPT4FREE( provider=provider, auth=self._auth_token,
-  max_tokens=self._max_tokens, chat_completion=self._chat_completion_enabled,
-          ignore_working=self._ignore_working, timeout=self._timeout,
-         intro=self._initial_prompt, filepath=self._history_filepath,
- update_file=self._update_history_file, proxies={}, # Load proxies from config
-                if needed history_offset=self._history_offset,
-   act=self._awesome_prompt_content, ) def process_query(self, query: str) -
- > None: """ Processes a user query, potentially enhancing it with web search
- results, passing it to the AI model, and handling the response. Args: query:
- The user's text input. Returns: None """ if self._web_search_enabled: query =
-    self._augment_query_with_web_search(query) # Apply code optimization if
-           configured if self._selected_optimizer == "code": query =
-webscout.AIutel.Optimizers.code(query) try: response: str = self._ai_model.chat
-    (query) except webscout.exceptions.FailedToGenerateResponseError as e:
- self._console.print(Markdown(f"LLM: [red]{e}[/red]")) return # Handle Rawdog
-  responses if enabled if self._rawdog_enabled: self._handle_rawdog_response
-    (response) else: self._console.print(Markdown(f"LLM: {response}")) def
-  _augment_query_with_web_search(self, query: str) -> str: """Performs a web
-   search and appends the results to the query. Args: query: The user's text
-     input. Returns: str: The augmented query with web search results. """
-      web_search_results = webscout.WEBS().text(query, max_results=3) if
-web_search_results: formatted_results = "\n".join( f"{i+1}. {result['title']} -
-    {result['href']}\n\nBody: {result['body']}" for i, result in enumerate
-     (web_search_results) ) query += f"\n\n## Web Search Results are:\n\n
- {formatted_results}" return query def _handle_rawdog_response(self, response:
-str) -> None: """Handles AI responses, potentially executing them as code with
-    Rawdog. Args: response: The AI model's response. Returns: None """ try:
-   is_feedback = self._rawdog_instance.main(response) except Exception as e:
-    self._console.print(Markdown(f"LLM: [red]Error: {e}[/red]")) return if
-    is_feedback: self._console.print(Markdown(f"LLM: {is_feedback}")) else:
-self._console.print(Markdown("LLM: (Script executed successfully)")) async def
- process_async_query(self, query: str) -> None: """ Asynchronously processes a
-user query, potentially enhancing it with web search results, passing it to the
-   AI model, and handling the response. Args: query: The user's text input.
-            Returns: None """ if self._web_search_enabled: query =
-    self._augment_query_with_web_search(query) # Apply code optimization if
-           configured if self._selected_optimizer == "code": query =
-webscout.AIutel.Optimizers.code(query) async_model = self._get_async_ai_model()
-       try: async for response in async_model.chat(query, stream=True):
-       self._console.print(Markdown(f"LLM: {response}"), end="") except
-  webscout.exceptions.FailedToGenerateResponseError as e: self._console.print
-(Markdown(f"LLM: [red]{e}[/red]")) return # Handle Rawdog responses if enabled
-     if self._rawdog_enabled: self._handle_rawdog_response(response) else:
-   self._console.print(Markdown(f"LLM: {response}")) def _get_async_ai_model
-   (self): """ Determines the appropriate asynchronous AI model based on the
-selected provider. """ if self._selected_provider == "g4fauto": # Automatically
-            select the best provider from g4f test = TestProviders
-(quiet=self._suppress_output, timeout=self._timeout) g4fauto = test.best if not
-       self._ignore_working else test.auto if isinstance(g4fauto, str):
-        self._selected_provider = "g4fauto+" + g4fauto self._ai_model =
- self._create_async_g4f_model(g4fauto) else: raise Exception( "No working g4f
-provider found. " "Consider running 'webscout gpt4free test -y' first" ) else:
-# Use the specified provider if self._selected_provider in async_provider_map:
-         self._ai_model = async_provider_map[self._selected_provider]
-  ( is_conversation=self._conversation_enabled, max_tokens=self._max_tokens,
-              timeout=self._timeout, intro=self._initial_prompt,
-    filepath=self._history_filepath, update_file=self._update_history_file,
-               proxies={}, # Load proxies from config if needed
-    history_offset=self._history_offset, act=self._awesome_prompt_content,
-model=self._selected_model, quiet=self._suppress_output, auth=self._auth_token,
- # Pass API key if required ) else: raise Exception( f"Asynchronous provider '
- {self._selected_provider}' is not yet supported" ) return self._ai_model def
- _create_async_g4f_model(self, provider: str): """ Creates an asynchronous g4f
- model instance using the provided provider and webscout.WEBS for web search.
-           """ return webscout.g4f.AsyncGPT4FREE( provider=provider,
-              auth=self._auth_token, max_tokens=self._max_tokens,
-                chat_completion=self._chat_completion_enabled,
-          ignore_working=self._ignore_working, timeout=self._timeout,
-         intro=self._initial_prompt, filepath=self._history_filepath,
- update_file=self._update_history_file, proxies={}, # Load proxies from config
-                if needed history_offset=self._history_offset,
-  act=self._awesome_prompt_content, ) if __name__ == "__main__": assistant =
-     TaskExecutor() while True: input_query = input("Enter your query: ")
-  assistant.process_query(input_query) ``` ```shell python -m webscout.webai
-                     webai --provider "phind" --rawdog ```
+ response") ``` ## `Webai` - terminal gpt and a open interpeter ```python from
+  webscout.webai import Main def use_rawdog_with_webai(prompt): """ Wrap the
+webscout default method in a try-except block to catch any unhandled exceptions
+    and print a helpful message. """ try: webai_bot = Main( max_tokens=500,
+  provider="cohere", temperature=0.7, top_k=40, top_p=0.95, model="command-r-
+ plus", # Replace with your desired model auth=None, # Replace with your auth
+  key/value (if needed) timeout=30, disable_conversation=True, filepath=None,
+       update_file=True, intro=None, rawdog=True, history_offset=10250,
+      awesome_prompt=None, proxy_path=None, quiet=True ) webai_response =
+webai_bot.default(prompt) except Exception as e: print("Unexpected error:", e)
+     if __name__ == "__main__": user_prompt = input("Enter your prompt: ")
+use_rawdog_with_webai(user_prompt) ``` ```shell python -m webscout.webai webai
+                        --provider "phind" --rawdog ```
                _[_T_e_l_e_g_r_a_m_]_[_I_n_s_t_a_g_r_a_m_]_[_L_i_n_k_e_d_I_n_]_[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
                           _➤_ _V_o_r_t_e_x_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
                        _➤_ _D_e_v_s_ _D_o_ _C_o_d_e_'_s_ _Y_o_u_T_u_b_e_ _C_h_a_n_n_e_l
```

### Comparing `webscout-3.0/setup.py` & `webscout-3.0b0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     README = f.read()
 
 setup(
     name="webscout",
-    version="3.0",
+    version="3.0-beta",
     description="Search for anything using Google, DuckDuckGo, phind.com, Contains AI models, can transcribe yt videos, temporary email and phone number generation, has TTS support, webai (terminal gpt and open interpreter) and offline LLMs",
     long_description=README,
     long_description_content_type="text/markdown",
     author="OEvortex",
     author_email="helpingai5@gmail.com",
     packages=find_packages(),
     classifiers=[
```

### Comparing `webscout-3.0/webscout/AIauto.py` & `webscout-3.0b0/webscout/AIauto.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/AIbase.py` & `webscout-3.0b0/webscout/AIbase.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/AIutel.py` & `webscout-3.0b0/webscout/AIutel.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/DWEBS.py` & `webscout-3.0b0/webscout/DWEBS.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/LLM.py` & `webscout-3.0b0/webscout/LLM.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/Local/formats.py` & `webscout-3.0b0/webscout/Local/formats.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/Local/model.py` & `webscout-3.0b0/webscout/Local/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,14 @@
 from os import cpu_count as os_cpu_count
 
 
 class ModelUnloadedException(Exception):
     """Exception raised when trying to use a Model that has been unloaded"""
     def __init__(self, message):
         self.message = message
-        self.tool_code_start = "```tool_code\n"  # Define tool code markers
-        self.tool_code_end = "\n```tool_code```"
         super().__init__(self.message)
         self.add_note('Are you trying to use a Model that has been unloaded?')
 
 class Model:
     """
     A high-level abstraction of a llama model
 
@@ -269,49 +267,59 @@
             print_verbose(f"param: n_threads            == {n_threads}")
             print_verbose(f"param: n_threads_batch      == {n_threads_batch}")
             print_verbose(f" gguf: n_ctx_train          == {n_ctx_train}")
             print_verbose(f"param: self.context_length  == {self.context_length}")
             print_verbose(f" gguf: rope_freq_base_train == {rope_freq_base_train}")
             print_verbose(f"param: rope_freq_base       == {rope_freq_base}")
     def register_tool(self, name: str, function: Callable):
-        """Registers a tool for function calling."""
+        """
+        Registers a tool for function calling.
+
+        Args:
+            name: The name of the tool.
+            function: The Python function to execute when the tool is called.
+        """
         self.tools[name] = function
 
     def _extract_tool_code(self, text: str) -> dict:
-        """Extracts tool code from the model's output."""
+        """
+        Extracts tool code from the model's output using the chatml-function-calling format.
+        
+        Args:
+            text: The model's generated text.
+
+        Returns:
+            A dictionary containing the tool name and arguments, or None if no tool call is found.
+        """
         try:
-            start = text.find(self.tool_code_start) + len(self.tool_code_start)
-            end = text.find(self.tool_code_end)
+            # Assuming tool code is enclosed in ```tool_code\n...\n```tool_code```
+            start = text.find("```tool_code\n") + len("```tool_code\n")
+            end = text.find("\n```tool_code```")
             tool_code_json = text[start:end]
             tool_code = json.loads(tool_code_json)
             return tool_code
         except (ValueError, json.JSONDecodeError):
             return None
-    def _should_call_tool(self, response_text: str) -> bool:
-        """Determines if the model suggests a tool call."""
-        # Simple check for tool code markers in response
-        return self.tool_code_start in response_text and self.tool_code_end in response_text
+
     def generate(
         self,
         prompt: Union[str, list[int]],
         stops: list[Union[str, int]] = [],
-        sampler: SamplerSettings = DefaultSampling,
-        max_iterations: int = 3, # Maximum iterations for tool calls
+        sampler: SamplerSettings = DefaultSampling
     ) -> str:
         """
-        Generates text and handles tool calls.
+        Given a prompt, return a generated string, potentially calling and executing tools.
 
         Args:
-            prompt (Union[str, list[int]]): The input prompt.
-            stops (list[Union[str, int]]): Stop sequences.
-            sampler (SamplerSettings): Sampler settings.
-            max_iterations (int): Maximum number of tool call iterations. 
+            prompt: The text from which to generate.
+            stops: A list of strings and/or token IDs at which to end the generation early.
+            sampler: The SamplerSettings object used to control text generation.
 
         Returns:
-            str: The generated text.
+            The generated string.
         """
         assert_model_is_loaded(self)
         response_text = self.llama.create_completion(
             prompt,
             max_tokens=sampler.max_len_tokens,
             temperature=sampler.temp,
             top_p=sampler.top_p,
@@ -319,29 +327,23 @@
             frequency_penalty=sampler.frequency_penalty,
             presence_penalty=sampler.presence_penalty,
             repeat_penalty=sampler.repeat_penalty,
             top_k=sampler.top_k,
             stop=stops
         )['choices'][0]['text']
 
-        iteration = 0
-        while self._should_call_tool(response_text) and iteration < max_iterations:
-            tool_code = self._extract_tool_code(response_text)
-            if tool_code:
-                tool_name = tool_code.get("function", {}).get("name")
-                arguments = tool_code.get("function", {}).get("arguments", "")
-                if tool_name and arguments and tool_name in self.tools:
-                    # Execute the tool and append its output
-                    tool_output = self.tools[tool_name](**json.loads(arguments))
-                    response_text = response_text.replace(
-                        f"{self.tool_code_start}{json.dumps(tool_code)}{self.tool_code_end}", 
-                        tool_output
-                    )
-            iteration += 1
-
+        tool_code = self._extract_tool_code(response_text)
+        if tool_code:
+            # Execute the tool and get its output
+            tool_name = tool_code.get("function", {}).get("name")
+            arguments = tool_code.get("function", {}).get("arguments", "")
+            if tool_name and arguments and tool_name in self.tools:
+                tool_output = self.tools[tool_name](**json.loads(arguments))
+                # Append the tool output to the response
+                response_text += f"\n{tool_output}" 
         return response_text
     def __repr__(self) -> str:
         return \
             f"Model({repr(self._model_path)}, " + \
             f"context_length={self._context_length}, " + \
             f"n_gpu_layers={self._n_gpu_layers}, " + \
             f"offload_kqv={self._offload_kqv}, "+ \
```

### Comparing `webscout-3.0/webscout/Local/samplers.py` & `webscout-3.0b0/webscout/Local/samplers.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/Local/thread.py` & `webscout-3.0b0/webscout/Local/thread.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,20 +162,23 @@
             print_verbose(f"sampler.top_p             == {self.sampler.top_p}")
             print_verbose(f"sampler.min_p             == {self.sampler.min_p}")
             print_verbose(f"sampler.frequency_penalty == {self.sampler.frequency_penalty}")
             print_verbose(f"sampler.presence_penalty  == {self.sampler.presence_penalty}")
             print_verbose(f"sampler.repeat_penalty    == {self.sampler.repeat_penalty}")
             print_verbose(f"sampler.top_k             == {self.sampler.top_k}")
     def add_tool(self, tool: dict):
-        """Adds a tool to the Thread for function calling."""
+        """
+        Adds a tool to the Thread for function calling.
+        ... (Rest of your add_tool docstring)
+        """
         self.tools.append(tool)
-        self.model.register_tool(tool['function']['name'], tool['function']['execute']) # Register the tool
+        self.model.register_tool(tool['function']['name'], tool['function'].get('execute', None))
 
-        # Include tool information in the system message (optional, but helpful)
-        self.messages[0]['content'] += f"\nYou have access to the following tool:\n{tool['function']['description']}" 
+        # Include tool information in the system message
+        self.messages[0]['content'] += f"\nYou have access to the following tool:\n```tool_code\n{json.dumps(tool)}\n```tool_code"
     def __repr__(self) -> str:
         return \
             f"Thread({repr(self.model)}, {repr(self.format)}, " + \
             f"{repr(self.sampler)}, {repr(self.messages)})"
     
     def __str__(self) -> str:
         return self.as_string()
```

### Comparing `webscout-3.0/webscout/Local/utils.py` & `webscout-3.0b0/webscout/Local/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/Provider/BasedGPT.py` & `webscout-3.0b0/webscout/Provider/Cohere.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,226 +1,223 @@
-import time
-import uuid
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import WebDriverWait
-import click
-import requests
-from requests import get
-from uuid import uuid4
-from re import findall
-from requests.exceptions import RequestException
-from curl_cffi.requests import get, RequestsError
-import g4f
-from random import randint
-from PIL import Image
-import io
-import re
-import json
-import yaml
-from ..AIutel import Optimizers
-from ..AIutel import Conversation
-from ..AIutel import AwesomePrompts, sanitize_stream
-from ..AIbase import  Provider, AsyncProvider
-from webscout import exceptions
-from typing import Any, AsyncGenerator, Dict
-import logging
-import httpx
-
-class BasedGPT(Provider):
-    def __init__(
-        self,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-        system_prompt: str = "Be Helpful and Friendly",
-    ):
-        """Instantiates BasedGPT
-
-        Args:
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-            system_prompt (str, optional): System prompt for BasedGPT. Defaults to "Be Helpful and Friendly".
-        """
-        self.session = requests.Session()
-        self.is_conversation = is_conversation
-        self.max_tokens_to_sample = max_tokens
-        self.chat_endpoint = "https://www.basedgpt.chat/api/chat"
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.system_prompt = system_prompt
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        self.session.headers.update(
-            {"Content-Type": "application/json"}
-        )
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session.proxies = proxies
-
-    def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict:
-        """Chat with AI
-
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict : {}
-        ```json
-        {
-            "id": "chatcmpl-TaREJpBZsRVQFRFic1wIA7Q7XfnaD",
-            "object": "chat.completion",
-            "created": 1704623244,
-            "model": "gpt-3.5-turbo",
-            "usage": {
-                "prompt_tokens": 0,
-                "completion_tokens": 0,
-                "total_tokens": 0
-                },
-            "choices": [
-                {
-                    "message": {
-                        "role": "assistant",
-                        "content": "Hello! How can I assist you today?"
-                },
-                "finish_reason": "stop",
-                "index": 0
-                }
-            ]
-        }
-        ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-
-        payload = {
-            "messages": [
-                {"role": "system", "content": self.system_prompt},
-                {"role": "user", "content": conversation_prompt},
-            ],
-        }
-
-        def for_stream():
-            response = self.session.post(
-                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
-            )
-            if not response.ok:
-                raise exceptions.FailedToGenerateResponseError(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
-                )
-
-            message_load = ""
-            for value in response.iter_lines(
-                decode_unicode=True,
-                delimiter="",
-                chunk_size=self.stream_chunk_size,
-            ):
-                try:
-                    message_load += value
-                    yield value if raw else dict(text=message_load)
-                except json.decoder.JSONDecodeError:
-                    pass
-            self.last_response.update(dict(text=message_load))
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
-
-        def for_non_stream():
-            for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else for_non_stream()
-
-    def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str:
-        """Generate response `str`
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str: Response generated
-        """
-
-        def for_stream():
-            for response in self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            ):
-                yield self.get_message(response)
-
-        def for_non_stream():
-            return self.get_message(
-                self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else for_non_stream()
-
-    def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        return response["text"]
+import time
+import uuid
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.ui import WebDriverWait
+import click
+import requests
+from requests import get
+from uuid import uuid4
+from re import findall
+from requests.exceptions import RequestException
+from curl_cffi.requests import get, RequestsError
+import g4f
+from random import randint
+from PIL import Image
+import io
+import re
+import json
+import yaml
+from ..AIutel import Optimizers
+from ..AIutel import Conversation
+from ..AIutel import AwesomePrompts, sanitize_stream
+from ..AIbase import  Provider, AsyncProvider
+from Helpingai_T2 import Perplexity
+from webscout import exceptions
+from typing import Any, AsyncGenerator, Dict
+import logging
+import httpx
+#-----------------------------------------------Cohere--------------------------------------------
+class Cohere(Provider):
+    def __init__(
+        self,
+        api_key: str,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        model: str = "command-r-plus",
+        temperature: float = 0.7,
+        system_prompt: str = "You are helpful AI",
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+        top_k: int = -1,
+        top_p: float = 0.999,
+    ):
+        """Initializes Cohere
+
+        Args:
+            api_key (str): Cohere API key.
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            model (str, optional): Model to use for generating text. Defaults to "command-r-plus".
+            temperature (float, optional): Diversity of the generated text. Higher values produce more diverse outputs.
+                            Defaults to 0.7.
+            system_prompt (str, optional): A system_prompt or context to set the style or tone of the generated text. 
+                            Defaults to "You are helpful AI".
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.session = requests.Session()
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.api_key = api_key
+        self.model = model
+        self.temperature = temperature
+        self.system_prompt = system_prompt
+        self.chat_endpoint = "https://production.api.os.cohere.ai/coral/v1/chat"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.headers = {
+            "Content-Type": "application/json",
+            "Authorization": f"Bearer {self.api_key}",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.session.headers.update(self.headers)
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+           "text" : "How may I assist you today?"
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+        self.session.headers.update(self.headers)
+        payload = {
+            "message": conversation_prompt,
+            "model": self.model,
+            "temperature": self.temperature,
+            "preamble": self.system_prompt,
+        }
+
+        def for_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
+            )
+            if not response.ok:
+                raise Exception(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+
+            for value in response.iter_lines(
+                decode_unicode=True,
+                chunk_size=self.stream_chunk_size,
+            ):
+                try:
+                    resp = json.loads(value.strip().split("\n")[-1])
+                    self.last_response.update(resp)
+                    yield value if raw else resp
+                except json.decoder.JSONDecodeError:
+                    pass
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            # let's make use of stream
+            for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response["result"]["chatStreamEndEvent"]["response"]["text"]
```

### Comparing `webscout-3.0/webscout/Provider/Berlin4h.py` & `webscout-3.0b0/webscout/Provider/Berlin4h.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,211 +1,211 @@
-import requests
-import json
-import uuid
-from typing import Any, Dict, Optional
-from ..AIutel import Optimizers
-from ..AIutel import Conversation
-from ..AIutel import AwesomePrompts, sanitize_stream
-from ..AIbase import Provider, AsyncProvider
-from webscout import exceptions
-
-class Berlin4h(Provider):
-    """
-    A class to interact with the Berlin4h AI API.
-    """
-
-    def __init__(
-        self,
-        api_token: str = "3bf369cd84339603f8a5361e964f9ebe",
-        api_endpoint: str = "https://ai.berlin4h.top/api/chat/completions",
-        model: str = "gpt-3.5-turbo",
-        temperature: float = 0.9,
-        presence_penalty: float = 0,
-        frequency_penalty: float = 0,
-        max_tokens: int = 4000,
-        is_conversation: bool = True,
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-    ) -> None:
-        """
-        Initializes the Berlin4h API with given parameters.
-
-        Args:
-            api_token (str): The API token for authentication.
-            api_endpoint (str): The API endpoint to use for requests.
-            model (str): The AI model to use for text generation.
-            temperature (float): The temperature parameter for the model.
-            presence_penalty (float): The presence penalty parameter for the model.
-            frequency_penalty (float): The frequency penalty parameter for the model.
-            max_tokens (int): The maximum number of tokens to generate.
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-        """
-        self.api_token = api_token
-        self.api_endpoint = api_endpoint
-        self.model = model
-        self.temperature = temperature
-        self.presence_penalty = presence_penalty
-        self.frequency_penalty = frequency_penalty
-        self.max_tokens = max_tokens
-        self.parent_message_id: Optional[str] = None
-        self.session = requests.Session()
-        self.is_conversation = is_conversation
-        self.max_tokens_to_sample = max_tokens
-        self.stream_chunk_size = 1
-        self.timeout = timeout
-        self.last_response = {}
-        self.headers = {"Content-Type": "application/json", "Token": self.api_token}
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        self.session.headers.update(self.headers)
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session.proxies = proxies
-
-    def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> Dict[str, Any]:
-        """
-        Sends a prompt to the Berlin4h AI API and returns the response.
-
-        Args:
-            prompt: The text prompt to generate text from.
-            stream (bool, optional): Whether to stream the response. Defaults to False.
-            raw (bool, optional): Whether to return the raw response. Defaults to False.
-            optimizer (str, optional): The name of the optimizer to use. Defaults to None.
-            conversationally (bool, optional): Whether to chat conversationally. Defaults to False.
-
-        Returns:
-            The response from the API.
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-
-        payload: Dict[str, any] = {
-            "prompt": conversation_prompt,
-            "parentMessageId": self.parent_message_id or str(uuid.uuid4()),
-            "options": {
-                "model": self.model,
-                "temperature": self.temperature,
-                "presence_penalty": self.presence_penalty,
-                "frequency_penalty": self.frequency_penalty,
-                "max_tokens": self.max_tokens,
-            },
-        }
-
-        def for_stream():
-            response = self.session.post(
-                self.api_endpoint, json=payload, headers=self.headers, stream=True, timeout=self.timeout
-            )
-
-            if not response.ok:
-                raise exceptions.FailedToGenerateResponseError(
-                    f"Failed to generate response - ({response.status_code}, {response.reason})"
-                )
-
-            streaming_response = ""
-            # Collect the entire line before processing
-            for line in response.iter_lines(decode_unicode=True): 
-                if line:
-                    try:
-                        json_data = json.loads(line)
-                        content = json_data['content']
-                        if ">" in content: break
-                        streaming_response += content
-                        yield content if raw else dict(text=streaming_response)  # Yield accumulated response
-                    except:
-                        continue
-            self.last_response.update(dict(text=streaming_response))
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
-
-        def for_non_stream():
-            for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else for_non_stream()
-
-    def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str:
-        """Generate response `str`
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str: Response generated
-        """
-
-        def for_stream():
-            for response in self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            ):
-                yield self.get_message(response)
-
-        def for_non_stream():
-            return self.get_message(
-                self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else for_non_stream()
-
-    def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
+import requests
+import json
+import uuid
+from typing import Any, Dict, Optional
+from ..AIutel import Optimizers
+from ..AIutel import Conversation
+from ..AIutel import AwesomePrompts, sanitize_stream
+from ..AIbase import Provider, AsyncProvider
+from webscout import exceptions
+
+class Berlin4h(Provider):
+    """
+    A class to interact with the Berlin4h AI API.
+    """
+
+    def __init__(
+        self,
+        api_token: str = "3bf369cd84339603f8a5361e964f9ebe",
+        api_endpoint: str = "https://ai.berlin4h.top/api/chat/completions",
+        model: str = "gpt-3.5-turbo",
+        temperature: float = 0.9,
+        presence_penalty: float = 0,
+        frequency_penalty: float = 0,
+        max_tokens: int = 4000,
+        is_conversation: bool = True,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ) -> None:
+        """
+        Initializes the Berlin4h API with given parameters.
+
+        Args:
+            api_token (str): The API token for authentication.
+            api_endpoint (str): The API endpoint to use for requests.
+            model (str): The AI model to use for text generation.
+            temperature (float): The temperature parameter for the model.
+            presence_penalty (float): The presence penalty parameter for the model.
+            frequency_penalty (float): The frequency penalty parameter for the model.
+            max_tokens (int): The maximum number of tokens to generate.
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.api_token = api_token
+        self.api_endpoint = api_endpoint
+        self.model = model
+        self.temperature = temperature
+        self.presence_penalty = presence_penalty
+        self.frequency_penalty = frequency_penalty
+        self.max_tokens = max_tokens
+        self.parent_message_id: Optional[str] = None
+        self.session = requests.Session()
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.stream_chunk_size = 1
+        self.timeout = timeout
+        self.last_response = {}
+        self.headers = {"Content-Type": "application/json", "Token": self.api_token}
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.session.headers.update(self.headers)
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> Dict[str, Any]:
+        """
+        Sends a prompt to the Berlin4h AI API and returns the response.
+
+        Args:
+            prompt: The text prompt to generate text from.
+            stream (bool, optional): Whether to stream the response. Defaults to False.
+            raw (bool, optional): Whether to return the raw response. Defaults to False.
+            optimizer (str, optional): The name of the optimizer to use. Defaults to None.
+            conversationally (bool, optional): Whether to chat conversationally. Defaults to False.
+
+        Returns:
+            The response from the API.
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        payload: Dict[str, any] = {
+            "prompt": conversation_prompt,
+            "parentMessageId": self.parent_message_id or str(uuid.uuid4()),
+            "options": {
+                "model": self.model,
+                "temperature": self.temperature,
+                "presence_penalty": self.presence_penalty,
+                "frequency_penalty": self.frequency_penalty,
+                "max_tokens": self.max_tokens,
+            },
+        }
+
+        def for_stream():
+            response = self.session.post(
+                self.api_endpoint, json=payload, headers=self.headers, stream=True, timeout=self.timeout
+            )
+
+            if not response.ok:
+                raise exceptions.FailedToGenerateResponseError(
+                    f"Failed to generate response - ({response.status_code}, {response.reason})"
+                )
+
+            streaming_response = ""
+            # Collect the entire line before processing
+            for line in response.iter_lines(decode_unicode=True): 
+                if line:
+                    try:
+                        json_data = json.loads(line)
+                        content = json_data['content']
+                        if ">" in content: break
+                        streaming_response += content
+                        yield content if raw else dict(text=streaming_response)  # Yield accumulated response
+                    except:
+                        continue
+            self.last_response.update(dict(text=streaming_response))
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
         return response["text"]
```

### Comparing `webscout-3.0/webscout/Provider/Blackboxai.py` & `webscout-3.0b0/webscout/Provider/Koboldai.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,440 +1,402 @@
-import time
-import uuid
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import WebDriverWait
-import click
-import requests
-from requests import get
-from uuid import uuid4
-from re import findall
-from requests.exceptions import RequestException
-from curl_cffi.requests import get, RequestsError
-import g4f
-from random import randint
-from PIL import Image
-import io
-import re
-import json
-import yaml
-from ..AIutel import Optimizers
-from ..AIutel import Conversation
-from ..AIutel import AwesomePrompts, sanitize_stream
-from ..AIbase import  Provider, AsyncProvider
-from Helpingai_T2 import Perplexity
-from webscout import exceptions
-from typing import Any, AsyncGenerator, Dict
-import logging
-import httpx
-
-#------------------------------------------------------BLACKBOXAI--------------------------------------------------------  
-class BLACKBOXAI:
-    def __init__(
-        self,
-        is_conversation: bool = True,
-        max_tokens: int = 8000,
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-        model: str = None,
-    ):
-        """Instantiates BLACKBOXAI
-
-        Args:
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-            model (str, optional): Model name. Defaults to "Phind Model".
-        """
-        self.session = requests.Session()
-        self.max_tokens_to_sample = max_tokens
-        self.is_conversation = is_conversation
-        self.chat_endpoint = "https://www.blackbox.ai/api/chat"
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.model = model
-        self.previewToken: str = None
-        self.userId: str = ""
-        self.codeModelMode: bool = True
-        self.id: str = ""
-        self.agentMode: dict = {}
-        self.trendingAgentMode: dict = {}
-        self.isMicMode: bool = False
-
-        self.headers = {
-            "Content-Type": "application/json",
-            "User-Agent": "",
-            "Accept": "*/*",
-            "Accept-Encoding": "Identity",
-        }
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        self.session.headers.update(self.headers)
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session.proxies = proxies
-
-    def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict:
-        """Chat with AI
-
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict : {}
-        ```json
-        {
-           "text" : "print('How may I help you today?')"
-        }
-        ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-
-        self.session.headers.update(self.headers)
-        payload = {
-            "messages": [
-                # json.loads(prev_messages),
-                {"content": conversation_prompt, "role": "user"}
-            ],
-            "id": self.id,
-            "previewToken": self.previewToken,
-            "userId": self.userId,
-            "codeModelMode": self.codeModelMode,
-            "agentMode": self.agentMode,
-            "trendingAgentMode": self.trendingAgentMode,
-            "isMicMode": self.isMicMode,
-        }
-
-        def for_stream():
-            response = self.session.post(
-                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
-            )
-            if (
-                not response.ok
-                or not response.headers.get("Content-Type")
-                == "text/plain; charset=utf-8"
-            ):
-                raise Exception(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
-                )
-            streaming_text = ""
-            for value in response.iter_lines(
-                decode_unicode=True,
-                chunk_size=self.stream_chunk_size,
-                delimiter="\n",
-            ):
-                try:
-                    if bool(value):
-                        streaming_text += value + ("\n" if stream else "")
-
-                        resp = dict(text=streaming_text)
-                        self.last_response.update(resp)
-                        yield value if raw else resp
-                except json.decoder.JSONDecodeError:
-                    pass
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
-
-        def for_non_stream():
-            for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else for_non_stream()
-
-    def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str:
-        """Generate response `str`
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str: Response generated
-        """
-
-        def for_stream():
-            for response in self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            ):
-                yield self.get_message(response)
-
-        def for_non_stream():
-            return self.get_message(
-                self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else for_non_stream()
-
-    def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        return response["text"]
-    @staticmethod
-    def chat_cli(prompt):
-        """Sends a request to the BLACKBOXAI API and processes the response."""
-        blackbox_ai = BLACKBOXAI()  # Initialize a BLACKBOXAI instance
-        response = blackbox_ai.ask(prompt)  # Perform a chat with the given prompt
-        processed_response = blackbox_ai.get_message(response)  # Process the response
-        print(processed_response)
-class AsyncBLACKBOXAI(AsyncProvider):
-    def __init__(
-        self,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-        model: str = None,
-    ):
-        """Instantiates BLACKBOXAI
-
-        Args:
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-            model (str, optional): Model name. Defaults to "Phind Model".
-        """
-        self.max_tokens_to_sample = max_tokens
-        self.is_conversation = is_conversation
-        self.chat_endpoint = "https://www.blackbox.ai/api/chat"
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.model = model
-        self.previewToken: str = None
-        self.userId: str = ""
-        self.codeModelMode: bool = True
-        self.id: str = ""
-        self.agentMode: dict = {}
-        self.trendingAgentMode: dict = {}
-        self.isMicMode: bool = False
-
-        self.headers = {
-            "Content-Type": "application/json",
-            "User-Agent": "",
-            "Accept": "*/*",
-            "Accept-Encoding": "Identity",
-        }
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session = httpx.AsyncClient(headers=self.headers, proxies=proxies)
-
-    async def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict | AsyncGenerator:
-        """Chat with AI asynchronously.
-
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict|AsyncGenerator : ai content
-        ```json
-        {
-           "text" : "print('How may I help you today?')"
-        }
-        ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-
-        payload = {
-            "messages": [
-                # json.loads(prev_messages),
-                {"content": conversation_prompt, "role": "user"}
-            ],
-            "id": self.id,
-            "previewToken": self.previewToken,
-            "userId": self.userId,
-            "codeModelMode": self.codeModelMode,
-            "agentMode": self.agentMode,
-            "trendingAgentMode": self.trendingAgentMode,
-            "isMicMode": self.isMicMode,
-        }
-
-        async def for_stream():
-            async with self.session.stream(
-                "POST", self.chat_endpoint, json=payload, timeout=self.timeout
-            ) as response:
-                if (
-                    not response.is_success
-                    or not response.headers.get("Content-Type")
-                    == "text/plain; charset=utf-8"
-                ):
-                    raise exceptions.FailedToGenerateResponseError(
-                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
-                    )
-                streaming_text = ""
-                async for value in response.aiter_lines():
-                    try:
-                        if bool(value):
-                            streaming_text += value + ("\n" if stream else "")
-                            resp = dict(text=streaming_text)
-                            self.last_response.update(resp)
-                            yield value if raw else resp
-                    except json.decoder.JSONDecodeError:
-                        pass
-            self.conversation.update_chat_history(
-                prompt, await self.get_message(self.last_response)
-            )
-
-        async def for_non_stream():
-            async for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else await for_non_stream()
-
-    async def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str | AsyncGenerator:
-        """Generate response `str` asynchronously.
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str|AsyncGenerator: Response generated
-        """
-
-        async def for_stream():
-            async_ask = await self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            )
-            async for response in async_ask:
-                yield await self.get_message(response)
-
-        async def for_non_stream():
-            return await self.get_message(
-                await self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else await for_non_stream()
-
-    async def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        return response["text"]
+import time
+import uuid
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.ui import WebDriverWait
+import click
+import requests
+from requests import get
+from uuid import uuid4
+from re import findall
+from requests.exceptions import RequestException
+from curl_cffi.requests import get, RequestsError
+import g4f
+from random import randint
+from PIL import Image
+import io
+import re
+import json
+import yaml
+from ..AIutel import Optimizers
+from ..AIutel import Conversation
+from ..AIutel import AwesomePrompts, sanitize_stream
+from ..AIbase import  Provider, AsyncProvider
+from Helpingai_T2 import Perplexity
+from webscout import exceptions
+from typing import Any, AsyncGenerator, Dict
+import logging
+import httpx
+#------------------------------------------------------KOBOLDAI-----------------------------------------------------------
+class KOBOLDAI(Provider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        temperature: float = 1,
+        top_p: float = 1,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiate TGPT
+
+        Args:
+            is_conversation (str, optional): Flag for chatting conversationally. Defaults to True.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.2.
+            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
+            timeout (int, optional): Http requesting timeout. Defaults to 30
+            intro (str, optional): Conversation introductory prompt. Defaults to `Conversation.intro`.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional) : Http reqiuest proxies (socks). Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.session = requests.Session()
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.temperature = temperature
+        self.top_p = top_p
+        self.chat_endpoint = (
+            "https://koboldai-koboldcpp-tiefighter.hf.space/api/extra/generate/stream"
+        )
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.headers = {
+            "Content-Type": "application/json",
+            "Accept": "application/json",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.session.headers.update(self.headers)
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+           "token" : "How may I assist you today?"
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        self.session.headers.update(self.headers)
+        payload = {
+            "prompt": conversation_prompt,
+            "temperature": self.temperature,
+            "top_p": self.top_p,
+        }
+
+        def for_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
+            )
+            if not response.ok:
+                raise Exception(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+
+            message_load = ""
+            for value in response.iter_lines(
+                decode_unicode=True,
+                delimiter="" if raw else "event: message\ndata:",
+                chunk_size=self.stream_chunk_size,
+            ):
+                try:
+                    resp = json.loads(value)
+                    message_load += self.get_message(resp)
+                    resp["token"] = message_load
+                    self.last_response.update(resp)
+                    yield value if raw else resp
+                except json.decoder.JSONDecodeError:
+                    pass
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            # let's make use of stream
+            for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response.get("token")
+class AsyncKOBOLDAI(AsyncProvider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        temperature: float = 1,
+        top_p: float = 1,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiate TGPT
+
+        Args:
+            is_conversation (str, optional): Flag for chatting conversationally. Defaults to True.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.2.
+            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
+            timeout (int, optional): Http requesting timeout. Defaults to 30
+            intro (str, optional): Conversation introductory prompt. Defaults to `Conversation.intro`.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional) : Http reqiuest proxies (socks). Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.temperature = temperature
+        self.top_p = top_p
+        self.chat_endpoint = (
+            "https://koboldai-koboldcpp-tiefighter.hf.space/api/extra/generate/stream"
+        )
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.headers = {
+            "Content-Type": "application/json",
+            "Accept": "application/json",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session = httpx.AsyncClient(headers=self.headers, proxies=proxies)
+
+    async def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict | AsyncGenerator:
+        """Chat with AI asynchronously.
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict|AsyncGenerator : ai content
+        ```json
+        {
+           "token" : "How may I assist you today?"
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        payload = {
+            "prompt": conversation_prompt,
+            "temperature": self.temperature,
+            "top_p": self.top_p,
+        }
+
+        async def for_stream():
+            async with self.session.stream(
+                "POST", self.chat_endpoint, json=payload, timeout=self.timeout
+            ) as response:
+                if not response.is_success:
+                    raise exceptions.FailedToGenerateResponseError(
+                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
+                    )
+
+                message_load = ""
+                async for value in response.aiter_lines():
+                    try:
+                        resp = sanitize_stream(value)
+                        message_load += await self.get_message(resp)
+                        resp["token"] = message_load
+                        self.last_response.update(resp)
+                        yield value if raw else resp
+                    except json.decoder.JSONDecodeError:
+                        pass
+
+            self.conversation.update_chat_history(
+                prompt, await self.get_message(self.last_response)
+            )
+
+        async def for_non_stream():
+            # let's make use of stream
+            async for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str | AsyncGenerator:
+        """Generate response `str` asynchronously.
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        async def for_stream():
+            async_ask = await self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            )
+            async for response in async_ask:
+                yield await self.get_message(response)
+
+        async def for_non_stream():
+            return await self.get_message(
+                await self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response.get("token")
```

### Comparing `webscout-3.0/webscout/Provider/ChatGPTUK.py` & `webscout-3.0b0/webscout/Provider/ChatGPTUK.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,214 +1,214 @@
-import requests
-from typing import Any, AsyncGenerator, Dict, Optional
-import json
-import re
-
-from ..AIutel import Optimizers
-from ..AIutel import Conversation
-from ..AIutel import AwesomePrompts, sanitize_stream
-from ..AIbase import  Provider, AsyncProvider
-from webscout import exceptions
-
-
-class ChatGPTUK(Provider):
-    """
-    A class to interact with the ChatGPT UK API.
-    """
-
-    def __init__(
-        self,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
-        temperature: float = 0.9,
-        presence_penalty: float = 0,
-        frequency_penalty: float = 0,
-        top_p: float = 1,
-        model: str = "google-gemini-pro",
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-    ) -> None:
-        """
-        Initializes the ChatGPTUK API with given parameters.
-
-        Args:
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.9.
-            presence_penalty (float, optional): Chances of topic being repeated. Defaults to 0.
-            frequency_penalty (float, optional): Chances of word being repeated. Defaults to 0.
-            top_p (float, optional): Sampling threshold during inference time. Defaults to 1.
-            model (str, optional): LLM model name. Defaults to "google-gemini-pro".
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-        """
-        self.session = requests.Session()
-        self.is_conversation = is_conversation
-        self.max_tokens_to_sample = max_tokens
-        self.api_endpoint = "https://free.chatgpt.org.uk/api/openai/v1/chat/completions"
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.model = model
-        self.temperature = temperature
-        self.presence_penalty = presence_penalty
-        self.frequency_penalty = frequency_penalty
-        self.top_p = top_p
-        self.headers = {"Content-Type": "application/json"}
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        self.session.headers.update(self.headers)
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session.proxies = proxies
-
-    def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict:
-        """Chat with AI
-
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict : {}
-        ```json
-        {
-           "text" : "How may I assist you today?"
-        }
-        ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-
-        self.session.headers.update(self.headers)
-        payload = {
-            "messages": [
-                {"role": "system", "content": "Keep your responses long and detailed"},
-                {"role": "user", "content": conversation_prompt}
-            ],
-            "stream": True,
-            "model": self.model,
-            "temperature": self.temperature,
-            "presence_penalty": self.presence_penalty,
-            "frequency_penalty": self.frequency_penalty,
-            "top_p": self.top_p,
-            "max_tokens": self.max_tokens_to_sample
-        }
-
-        def for_stream():
-            response = self.session.post(
-                self.api_endpoint, json=payload, stream=True, timeout=self.timeout
-            )
-            if not response.ok:
-                raise exceptions.FailedToGenerateResponseError(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
-                )
-
-            streaming_response = ""
-            for line in response.iter_lines(decode_unicode=True, chunk_size=1):
-                if line:
-                    modified_line = re.sub("data:", "", line)
-                    try:
-                        json_data = json.loads(modified_line)
-                        content = json_data['choices'][0]['delta']['content']
-                        streaming_response += content
-                        yield content if raw else dict(text=streaming_response)
-                    except:
-                        continue
-            self.last_response.update(dict(text=streaming_response))
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
-
-        def for_non_stream():
-            for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else for_non_stream()
-
-    def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str:
-        """Generate response `str`
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str: Response generated
-        """
-
-        def for_stream():
-            for response in self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            ):
-                yield self.get_message(response)
-
-        def for_non_stream():
-            return self.get_message(
-                self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else for_non_stream()
-
-    def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
+import requests
+from typing import Any, AsyncGenerator, Dict, Optional
+import json
+import re
+
+from ..AIutel import Optimizers
+from ..AIutel import Conversation
+from ..AIutel import AwesomePrompts, sanitize_stream
+from ..AIbase import  Provider, AsyncProvider
+from webscout import exceptions
+
+
+class ChatGPTUK(Provider):
+    """
+    A class to interact with the ChatGPT UK API.
+    """
+
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        temperature: float = 0.9,
+        presence_penalty: float = 0,
+        frequency_penalty: float = 0,
+        top_p: float = 1,
+        model: str = "google-gemini-pro",
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ) -> None:
+        """
+        Initializes the ChatGPTUK API with given parameters.
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.9.
+            presence_penalty (float, optional): Chances of topic being repeated. Defaults to 0.
+            frequency_penalty (float, optional): Chances of word being repeated. Defaults to 0.
+            top_p (float, optional): Sampling threshold during inference time. Defaults to 1.
+            model (str, optional): LLM model name. Defaults to "google-gemini-pro".
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.session = requests.Session()
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.api_endpoint = "https://free.chatgpt.org.uk/api/openai/v1/chat/completions"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.model = model
+        self.temperature = temperature
+        self.presence_penalty = presence_penalty
+        self.frequency_penalty = frequency_penalty
+        self.top_p = top_p
+        self.headers = {"Content-Type": "application/json"}
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.session.headers.update(self.headers)
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+           "text" : "How may I assist you today?"
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        self.session.headers.update(self.headers)
+        payload = {
+            "messages": [
+                {"role": "system", "content": "Keep your responses long and detailed"},
+                {"role": "user", "content": conversation_prompt}
+            ],
+            "stream": True,
+            "model": self.model,
+            "temperature": self.temperature,
+            "presence_penalty": self.presence_penalty,
+            "frequency_penalty": self.frequency_penalty,
+            "top_p": self.top_p,
+            "max_tokens": self.max_tokens_to_sample
+        }
+
+        def for_stream():
+            response = self.session.post(
+                self.api_endpoint, json=payload, stream=True, timeout=self.timeout
+            )
+            if not response.ok:
+                raise exceptions.FailedToGenerateResponseError(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+
+            streaming_response = ""
+            for line in response.iter_lines(decode_unicode=True, chunk_size=1):
+                if line:
+                    modified_line = re.sub("data:", "", line)
+                    try:
+                        json_data = json.loads(modified_line)
+                        content = json_data['choices'][0]['delta']['content']
+                        streaming_response += content
+                        yield content if raw else dict(text=streaming_response)
+                    except:
+                        continue
+            self.last_response.update(dict(text=streaming_response))
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
         return response["text"]
```

### Comparing `webscout-3.0/webscout/Provider/Cohere.py` & `webscout-3.0b0/webscout/Provider/Youchat.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,223 +1,221 @@
-import time
-import uuid
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import WebDriverWait
-import click
-import requests
-from requests import get
-from uuid import uuid4
-from re import findall
-from requests.exceptions import RequestException
-from curl_cffi.requests import get, RequestsError
-import g4f
-from random import randint
-from PIL import Image
-import io
-import re
-import json
-import yaml
-from ..AIutel import Optimizers
-from ..AIutel import Conversation
-from ..AIutel import AwesomePrompts, sanitize_stream
-from ..AIbase import  Provider, AsyncProvider
-from Helpingai_T2 import Perplexity
-from webscout import exceptions
-from typing import Any, AsyncGenerator, Dict
-import logging
-import httpx
-#-----------------------------------------------Cohere--------------------------------------------
-class Cohere(Provider):
-    def __init__(
-        self,
-        api_key: str,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
-        model: str = "command-r-plus",
-        temperature: float = 0.7,
-        system_prompt: str = "You are helpful AI",
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-        top_k: int = -1,
-        top_p: float = 0.999,
-    ):
-        """Initializes Cohere
-
-        Args:
-            api_key (str): Cohere API key.
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            model (str, optional): Model to use for generating text. Defaults to "command-r-plus".
-            temperature (float, optional): Diversity of the generated text. Higher values produce more diverse outputs.
-                            Defaults to 0.7.
-            system_prompt (str, optional): A system_prompt or context to set the style or tone of the generated text. 
-                            Defaults to "You are helpful AI".
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-        """
-        self.session = requests.Session()
-        self.is_conversation = is_conversation
-        self.max_tokens_to_sample = max_tokens
-        self.api_key = api_key
-        self.model = model
-        self.temperature = temperature
-        self.system_prompt = system_prompt
-        self.chat_endpoint = "https://production.api.os.cohere.ai/coral/v1/chat"
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.headers = {
-            "Content-Type": "application/json",
-            "Authorization": f"Bearer {self.api_key}",
-        }
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        self.session.headers.update(self.headers)
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session.proxies = proxies
-
-    def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict:
-        """Chat with AI
-
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict : {}
-        ```json
-        {
-           "text" : "How may I assist you today?"
-        }
-        ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-        self.session.headers.update(self.headers)
-        payload = {
-            "message": conversation_prompt,
-            "model": self.model,
-            "temperature": self.temperature,
-            "preamble": self.system_prompt,
-        }
-
-        def for_stream():
-            response = self.session.post(
-                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
-            )
-            if not response.ok:
-                raise Exception(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
-                )
-
-            for value in response.iter_lines(
-                decode_unicode=True,
-                chunk_size=self.stream_chunk_size,
-            ):
-                try:
-                    resp = json.loads(value.strip().split("\n")[-1])
-                    self.last_response.update(resp)
-                    yield value if raw else resp
-                except json.decoder.JSONDecodeError:
-                    pass
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
-
-        def for_non_stream():
-            # let's make use of stream
-            for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else for_non_stream()
-
-    def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str:
-        """Generate response `str`
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str: Response generated
-        """
-
-        def for_stream():
-            for response in self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            ):
-                yield self.get_message(response)
-
-        def for_non_stream():
-            return self.get_message(
-                self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else for_non_stream()
-
-    def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        return response["result"]["chatStreamEndEvent"]["response"]["text"]
+import time
+import uuid
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.ui import WebDriverWait
+import click
+import requests
+from requests import get
+from uuid import uuid4
+from re import findall
+from requests.exceptions import RequestException
+from curl_cffi.requests import get, RequestsError
+import g4f
+from random import randint
+from PIL import Image
+import io
+import re
+import json
+import yaml
+from ..AIutel import Optimizers
+from ..AIutel import Conversation
+from ..AIutel import AwesomePrompts, sanitize_stream
+from ..AIbase import  Provider, AsyncProvider
+from Helpingai_T2 import Perplexity
+from webscout import exceptions
+from typing import Any, AsyncGenerator, Dict
+import logging
+import httpx
+
+#-------------------------------------------------------youchat--------------------------------------------------------   
+class YouChat(Provider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        self.session = requests.Session()
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.chat_endpoint = "https://you.com/api/streamingSearch"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+
+        self.payload = {
+            "q": "",
+            "page": 1,
+            "count": 10,
+            "safeSearch": "Off",
+            "onShoppingPage": False,
+            "mkt": "",
+            "responseFilter": "WebPages,Translations,TimeZone,Computation,RelatedSearches",
+            "domain": "youchat",
+            "queryTraceId": uuid.uuid4(),
+            "conversationTurnId": uuid.uuid4(),
+            "pastChatLength": 0,
+            "selectedChatMode": "default",
+            "chat": "[]",
+        }
+
+        self.headers = {
+            "cache-control": "no-cache",
+            'User-Agent': 'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36',
+            'Referer': f'https://you.com/search?q={self.payload["q"]}&fromSearchBar=true&tbm=youchat&chatMode=default'
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.session.headers.update(self.headers)
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+        self.session.headers.update(self.headers)
+        self.session.headers.update(
+            dict(
+                cookie=f"safesearch_guest=Off; uuid_guest={str(uuid4())}",
+            )
+        )
+        self.payload["q"] = prompt
+
+        def for_stream():
+            response = self.session.get(
+                self.chat_endpoint,
+                params=self.payload,
+                stream=True,
+                timeout=self.timeout,
+            )
+
+            if not response.ok:
+                raise exceptions.FailedToGenerateResponseError(
+                    f"Failed to generate response - ({response.status_code}, {response.reason})"
+                )
+
+            streaming_response = ""
+            for line in response.iter_lines(decode_unicode=True, chunk_size=64):
+                if line:
+                    modified_value = re.sub("data:", "", line)
+                    try:
+                        json_modified_value = json.loads(modified_value)
+                        if "youChatToken" in json_modified_value:
+                            streaming_response += json_modified_value["youChatToken"]
+                            if print:
+                                print(json_modified_value["youChatToken"], end="")
+                    except:
+                        continue
+            self.last_response.update(dict(text=streaming_response))
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+            return streaming_response
+
+        def for_non_stream():
+            for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response["text"]
```

### Comparing `webscout-3.0/webscout/Provider/Gemini.py` & `webscout-3.0b0/webscout/Provider/BasedGPT.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,217 +1,226 @@
-import time
-import uuid
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import WebDriverWait
-import click
-import requests
-from requests import get
-from uuid import uuid4
-from re import findall
-from requests.exceptions import RequestException
-from curl_cffi.requests import get, RequestsError
-import g4f
-from random import randint
-from PIL import Image
-import io
-import re
-import json
-import yaml
-from ..AIutel import Optimizers
-from ..AIutel import Conversation
-from ..AIutel import AwesomePrompts, sanitize_stream
-from ..AIbase import  Provider, AsyncProvider
-from Helpingai_T2 import Perplexity
-from webscout import exceptions
-from typing import Any, AsyncGenerator, Dict
-import logging
-import httpx    
-from Bard import Chatbot
-import logging
-from os import path
-from json import load
-from json import dumps
-import warnings
-logging.getLogger("httpx").setLevel(logging.ERROR)
-warnings.simplefilter("ignore", category=UserWarning)
-class GEMINI(Provider):
-    def __init__(
-        self,
-        cookie_file: str,
-        proxy: dict = {},
-        timeout: int = 30,
-    ):
-        """Initializes GEMINI
-
-        Args:
-            cookie_file (str): Path to `bard.google.com.cookies.json` file
-            proxy (dict, optional): Http request proxy. Defaults to {}.
-            timeout (int, optional): Http request timeout. Defaults to 30.
-        """
-        self.conversation = Conversation(False)
-        self.session_auth1 = None
-        self.session_auth2 = None
-        assert isinstance(
-            cookie_file, str
-        ), f"cookie_file should be of {str} only not '{type(cookie_file)}'"
-        if path.isfile(cookie_file):
-            # let's assume auth is a path to exported .json cookie-file
-            with open(cookie_file) as fh:
-                entries = load(fh)
-            for entry in entries:
-                if entry["name"] == "__Secure-1PSID":
-                    self.session_auth1 = entry["value"]
-                elif entry["name"] == "__Secure-1PSIDTS":
-                    self.session_auth2 = entry["value"]
-
-            assert all(
-                [self.session_auth1, self.session_auth2]
-            ), f"Failed to extract the required cookie value from file '{cookie_file}'"
-        else:
-            raise Exception(f"{cookie_file} is not a valid file path")
-
-        self.session = Chatbot(self.session_auth1, self.session_auth2, proxy, timeout)
-        self.last_response = {}
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-
-    def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict:
-        """Chat with AI
-
-            Args:
-                prompt (str): Prompt to be send.
-                stream (bool, optional): Flag for streaming response. Defaults to False.
-                raw (bool, optional): Stream back raw response as received. Defaults to False.
-                optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defeaults to None
-                conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-            Returns:
-               dict : {}
-            ```json
-            {
-                "content": "General Kenobi! \n\n(I couldn't help but respond with the iconic Star Wars greeting since you used it first. )\n\nIs there anything I can help you with today?\n[Image of Hello there General Kenobi]",
-                "conversation_id": "c_f13f6217f9a997aa",
-                "response_id": "r_d3665f95975c368f",
-                "factualityQueries": null,
-                "textQuery": [
-                    "hello there",
-                    1
-                    ],
-                "choices": [
-                    {
-                        "id": "rc_ea075c9671bfd8cb",
-                        "content": [
-                            "General Kenobi! \n\n(I couldn't help but respond with the iconic Star Wars greeting since you used it first. )\n\nIs there anything I can help you with today?\n[Image of Hello there General Kenobi]"
-                        ]
-                    },
-                    {
-                        "id": "rc_de6dd3fb793a5402",
-                        "content": [
-                            "General Kenobi! (or just a friendly hello, whichever you prefer!). \n\nI see you're a person of culture as well. *Star Wars* references are always appreciated.  \n\nHow can I help you today?\n"
-                            ]
-                    },
-                {
-                    "id": "rc_a672ac089caf32db",
-                    "content": [
-                        "General Kenobi! (or just a friendly hello if you're not a Star Wars fan!). \n\nHow can I help you today? Feel free to ask me anything, or tell me what you'd like to chat about. I'm here to assist in any way I can.\n[Image of Obi-Wan Kenobi saying hello there]"
-                    ]
-                }
-            ],
-
-            "images": [
-                "https://i.pinimg.com/originals/40/74/60/407460925c9e419d82b93313f0b42f71.jpg"
-            ]
-        }
-
-            ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-
-        def for_stream():
-            response = self.session.ask(prompt)
-            self.last_response.update(response)
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
-            yield dumps(response) if raw else response
-
-        def for_non_stream():
-            # let's make use of stream
-            for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else for_non_stream()
-
-    def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str:
-        """Generate response `str`
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str: Response generated
-        """
-
-        def for_stream():
-            for response in self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            ):
-                yield self.get_message(response)
-
-        def for_non_stream():
-            return self.get_message(
-                self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else for_non_stream()
-
-    def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        return response["content"]
-
-    def reset(self):
-        """Reset the current conversation"""
-        self.session.async_chatbot.conversation_id = ""
-        self.session.async_chatbot.response_id = ""
-        self.session.async_chatbot.choice_id = ""
+import time
+import uuid
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.ui import WebDriverWait
+import click
+import requests
+from requests import get
+from uuid import uuid4
+from re import findall
+from requests.exceptions import RequestException
+from curl_cffi.requests import get, RequestsError
+import g4f
+from random import randint
+from PIL import Image
+import io
+import re
+import json
+import yaml
+from ..AIutel import Optimizers
+from ..AIutel import Conversation
+from ..AIutel import AwesomePrompts, sanitize_stream
+from ..AIbase import  Provider, AsyncProvider
+from webscout import exceptions
+from typing import Any, AsyncGenerator, Dict
+import logging
+import httpx
+
+class BasedGPT(Provider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+        system_prompt: str = "Be Helpful and Friendly",
+    ):
+        """Instantiates BasedGPT
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+            system_prompt (str, optional): System prompt for BasedGPT. Defaults to "Be Helpful and Friendly".
+        """
+        self.session = requests.Session()
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.chat_endpoint = "https://www.basedgpt.chat/api/chat"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.system_prompt = system_prompt
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.session.headers.update(
+            {"Content-Type": "application/json"}
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+            "id": "chatcmpl-TaREJpBZsRVQFRFic1wIA7Q7XfnaD",
+            "object": "chat.completion",
+            "created": 1704623244,
+            "model": "gpt-3.5-turbo",
+            "usage": {
+                "prompt_tokens": 0,
+                "completion_tokens": 0,
+                "total_tokens": 0
+                },
+            "choices": [
+                {
+                    "message": {
+                        "role": "assistant",
+                        "content": "Hello! How can I assist you today?"
+                },
+                "finish_reason": "stop",
+                "index": 0
+                }
+            ]
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        payload = {
+            "messages": [
+                {"role": "system", "content": self.system_prompt},
+                {"role": "user", "content": conversation_prompt},
+            ],
+        }
+
+        def for_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
+            )
+            if not response.ok:
+                raise exceptions.FailedToGenerateResponseError(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+
+            message_load = ""
+            for value in response.iter_lines(
+                decode_unicode=True,
+                delimiter="",
+                chunk_size=self.stream_chunk_size,
+            ):
+                try:
+                    message_load += value
+                    yield value if raw else dict(text=message_load)
+                except json.decoder.JSONDecodeError:
+                    pass
+            self.last_response.update(dict(text=message_load))
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response["text"]
```

### Comparing `webscout-3.0/webscout/Provider/Groq.py` & `webscout-3.0b0/webscout/Provider/Leo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,512 +1,469 @@
-import time
-import uuid
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import WebDriverWait
-import click
-import requests
-from requests import get
-from uuid import uuid4
-from re import findall
-from requests.exceptions import RequestException
-from curl_cffi.requests import get, RequestsError
-import g4f
-from random import randint
-from PIL import Image
-import io
-import re
-import json
-import yaml
-from ..AIutel import Optimizers
-from ..AIutel import Conversation
-from ..AIutel import AwesomePrompts, sanitize_stream
-from ..AIbase import  Provider, AsyncProvider
-from Helpingai_T2 import Perplexity
-from webscout import exceptions
-from typing import Any, AsyncGenerator, Dict
-import logging
-import httpx
-
-class GROQ(Provider):
-    def __init__(
-        self,
-        api_key: str,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
-        temperature: float = 1,
-        presence_penalty: int = 0,
-        frequency_penalty: int = 0,
-        top_p: float = 1,
-        model: str = "mixtral-8x7b-32768",
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-    ):
-        """Instantiates GROQ
-
-        Args:
-            api_key (key): GROQ's API key.
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            temperature (float, optional): Charge of the generated text's randomness. Defaults to 1.
-            presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
-            frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
-            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
-            model (str, optional): LLM model name. Defaults to "gpt-3.5-turbo".
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-        """
-        self.session = requests.Session()
-        self.is_conversation = is_conversation
-        self.max_tokens_to_sample = max_tokens
-        self.api_key = api_key
-        self.model = model
-        self.temperature = temperature
-        self.presence_penalty = presence_penalty
-        self.frequency_penalty = frequency_penalty
-        self.top_p = top_p
-        self.chat_endpoint = "https://api.groq.com/openai/v1/chat/completions"
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.headers = {
-            "Content-Type": "application/json",
-            "Authorization": f"Bearer {self.api_key}",
-        }
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        self.session.headers.update(self.headers)
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session.proxies = proxies
-
-    def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict:
-        """Chat with AI
-
-                Args:
-                    prompt (str): Prompt to be send.
-                    stream (bool, optional): Flag for streaming response. Defaults to False.
-                    raw (bool, optional): Stream back raw response as received. Defaults to False.
-                    optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-                    conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-                Returns:
-                   dict : {}
-                ```json
-        {
-            "id": "c0c8d139-d2b9-9909-8aa1-14948bc28404",
-            "object": "chat.completion",
-            "created": 1710852779,
-            "model": "mixtral-8x7b-32768",
-            "choices": [
-                {
-                    "index": 0,
-                    "message": {
-                        "role": "assistant",
-                        "content": "Hello! How can I assist you today? I'm here to help answer your questions and engage in conversation on a wide variety of topics. Feel free to ask me anything!"
-                    },
-                    "logprobs": null,
-                    "finish_reason": "stop"
-                }
-            ],
-            "usage": {
-                "prompt_tokens": 47,
-                "prompt_time": 0.03,
-                "completion_tokens": 37,
-                "completion_time": 0.069,
-                "total_tokens": 84,
-                "total_time": 0.099
-            },
-            "system_fingerprint": null
-        }
-                ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-        self.session.headers.update(self.headers)
-        payload = {
-            "frequency_penalty": self.frequency_penalty,
-            "messages": [{"content": conversation_prompt, "role": "user"}],
-            "model": self.model,
-            "presence_penalty": self.presence_penalty,
-            "stream": stream,
-            "temperature": self.temperature,
-            "top_p": self.top_p,
-        }
-
-        def for_stream():
-            response = self.session.post(
-                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
-            )
-            if not response.ok:
-                raise Exception(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
-                )
-
-            message_load = ""
-            for value in response.iter_lines(
-                decode_unicode=True,
-                delimiter="" if raw else "data:",
-                chunk_size=self.stream_chunk_size,
-            ):
-                try:
-                    resp = json.loads(value)
-                    incomplete_message = self.get_message(resp)
-                    if incomplete_message:
-                        message_load += incomplete_message
-                        resp["choices"][0]["delta"]["content"] = message_load
-                        self.last_response.update(resp)
-                        yield value if raw else resp
-                    elif raw:
-                        yield value
-                except json.decoder.JSONDecodeError:
-                    pass
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
-
-        def for_non_stream():
-            response = self.session.post(
-                self.chat_endpoint, json=payload, stream=False, timeout=self.timeout
-            )
-            if not response.ok:
-                raise Exception(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
-                )
-            resp = response.json()
-            self.last_response.update(resp)
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
-            return resp
-
-        return for_stream() if stream else for_non_stream()
-
-    def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str:
-        """Generate response `str`
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str: Response generated
-        """
-
-        def for_stream():
-            for response in self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            ):
-                yield self.get_message(response)
-
-        def for_non_stream():
-            return self.get_message(
-                self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else for_non_stream()
-
-    def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        try:
-            if response["choices"][0].get("delta"):
-                return response["choices"][0]["delta"]["content"]
-            return response["choices"][0]["message"]["content"]
-        except KeyError:
-            return ""
-class AsyncGROQ(AsyncProvider):
-    def __init__(
-        self,
-        api_key: str,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
-        temperature: float = 1,
-        presence_penalty: int = 0,
-        frequency_penalty: int = 0,
-        top_p: float = 1,
-        model: str = "mixtral-8x7b-32768",
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-    ):
-        """Instantiates GROQ
-
-        Args:
-            api_key (key): GROQ's API key.
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            temperature (float, optional): Charge of the generated text's randomness. Defaults to 1.
-            presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
-            frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
-            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
-            model (str, optional): LLM model name. Defaults to "gpt-3.5-turbo".
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-        """
-        self.is_conversation = is_conversation
-        self.max_tokens_to_sample = max_tokens
-        self.api_key = api_key
-        self.model = model
-        self.temperature = temperature
-        self.presence_penalty = presence_penalty
-        self.frequency_penalty = frequency_penalty
-        self.top_p = top_p
-        self.chat_endpoint = "https://api.groq.com/openai/v1/chat/completions"
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.headers = {
-            "Content-Type": "application/json",
-            "Authorization": f"Bearer {self.api_key}",
-        }
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session = httpx.AsyncClient(headers=self.headers, proxies=proxies)
-
-    async def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict | AsyncGenerator:
-        """Chat with AI asynchronously.
-
-                Args:
-                    prompt (str): Prompt to be send.
-                    stream (bool, optional): Flag for streaming response. Defaults to False.
-                    raw (bool, optional): Stream back raw response as received. Defaults to False.
-                    optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-                    conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-                Returns:
-                   dict|AsyncGenerator : ai content
-                ```json
-        {
-            "id": "c0c8d139-d2b9-9909-8aa1-14948bc28404",
-            "object": "chat.completion",
-            "created": 1710852779,
-            "model": "mixtral-8x7b-32768",
-            "choices": [
-                {
-                    "index": 0,
-                    "message": {
-                        "role": "assistant",
-                        "content": "Hello! How can I assist you today? I'm here to help answer your questions and engage in conversation on a wide variety of topics. Feel free to ask me anything!"
-                    },
-                    "logprobs": null,
-                    "finish_reason": "stop"
-                }
-            ],
-            "usage": {
-                "prompt_tokens": 47,
-                "prompt_time": 0.03,
-                "completion_tokens": 37,
-                "completion_time": 0.069,
-                "total_tokens": 84,
-                "total_time": 0.099
-            },
-            "system_fingerprint": null
-        }
-                ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-        payload = {
-            "frequency_penalty": self.frequency_penalty,
-            "messages": [{"content": conversation_prompt, "role": "user"}],
-            "model": self.model,
-            "presence_penalty": self.presence_penalty,
-            "stream": stream,
-            "temperature": self.temperature,
-            "top_p": self.top_p,
-        }
-
-        async def for_stream():
-            async with self.session.stream(
-                "POST", self.chat_endpoint, json=payload, timeout=self.timeout
-            ) as response:
-                if not response.is_success:
-                    raise Exception(
-                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
-                    )
-
-                message_load = ""
-                intro_value = "data:"
-                async for value in response.aiter_lines():
-                    try:
-                        if value.startswith(intro_value):
-                            value = value[len(intro_value) :]
-                        resp = json.loads(value)
-                        incomplete_message = await self.get_message(resp)
-                        if incomplete_message:
-                            message_load += incomplete_message
-                            resp["choices"][0]["delta"]["content"] = message_load
-                            self.last_response.update(resp)
-                            yield value if raw else resp
-                        elif raw:
-                            yield value
-                    except json.decoder.JSONDecodeError:
-                        pass
-            self.conversation.update_chat_history(
-                prompt, await self.get_message(self.last_response)
-            )
-
-        async def for_non_stream():
-            response = httpx.post(
-                self.chat_endpoint, json=payload, timeout=self.timeout
-            )
-            if not response.is_success:
-                raise Exception(
-                    f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
-                )
-            resp = response.json()
-            self.last_response.update(resp)
-            self.conversation.update_chat_history(
-                prompt, await self.get_message(self.last_response)
-            )
-            return resp
-
-        return for_stream() if stream else await for_non_stream()
-
-    async def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str | AsyncGenerator:
-        """Generate response `str` asynchronously.
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str|AsyncGenerator: Response generated
-        """
-
-        async def for_stream():
-            async_ask = await self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            )
-            async for response in async_ask:
-                yield await self.get_message(response)
-
-        async def for_non_stream():
-            return await self.get_message(
-                await self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else await for_non_stream()
-
-    async def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        try:
-            if response["choices"][0].get("delta"):
-                return response["choices"][0]["delta"]["content"]
-            return response["choices"][0]["message"]["content"]
-        except KeyError:
-            return ""
+import time
+import uuid
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.ui import WebDriverWait
+import click
+import requests
+from requests import get
+from uuid import uuid4
+from re import findall
+from requests.exceptions import RequestException
+from curl_cffi.requests import get, RequestsError
+import g4f
+from random import randint
+from PIL import Image
+import io
+import re
+import json
+import yaml
+from ..AIutel import Optimizers
+from ..AIutel import Conversation
+from ..AIutel import AwesomePrompts, sanitize_stream
+from ..AIbase import  Provider, AsyncProvider
+from Helpingai_T2 import Perplexity
+from webscout import exceptions
+from typing import Any, AsyncGenerator, Dict
+import logging
+import httpx
+#--------------------------------------LEO-----------------------------------------
+class LEO(Provider):
+    
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        temperature: float = 0.2,
+        top_k: int = -1,
+        top_p: float = 0.999,
+        model: str = "llama-2-13b-chat",
+        brave_key: str = "qztbjzBqJueQZLFkwTTJrieu8Vw3789u",
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiate TGPT
+
+        Args:
+            is_conversation (str, optional): Flag for chatting conversationally. Defaults to True.
+            brave_key (str, optional): Brave API access key. Defaults to "qztbjzBqJueQZLFkwTTJrieu8Vw3789u".
+            model (str, optional): Text generation model name. Defaults to "llama-2-13b-chat".
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.2.
+            top_k (int, optional): Chance of topic being repeated. Defaults to -1.
+            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
+            timeput (int, optional): Http requesting timeout. Defaults to 30
+            intro (str, optional): Conversation introductory prompt. Defaults to `Conversation.intro`.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional) : Http reqiuest proxies (socks). Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.session = requests.Session()
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.model = model
+        self.stop_sequences = ["</response>", "</s>"]
+        self.temperature = temperature
+        self.top_k = top_k
+        self.top_p = top_p
+        self.chat_endpoint = "https://ai-chat.bsg.brave.com/v1/complete"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.headers = {
+            "Content-Type": "application/json",
+            "accept": "text/event-stream",
+            "x-brave-key": brave_key,
+            "accept-language": "en-US,en;q=0.9",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:99.0) Gecko/20100101 Firefox/110.0",
+        }
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.session.headers.update(self.headers)
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+        self.system_prompt = (
+            "\n\nYour name is Leo, a helpful"
+            "respectful and honest AI assistant created by the company Brave. You will be replying to a user of the Brave browser. "
+            "Always respond in a neutral tone. Be polite and courteous. Answer concisely in no more than 50-80 words."
+            "\n\nPlease ensure that your responses are socially unbiased and positive in nature."
+            "If a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. "
+            "If you don't know the answer to a question, please don't share false information.\n"
+        )
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+            "completion": "\nNext: domestic cat breeds with short hair >>",
+            "stop_reason": null,
+            "truncated": false,
+            "stop": null,
+            "model": "llama-2-13b-chat",
+            "log_id": "cmpl-3kYiYxSNDvgMShSzFooz6t",
+            "exception": null
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        self.session.headers.update(self.headers)
+        payload = {
+            "max_tokens_to_sample": self.max_tokens_to_sample,
+            "model": self.model,
+            "prompt": f"<s>[INST] <<SYS>>{self.system_prompt}<</SYS>>{conversation_prompt} [/INST]",
+            "self.stop_sequence": self.stop_sequences,
+            "stream": stream,
+            "top_k": self.top_k,
+            "top_p": self.top_p,
+        }
+
+        def for_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
+            )
+            if (
+                not response.ok
+                or not response.headers.get("Content-Type")
+                == "text/event-stream; charset=utf-8"
+            ):
+                raise Exception(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+
+            for value in response.iter_lines(
+                decode_unicode=True,
+                delimiter="" if raw else "data:",
+                chunk_size=self.stream_chunk_size,
+            ):
+                try:
+                    resp = json.loads(value)
+                    self.last_response.update(resp)
+                    yield value if raw else resp
+                except json.decoder.JSONDecodeError:
+                    pass
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=False, timeout=self.timeout
+            )
+            if (
+                not response.ok
+                or not response.headers.get("Content-Type", "") == "application/json"
+            ):
+                raise Exception(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+            resp = response.json()
+            self.last_response.update(resp)
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+            return resp
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response.get("completion")
+class AsyncLEO(AsyncProvider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        temperature: float = 0.2,
+        top_k: int = -1,
+        top_p: float = 0.999,
+        model: str = "llama-2-13b-chat",
+        brave_key: str = "qztbjzBqJueQZLFkwTTJrieu8Vw3789u",
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiate TGPT
+
+        Args:
+            is_conversation (str, optional): Flag for chatting conversationally. Defaults to True.
+            brave_key (str, optional): Brave API access key. Defaults to "qztbjzBqJueQZLFkwTTJrieu8Vw3789u".
+            model (str, optional): Text generation model name. Defaults to "llama-2-13b-chat".
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.2.
+            top_k (int, optional): Chance of topic being repeated. Defaults to -1.
+            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
+            timeput (int, optional): Http requesting timeout. Defaults to 30
+            intro (str, optional): Conversation introductory prompt. Defaults to `Conversation.intro`.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional) : Http reqiuest proxies (socks). Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.model = model
+        self.stop_sequences = ["</response>", "</s>"]
+        self.temperature = temperature
+        self.top_k = top_k
+        self.top_p = top_p
+        self.chat_endpoint = "https://ai-chat.bsg.brave.com/v1/complete"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.headers = {
+            "Content-Type": "application/json",
+            "accept": "text/event-stream",
+            "x-brave-key": brave_key,
+            "accept-language": "en-US,en;q=0.9",
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:99.0) Gecko/20100101 Firefox/110.0",
+        }
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.system_prompt = (
+            "\n\nYour name is Leo, a helpful"
+            "respectful and honest AI assistant created by the company Brave. You will be replying to a user of the Brave browser. "
+            "Always respond in a neutral tone. Be polite and courteous. Answer concisely in no more than 50-80 words."
+            "\n\nPlease ensure that your responses are socially unbiased and positive in nature."
+            "If a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. "
+            "If you don't know the answer to a question, please don't share false information.\n"
+        )
+        self.session = httpx.AsyncClient(headers=self.headers, proxies=proxies)
+
+    async def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict | AsyncGenerator:
+        """Chat with AI asynchronously.
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict|AsyncGenerator : ai content
+        ```json
+        {
+            "completion": "\nNext: domestic cat breeds with short hair >>",
+            "stop_reason": null,
+            "truncated": false,
+            "stop": null,
+            "model": "llama-2-13b-chat",
+            "log_id": "cmpl-3kYiYxSNDvgMShSzFooz6t",
+            "exception": null
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        payload = {
+            "max_tokens_to_sample": self.max_tokens_to_sample,
+            "model": self.model,
+            "prompt": f"<s>[INST] <<SYS>>{self.system_prompt}<</SYS>>{conversation_prompt} [/INST]",
+            "self.stop_sequence": self.stop_sequences,
+            "stream": stream,
+            "top_k": self.top_k,
+            "top_p": self.top_p,
+        }
+
+        async def for_stream():
+            async with self.session.stream(
+                "POST", self.chat_endpoint, json=payload, timeout=self.timeout
+            ) as response:
+                if (
+                    not response.is_success
+                    or not response.headers.get("Content-Type")
+                    == "text/event-stream; charset=utf-8"
+                ):
+                    raise exceptions.FailedToGenerateResponseError(
+                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
+                    )
+                async for value in response.aiter_lines():
+                    try:
+                        resp = sanitize_stream(value)
+                        self.last_response.update(resp)
+                        yield value if raw else resp
+                    except json.decoder.JSONDecodeError:
+                        pass
+
+            self.conversation.update_chat_history(
+                prompt, await self.get_message(self.last_response)
+            )
+
+        async def for_non_stream():
+            async for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str | AsyncGenerator:
+        """Generate response `str` asynchronously.
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str|AsyncGenerator: Response generated
+        """
+
+        async def for_stream():
+            async_ask = await self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            )
+            async for response in async_ask:
+                yield await self.get_message(response)
+
+        async def for_non_stream():
+            return await self.get_message(
+                await self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response.get("completion")
```

### Comparing `webscout-3.0/webscout/Provider/Koboldai.py` & `webscout-3.0b0/webscout/Provider/Blackboxai.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,402 +1,440 @@
-import time
-import uuid
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import WebDriverWait
-import click
-import requests
-from requests import get
-from uuid import uuid4
-from re import findall
-from requests.exceptions import RequestException
-from curl_cffi.requests import get, RequestsError
-import g4f
-from random import randint
-from PIL import Image
-import io
-import re
-import json
-import yaml
-from ..AIutel import Optimizers
-from ..AIutel import Conversation
-from ..AIutel import AwesomePrompts, sanitize_stream
-from ..AIbase import  Provider, AsyncProvider
-from Helpingai_T2 import Perplexity
-from webscout import exceptions
-from typing import Any, AsyncGenerator, Dict
-import logging
-import httpx
-#------------------------------------------------------KOBOLDAI-----------------------------------------------------------
-class KOBOLDAI(Provider):
-    def __init__(
-        self,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
-        temperature: float = 1,
-        top_p: float = 1,
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-    ):
-        """Instantiate TGPT
-
-        Args:
-            is_conversation (str, optional): Flag for chatting conversationally. Defaults to True.
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.2.
-            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
-            timeout (int, optional): Http requesting timeout. Defaults to 30
-            intro (str, optional): Conversation introductory prompt. Defaults to `Conversation.intro`.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional) : Http reqiuest proxies (socks). Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-        """
-        self.session = requests.Session()
-        self.is_conversation = is_conversation
-        self.max_tokens_to_sample = max_tokens
-        self.temperature = temperature
-        self.top_p = top_p
-        self.chat_endpoint = (
-            "https://koboldai-koboldcpp-tiefighter.hf.space/api/extra/generate/stream"
-        )
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.headers = {
-            "Content-Type": "application/json",
-            "Accept": "application/json",
-        }
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        self.session.headers.update(self.headers)
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session.proxies = proxies
-
-    def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict:
-        """Chat with AI
-
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict : {}
-        ```json
-        {
-           "token" : "How may I assist you today?"
-        }
-        ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-
-        self.session.headers.update(self.headers)
-        payload = {
-            "prompt": conversation_prompt,
-            "temperature": self.temperature,
-            "top_p": self.top_p,
-        }
-
-        def for_stream():
-            response = self.session.post(
-                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
-            )
-            if not response.ok:
-                raise Exception(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
-                )
-
-            message_load = ""
-            for value in response.iter_lines(
-                decode_unicode=True,
-                delimiter="" if raw else "event: message\ndata:",
-                chunk_size=self.stream_chunk_size,
-            ):
-                try:
-                    resp = json.loads(value)
-                    message_load += self.get_message(resp)
-                    resp["token"] = message_load
-                    self.last_response.update(resp)
-                    yield value if raw else resp
-                except json.decoder.JSONDecodeError:
-                    pass
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
-
-        def for_non_stream():
-            # let's make use of stream
-            for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else for_non_stream()
-
-    def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str:
-        """Generate response `str`
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str: Response generated
-        """
-
-        def for_stream():
-            for response in self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            ):
-                yield self.get_message(response)
-
-        def for_non_stream():
-            return self.get_message(
-                self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else for_non_stream()
-
-    def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        return response.get("token")
-class AsyncKOBOLDAI(AsyncProvider):
-    def __init__(
-        self,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
-        temperature: float = 1,
-        top_p: float = 1,
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-    ):
-        """Instantiate TGPT
-
-        Args:
-            is_conversation (str, optional): Flag for chatting conversationally. Defaults to True.
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.2.
-            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
-            timeout (int, optional): Http requesting timeout. Defaults to 30
-            intro (str, optional): Conversation introductory prompt. Defaults to `Conversation.intro`.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional) : Http reqiuest proxies (socks). Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-        """
-        self.is_conversation = is_conversation
-        self.max_tokens_to_sample = max_tokens
-        self.temperature = temperature
-        self.top_p = top_p
-        self.chat_endpoint = (
-            "https://koboldai-koboldcpp-tiefighter.hf.space/api/extra/generate/stream"
-        )
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.headers = {
-            "Content-Type": "application/json",
-            "Accept": "application/json",
-        }
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session = httpx.AsyncClient(headers=self.headers, proxies=proxies)
-
-    async def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict | AsyncGenerator:
-        """Chat with AI asynchronously.
-
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict|AsyncGenerator : ai content
-        ```json
-        {
-           "token" : "How may I assist you today?"
-        }
-        ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-
-        payload = {
-            "prompt": conversation_prompt,
-            "temperature": self.temperature,
-            "top_p": self.top_p,
-        }
-
-        async def for_stream():
-            async with self.session.stream(
-                "POST", self.chat_endpoint, json=payload, timeout=self.timeout
-            ) as response:
-                if not response.is_success:
-                    raise exceptions.FailedToGenerateResponseError(
-                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
-                    )
-
-                message_load = ""
-                async for value in response.aiter_lines():
-                    try:
-                        resp = sanitize_stream(value)
-                        message_load += await self.get_message(resp)
-                        resp["token"] = message_load
-                        self.last_response.update(resp)
-                        yield value if raw else resp
-                    except json.decoder.JSONDecodeError:
-                        pass
-
-            self.conversation.update_chat_history(
-                prompt, await self.get_message(self.last_response)
-            )
-
-        async def for_non_stream():
-            # let's make use of stream
-            async for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else await for_non_stream()
-
-    async def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str | AsyncGenerator:
-        """Generate response `str` asynchronously.
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str: Response generated
-        """
-
-        async def for_stream():
-            async_ask = await self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            )
-            async for response in async_ask:
-                yield await self.get_message(response)
-
-        async def for_non_stream():
-            return await self.get_message(
-                await self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else await for_non_stream()
-
-    async def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        return response.get("token")
+import time
+import uuid
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.ui import WebDriverWait
+import click
+import requests
+from requests import get
+from uuid import uuid4
+from re import findall
+from requests.exceptions import RequestException
+from curl_cffi.requests import get, RequestsError
+import g4f
+from random import randint
+from PIL import Image
+import io
+import re
+import json
+import yaml
+from ..AIutel import Optimizers
+from ..AIutel import Conversation
+from ..AIutel import AwesomePrompts, sanitize_stream
+from ..AIbase import  Provider, AsyncProvider
+from Helpingai_T2 import Perplexity
+from webscout import exceptions
+from typing import Any, AsyncGenerator, Dict
+import logging
+import httpx
+
+#------------------------------------------------------BLACKBOXAI--------------------------------------------------------  
+class BLACKBOXAI:
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 8000,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+        model: str = None,
+    ):
+        """Instantiates BLACKBOXAI
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+            model (str, optional): Model name. Defaults to "Phind Model".
+        """
+        self.session = requests.Session()
+        self.max_tokens_to_sample = max_tokens
+        self.is_conversation = is_conversation
+        self.chat_endpoint = "https://www.blackbox.ai/api/chat"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.model = model
+        self.previewToken: str = None
+        self.userId: str = ""
+        self.codeModelMode: bool = True
+        self.id: str = ""
+        self.agentMode: dict = {}
+        self.trendingAgentMode: dict = {}
+        self.isMicMode: bool = False
+
+        self.headers = {
+            "Content-Type": "application/json",
+            "User-Agent": "",
+            "Accept": "*/*",
+            "Accept-Encoding": "Identity",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.session.headers.update(self.headers)
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+           "text" : "print('How may I help you today?')"
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        self.session.headers.update(self.headers)
+        payload = {
+            "messages": [
+                # json.loads(prev_messages),
+                {"content": conversation_prompt, "role": "user"}
+            ],
+            "id": self.id,
+            "previewToken": self.previewToken,
+            "userId": self.userId,
+            "codeModelMode": self.codeModelMode,
+            "agentMode": self.agentMode,
+            "trendingAgentMode": self.trendingAgentMode,
+            "isMicMode": self.isMicMode,
+        }
+
+        def for_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
+            )
+            if (
+                not response.ok
+                or not response.headers.get("Content-Type")
+                == "text/plain; charset=utf-8"
+            ):
+                raise Exception(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+            streaming_text = ""
+            for value in response.iter_lines(
+                decode_unicode=True,
+                chunk_size=self.stream_chunk_size,
+                delimiter="\n",
+            ):
+                try:
+                    if bool(value):
+                        streaming_text += value + ("\n" if stream else "")
+
+                        resp = dict(text=streaming_text)
+                        self.last_response.update(resp)
+                        yield value if raw else resp
+                except json.decoder.JSONDecodeError:
+                    pass
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response["text"]
+    @staticmethod
+    def chat_cli(prompt):
+        """Sends a request to the BLACKBOXAI API and processes the response."""
+        blackbox_ai = BLACKBOXAI()  # Initialize a BLACKBOXAI instance
+        response = blackbox_ai.ask(prompt)  # Perform a chat with the given prompt
+        processed_response = blackbox_ai.get_message(response)  # Process the response
+        print(processed_response)
+class AsyncBLACKBOXAI(AsyncProvider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+        model: str = None,
+    ):
+        """Instantiates BLACKBOXAI
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+            model (str, optional): Model name. Defaults to "Phind Model".
+        """
+        self.max_tokens_to_sample = max_tokens
+        self.is_conversation = is_conversation
+        self.chat_endpoint = "https://www.blackbox.ai/api/chat"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.model = model
+        self.previewToken: str = None
+        self.userId: str = ""
+        self.codeModelMode: bool = True
+        self.id: str = ""
+        self.agentMode: dict = {}
+        self.trendingAgentMode: dict = {}
+        self.isMicMode: bool = False
+
+        self.headers = {
+            "Content-Type": "application/json",
+            "User-Agent": "",
+            "Accept": "*/*",
+            "Accept-Encoding": "Identity",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session = httpx.AsyncClient(headers=self.headers, proxies=proxies)
+
+    async def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict | AsyncGenerator:
+        """Chat with AI asynchronously.
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict|AsyncGenerator : ai content
+        ```json
+        {
+           "text" : "print('How may I help you today?')"
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        payload = {
+            "messages": [
+                # json.loads(prev_messages),
+                {"content": conversation_prompt, "role": "user"}
+            ],
+            "id": self.id,
+            "previewToken": self.previewToken,
+            "userId": self.userId,
+            "codeModelMode": self.codeModelMode,
+            "agentMode": self.agentMode,
+            "trendingAgentMode": self.trendingAgentMode,
+            "isMicMode": self.isMicMode,
+        }
+
+        async def for_stream():
+            async with self.session.stream(
+                "POST", self.chat_endpoint, json=payload, timeout=self.timeout
+            ) as response:
+                if (
+                    not response.is_success
+                    or not response.headers.get("Content-Type")
+                    == "text/plain; charset=utf-8"
+                ):
+                    raise exceptions.FailedToGenerateResponseError(
+                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
+                    )
+                streaming_text = ""
+                async for value in response.aiter_lines():
+                    try:
+                        if bool(value):
+                            streaming_text += value + ("\n" if stream else "")
+                            resp = dict(text=streaming_text)
+                            self.last_response.update(resp)
+                            yield value if raw else resp
+                    except json.decoder.JSONDecodeError:
+                        pass
+            self.conversation.update_chat_history(
+                prompt, await self.get_message(self.last_response)
+            )
+
+        async def for_non_stream():
+            async for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str | AsyncGenerator:
+        """Generate response `str` asynchronously.
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str|AsyncGenerator: Response generated
+        """
+
+        async def for_stream():
+            async_ask = await self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            )
+            async for response in async_ask:
+                yield await self.get_message(response)
+
+        async def for_non_stream():
+            return await self.get_message(
+                await self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response["text"]
```

### Comparing `webscout-3.0/webscout/Provider/Leo.py` & `webscout-3.0b0/webscout/Provider/Openai.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,469 +1,511 @@
-import time
-import uuid
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import WebDriverWait
-import click
-import requests
-from requests import get
-from uuid import uuid4
-from re import findall
-from requests.exceptions import RequestException
-from curl_cffi.requests import get, RequestsError
-import g4f
-from random import randint
-from PIL import Image
-import io
-import re
-import json
-import yaml
-from ..AIutel import Optimizers
-from ..AIutel import Conversation
-from ..AIutel import AwesomePrompts, sanitize_stream
-from ..AIbase import  Provider, AsyncProvider
-from Helpingai_T2 import Perplexity
-from webscout import exceptions
-from typing import Any, AsyncGenerator, Dict
-import logging
-import httpx
-#--------------------------------------LEO-----------------------------------------
-class LEO(Provider):
-    
-    def __init__(
-        self,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
-        temperature: float = 0.2,
-        top_k: int = -1,
-        top_p: float = 0.999,
-        model: str = "llama-2-13b-chat",
-        brave_key: str = "qztbjzBqJueQZLFkwTTJrieu8Vw3789u",
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-    ):
-        """Instantiate TGPT
-
-        Args:
-            is_conversation (str, optional): Flag for chatting conversationally. Defaults to True.
-            brave_key (str, optional): Brave API access key. Defaults to "qztbjzBqJueQZLFkwTTJrieu8Vw3789u".
-            model (str, optional): Text generation model name. Defaults to "llama-2-13b-chat".
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.2.
-            top_k (int, optional): Chance of topic being repeated. Defaults to -1.
-            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
-            timeput (int, optional): Http requesting timeout. Defaults to 30
-            intro (str, optional): Conversation introductory prompt. Defaults to `Conversation.intro`.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional) : Http reqiuest proxies (socks). Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-        """
-        self.session = requests.Session()
-        self.is_conversation = is_conversation
-        self.max_tokens_to_sample = max_tokens
-        self.model = model
-        self.stop_sequences = ["</response>", "</s>"]
-        self.temperature = temperature
-        self.top_k = top_k
-        self.top_p = top_p
-        self.chat_endpoint = "https://ai-chat.bsg.brave.com/v1/complete"
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.headers = {
-            "Content-Type": "application/json",
-            "accept": "text/event-stream",
-            "x-brave-key": brave_key,
-            "accept-language": "en-US,en;q=0.9",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:99.0) Gecko/20100101 Firefox/110.0",
-        }
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        self.session.headers.update(self.headers)
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session.proxies = proxies
-        self.system_prompt = (
-            "\n\nYour name is Leo, a helpful"
-            "respectful and honest AI assistant created by the company Brave. You will be replying to a user of the Brave browser. "
-            "Always respond in a neutral tone. Be polite and courteous. Answer concisely in no more than 50-80 words."
-            "\n\nPlease ensure that your responses are socially unbiased and positive in nature."
-            "If a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. "
-            "If you don't know the answer to a question, please don't share false information.\n"
-        )
-
-    def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict:
-        """Chat with AI
-
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict : {}
-        ```json
-        {
-            "completion": "\nNext: domestic cat breeds with short hair >>",
-            "stop_reason": null,
-            "truncated": false,
-            "stop": null,
-            "model": "llama-2-13b-chat",
-            "log_id": "cmpl-3kYiYxSNDvgMShSzFooz6t",
-            "exception": null
-        }
-        ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-
-        self.session.headers.update(self.headers)
-        payload = {
-            "max_tokens_to_sample": self.max_tokens_to_sample,
-            "model": self.model,
-            "prompt": f"<s>[INST] <<SYS>>{self.system_prompt}<</SYS>>{conversation_prompt} [/INST]",
-            "self.stop_sequence": self.stop_sequences,
-            "stream": stream,
-            "top_k": self.top_k,
-            "top_p": self.top_p,
-        }
-
-        def for_stream():
-            response = self.session.post(
-                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
-            )
-            if (
-                not response.ok
-                or not response.headers.get("Content-Type")
-                == "text/event-stream; charset=utf-8"
-            ):
-                raise Exception(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
-                )
-
-            for value in response.iter_lines(
-                decode_unicode=True,
-                delimiter="" if raw else "data:",
-                chunk_size=self.stream_chunk_size,
-            ):
-                try:
-                    resp = json.loads(value)
-                    self.last_response.update(resp)
-                    yield value if raw else resp
-                except json.decoder.JSONDecodeError:
-                    pass
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
-
-        def for_non_stream():
-            response = self.session.post(
-                self.chat_endpoint, json=payload, stream=False, timeout=self.timeout
-            )
-            if (
-                not response.ok
-                or not response.headers.get("Content-Type", "") == "application/json"
-            ):
-                raise Exception(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
-                )
-            resp = response.json()
-            self.last_response.update(resp)
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
-            return resp
-
-        return for_stream() if stream else for_non_stream()
-
-    def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str:
-        """Generate response `str`
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str: Response generated
-        """
-
-        def for_stream():
-            for response in self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            ):
-                yield self.get_message(response)
-
-        def for_non_stream():
-            return self.get_message(
-                self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else for_non_stream()
-
-    def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        return response.get("completion")
-class AsyncLEO(AsyncProvider):
-    def __init__(
-        self,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
-        temperature: float = 0.2,
-        top_k: int = -1,
-        top_p: float = 0.999,
-        model: str = "llama-2-13b-chat",
-        brave_key: str = "qztbjzBqJueQZLFkwTTJrieu8Vw3789u",
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-    ):
-        """Instantiate TGPT
-
-        Args:
-            is_conversation (str, optional): Flag for chatting conversationally. Defaults to True.
-            brave_key (str, optional): Brave API access key. Defaults to "qztbjzBqJueQZLFkwTTJrieu8Vw3789u".
-            model (str, optional): Text generation model name. Defaults to "llama-2-13b-chat".
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.2.
-            top_k (int, optional): Chance of topic being repeated. Defaults to -1.
-            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
-            timeput (int, optional): Http requesting timeout. Defaults to 30
-            intro (str, optional): Conversation introductory prompt. Defaults to `Conversation.intro`.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional) : Http reqiuest proxies (socks). Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-        """
-        self.is_conversation = is_conversation
-        self.max_tokens_to_sample = max_tokens
-        self.model = model
-        self.stop_sequences = ["</response>", "</s>"]
-        self.temperature = temperature
-        self.top_k = top_k
-        self.top_p = top_p
-        self.chat_endpoint = "https://ai-chat.bsg.brave.com/v1/complete"
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.headers = {
-            "Content-Type": "application/json",
-            "accept": "text/event-stream",
-            "x-brave-key": brave_key,
-            "accept-language": "en-US,en;q=0.9",
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:99.0) Gecko/20100101 Firefox/110.0",
-        }
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.system_prompt = (
-            "\n\nYour name is Leo, a helpful"
-            "respectful and honest AI assistant created by the company Brave. You will be replying to a user of the Brave browser. "
-            "Always respond in a neutral tone. Be polite and courteous. Answer concisely in no more than 50-80 words."
-            "\n\nPlease ensure that your responses are socially unbiased and positive in nature."
-            "If a question does not make any sense, or is not factually coherent, explain why instead of answering something not correct. "
-            "If you don't know the answer to a question, please don't share false information.\n"
-        )
-        self.session = httpx.AsyncClient(headers=self.headers, proxies=proxies)
-
-    async def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict | AsyncGenerator:
-        """Chat with AI asynchronously.
-
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict|AsyncGenerator : ai content
-        ```json
-        {
-            "completion": "\nNext: domestic cat breeds with short hair >>",
-            "stop_reason": null,
-            "truncated": false,
-            "stop": null,
-            "model": "llama-2-13b-chat",
-            "log_id": "cmpl-3kYiYxSNDvgMShSzFooz6t",
-            "exception": null
-        }
-        ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-
-        payload = {
-            "max_tokens_to_sample": self.max_tokens_to_sample,
-            "model": self.model,
-            "prompt": f"<s>[INST] <<SYS>>{self.system_prompt}<</SYS>>{conversation_prompt} [/INST]",
-            "self.stop_sequence": self.stop_sequences,
-            "stream": stream,
-            "top_k": self.top_k,
-            "top_p": self.top_p,
-        }
-
-        async def for_stream():
-            async with self.session.stream(
-                "POST", self.chat_endpoint, json=payload, timeout=self.timeout
-            ) as response:
-                if (
-                    not response.is_success
-                    or not response.headers.get("Content-Type")
-                    == "text/event-stream; charset=utf-8"
-                ):
-                    raise exceptions.FailedToGenerateResponseError(
-                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
-                    )
-                async for value in response.aiter_lines():
-                    try:
-                        resp = sanitize_stream(value)
-                        self.last_response.update(resp)
-                        yield value if raw else resp
-                    except json.decoder.JSONDecodeError:
-                        pass
-
-            self.conversation.update_chat_history(
-                prompt, await self.get_message(self.last_response)
-            )
-
-        async def for_non_stream():
-            async for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else await for_non_stream()
-
-    async def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str | AsyncGenerator:
-        """Generate response `str` asynchronously.
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str|AsyncGenerator: Response generated
-        """
-
-        async def for_stream():
-            async_ask = await self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            )
-            async for response in async_ask:
-                yield await self.get_message(response)
-
-        async def for_non_stream():
-            return await self.get_message(
-                await self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else await for_non_stream()
-
-    async def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        return response.get("completion")
+import time
+import uuid
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.ui import WebDriverWait
+import click
+import requests
+from requests import get
+from uuid import uuid4
+from re import findall
+from requests.exceptions import RequestException
+from curl_cffi.requests import get, RequestsError
+import g4f
+from random import randint
+from PIL import Image
+import io
+import re
+import json
+import yaml
+from ..AIutel import Optimizers
+from ..AIutel import Conversation
+from ..AIutel import AwesomePrompts, sanitize_stream
+from ..AIbase import  Provider, AsyncProvider
+from Helpingai_T2 import Perplexity
+from webscout import exceptions
+from typing import Any, AsyncGenerator, Dict
+import logging
+import httpx
+#----------------------------------------------------------OpenAI-----------------------------------
+class OPENAI(Provider):
+    def __init__(
+        self,
+        api_key: str,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        temperature: float = 1,
+        presence_penalty: int = 0,
+        frequency_penalty: int = 0,
+        top_p: float = 1,
+        model: str = "gpt-3.5-turbo",
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiates OPENAI
+
+        Args:
+            api_key (key): OpenAI's API key.
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 1.
+            presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
+            frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
+            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
+            model (str, optional): LLM model name. Defaults to "gpt-3.5-turbo".
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.api_key = api_key
+        self.model = model
+        self.temperature = temperature
+        self.presence_penalty = presence_penalty
+        self.frequency_penalty = frequency_penalty
+        self.top_p = top_p
+        self.chat_endpoint = "https://api.openai.com/v1/chat/completions"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.headers = {
+            "Content-Type": "application/json",
+            "Authorization": f"Bearer {self.api_key}",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.session.headers.update(self.headers)
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+            "id": "chatcmpl-TaREJpBZsRVQFRFic1wIA7Q7XfnaD",
+            "object": "chat.completion",
+            "created": 1704623244,
+            "model": "gpt-3.5-turbo",
+            "usage": {
+                "prompt_tokens": 0,
+                "completion_tokens": 0,
+                "total_tokens": 0
+                },
+            "choices": [
+                {
+                    "message": {
+                        "role": "assistant",
+                        "content": "Hello! How can I assist you today?"
+                },
+                "finish_reason": "stop",
+                "index": 0
+                }
+            ]
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise exceptions.FailedToGenerateResponseError(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+        self.session.headers.update(self.headers)
+        payload = {
+            "frequency_penalty": self.frequency_penalty,
+            "messages": [{"content": conversation_prompt, "role": "user"}],
+            "model": self.model,
+            "presence_penalty": self.presence_penalty,
+            "stream": stream,
+            "temperature": self.temperature,
+            "top_p": self.top_p,
+        }
+
+        def for_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
+            )
+            if not response.ok:
+                raise exceptions.FailedToGenerateResponseError(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+
+            message_load = ""
+            for value in response.iter_lines(
+                decode_unicode=True,
+                delimiter="" if raw else "data:",
+                chunk_size=self.stream_chunk_size,
+            ):
+                try:
+                    resp = json.loads(value)
+                    incomplete_message = self.get_message(resp)
+                    if incomplete_message:
+                        message_load += incomplete_message
+                        resp["choices"][0]["delta"]["content"] = message_load
+                        self.last_response.update(resp)
+                        yield value if raw else resp
+                    elif raw:
+                        yield value
+                except json.decoder.JSONDecodeError:
+                    pass
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=False, timeout=self.timeout
+            )
+            if (
+                not response.ok
+                or not response.headers.get("Content-Type", "") == "application/json"
+            ):
+                raise exceptions.FailedToGenerateResponseError(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+            resp = response.json()
+            self.last_response.update(resp)
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+            return resp
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        try:
+            if response["choices"][0].get("delta"):
+                return response["choices"][0]["delta"]["content"]
+            return response["choices"][0]["message"]["content"]
+        except KeyError:
+            return ""
+class AsyncOPENAI(AsyncProvider):
+    def __init__(
+        self,
+        api_key: str,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        temperature: float = 1,
+        presence_penalty: int = 0,
+        frequency_penalty: int = 0,
+        top_p: float = 1,
+        model: str = "gpt-3.5-turbo",
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiates OPENAI
+
+        Args:
+            api_key (key): OpenAI's API key.
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 1.
+            presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
+            frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
+            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
+            model (str, optional): LLM model name. Defaults to "gpt-3.5-turbo".
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.api_key = api_key
+        self.model = model
+        self.temperature = temperature
+        self.presence_penalty = presence_penalty
+        self.frequency_penalty = frequency_penalty
+        self.top_p = top_p
+        self.chat_endpoint = "https://api.openai.com/v1/chat/completions"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.headers = {
+            "Content-Type": "application/json",
+            "Authorization": f"Bearer {self.api_key}",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session = httpx.AsyncClient(
+            headers=self.headers,
+            proxies=proxies,
+        )
+
+    async def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict | AsyncGenerator:
+        """Chat with AI asynchronously.
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict|AsyncGenerator : ai content.
+        ```json
+        {
+            "id": "chatcmpl-TaREJpBZsRVQFRFic1wIA7Q7XfnaD",
+            "object": "chat.completion",
+            "created": 1704623244,
+            "model": "gpt-3.5-turbo",
+            "usage": {
+                "prompt_tokens": 0,
+                "completion_tokens": 0,
+                "total_tokens": 0
+                },
+            "choices": [
+                {
+                    "message": {
+                        "role": "assistant",
+                        "content": "Hello! How can I assist you today?"
+                },
+                "finish_reason": "stop",
+                "index": 0
+                }
+            ]
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+        payload = {
+            "frequency_penalty": self.frequency_penalty,
+            "messages": [{"content": conversation_prompt, "role": "user"}],
+            "model": self.model,
+            "presence_penalty": self.presence_penalty,
+            "stream": stream,
+            "temperature": self.temperature,
+            "top_p": self.top_p,
+        }
+
+        async def for_stream():
+            async with self.session.stream(
+                "POST", self.chat_endpoint, json=payload, timeout=self.timeout
+            ) as response:
+                if not response.is_success:
+                    raise Exception(
+                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
+                    )
+
+                message_load = ""
+                async for value in response.aiter_lines():
+                    try:
+
+                        resp = sanitize_stream(value)
+                        incomplete_message = await self.get_message(resp)
+                        if incomplete_message:
+                            message_load += incomplete_message
+                            resp["choices"][0]["delta"]["content"] = message_load
+                            self.last_response.update(resp)
+                            yield value if raw else resp
+                        elif raw:
+                            yield value
+                    except json.decoder.JSONDecodeError:
+                        pass
+            self.conversation.update_chat_history(
+                prompt, await self.get_message(self.last_response)
+            )
+
+        async def for_non_stream():
+            response = httpx.post(
+                self.chat_endpoint,
+                json=payload,
+                timeout=self.timeout,
+                headers=self.headers,
+            )
+            if (
+                not response.is_success
+                or not response.headers.get("Content-Type", "") == "application/json"
+            ):
+                raise Exception(
+                    f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
+                )
+            resp = response.json()
+            self.last_response.update(resp)
+            self.conversation.update_chat_history(
+                prompt, await self.get_message(self.last_response)
+            )
+            return resp
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str | AsyncGenerator:
+        """Generate response `str` asynchronously.
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str|AsyncGenerator: Response generated
+        """
+
+        async def for_stream():
+            async_ask = await self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            )
+            async for response in async_ask:
+                yield await self.get_message(response)
+
+        async def for_non_stream():
+            return await self.get_message(
+                await self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def get_message(self, response: dict) -> str:
+        """Retrieves message only from response asynchronously.
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        try:
+            if response["choices"][0].get("delta"):
+                return response["choices"][0]["delta"]["content"]
+            return response["choices"][0]["message"]["content"]
+        except KeyError:
+            return ""
```

### Comparing `webscout-3.0/webscout/Provider/Llama2.py` & `webscout-3.0b0/webscout/Provider/OpenGPT.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,437 +1,487 @@
-import time
-import uuid
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import WebDriverWait
-import click
-import requests
-from requests import get
-from uuid import uuid4
-from re import findall
-from requests.exceptions import RequestException
-from curl_cffi.requests import get, RequestsError
-import g4f
-from random import randint
-from PIL import Image
-import io
-import re
-import json
-import yaml
-from ..AIutel import Optimizers
-from ..AIutel import Conversation
-from ..AIutel import AwesomePrompts, sanitize_stream
-from ..AIbase import  Provider, AsyncProvider
-from Helpingai_T2 import Perplexity
-from webscout import exceptions
-from typing import Any, AsyncGenerator, Dict
-import logging
-import httpx
-
-class AsyncLLAMA2(AsyncProvider):
-    def __init__(
-        self,
-        is_conversation: bool = True,
-        max_tokens: int = 800,
-        temperature: float = 0.75,
-        presence_penalty: int = 0,
-        frequency_penalty: int = 0,
-        top_p: float = 0.9,
-        model: str = "meta/meta-llama-3-70b-instruct",
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-    ):
-        """Instantiates LLAMA2
-
-        Args:
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 800.
-            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.75.
-            presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
-            frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
-            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.9.
-            model (str, optional): LLM model name. Defaults to "meta/llama-2-70b-chat".
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-        """
-        self.is_conversation = is_conversation
-        self.max_tokens_to_sample = max_tokens
-        self.model = model
-        self.temperature = temperature
-        self.presence_penalty = presence_penalty
-        self.frequency_penalty = frequency_penalty
-        self.top_p = top_p
-        self.chat_endpoint = "https://www.llama2.ai/api"
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.headers = {
-            "Content-Type": "application/json",
-            "Referer": "https://www.llama2.ai/",
-            "Content-Type": "text/plain;charset=UTF-8",
-            "Origin": "https://www.llama2.ai",
-        }
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session = httpx.AsyncClient(
-            headers=self.headers,
-            proxies=proxies,
-        )
-
-    async def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict | AsyncGenerator:
-        """Chat with AI asynchronously.
-
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict|AsyncGeneraror[dict] : ai content
-        ```json
-        {
-           "text" : "How may I help you today?"
-        }
-        ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-
-        payload = {
-            "prompt": f"{conversation_prompt}<s>[INST] {prompt} [/INST]",
-            "model": self.model,
-            "systemPrompt": "You are a helpful assistant.",
-            "temperature": self.temperature,
-            "topP": self.top_p,
-            "maxTokens": self.max_tokens_to_sample,
-            "image": None,
-            "audio": None,
-        }
-
-        async def for_stream():
-            async with self.session.stream(
-                "POST", self.chat_endpoint, json=payload, timeout=self.timeout
-            ) as response:
-                if (
-                    not response.is_success
-                    or not response.headers.get("Content-Type")
-                    == "text/plain; charset=utf-8"
-                ):
-                    raise exceptions.FailedToGenerateResponseError(
-                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
-                    )
-                message_load: str = ""
-                async for value in response.aiter_lines():
-                    try:
-                        if bool(value.strip()):
-                            message_load += value + "\n"
-                            resp: dict = dict(text=message_load)
-                            yield value if raw else resp
-                            self.last_response.update(resp)
-                    except json.decoder.JSONDecodeError:
-                        pass
-            self.conversation.update_chat_history(
-                prompt, await self.get_message(self.last_response)
-            )
-
-        async def for_non_stream():
-            async for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else await for_non_stream()
-
-    async def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str | AsyncGenerator:
-        """Generate response `str` asynchronously.
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str|AsyncGenerator: Response generated
-        """
-
-        async def for_stream():
-            async_ask = await self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            )
-            async for response in async_ask:
-                yield await self.get_message(response)
-
-        async def for_non_stream():
-            return await self.get_message(
-                await self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else await for_non_stream()
-
-    async def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (str): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        return response["text"]
-class LLAMA2(Provider):
-    def __init__(
-        self,
-        is_conversation: bool = True,
-        max_tokens: int = 800,
-        temperature: float = 0.75,
-        presence_penalty: int = 0,
-        frequency_penalty: int = 0,
-        top_p: float = 0.9,
-        model: str = "meta/meta-llama-3-70b-instruct",
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-    ):
-        """Instantiates LLAMA2
-
-        Args:
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 800.
-            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.75.
-            presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
-            frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
-            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.9.
-            model (str, optional): LLM model name. Defaults to "meta/llama-2-70b-chat".
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-        """
-        self.session = requests.Session()
-        self.is_conversation = is_conversation
-        self.max_tokens_to_sample = max_tokens
-        self.model = model
-        self.temperature = temperature
-        self.presence_penalty = presence_penalty
-        self.frequency_penalty = frequency_penalty
-        self.top_p = top_p
-        self.chat_endpoint = "https://www.llama2.ai/api"
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.headers = {
-            "Content-Type": "application/json",
-            "Referer": "https://www.llama2.ai/",
-            "Content-Type": "text/plain;charset=UTF-8",
-            "Origin": "https://www.llama2.ai",
-        }
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        self.session.headers.update(self.headers)
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session.proxies = proxies
-
-    def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict:
-        """Chat with AI
-
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict : {}
-        ```json
-        {
-           "text" : "How may I help you today?"
-        }
-        ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-        self.session.headers.update(self.headers)
-
-        payload = {
-            "prompt": f"{conversation_prompt}<s>[INST] {prompt} [/INST]",
-            "model": self.model,
-            "systemPrompt": "You are a helpful assistant.",
-            "temperature": self.temperature,
-            "topP": self.top_p,
-            "maxTokens": self.max_tokens_to_sample,
-            "image": None,
-            "audio": None,
-        }
-
-        def for_stream():
-            response = self.session.post(
-                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
-            )
-            if (
-                not response.ok
-                or not response.headers.get("Content-Type")
-                == "text/plain; charset=utf-8"
-            ):
-                raise exceptions.FailedToGenerateResponseError(
-                    f"Failed to generate response - ({response.status_code}, {response.reason})"
-                )
-
-            message_load: str = ""
-            for value in response.iter_lines(
-                decode_unicode=True,
-                delimiter="\n",
-                chunk_size=self.stream_chunk_size,
-            ):
-                try:
-                    if bool(value.strip()):
-                        message_load += value + "\n"
-                        resp: dict = dict(text=message_load)
-                        yield value if raw else resp
-                        self.last_response.update(resp)
-                except json.decoder.JSONDecodeError:
-                    pass
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
-
-        def for_non_stream():
-            for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else for_non_stream()
-
-    def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str:
-        """Generate response `str`
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str: Response generated
-        """
-
-        def for_stream():
-            for response in self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            ):
-                yield self.get_message(response)
-
-        def for_non_stream():
-            return self.get_message(
-                self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else for_non_stream()
-
-    def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (str): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        return response["text"]
+import time
+import uuid
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.ui import WebDriverWait
+import click
+import requests
+from requests import get
+from uuid import uuid4
+from re import findall
+from requests.exceptions import RequestException
+from curl_cffi.requests import get, RequestsError
+import g4f
+from random import randint
+from PIL import Image
+import io
+import re
+import json
+import yaml
+from ..AIutel import Optimizers
+from ..AIutel import Conversation
+from ..AIutel import AwesomePrompts, sanitize_stream
+from ..AIbase import  Provider, AsyncProvider
+from Helpingai_T2 import Perplexity
+from webscout import exceptions
+from typing import Any, AsyncGenerator, Dict
+import logging
+import httpx
+#------------------------------------------------------OpenGPT-----------------------------------------------------------
+class OPENGPT:
+    def __init__(
+        self,
+        assistant_id,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiates OPENGPT
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.session = requests.Session()
+        self.max_tokens_to_sample = max_tokens
+        self.is_conversation = is_conversation
+        self.chat_endpoint = (
+            "https://opengpts-example-vz4y4ooboq-uc.a.run.app/runs/stream"
+        )
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.assistant_id = assistant_id
+        self.authority = "opengpts-example-vz4y4ooboq-uc.a.run.app"
+
+        self.headers = {
+            "authority": self.authority,
+            "accept": "text/event-stream",
+            "accept-language": "en-US,en;q=0.7",
+            "cache-control": "no-cache",
+            "content-type": "application/json",
+            "origin": "https://opengpts-example-vz4y4ooboq-uc.a.run.app",
+            "pragma": "no-cache",
+            "referer": "https://opengpts-example-vz4y4ooboq-uc.a.run.app/",
+            "sec-fetch-site": "same-origin",
+            "sec-gpc": "1",
+            "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.session.headers.update(self.headers)
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+            "messages": [
+                {
+                    "content": "Hello there",
+                    "additional_kwargs": {},
+                    "type": "human",
+                    "example": false
+                },
+                {
+                    "content": "Hello! How can I assist you today?",
+                    "additional_kwargs": {
+                    "agent": {
+                        "return_values": {
+                            "output": "Hello! How can I assist you today?"
+                            },
+                        "log": "Hello! How can I assist you today?",
+                        "type": "AgentFinish"
+                    }
+                },
+                "type": "ai",
+                "example": false
+                }]
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        self.session.headers.update(self.headers)
+        self.session.headers.update(
+            dict(
+                cookie=f"opengpts_user_id={uuid4().__str__()}",
+            )
+        )
+        payload = {
+            "input": [
+                {
+                    "content": conversation_prompt,
+                    "additional_kwargs": {},
+                    "type": "human",
+                    "example": False,
+                },
+            ],
+            "assistant_id": self.assistant_id,
+            "thread_id": "",
+        }
+
+        def for_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
+            )
+            if (
+                not response.ok
+                or not response.headers.get("Content-Type")
+                == "text/event-stream; charset=utf-8"
+            ):
+                raise Exception(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+
+            for value in response.iter_lines(
+                decode_unicode=True,
+                chunk_size=self.stream_chunk_size,
+            ):
+                try:
+                    modified_value = re.sub("data:", "", value)
+                    resp = json.loads(modified_value)
+                    if len(resp) == 1:
+                        continue
+                    self.last_response.update(resp[1])
+                    yield value if raw else resp[1]
+                except json.decoder.JSONDecodeError:
+                    pass
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response["content"]
+class AsyncOPENGPT(AsyncProvider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiates OPENGPT
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.max_tokens_to_sample = max_tokens
+        self.is_conversation = is_conversation
+        self.chat_endpoint = (
+            "https://opengpts-example-vz4y4ooboq-uc.a.run.app/runs/stream"
+        )
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.assistant_id = "bca37014-6f97-4f2b-8928-81ea8d478d88"
+        self.authority = "opengpts-example-vz4y4ooboq-uc.a.run.app"
+
+        self.headers = {
+            "authority": self.authority,
+            "accept": "text/event-stream",
+            "accept-language": "en-US,en;q=0.7",
+            "cache-control": "no-cache",
+            "content-type": "application/json",
+            "origin": "https://opengpts-example-vz4y4ooboq-uc.a.run.app",
+            "pragma": "no-cache",
+            "referer": "https://opengpts-example-vz4y4ooboq-uc.a.run.app/",
+            "sec-fetch-site": "same-origin",
+            "sec-gpc": "1",
+            "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session = httpx.AsyncClient(headers=self.headers, proxies=proxies)
+
+    async def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict | AsyncGenerator:
+        """Chat with AI asynchronously
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict|AsyncGenerator : ai content.
+        ```json
+        {
+            "messages": [
+                {
+                    "content": "Hello there",
+                    "additional_kwargs": {},
+                    "type": "human",
+                    "example": false
+                },
+                {
+                    "content": "Hello! How can I assist you today?",
+                    "additional_kwargs": {
+                    "agent": {
+                        "return_values": {
+                            "output": "Hello! How can I assist you today?"
+                            },
+                        "log": "Hello! How can I assist you today?",
+                        "type": "AgentFinish"
+                    }
+                },
+                "type": "ai",
+                "example": false
+                }]
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+        self.headers.update(
+            dict(
+                cookie=f"opengpts_user_id={uuid4().__str__()}",
+            )
+        )
+        payload = {
+            "input": [
+                {
+                    "content": conversation_prompt,
+                    "additional_kwargs": {},
+                    "type": "human",
+                    "example": False,
+                },
+            ],
+            "assistant_id": self.assistant_id,
+            "thread_id": "",
+        }
+
+        async def for_stream():
+            async with self.session.stream(
+                "POST",
+                self.chat_endpoint,
+                json=payload,
+                timeout=self.timeout,
+                headers=self.headers,
+            ) as response:
+                if (
+                    not response.is_success
+                    or not response.headers.get("Content-Type")
+                    == "text/event-stream; charset=utf-8"
+                ):
+                    raise exceptions.FailedToGenerateResponseError(
+                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase}) - {response.text}"
+                    )
+
+                async for value in response.aiter_lines():
+                    try:
+                        modified_value = re.sub("data:", "", value)
+                        resp = json.loads(modified_value)
+                        if len(resp) == 1:
+                            continue
+                        self.last_response.update(resp[1])
+                        yield value if raw else resp[1]
+                    except json.decoder.JSONDecodeError:
+                        pass
+
+            self.conversation.update_chat_history(
+                prompt, await self.get_message(self.last_response)
+            )
+
+        async def for_non_stream():
+            async for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str | AsyncGenerator:
+        """Generate response `str` asynchronously.
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str|AsyncGenerator: Response generated
+        """
+
+        async def for_stream():
+            async_ask = await self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            )
+            async for response in async_ask:
+                yield await self.get_message(response)
+
+        async def for_non_stream():
+            return await self.get_message(
+                await self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response["content"]
```

### Comparing `webscout-3.0/webscout/Provider/OpenGPT.py` & `webscout-3.0b0/webscout/Provider/Phind.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,487 +1,518 @@
-import time
-import uuid
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import WebDriverWait
-import click
-import requests
-from requests import get
-from uuid import uuid4
-from re import findall
-from requests.exceptions import RequestException
-from curl_cffi.requests import get, RequestsError
-import g4f
-from random import randint
-from PIL import Image
-import io
-import re
-import json
-import yaml
-from ..AIutel import Optimizers
-from ..AIutel import Conversation
-from ..AIutel import AwesomePrompts, sanitize_stream
-from ..AIbase import  Provider, AsyncProvider
-from Helpingai_T2 import Perplexity
-from webscout import exceptions
-from typing import Any, AsyncGenerator, Dict
-import logging
-import httpx
-#------------------------------------------------------OpenGPT-----------------------------------------------------------
-class OPENGPT:
-    def __init__(
-        self,
-        assistant_id,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-    ):
-        """Instantiates OPENGPT
-
-        Args:
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-        """
-        self.session = requests.Session()
-        self.max_tokens_to_sample = max_tokens
-        self.is_conversation = is_conversation
-        self.chat_endpoint = (
-            "https://opengpts-example-vz4y4ooboq-uc.a.run.app/runs/stream"
-        )
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.assistant_id = assistant_id
-        self.authority = "opengpts-example-vz4y4ooboq-uc.a.run.app"
-
-        self.headers = {
-            "authority": self.authority,
-            "accept": "text/event-stream",
-            "accept-language": "en-US,en;q=0.7",
-            "cache-control": "no-cache",
-            "content-type": "application/json",
-            "origin": "https://opengpts-example-vz4y4ooboq-uc.a.run.app",
-            "pragma": "no-cache",
-            "referer": "https://opengpts-example-vz4y4ooboq-uc.a.run.app/",
-            "sec-fetch-site": "same-origin",
-            "sec-gpc": "1",
-            "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
-        }
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        self.session.headers.update(self.headers)
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session.proxies = proxies
-
-    def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict:
-        """Chat with AI
-
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict : {}
-        ```json
-        {
-            "messages": [
-                {
-                    "content": "Hello there",
-                    "additional_kwargs": {},
-                    "type": "human",
-                    "example": false
-                },
-                {
-                    "content": "Hello! How can I assist you today?",
-                    "additional_kwargs": {
-                    "agent": {
-                        "return_values": {
-                            "output": "Hello! How can I assist you today?"
-                            },
-                        "log": "Hello! How can I assist you today?",
-                        "type": "AgentFinish"
-                    }
-                },
-                "type": "ai",
-                "example": false
-                }]
-        }
-        ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-
-        self.session.headers.update(self.headers)
-        self.session.headers.update(
-            dict(
-                cookie=f"opengpts_user_id={uuid4().__str__()}",
-            )
-        )
-        payload = {
-            "input": [
-                {
-                    "content": conversation_prompt,
-                    "additional_kwargs": {},
-                    "type": "human",
-                    "example": False,
-                },
-            ],
-            "assistant_id": self.assistant_id,
-            "thread_id": "",
-        }
-
-        def for_stream():
-            response = self.session.post(
-                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
-            )
-            if (
-                not response.ok
-                or not response.headers.get("Content-Type")
-                == "text/event-stream; charset=utf-8"
-            ):
-                raise Exception(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
-                )
-
-            for value in response.iter_lines(
-                decode_unicode=True,
-                chunk_size=self.stream_chunk_size,
-            ):
-                try:
-                    modified_value = re.sub("data:", "", value)
-                    resp = json.loads(modified_value)
-                    if len(resp) == 1:
-                        continue
-                    self.last_response.update(resp[1])
-                    yield value if raw else resp[1]
-                except json.decoder.JSONDecodeError:
-                    pass
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
-
-        def for_non_stream():
-            for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else for_non_stream()
-
-    def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str:
-        """Generate response `str`
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str: Response generated
-        """
-
-        def for_stream():
-            for response in self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            ):
-                yield self.get_message(response)
-
-        def for_non_stream():
-            return self.get_message(
-                self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else for_non_stream()
-
-    def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        return response["content"]
-class AsyncOPENGPT(AsyncProvider):
-    def __init__(
-        self,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-    ):
-        """Instantiates OPENGPT
-
-        Args:
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-        """
-        self.max_tokens_to_sample = max_tokens
-        self.is_conversation = is_conversation
-        self.chat_endpoint = (
-            "https://opengpts-example-vz4y4ooboq-uc.a.run.app/runs/stream"
-        )
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.assistant_id = "bca37014-6f97-4f2b-8928-81ea8d478d88"
-        self.authority = "opengpts-example-vz4y4ooboq-uc.a.run.app"
-
-        self.headers = {
-            "authority": self.authority,
-            "accept": "text/event-stream",
-            "accept-language": "en-US,en;q=0.7",
-            "cache-control": "no-cache",
-            "content-type": "application/json",
-            "origin": "https://opengpts-example-vz4y4ooboq-uc.a.run.app",
-            "pragma": "no-cache",
-            "referer": "https://opengpts-example-vz4y4ooboq-uc.a.run.app/",
-            "sec-fetch-site": "same-origin",
-            "sec-gpc": "1",
-            "user-agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
-        }
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session = httpx.AsyncClient(headers=self.headers, proxies=proxies)
-
-    async def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict | AsyncGenerator:
-        """Chat with AI asynchronously
-
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict|AsyncGenerator : ai content.
-        ```json
-        {
-            "messages": [
-                {
-                    "content": "Hello there",
-                    "additional_kwargs": {},
-                    "type": "human",
-                    "example": false
-                },
-                {
-                    "content": "Hello! How can I assist you today?",
-                    "additional_kwargs": {
-                    "agent": {
-                        "return_values": {
-                            "output": "Hello! How can I assist you today?"
-                            },
-                        "log": "Hello! How can I assist you today?",
-                        "type": "AgentFinish"
-                    }
-                },
-                "type": "ai",
-                "example": false
-                }]
-        }
-        ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-        self.headers.update(
-            dict(
-                cookie=f"opengpts_user_id={uuid4().__str__()}",
-            )
-        )
-        payload = {
-            "input": [
-                {
-                    "content": conversation_prompt,
-                    "additional_kwargs": {},
-                    "type": "human",
-                    "example": False,
-                },
-            ],
-            "assistant_id": self.assistant_id,
-            "thread_id": "",
-        }
-
-        async def for_stream():
-            async with self.session.stream(
-                "POST",
-                self.chat_endpoint,
-                json=payload,
-                timeout=self.timeout,
-                headers=self.headers,
-            ) as response:
-                if (
-                    not response.is_success
-                    or not response.headers.get("Content-Type")
-                    == "text/event-stream; charset=utf-8"
-                ):
-                    raise exceptions.FailedToGenerateResponseError(
-                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase}) - {response.text}"
-                    )
-
-                async for value in response.aiter_lines():
-                    try:
-                        modified_value = re.sub("data:", "", value)
-                        resp = json.loads(modified_value)
-                        if len(resp) == 1:
-                            continue
-                        self.last_response.update(resp[1])
-                        yield value if raw else resp[1]
-                    except json.decoder.JSONDecodeError:
-                        pass
-
-            self.conversation.update_chat_history(
-                prompt, await self.get_message(self.last_response)
-            )
-
-        async def for_non_stream():
-            async for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else await for_non_stream()
-
-    async def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str | AsyncGenerator:
-        """Generate response `str` asynchronously.
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str|AsyncGenerator: Response generated
-        """
-
-        async def for_stream():
-            async_ask = await self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            )
-            async for response in async_ask:
-                yield await self.get_message(response)
-
-        async def for_non_stream():
-            return await self.get_message(
-                await self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else await for_non_stream()
-
-    async def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        return response["content"]
+import time
+import uuid
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.ui import WebDriverWait
+import click
+import requests
+from requests import get
+from uuid import uuid4
+from re import findall
+from requests.exceptions import RequestException
+from curl_cffi.requests import get, RequestsError
+import g4f
+from random import randint
+from PIL import Image
+import io
+import re
+import json
+import yaml
+from ..AIutel import Optimizers
+from ..AIutel import Conversation
+from ..AIutel import AwesomePrompts, sanitize_stream
+from ..AIbase import  Provider, AsyncProvider
+from Helpingai_T2 import Perplexity
+from webscout import exceptions
+from typing import Any, AsyncGenerator, Dict
+import logging
+import httpx
+
+#------------------------------------------------------phind-------------------------------------------------------------
+class PhindSearch:
+    # default_model = "Phind Model"
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 8000,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+        model: str = "Phind Model",
+        quiet: bool = False,
+    ):
+        """Instantiates PHIND
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+            model (str, optional): Model name. Defaults to "Phind Model".
+            quiet (bool, optional): Ignore web search-results and yield final response only. Defaults to False.
+        """
+        self.session = requests.Session()
+        self.max_tokens_to_sample = max_tokens
+        self.is_conversation = is_conversation
+        self.chat_endpoint = "https://https.extension.phind.com/agent/"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.model = model
+        self.quiet = quiet
+
+        self.headers = {
+            "Content-Type": "application/json",
+            "User-Agent": "",
+            "Accept": "*/*",
+            "Accept-Encoding": "Identity",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.session.headers.update(self.headers)
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+            "id": "chatcmpl-r0wujizf2i2xb60mjiwt",
+            "object": "chat.completion.chunk",
+            "created": 1706775384,
+            "model": "trt-llm-phind-model-serving",
+            "choices": [
+                {
+                    "index": 0,
+                    "delta": {
+                        "content": "Hello! How can I assist you with your programming today?"
+                        },
+                    "finish_reason": null
+                }
+            ]
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        self.session.headers.update(self.headers)
+        payload = {
+            "additional_extension_context": "",
+            "allow_magic_buttons": True,
+            "is_vscode_extension": True,
+            "message_history": [
+                {"content": conversation_prompt, "metadata": {}, "role": "user"}
+            ],
+            "requested_model": self.model,
+            "user_input": prompt,
+        }
+
+        def for_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
+            )
+            if (
+                not response.ok
+                or not response.headers.get("Content-Type")
+                == "text/event-stream; charset=utf-8"
+            ):
+                raise exceptions.FailedToGenerateResponseError(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+            streaming_text = ""
+            for value in response.iter_lines(
+                decode_unicode=True,
+                chunk_size=self.stream_chunk_size,
+            ):
+                try:
+                    modified_value = re.sub("data:", "", value)
+                    json_modified_value = json.loads(modified_value)
+                    retrieved_text = self.get_message(json_modified_value)
+                    if not retrieved_text:
+                        continue
+                    streaming_text += retrieved_text
+                    json_modified_value["choices"][0]["delta"][
+                        "content"
+                    ] = streaming_text
+                    self.last_response.update(json_modified_value)
+                    yield value if raw else json_modified_value
+                except json.decoder.JSONDecodeError:
+                    pass
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        if response.get("type", "") == "metadata":
+            return
+
+        delta: dict = response["choices"][0]["delta"]
+
+        if not delta:
+            return ""
+
+        elif delta.get("function_call"):
+            if self.quiet:
+                return ""
+
+            function_call: dict = delta["function_call"]
+            if function_call.get("name"):
+                return function_call["name"]
+            elif function_call.get("arguments"):
+                return function_call.get("arguments")
+
+        elif delta.get("metadata"):
+            if self.quiet:
+                return ""
+            return yaml.dump(delta["metadata"])
+
+        else:
+            return (
+                response["choices"][0]["delta"].get("content")
+                if response["choices"][0].get("finish_reason") is None
+                else ""
+            )
+class AsyncPhindSearch(AsyncProvider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+        model: str = "Phind Model",
+        quiet: bool = False,
+    ):
+        """Instantiates PHIND
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+            model (str, optional): Model name. Defaults to "Phind Model".
+            quiet (bool, optional): Ignore web search-results and yield final response only. Defaults to False.
+        """
+        self.max_tokens_to_sample = max_tokens
+        self.is_conversation = is_conversation
+        self.chat_endpoint = "https://https.extension.phind.com/agent/"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.model = model
+        self.quiet = quiet
+
+        self.headers = {
+            "Content-Type": "application/json",
+            "User-Agent": "",
+            "Accept": "*/*",
+            "Accept-Encoding": "Identity",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session = httpx.AsyncClient(headers=self.headers, proxies=proxies)
+
+    async def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+        synchronous_generator=False,
+    ) -> dict | AsyncGenerator:
+        """Asynchronously Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict|AsyncGenerator : ai content.
+        ```json
+        {
+            "id": "chatcmpl-r0wujizf2i2xb60mjiwt",
+            "object": "chat.completion.chunk",
+            "created": 1706775384,
+            "model": "trt-llm-phind-model-serving",
+            "choices": [
+                {
+                    "index": 0,
+                    "delta": {
+                        "content": "Hello! How can I assist you with your programming today?"
+                        },
+                    "finish_reason": null
+                }
+            ]
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        payload = {
+            "additional_extension_context": "",
+            "allow_magic_buttons": True,
+            "is_vscode_extension": True,
+            "message_history": [
+                {"content": conversation_prompt, "metadata": {}, "role": "user"}
+            ],
+            "requested_model": self.model,
+            "user_input": prompt,
+        }
+
+        async def for_stream():
+            async with self.session.stream(
+                "POST",
+                self.chat_endpoint,
+                json=payload,
+                timeout=self.timeout,
+            ) as response:
+                if (
+                    not response.is_success
+                    or not response.headers.get("Content-Type")
+                    == "text/event-stream; charset=utf-8"
+                ):
+                    raise exceptions.FailedToGenerateResponseError(
+                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
+                    )
+                streaming_text = ""
+                async for value in response.aiter_lines():
+                    try:
+                        modified_value = re.sub("data:", "", value)
+                        json_modified_value = json.loads(modified_value)
+                        retrieved_text = await self.get_message(json_modified_value)
+                        if not retrieved_text:
+                            continue
+                        streaming_text += retrieved_text
+                        json_modified_value["choices"][0]["delta"][
+                            "content"
+                        ] = streaming_text
+                        self.last_response.update(json_modified_value)
+                        yield value if raw else json_modified_value
+                    except json.decoder.JSONDecodeError:
+                        pass
+                self.conversation.update_chat_history(
+                    prompt, await self.get_message(self.last_response)
+                )
+
+        async def for_non_stream():
+            async for _ in for_stream():
+                pass
+            return self.last_response
+
+        return (
+            for_stream()
+            if stream and not synchronous_generator
+            else await for_non_stream()
+        )
+
+    async def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str | AsyncGenerator:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str|AsyncGenerator: Response generated
+        """
+
+        async def for_stream():
+            ask_resp = await self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            )
+            async for response in ask_resp:
+                yield await self.get_message(response)
+
+        async def for_non_stream():
+            return await self.get_message(
+                await self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        if response.get("type", "") == "metadata":
+            return
+
+        delta: dict = response["choices"][0]["delta"]
+
+        if not delta:
+            return ""
+
+        elif delta.get("function_call"):
+            if self.quiet:
+                return ""
+
+            function_call: dict = delta["function_call"]
+            if function_call.get("name"):
+                return function_call["name"]
+            elif function_call.get("arguments"):
+                return function_call.get("arguments")
+
+        elif delta.get("metadata"):
+            if self.quiet:
+                return ""
+            return yaml.dump(delta["metadata"])
+
+        else:
+            return (
+                response["choices"][0]["delta"].get("content")
+                if response["choices"][0].get("finish_reason") is None
+                else ""
+            )
```

### Comparing `webscout-3.0/webscout/Provider/Openai.py` & `webscout-3.0b0/webscout/g4f.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,511 +1,666 @@
-import time
-import uuid
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import WebDriverWait
-import click
-import requests
-from requests import get
-from uuid import uuid4
-from re import findall
-from requests.exceptions import RequestException
-from curl_cffi.requests import get, RequestsError
 import g4f
-from random import randint
-from PIL import Image
-import io
-import re
-import json
-import yaml
-from ..AIutel import Optimizers
-from ..AIutel import Conversation
-from ..AIutel import AwesomePrompts, sanitize_stream
-from ..AIbase import  Provider, AsyncProvider
-from Helpingai_T2 import Perplexity
-from webscout import exceptions
-from typing import Any, AsyncGenerator, Dict
-import logging
-import httpx
-#----------------------------------------------------------OpenAI-----------------------------------
-class OPENAI(Provider):
+from webscout.AIutel import Optimizers
+from webscout.AIutel import Conversation
+from webscout.AIutel import AwesomePrompts
+from webscout.AIbase import Provider, AsyncProvider
+from webscout.AIutel import available_providers
+from typing import Any, AsyncGenerator
+
+g4f.debug.version_check = False
+
+working_providers = available_providers
+
+completion_allowed_models = [
+    "code-davinci-002",
+    "text-ada-001",
+    "text-babbage-001",
+    "text-curie-001",
+    "text-davinci-002",
+    "text-davinci-003",
+]
+
+default_models = {
+    "completion": "text-davinci-003",
+    "chat_completion": "gpt-3.5-turbo",
+}
+
+default_provider = "Koala"
+
+class AsyncGPT4FREE(AsyncProvider):
     def __init__(
         self,
-        api_key: str,
+        provider: str = default_provider,
         is_conversation: bool = True,
+        auth: str = None,
         max_tokens: int = 600,
-        temperature: float = 1,
-        presence_penalty: int = 0,
-        frequency_penalty: int = 0,
-        top_p: float = 1,
-        model: str = "gpt-3.5-turbo",
+        model: str = None,
+        ignore_working: bool = False,
         timeout: int = 30,
         intro: str = None,
         filepath: str = None,
         update_file: bool = True,
         proxies: dict = {},
         history_offset: int = 10250,
         act: str = None,
     ):
-        """Instantiates OPENAI
+        """Initialies GPT4FREE
 
         Args:
-            api_key (key): OpenAI's API key.
+            provider (str, optional): gpt4free based provider name. Defaults to Koala.
             is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            auth (str, optional): Authentication value for the provider incase it needs. Defaults to None.
             max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            temperature (float, optional): Charge of the generated text's randomness. Defaults to 1.
-            presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
-            frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
-            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
-            model (str, optional): LLM model name. Defaults to "gpt-3.5-turbo".
+            model (str, optional): LLM model name. Defaults to text-davinci-003|gpt-3.5-turbo.
+            ignore_working (bool, optional): Ignore working status of the provider. Defaults to False.
             timeout (int, optional): Http request timeout. Defaults to 30.
             intro (str, optional): Conversation introductory prompt. Defaults to None.
             filepath (str, optional): Path to file containing conversation history. Defaults to None.
             update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
             proxies (dict, optional): Http request proxies. Defaults to {}.
             history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
             act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
         """
+        assert provider in available_providers, (
+            f"Provider '{provider}' is not yet supported. "
+            f"Try others like {', '.join(available_providers)}"
+        )
+        if model is None:
+            model = default_models["chat_completion"]
+
         self.is_conversation = is_conversation
         self.max_tokens_to_sample = max_tokens
-        self.api_key = api_key
-        self.model = model
-        self.temperature = temperature
-        self.presence_penalty = presence_penalty
-        self.frequency_penalty = frequency_penalty
-        self.top_p = top_p
-        self.chat_endpoint = "https://api.openai.com/v1/chat/completions"
         self.stream_chunk_size = 64
         self.timeout = timeout
         self.last_response = {}
-        self.headers = {
-            "Content-Type": "application/json",
-            "Authorization": f"Bearer {self.api_key}",
-        }
 
         self.__available_optimizers = (
             method
             for method in dir(Optimizers)
             if callable(getattr(Optimizers, method)) and not method.startswith("__")
         )
-        self.session.headers.update(self.headers)
         Conversation.intro = (
             AwesomePrompts().get_act(
                 act, raise_not_found=True, default=None, case_insensitive=True
             )
             if act
             else intro or Conversation.intro
         )
         self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
+            is_conversation,
+            self.max_tokens_to_sample,
+            filepath,
+            update_file,
         )
         self.conversation.history_offset = history_offset
-        self.session.proxies = proxies
+        self.model = model
+        self.provider = provider
+        self.ignore_working = ignore_working
+        self.auth = auth
+        self.proxy = None if not proxies else list(proxies.values())[0]
 
-    def ask(
+    def __str__(self):
+        return f"AsyncGPTFREE(provider={self.provider})"
+
+    async def ask(
         self,
         prompt: str,
         stream: bool = False,
         raw: bool = False,
         optimizer: str = None,
         conversationally: bool = False,
-    ) -> dict:
-        """Chat with AI
+    ) -> dict | AsyncGenerator:
+        """Chat with AI asynchronously.
 
         Args:
             prompt (str): Prompt to be send.
             stream (bool, optional): Flag for streaming response. Defaults to False.
             raw (bool, optional): Stream back raw response as received. Defaults to False.
             optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
             conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
         Returns:
-           dict : {}
+           dict|AsyncGenerator : ai content
         ```json
         {
-            "id": "chatcmpl-TaREJpBZsRVQFRFic1wIA7Q7XfnaD",
-            "object": "chat.completion",
-            "created": 1704623244,
-            "model": "gpt-3.5-turbo",
-            "usage": {
-                "prompt_tokens": 0,
-                "completion_tokens": 0,
-                "total_tokens": 0
-                },
-            "choices": [
-                {
-                    "message": {
-                        "role": "assistant",
-                        "content": "Hello! How can I assist you today?"
-                },
-                "finish_reason": "stop",
-                "index": 0
-                }
-            ]
+          "text" : "How may I help you today?"
         }
         ```
         """
         conversation_prompt = self.conversation.gen_complete_prompt(prompt)
         if optimizer:
             if optimizer in self.__available_optimizers:
                 conversation_prompt = getattr(Optimizers, optimizer)(
                     conversation_prompt if conversationally else prompt
                 )
             else:
-                raise exceptions.FailedToGenerateResponseError(
+                raise Exception(
                     f"Optimizer is not one of {self.__available_optimizers}"
                 )
-        self.session.headers.update(self.headers)
-        payload = {
-            "frequency_penalty": self.frequency_penalty,
-            "messages": [{"content": conversation_prompt, "role": "user"}],
-            "model": self.model,
-            "presence_penalty": self.presence_penalty,
-            "stream": stream,
-            "temperature": self.temperature,
-            "top_p": self.top_p,
-        }
 
-        def for_stream():
-            response = self.session.post(
-                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
-            )
-            if not response.ok:
-                raise exceptions.FailedToGenerateResponseError(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
-                )
+        payload = dict(
+            model=self.model,
+            provider=self.provider,  # g4f.Provider.Aichat,
+            messages=[{"role": "user", "content": conversation_prompt}],
+            stream=True,
+            ignore_working=self.ignore_working,
+            auth=self.auth,
+            proxy=self.proxy,
+            timeout=self.timeout,
+        )
 
-            message_load = ""
-            for value in response.iter_lines(
-                decode_unicode=True,
-                delimiter="" if raw else "data:",
-                chunk_size=self.stream_chunk_size,
-            ):
-                try:
-                    resp = json.loads(value)
-                    incomplete_message = self.get_message(resp)
-                    if incomplete_message:
-                        message_load += incomplete_message
-                        resp["choices"][0]["delta"]["content"] = message_load
-                        self.last_response.update(resp)
-                        yield value if raw else resp
-                    elif raw:
-                        yield value
-                except json.decoder.JSONDecodeError:
-                    pass
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
+        async def format_response(response):
+            return dict(text=response)
+
+        async def for_stream():
+            previous_chunks = ""
+            response = g4f.ChatCompletion.create_async(**payload)
+
+            async for chunk in response:
+                previous_chunks += chunk
+                formatted_resp = await format_response(previous_chunks)
+                self.last_response.update(formatted_resp)
+                yield previous_chunks if raw else formatted_resp
 
-        def for_non_stream():
-            response = self.session.post(
-                self.chat_endpoint, json=payload, stream=False, timeout=self.timeout
-            )
-            if (
-                not response.ok
-                or not response.headers.get("Content-Type", "") == "application/json"
-            ):
-                raise exceptions.FailedToGenerateResponseError(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
-                )
-            resp = response.json()
-            self.last_response.update(resp)
             self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
+                prompt,
+                previous_chunks,
             )
-            return resp
 
-        return for_stream() if stream else for_non_stream()
+        async def for_non_stream():
+            async for _ in for_stream():
+                pass
+            return self.last_response
 
-    def chat(
+        return for_stream() if stream else await for_non_stream()
+
+    async def chat(
         self,
         prompt: str,
         stream: bool = False,
         optimizer: str = None,
         conversationally: bool = False,
-    ) -> str:
-        """Generate response `str`
+    ) -> dict | AsyncGenerator:
+        """Generate response `str` asynchronously.
         Args:
             prompt (str): Prompt to be send.
             stream (bool, optional): Flag for streaming response. Defaults to False.
             optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
             conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
         Returns:
-            str: Response generated
+            str|AsyncGenerator: Response generated
         """
 
-        def for_stream():
-            for response in self.ask(
+        async def for_stream():
+            async_ask = await self.ask(
                 prompt, True, optimizer=optimizer, conversationally=conversationally
-            ):
-                yield self.get_message(response)
+            )
+            async for response in async_ask:
+                yield await self.get_message(response)
 
-        def for_non_stream():
-            return self.get_message(
-                self.ask(
+        async def for_non_stream():
+            return await self.get_message(
+                await self.ask(
                     prompt,
                     False,
                     optimizer=optimizer,
                     conversationally=conversationally,
                 )
             )
 
-        return for_stream() if stream else for_non_stream()
+        return for_stream() if stream else await for_non_stream()
 
-    def get_message(self, response: dict) -> str:
+    async def get_message(self, response: dict) -> str:
         """Retrieves message only from response
 
         Args:
             response (dict): Response generated by `self.ask`
 
         Returns:
             str: Message extracted
         """
         assert isinstance(response, dict), "Response should be of dict data-type only"
-        try:
-            if response["choices"][0].get("delta"):
-                return response["choices"][0]["delta"]["content"]
-            return response["choices"][0]["message"]["content"]
-        except KeyError:
-            return ""
-class AsyncOPENAI(AsyncProvider):
+        return response["text"]
+class GPT4FREE(Provider):
     def __init__(
         self,
-        api_key: str,
+        provider: str = default_provider,
         is_conversation: bool = True,
+        auth: str = None,
         max_tokens: int = 600,
-        temperature: float = 1,
-        presence_penalty: int = 0,
-        frequency_penalty: int = 0,
-        top_p: float = 1,
-        model: str = "gpt-3.5-turbo",
+        model: str = None,
+        chat_completion: bool = True,
+        ignore_working: bool = True,
         timeout: int = 30,
         intro: str = None,
         filepath: str = None,
         update_file: bool = True,
         proxies: dict = {},
         history_offset: int = 10250,
         act: str = None,
     ):
-        """Instantiates OPENAI
+        """Initialies GPT4FREE
 
         Args:
-            api_key (key): OpenAI's API key.
+            provider (str, optional): gpt4free based provider name. Defaults to Koala.
             is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            auth (str, optional): Authentication value for the provider incase it needs. Defaults to None.
             max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            temperature (float, optional): Charge of the generated text's randomness. Defaults to 1.
-            presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
-            frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
-            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.999.
-            model (str, optional): LLM model name. Defaults to "gpt-3.5-turbo".
+            model (str, optional): LLM model name. Defaults to text-davinci-003|gpt-3.5-turbo.
+            chat_completion(bool, optional): Provide native auto-contexting (conversationally). Defaults to False.
+            ignore_working (bool, optional): Ignore working status of the provider. Defaults to False.
             timeout (int, optional): Http request timeout. Defaults to 30.
             intro (str, optional): Conversation introductory prompt. Defaults to None.
             filepath (str, optional): Path to file containing conversation history. Defaults to None.
             update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
             proxies (dict, optional): Http request proxies. Defaults to {}.
             history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
             act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
         """
+        assert provider in available_providers, (
+            f"Provider '{provider}' is not yet supported. "
+            f"Try others like {', '.join(available_providers)}"
+        )
+        if model is None:
+            model = (
+                default_models["chat_completion"]
+                if chat_completion
+                else default_models["completion"]
+            )
+
+        elif not chat_completion:
+            assert model in completion_allowed_models, (
+                f"Model '{model}' is not yet supported for completion. "
+                f"Try other models like {', '.join(completion_allowed_models)}"
+            )
         self.is_conversation = is_conversation
         self.max_tokens_to_sample = max_tokens
-        self.api_key = api_key
-        self.model = model
-        self.temperature = temperature
-        self.presence_penalty = presence_penalty
-        self.frequency_penalty = frequency_penalty
-        self.top_p = top_p
-        self.chat_endpoint = "https://api.openai.com/v1/chat/completions"
         self.stream_chunk_size = 64
         self.timeout = timeout
         self.last_response = {}
-        self.headers = {
-            "Content-Type": "application/json",
-            "Authorization": f"Bearer {self.api_key}",
-        }
 
         self.__available_optimizers = (
             method
             for method in dir(Optimizers)
             if callable(getattr(Optimizers, method)) and not method.startswith("__")
         )
         Conversation.intro = (
             AwesomePrompts().get_act(
                 act, raise_not_found=True, default=None, case_insensitive=True
             )
             if act
             else intro or Conversation.intro
         )
         self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
+            False if chat_completion else is_conversation,
+            self.max_tokens_to_sample,
+            filepath,
+            update_file,
         )
         self.conversation.history_offset = history_offset
-        self.session = httpx.AsyncClient(
-            headers=self.headers,
-            proxies=proxies,
-        )
+        self.model = model
+        self.provider = provider
+        self.chat_completion = chat_completion
+        self.ignore_working = ignore_working
+        self.auth = auth
+        self.proxy = None if not proxies else list(proxies.values())[0]
+        self.__chat_class = g4f.ChatCompletion if chat_completion else g4f.Completion
 
-    async def ask(
+    def ask(
         self,
         prompt: str,
         stream: bool = False,
         raw: bool = False,
         optimizer: str = None,
         conversationally: bool = False,
-    ) -> dict | AsyncGenerator:
-        """Chat with AI asynchronously.
+    ) -> dict:
+        """Chat with AI
 
         Args:
             prompt (str): Prompt to be send.
             stream (bool, optional): Flag for streaming response. Defaults to False.
             raw (bool, optional): Stream back raw response as received. Defaults to False.
             optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
             conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
         Returns:
-           dict|AsyncGenerator : ai content.
+           dict : {}
         ```json
         {
-            "id": "chatcmpl-TaREJpBZsRVQFRFic1wIA7Q7XfnaD",
-            "object": "chat.completion",
-            "created": 1704623244,
-            "model": "gpt-3.5-turbo",
-            "usage": {
-                "prompt_tokens": 0,
-                "completion_tokens": 0,
-                "total_tokens": 0
-                },
-            "choices": [
-                {
-                    "message": {
-                        "role": "assistant",
-                        "content": "Hello! How can I assist you today?"
-                },
-                "finish_reason": "stop",
-                "index": 0
-                }
-            ]
+          "text" : "How may I help you today?"
         }
         ```
         """
         conversation_prompt = self.conversation.gen_complete_prompt(prompt)
         if optimizer:
             if optimizer in self.__available_optimizers:
                 conversation_prompt = getattr(Optimizers, optimizer)(
                     conversation_prompt if conversationally else prompt
                 )
             else:
                 raise Exception(
                     f"Optimizer is not one of {self.__available_optimizers}"
                 )
-        payload = {
-            "frequency_penalty": self.frequency_penalty,
-            "messages": [{"content": conversation_prompt, "role": "user"}],
-            "model": self.model,
-            "presence_penalty": self.presence_penalty,
-            "stream": stream,
-            "temperature": self.temperature,
-            "top_p": self.top_p,
-        }
 
-        async def for_stream():
-            async with self.session.stream(
-                "POST", self.chat_endpoint, json=payload, timeout=self.timeout
-            ) as response:
-                if not response.is_success:
-                    raise Exception(
-                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
-                    )
-
-                message_load = ""
-                async for value in response.aiter_lines():
-                    try:
-
-                        resp = sanitize_stream(value)
-                        incomplete_message = await self.get_message(resp)
-                        if incomplete_message:
-                            message_load += incomplete_message
-                            resp["choices"][0]["delta"]["content"] = message_load
-                            self.last_response.update(resp)
-                            yield value if raw else resp
-                        elif raw:
-                            yield value
-                    except json.decoder.JSONDecodeError:
-                        pass
-            self.conversation.update_chat_history(
-                prompt, await self.get_message(self.last_response)
-            )
+        def payload():
+            if self.chat_completion:
+                return dict(
+                    model=self.model,
+                    provider=self.provider,  # g4f.Provider.Aichat,
+                    messages=[{"role": "user", "content": conversation_prompt}],
+                    stream=stream,
+                    ignore_working=self.ignore_working,
+                    auth=self.auth,
+                    proxy=self.proxy,
+                    timeout=self.timeout,
+                )
 
-        async def for_non_stream():
-            response = httpx.post(
-                self.chat_endpoint,
-                json=payload,
-                timeout=self.timeout,
-                headers=self.headers,
-            )
-            if (
-                not response.is_success
-                or not response.headers.get("Content-Type", "") == "application/json"
-            ):
-                raise Exception(
-                    f"Failed to generate response - ({response.status_code}, {response.reason_phrase})"
+            else:
+                return dict(
+                    model=self.model,
+                    prompt=conversation_prompt,
+                    provider=self.provider,
+                    stream=stream,
+                    ignore_working=self.ignore_working,
+                    auth=self.auth,
+                    proxy=self.proxy,
+                    timeout=self.timeout,
                 )
-            resp = response.json()
-            self.last_response.update(resp)
+
+        def format_response(response):
+            return dict(text=response)
+
+        def for_stream():
+            previous_chunks = ""
+            response = self.__chat_class.create(**payload())
+
+            for chunk in response:
+                previous_chunks += chunk
+                formatted_resp = format_response(previous_chunks)
+                self.last_response.update(formatted_resp)
+                yield previous_chunks if raw else formatted_resp
+
             self.conversation.update_chat_history(
-                prompt, await self.get_message(self.last_response)
+                prompt,
+                previous_chunks,
             )
-            return resp
 
-        return for_stream() if stream else await for_non_stream()
+        def for_non_stream():
+            response = self.__chat_class.create(**payload())
+            formatted_resp = format_response(response)
 
-    async def chat(
+            self.last_response.update(formatted_resp)
+            self.conversation.update_chat_history(prompt, response)
+
+            return response if raw else formatted_resp
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
         self,
         prompt: str,
         stream: bool = False,
         optimizer: str = None,
         conversationally: bool = False,
-    ) -> str | AsyncGenerator:
-        """Generate response `str` asynchronously.
+    ) -> str:
+        """Generate response `str`
         Args:
             prompt (str): Prompt to be send.
             stream (bool, optional): Flag for streaming response. Defaults to False.
             optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
             conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
         Returns:
-            str|AsyncGenerator: Response generated
+            str: Response generated
         """
 
-        async def for_stream():
-            async_ask = await self.ask(
+        def for_stream():
+            for response in self.ask(
                 prompt, True, optimizer=optimizer, conversationally=conversationally
-            )
-            async for response in async_ask:
-                yield await self.get_message(response)
+            ):
+                yield self.get_message(response)
 
-        async def for_non_stream():
-            return await self.get_message(
-                await self.ask(
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
                     prompt,
                     False,
                     optimizer=optimizer,
                     conversationally=conversationally,
                 )
             )
 
-        return for_stream() if stream else await for_non_stream()
+        return for_stream() if stream else for_non_stream()
 
-    async def get_message(self, response: dict) -> str:
-        """Retrieves message only from response asynchronously.
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
 
         Args:
             response (dict): Response generated by `self.ask`
 
         Returns:
             str: Message extracted
         """
         assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response["text"]
+from pathlib import Path
+from webscout.AIutel import default_path
+from json import dump, load
+from time import time
+from threading import Thread as thr
+from functools import wraps
+from rich.progress import Progress
+import logging
+
+results_path = Path(default_path) / "provider_test.json"
+
+
+def exception_handler(func):
+
+    @wraps(func)
+    def decorator(*args, **kwargs):
         try:
-            if response["choices"][0].get("delta"):
-                return response["choices"][0]["delta"]["content"]
-            return response["choices"][0]["message"]["content"]
-        except KeyError:
-            return ""
+            return func(*args, **kwargs)
+        except Exception as e:
+            pass
+
+    return decorator
+
+
+@exception_handler
+def is_working(provider: str) -> bool:
+    """Test working status of a provider
+
+    Args:
+        provider (str): Provider name
+
+    Returns:
+        bool: is_working status
+    """
+    bot = GPT4FREE(provider=provider, is_conversation=False)
+    text = bot.chat("hello")
+    assert isinstance(text, str)
+    assert bool(text.strip())
+    assert "</" not in text
+    assert ":" not in text
+    assert len(text) > 2
+    return True
+
+
+class TestProviders:
+
+    def __init__(
+        self,
+        test_at_once: int = 5,
+        quiet: bool = False,
+        timeout: int = 20,
+        selenium: bool = False,
+        do_log: bool = True,
+    ):
+        """Constructor
+
+        Args:
+            test_at_once (int, optional): Test n providers at once. Defaults to 5.
+            quiet (bool, optinal): Disable stdout. Defaults to False.
+            timout (int, optional): Thread timeout for each provider. Defaults to 20.
+            selenium (bool, optional): Test even selenium dependent providers. Defaults to False.
+            do_log (bool, optional): Flag to control logging. Defaults to True.
+        """
+        self.test_at_once: int = test_at_once
+        self.quiet = quiet
+        self.timeout = timeout
+        self.do_log = do_log
+        self.__logger = logging.getLogger(__name__)
+        self.working_providers: list = [
+            provider.__name__
+            for provider in g4f.Provider.__providers__
+            if provider.working
+        ]
+
+        if not selenium:
+            import g4f.Provider.selenium as selenium_based
+            from g4f import webdriver
+
+            webdriver.has_requirements = False
+            selenium_based_providers: list = dir(selenium_based)
+            for provider in self.working_providers:
+                try:
+                    selenium_based_providers.index(provider)
+                except ValueError:
+                    pass
+                else:
+                    self.__log(
+                        10, f"Dropping provider - {provider} - [Selenium dependent]"
+                    )
+                    self.working_providers.remove(provider)
+
+        self.results_path: Path = results_path
+        self.__create_empty_file(ignore_if_found=True)
+        self.results_file_is_empty: bool = False
+
+    def __log(
+        self,
+        level: int,
+        message: str,
+    ):
+        """class logger"""
+        if self.do_log:
+            self.__logger.log(level, message)
+        else:
+            pass
+
+    def __create_empty_file(self, ignore_if_found: bool = False):
+        if ignore_if_found and self.results_path.is_file():
+            return
+        with self.results_path.open("w") as fh:
+            dump({"results": []}, fh)
+        self.results_file_is_empty = True
+
+    def test_provider(self, name: str):
+        """Test each provider and save successful ones
+
+        Args:
+            name (str): Provider name
+        """
+
+        try:
+            bot = GPT4FREE(provider=name, is_conversation=False)
+            start_time = time()
+            text = bot.chat("hello there")
+            assert isinstance(text, str), "Non-string response returned"
+            assert bool(text.strip()), "Empty string"
+            assert "</" not in text, "Html code returned."
+            assert ":" not in text, "Json formatted response returned"
+            assert len(text) > 2
+        except Exception as e:
+            pass
+        else:
+            self.results_file_is_empty = False
+            with self.results_path.open() as fh:
+                current_results = load(fh)
+            new_result = dict(time=time() - start_time, name=name)
+            current_results["results"].append(new_result)
+            self.__log(20, f"Test result - {new_result['name']} - {new_result['time']}")
+
+            with self.results_path.open("w") as fh:
+                dump(current_results, fh)
+
+    @exception_handler
+    def main(
+        self,
+    ):
+        self.__create_empty_file()
+        threads = []
+        # Create a progress bar
+        total = len(self.working_providers)
+        with Progress() as progress:
+            self.__log(20, f"Testing {total} providers : {self.working_providers}")
+            task = progress.add_task(
+                f"[cyan]Testing...[{self.test_at_once}]",
+                total=total,
+                visible=self.quiet == False,
+            )
+            while not progress.finished:
+                for count, provider in enumerate(self.working_providers, start=1):
+                    t1 = thr(
+                        target=self.test_provider,
+                        args=(provider,),
+                    )
+                    t1.start()
+                    if count % self.test_at_once == 0 or count == len(provider):
+                        for t in threads:
+                            try:
+                                t.join(self.timeout)
+                            except Exception as e:
+                                pass
+                        threads.clear()
+                    else:
+                        threads.append(t1)
+                    progress.update(task, advance=1)
+
+    def get_results(self, run: bool = False, best: bool = False) -> list[dict]:
+        """Get test results
+
+        Args:
+            run (bool, optional): Run the test first. Defaults to False.
+            best (bool, optional): Return name of the best provider. Defaults to False.
+
+        Returns:
+            list[dict]|str: Test results.
+        """
+        if run or self.results_file_is_empty:
+            self.main()
+
+        with self.results_path.open() as fh:
+            results: dict = load(fh)
+
+        results = results["results"]
+        if not results:
+            if run:
+                raise Exception("Unable to find working g4f provider")
+            else:
+                self.__log(30, "Hunting down working g4f providers.")
+                return self.get_results(run=True, best=best)
+
+        time_list = []
+
+        sorted_list = []
+        for entry in results:
+            time_list.append(entry["time"])
+
+        time_list.sort()
+
+        for time_value in time_list:
+            for entry in results:
+                if entry["time"] == time_value:
+                    sorted_list.append(entry)
+        return sorted_list[0]["name"] if best else sorted_list
+
+    @property
+    def best(self):
+        """Fastest provider overally"""
+        return self.get_results(run=False, best=True)
+
+    @property
+    def auto(self):
+        """Best working provider"""
+        for result in self.get_results(run=False, best=False):
+            self.__log(20, "Confirming working status of provider : " + result["name"])
+            if is_working(result["name"]):
+                return result["name"]
```

### Comparing `webscout-3.0/webscout/Provider/Perplexity.py` & `webscout-3.0b0/webscout/Provider/Reka.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,230 +1,226 @@
-import time
-import uuid
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import WebDriverWait
-import click
-import requests
-from requests import get
-from uuid import uuid4
-from re import findall
-from requests.exceptions import RequestException
-from curl_cffi.requests import get, RequestsError
-import g4f
-from random import randint
-from PIL import Image
-import io
-import re
-import json
-import yaml
-from ..AIutel import Optimizers
-from ..AIutel import Conversation
-from ..AIutel import AwesomePrompts, sanitize_stream
-from ..AIbase import  Provider, AsyncProvider
-from Helpingai_T2 import Perplexity
-from webscout import exceptions
-from typing import Any, AsyncGenerator, Dict
-import logging
-import httpx
-#------------------------------------------------------PERPLEXITY--------------------------------------------------------  
-class PERPLEXITY(Provider):
-    def __init__(
-        self,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-        quiet: bool = False,
-    ):
-        """Instantiates PERPLEXITY
-
-        Args:
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-            quiet (bool, optional): Ignore web search-results and yield final response only. Defaults to False.
-        """
-        self.max_tokens_to_sample = max_tokens
-        self.is_conversation = is_conversation
-        self.last_response = {}
-        self.web_results: dict = {}
-        self.quiet = quiet
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-
-    def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict:
-        """Chat with AI
-
-                Args:
-                    prompt (str): Prompt to be send.
-                    stream (bool, optional): Flag for streaming response. Defaults to False.
-                    raw (bool, optional): Stream back raw response as received. Defaults to False.
-                    optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-                    conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-                Returns:
-                   dict : {}
-                ```json
-        {
-            "status": "pending",
-            "uuid": "3604dfcc-611f-4b7d-989d-edca2a7233c7",
-            "read_write_token": null,
-            "frontend_context_uuid": "f6d43119-5231-481d-b692-f52e1f52d2c6",
-            "final": false,
-            "backend_uuid": "a6d6ec9e-da69-4841-af74-0de0409267a8",
-            "media_items": [],
-            "widget_data": [],
-            "knowledge_cards": [],
-            "expect_search_results": "false",
-            "mode": "concise",
-            "search_focus": "internet",
-            "gpt4": false,
-            "display_model": "turbo",
-            "attachments": null,
-            "answer": "",
-            "web_results": [],
-            "chunks": [],
-            "extra_web_results": []
-        }
-                ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-
-        def for_stream():
-            for response in Perplexity().generate_answer(conversation_prompt):
-                yield json.dumps(response) if raw else response
-                self.last_response.update(response)
-
-            self.conversation.update_chat_history(
-                prompt,
-                self.get_message(self.last_response),
-            )
-
-        def for_non_stream():
-            for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else for_non_stream()
-
-    def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str:
-        """Generate response `str`
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str: Response generated
-        """
-
-        def for_stream():
-            for response in self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            ):
-                yield self.get_message(response)
-
-        def for_non_stream():
-            return self.get_message(
-                self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else for_non_stream()
-
-    def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        text_str: str = response.get("answer", "")
-
-        def update_web_results(web_results: list) -> None:
-            for index, results in enumerate(web_results, start=1):
-                self.web_results[str(index) + ". " + results["name"]] = dict(
-                    url=results.get("url"), snippet=results.get("snippet")
-                )
-
-        if response.get("text"):
-            # last chunk
-            target: dict[str, Any] = json.loads(response.get("text"))
-            text_str = target.get("answer")
-            web_results: list[dict] = target.get("web_results")
-            self.web_results.clear()
-            update_web_results(web_results)
-
-            return (
-                text_str
-                if self.quiet or not self.web_results
-                else text_str + "\n\n# WEB-RESULTS\n\n" + yaml.dump(self.web_results)
-            )
-
-        else:
-            if str(response.get("expect_search_results")).lower() == "true":
-                return (
-                    text_str
-                    if self.quiet
-                    else text_str
-                    + "\n\n# WEB-RESULTS\n\n"
-                    + yaml.dump(response.get("web_results"))
-                )
-            else:
-                return text_str
+import time
+import uuid
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.ui import WebDriverWait
+import click
+import requests
+from requests import get
+from uuid import uuid4
+from re import findall
+from requests.exceptions import RequestException
+from curl_cffi.requests import get, RequestsError
+import g4f
+from random import randint
+from PIL import Image
+import io
+import re
+import json
+import yaml
+from ..AIutel import Optimizers
+from ..AIutel import Conversation
+from ..AIutel import AwesomePrompts, sanitize_stream
+from ..AIbase import  Provider, AsyncProvider
+from Helpingai_T2 import Perplexity
+from webscout import exceptions
+from typing import Any, AsyncGenerator, Dict
+import logging
+import httpx
+#-----------------------------------------------REKA-----------------------------------------------
+class REKA(Provider):
+    def __init__(
+        self,
+        api_key: str,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+        model: str = "reka-core",
+        system_prompt: str = "Be Helpful and Friendly. Keep your response straightforward, short and concise",
+        use_search_engine: bool = False,
+        use_code_interpreter: bool = False,
+    ):
+        """Instantiates REKA
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+            model (str, optional): REKA model name. Defaults to "reka-core".
+            system_prompt (str, optional): System prompt for REKA. Defaults to "Be Helpful and Friendly. Keep your response straightforward, short and concise".
+            use_search_engine (bool, optional): Whether to use the search engine. Defaults to False.
+            use_code_interpreter (bool, optional): Whether to use the code interpreter. Defaults to False.
+        """
+        self.session = requests.Session()
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.api_endpoint = "https://chat.reka.ai/api/chat"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.model = model
+        self.system_prompt = system_prompt
+        self.use_search_engine = use_search_engine
+        self.use_code_interpreter = use_code_interpreter
+        self.access_token = api_key
+        self.headers = {
+            "Authorization": f"Bearer {self.access_token}",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.session.headers.update(self.headers)
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+           "text" : "How may I assist you today?"
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        self.session.headers.update(self.headers)
+        payload = {
+
+            "conversation_history": [
+                {"type": "human", "text": f"## SYSTEM PROMPT: {self.system_prompt}\n\n## QUERY: {conversation_prompt}"},
+            ],
+
+            "stream": stream,
+            "use_search_engine": self.use_search_engine,
+            "use_code_interpreter": self.use_code_interpreter,
+            "model_name": self.model,
+            # "model_name": "reka-flash",
+            # "model_name": "reka-edge",
+        }
+
+        def for_stream():
+            response = self.session.post(self.api_endpoint, json=payload, stream=True, timeout=self.timeout)
+            if not response.ok:
+                raise Exception(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+
+            for value in response.iter_lines(
+                decode_unicode=True,
+                chunk_size=self.stream_chunk_size,
+            ):
+                try:
+                    resp = json.loads(value)
+                    self.last_response.update(resp)
+                    yield value if raw else resp
+                except json.decoder.JSONDecodeError:
+                    pass
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            # let's make use of stream
+            for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        return response.get("text")
```

### Comparing `webscout-3.0/webscout/Provider/Poe.py` & `webscout-3.0b0/webscout/Provider/Poe.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,208 +1,208 @@
-from poe_api_wrapper import PoeApi
-from poe_api_wrapper.api import BOTS_LIST
-from ..AIbase import Provider
-from ..AIutel import Conversation
-from ..AIutel  import Optimizers
-from ..AIutel  import AwesomePrompts
-from pathlib import Path
-from json import loads
-from json import dumps
-from loguru import logger
-import logging
-
-logger.remove()
-
-
-class POE(Provider):
-    def __init__(
-        self,
-        cookie: str,
-        model: str = "Assistant",
-        proxy: bool = False,
-        timeout: int = 30,
-        filepath: str = None,
-        update_file: str = True,
-        intro: str = None,
-        act: str = None,
-        init: bool = True,
-    ):
-        """Initializes POE
-
-        Args:
-            cookie (str): Path to `poe.com.cookies.json` file or 'p-b' cookie-value.
-            model (str, optional): Model name. Default to Assistant.
-            proxy (bool, optional): Flag for Httpx request proxy. Defaults to False.
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            filepath (str, optional): Path to save the chat history. Defaults to None.
-            update_file (str, optional): Flag for controlling chat history updates. Defaults to True.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-            init (bool, optional): Resend the intro prompt. Defaults to True.
-        """
-        assert isinstance(
-            cookie, str
-        ), f"Cookie must be of {str} datatype only not {type(cookie)}"
-        assert (
-            model in BOTS_LIST.keys()
-        ), f"model name '{model}' is not one of {', '.join(list(BOTS_LIST.keys()))}"
-        cookie_path = Path(cookie)
-
-        if cookie_path.exists() or any(["/" in cookie, ".json" in cookie]):
-            cookie = None
-            all_cookies = loads(cookie_path.read_text())
-            for entry in all_cookies:
-                if entry["name"] == "p-b":
-                    cookie = entry["value"]
-            assert (
-                cookie
-            ), f'Required cookie value cannot be retrieved from the path  "{cookie_path.as_posix()}"'
-
-        if proxy:
-            import poe_api_wrapper.proxies as proxies
-
-            proxies.PROXY = True
-
-        self.bot = BOTS_LIST[model]
-        self.session = PoeApi(cookie)
-        self.last_response = {}
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            status=False, filepath=filepath, update_file=update_file
-        )
-        if init:
-            self.ask(self.conversation.intro)  # Init
-
-    def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict:
-        """Chat with AI
-
-            Args:
-                prompt (str): Prompt to be send.
-                stream (bool, optional): Flag for streaming response. Defaults to False.
-                raw (bool, optional): Stream back raw response as received. Defaults to False.
-                optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defeaults to None
-                conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-            Returns:
-               dict : {}
-        ```json
-        {
-            "id": "TWVzc2FnZToxMTU0MzgyNDQ1ODU=",
-            "messageId": 115438244585,
-            "creationTime": 1707777376544407,
-            "clientNonce": null,
-            "state": "complete",
-            "text": "Hello! How can I assist you today?",
-            "author": "capybara",
-            "contentType": "text_markdown",
-            "sourceType": "chat_input",
-            "attachmentTruncationState": "not_truncated",
-            "attachments": [],
-            "vote": null,
-            "suggestedReplies": [],
-            "hasCitations": false,
-            "__isNode": "Message",
-            "textLengthOnCancellation": null,
-            "chatCode": "21a2jn0yrq9phxiy478",
-            "chatId": 328236777,
-            "title": null,
-            "response": ""
-        }
-        ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-
-        def for_stream():
-            for response in self.session.send_message(self.bot, conversation_prompt):
-                if raw:
-                    yield dumps(response)
-                else:
-                    yield response
-
-                self.last_response.update(response)
-
-            self.conversation.update_chat_history(
-                prompt,
-                self.get_message(self.last_response),
-                force=True,
-            )
-
-        def for_non_stream():
-            # let's make use of stream
-            for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else for_non_stream()
-
-    def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str:
-        """Generate response `str`
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str: Response generated
-        """
-
-        def for_stream():
-            for response in self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            ):
-                yield self.get_message(response)
-
-        def for_non_stream():
-            return self.get_message(
-                self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else for_non_stream()
-
-    def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
+from poe_api_wrapper import PoeApi
+from poe_api_wrapper.api import BOTS_LIST
+from ..AIbase import Provider
+from ..AIutel import Conversation
+from ..AIutel  import Optimizers
+from ..AIutel  import AwesomePrompts
+from pathlib import Path
+from json import loads
+from json import dumps
+from loguru import logger
+import logging
+
+logger.remove()
+
+
+class POE(Provider):
+    def __init__(
+        self,
+        cookie: str,
+        model: str = "Assistant",
+        proxy: bool = False,
+        timeout: int = 30,
+        filepath: str = None,
+        update_file: str = True,
+        intro: str = None,
+        act: str = None,
+        init: bool = True,
+    ):
+        """Initializes POE
+
+        Args:
+            cookie (str): Path to `poe.com.cookies.json` file or 'p-b' cookie-value.
+            model (str, optional): Model name. Default to Assistant.
+            proxy (bool, optional): Flag for Httpx request proxy. Defaults to False.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            filepath (str, optional): Path to save the chat history. Defaults to None.
+            update_file (str, optional): Flag for controlling chat history updates. Defaults to True.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+            init (bool, optional): Resend the intro prompt. Defaults to True.
+        """
+        assert isinstance(
+            cookie, str
+        ), f"Cookie must be of {str} datatype only not {type(cookie)}"
+        assert (
+            model in BOTS_LIST.keys()
+        ), f"model name '{model}' is not one of {', '.join(list(BOTS_LIST.keys()))}"
+        cookie_path = Path(cookie)
+
+        if cookie_path.exists() or any(["/" in cookie, ".json" in cookie]):
+            cookie = None
+            all_cookies = loads(cookie_path.read_text())
+            for entry in all_cookies:
+                if entry["name"] == "p-b":
+                    cookie = entry["value"]
+            assert (
+                cookie
+            ), f'Required cookie value cannot be retrieved from the path  "{cookie_path.as_posix()}"'
+
+        if proxy:
+            import poe_api_wrapper.proxies as proxies
+
+            proxies.PROXY = True
+
+        self.bot = BOTS_LIST[model]
+        self.session = PoeApi(cookie)
+        self.last_response = {}
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            status=False, filepath=filepath, update_file=update_file
+        )
+        if init:
+            self.ask(self.conversation.intro)  # Init
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+            Args:
+                prompt (str): Prompt to be send.
+                stream (bool, optional): Flag for streaming response. Defaults to False.
+                raw (bool, optional): Stream back raw response as received. Defaults to False.
+                optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defeaults to None
+                conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+            Returns:
+               dict : {}
+        ```json
+        {
+            "id": "TWVzc2FnZToxMTU0MzgyNDQ1ODU=",
+            "messageId": 115438244585,
+            "creationTime": 1707777376544407,
+            "clientNonce": null,
+            "state": "complete",
+            "text": "Hello! How can I assist you today?",
+            "author": "capybara",
+            "contentType": "text_markdown",
+            "sourceType": "chat_input",
+            "attachmentTruncationState": "not_truncated",
+            "attachments": [],
+            "vote": null,
+            "suggestedReplies": [],
+            "hasCitations": false,
+            "__isNode": "Message",
+            "textLengthOnCancellation": null,
+            "chatCode": "21a2jn0yrq9phxiy478",
+            "chatId": 328236777,
+            "title": null,
+            "response": ""
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        def for_stream():
+            for response in self.session.send_message(self.bot, conversation_prompt):
+                if raw:
+                    yield dumps(response)
+                else:
+                    yield response
+
+                self.last_response.update(response)
+
+            self.conversation.update_chat_history(
+                prompt,
+                self.get_message(self.last_response),
+                force=True,
+            )
+
+        def for_non_stream():
+            # let's make use of stream
+            for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
         return response["text"]
```

### Comparing `webscout-3.0/webscout/Provider/ThinkAnyAI.py` & `webscout-3.0b0/webscout/Provider/ThinkAnyAI.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/Provider/Xjai.py` & `webscout-3.0b0/webscout/Provider/Xjai.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,230 +1,230 @@
-import time
-import uuid
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import WebDriverWait
-import click
-import requests
-from requests import get
-from uuid import uuid4
-from re import findall
-from requests.exceptions import RequestException
-from curl_cffi.requests import get, RequestsError
-import g4f
-from random import randint
-from PIL import Image
-import io
-import re
-import json
-import yaml
-from ..AIutel import Optimizers
-from ..AIutel import Conversation
-from ..AIutel import AwesomePrompts, sanitize_stream
-from ..AIbase import  Provider, AsyncProvider
-from webscout import exceptions
-from typing import Any, AsyncGenerator, Dict
-import logging
-import httpx
-#-----------------------------------------------xjai-------------------------------------------
-class Xjai(Provider):
-    def __init__(
-        self,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
-        temperature: float = 0.8,
-        top_p: float = 1,
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-    ):
-        """
-        Initializes the Xjai class for interacting with the Xjai AI chat API.
-
-        Args:
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            temperature (float, optional): The creativity level of the AI's response. Defaults to 0.8.
-            top_p (float, optional): The probability threshold for token selection. Defaults to 1.
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-        """
-        self.session = requests.Session()
-        self.is_conversation = is_conversation
-        self.max_tokens_to_sample = max_tokens
-        self.temperature = temperature
-        self.top_p = top_p
-        self.chat_endpoint = "https://p1api.xjai.pro/freeapi/chat-process"
-        self.stream_chunk_size = 1  # Process response line by line
-        self.timeout = timeout
-        self.last_response = {}
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session.proxies = proxies
-
-    def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> Any:
-        """
-        Sends a chat request to the Xjai AI chat API and returns the response.
-
-        Args:
-            prompt (str): The query to send to the AI.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-
-        Returns:
-            Any: The response from the AI, either as a dictionary or a generator 
-                 depending on the `stream` and `raw` parameters.
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-
-        headers = {
-            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 "
-                          "(KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36"
-        }
-
-        payload = {
-            "prompt": conversation_prompt + "\n\nReply in English Only",
-            "systemMessage": "Reply in English Only",
-            "temperature": self.temperature,
-            "top_p": self.top_p
-        }
-
-        def generate_response():
-            response = self.session.post(
-                self.chat_endpoint, headers=headers, json=payload, stream=True, timeout=self.timeout
-            )
-            output = ""
-            print_next = False
-
-            for line in response.iter_lines(decode_unicode=True, chunk_size=self.stream_chunk_size):
-                line_content = line.decode("utf-8")
-                # Filter out irrelevant content
-                if '[ChatAI](https://srv.aiflarepro.com/#/?cid=4111)' in line_content:
-                    continue
-                if '&KFw6loC9Qvy&' in line_content:
-                    parts = line_content.split('&KFw6loC9Qvy&')
-                    if print_next:
-                        output += parts[0]
-                        print_next = False
-                    else:
-                        output += parts[1]
-                        print_next = True
-                        if len(parts) > 2:
-                            print_next = False
-                elif print_next:
-                    output += line_content + '\n'
-
-            # Update chat history
-            self.conversation.update_chat_history(prompt, output)
-
-            return output
-
-        def for_stream():
-            response = generate_response()
-            for line in response.splitlines():
-                yield line if raw else dict(text=line)
-
-        def for_non_stream():
-            response = generate_response()
-            return response if raw else dict(text=response)
-
-        return for_stream() if stream else for_non_stream()
-
-    def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> Any:
-        """
-        Generates a response from the Xjai AI chat API.
-
-        Args:
-            prompt (str): The query to send to the AI.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-
-        Returns:
-            Any: The response from the AI, either as a string or a generator 
-                 depending on the `stream` parameter. 
-        """
-
-        def for_stream():
-            for response in self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            ):
-                yield self.get_message(response)
-
-        def for_non_stream():
-            return self.get_message(
-                self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else for_non_stream()
-
-    def get_message(self, response: Any) -> str:
-        """
-        Retrieves the message from the AI's response. 
-
-        Args:
-            response (Any): The response from the AI, either a dictionary 
-                            or a raw string.
-
-        Returns:
-            str: The extracted message from the AI's response. 
-        """
-        if isinstance(response, dict): 
-            return response["text"]
-        else:  # Assume raw string
-            return response
-
+import time
+import uuid
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.ui import WebDriverWait
+import click
+import requests
+from requests import get
+from uuid import uuid4
+from re import findall
+from requests.exceptions import RequestException
+from curl_cffi.requests import get, RequestsError
+import g4f
+from random import randint
+from PIL import Image
+import io
+import re
+import json
+import yaml
+from ..AIutel import Optimizers
+from ..AIutel import Conversation
+from ..AIutel import AwesomePrompts, sanitize_stream
+from ..AIbase import  Provider, AsyncProvider
+from webscout import exceptions
+from typing import Any, AsyncGenerator, Dict
+import logging
+import httpx
+#-----------------------------------------------xjai-------------------------------------------
+class Xjai(Provider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        temperature: float = 0.8,
+        top_p: float = 1,
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """
+        Initializes the Xjai class for interacting with the Xjai AI chat API.
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            temperature (float, optional): The creativity level of the AI's response. Defaults to 0.8.
+            top_p (float, optional): The probability threshold for token selection. Defaults to 1.
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.session = requests.Session()
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.temperature = temperature
+        self.top_p = top_p
+        self.chat_endpoint = "https://p1api.xjai.pro/freeapi/chat-process"
+        self.stream_chunk_size = 1  # Process response line by line
+        self.timeout = timeout
+        self.last_response = {}
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> Any:
+        """
+        Sends a chat request to the Xjai AI chat API and returns the response.
+
+        Args:
+            prompt (str): The query to send to the AI.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+
+        Returns:
+            Any: The response from the AI, either as a dictionary or a generator 
+                 depending on the `stream` and `raw` parameters.
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+
+        headers = {
+            "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 "
+                          "(KHTML, like Gecko) Chrome/124.0.0.0 Safari/537.36"
+        }
+
+        payload = {
+            "prompt": conversation_prompt + "\n\nReply in English Only",
+            "systemMessage": "Reply in English Only",
+            "temperature": self.temperature,
+            "top_p": self.top_p
+        }
+
+        def generate_response():
+            response = self.session.post(
+                self.chat_endpoint, headers=headers, json=payload, stream=True, timeout=self.timeout
+            )
+            output = ""
+            print_next = False
+
+            for line in response.iter_lines(decode_unicode=True, chunk_size=self.stream_chunk_size):
+                line_content = line.decode("utf-8")
+                # Filter out irrelevant content
+                if '[ChatAI](https://srv.aiflarepro.com/#/?cid=4111)' in line_content:
+                    continue
+                if '&KFw6loC9Qvy&' in line_content:
+                    parts = line_content.split('&KFw6loC9Qvy&')
+                    if print_next:
+                        output += parts[0]
+                        print_next = False
+                    else:
+                        output += parts[1]
+                        print_next = True
+                        if len(parts) > 2:
+                            print_next = False
+                elif print_next:
+                    output += line_content + '\n'
+
+            # Update chat history
+            self.conversation.update_chat_history(prompt, output)
+
+            return output
+
+        def for_stream():
+            response = generate_response()
+            for line in response.splitlines():
+                yield line if raw else dict(text=line)
+
+        def for_non_stream():
+            response = generate_response()
+            return response if raw else dict(text=response)
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> Any:
+        """
+        Generates a response from the Xjai AI chat API.
+
+        Args:
+            prompt (str): The query to send to the AI.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+
+        Returns:
+            Any: The response from the AI, either as a string or a generator 
+                 depending on the `stream` parameter. 
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: Any) -> str:
+        """
+        Retrieves the message from the AI's response. 
+
+        Args:
+            response (Any): The response from the AI, either a dictionary 
+                            or a raw string.
+
+        Returns:
+            str: The extracted message from the AI's response. 
+        """
+        if isinstance(response, dict): 
+            return response["text"]
+        else:  # Assume raw string
+            return response
+
```

### Comparing `webscout-3.0/webscout/Provider/Yepchat.py` & `webscout-3.0b0/webscout/Provider/Yepchat.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,478 +1,478 @@
-import time
-import uuid
-from selenium import webdriver
-from selenium.webdriver.chrome.options import Options
-from selenium.webdriver.common.by import By
-from selenium.webdriver.support import expected_conditions as EC
-from selenium.webdriver.support.ui import WebDriverWait
-import click
-import requests
-from requests import get
-from uuid import uuid4
-from re import findall
-from requests.exceptions import RequestException
-from curl_cffi.requests import get, RequestsError
-import g4f
-from random import randint
-from PIL import Image
-import io
-import re
-import json
-import yaml
-from ..AIutel import Optimizers
-from ..AIutel import Conversation
-from ..AIutel import AwesomePrompts, sanitize_stream
-from ..AIbase import  Provider, AsyncProvider
-from Helpingai_T2 import Perplexity
-from webscout import exceptions
-from typing import Any, AsyncGenerator, Dict
-import logging
-import httpx
-
-#-------------------------------------------------------yep.com--------------------------------------------------------   
-class YEPCHAT(Provider):
-    def __init__(
-        self,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
-        temperature: float = 0.6,
-        presence_penalty: int = 0,
-        frequency_penalty: int = 0,
-        top_p: float = 0.7,
-        model: str = "Mixtral-8x7B-Instruct-v0.1",
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-    ):
-        """Instantiates YEPCHAT
-
-        Args:
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.6.
-            presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
-            frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
-            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.7.
-            model (str, optional): LLM model name. Defaults to "gpt-3.5-turbo".
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-        """
-        self.session = requests.Session()
-        self.is_conversation = is_conversation
-        self.max_tokens_to_sample = max_tokens
-        self.model = model
-        self.temperature = temperature
-        self.presence_penalty = presence_penalty
-        self.frequency_penalty = frequency_penalty
-        self.top_p = top_p
-        self.chat_endpoint = "https://api.yep.com/v1/chat/completions"
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.headers = {
-            "Accept": "*/*",
-            "Accept-Encoding": "gzip, deflate",
-            "Accept-Language": "en-US,en;q=0.9",
-            "Content-Type": "application/json; charset=utf-8",
-            "Origin": "https://yep.com",
-            "Referer": "https://yep.com/",
-            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
-        }
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        self.session.headers.update(self.headers)
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session.proxies = proxies
-
-    def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict:
-        """Chat with AI
-
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict : {}
-        ```json
-        {
-            "id": "cmpl-c61c1c88de4e4ad3a79134775d17ea0c",
-            "object": "chat.completion.chunk",
-            "created": 1713876886,
-            "model": "Mixtral-8x7B-Instruct-v0.1",
-            "choices": [
-                {
-                    "index": 0,
-                    "delta": {
-                        "role": null,
-                        "content": " Sure, I can help with that. Are you looking for information on how to start coding, or do you need help with a specific coding problem? We can discuss various programming languages like Python, JavaScript, Java, C++, or others. Please provide more details so I can assist you better."
-                        },
-                    "finish_reason": null
-                }
-            ]
-        }
-        ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-        self.session.headers.update(self.headers)
-        payload = {
-            "stream": True,
-            "max_tokens": 1280,
-            "top_p": self.top_p,
-            "temperature": self.temperature,
-            "messages": [{"content": conversation_prompt, "role": "user"}],
-            "model": self.model,
-        }
-
-        def for_stream():
-            response = self.session.post(
-                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
-            )
-            if not response.ok:
-                raise exceptions.FailedToGenerateResponseError(
-                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
-                )
-
-            message_load = ""
-            for value in response.iter_lines(
-                decode_unicode=True,
-                delimiter="" if raw else "data:",
-                chunk_size=self.stream_chunk_size,
-            ):
-                try:
-                    resp = json.loads(value)
-                    incomplete_message = self.get_message(resp)
-                    if incomplete_message:
-                        message_load += incomplete_message
-                        resp["choices"][0]["delta"]["content"] = message_load
-                        self.last_response.update(resp)
-                        yield value if raw else resp
-                    elif raw:
-                        yield value
-                except json.decoder.JSONDecodeError:
-                    pass
-            self.conversation.update_chat_history(
-                prompt, self.get_message(self.last_response)
-            )
-
-        def for_non_stream():
-            for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else for_non_stream()
-
-    def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str:
-        """Generate response `str`
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str: Response generated
-        """
-
-        def for_stream():
-            for response in self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            ):
-                yield self.get_message(response)
-
-        def for_non_stream():
-            return self.get_message(
-                self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else for_non_stream()
-
-    def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        try:
-            if response["choices"][0].get("delta"):
-                return response["choices"][0]["delta"]["content"]
-            return response["choices"][0]["message"]["content"]
-        except KeyError:
-            return ""
-class AsyncYEPCHAT(AsyncProvider):
-    def __init__(
-        self,
-        is_conversation: bool = True,
-        max_tokens: int = 600,
-        temperature: float = 0.6,
-        presence_penalty: int = 0,
-        frequency_penalty: int = 0,
-        top_p: float = 0.7,
-        model: str = "Mixtral-8x7B-Instruct-v0.1",
-        timeout: int = 30,
-        intro: str = None,
-        filepath: str = None,
-        update_file: bool = True,
-        proxies: dict = {},
-        history_offset: int = 10250,
-        act: str = None,
-    ):
-        """Instantiates YEPCHAT
-
-        Args:
-            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
-            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
-            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.6.
-            presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
-            frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
-            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.7.
-            model (str, optional): LLM model name. Defaults to "gpt-3.5-turbo".
-            timeout (int, optional): Http request timeout. Defaults to 30.
-            intro (str, optional): Conversation introductory prompt. Defaults to None.
-            filepath (str, optional): Path to file containing conversation history. Defaults to None.
-            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
-            proxies (dict, optional): Http request proxies. Defaults to {}.
-            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
-            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
-        """
-        self.session = requests.Session()
-        self.is_conversation = is_conversation
-        self.max_tokens_to_sample = max_tokens
-        self.model = model
-        self.temperature = temperature
-        self.presence_penalty = presence_penalty
-        self.frequency_penalty = frequency_penalty
-        self.top_p = top_p
-        self.chat_endpoint = "https://api.yep.com/v1/chat/completions"
-        self.stream_chunk_size = 64
-        self.timeout = timeout
-        self.last_response = {}
-        self.headers = {
-            "Accept": "*/*",
-            "Accept-Encoding": "gzip, deflate",
-            "Accept-Language": "en-US,en;q=0.9",
-            "Content-Type": "application/json; charset=utf-8",
-            "Origin": "https://yep.com",
-            "Referer": "https://yep.com/",
-            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
-        }
-
-        self.__available_optimizers = (
-            method
-            for method in dir(Optimizers)
-            if callable(getattr(Optimizers, method)) and not method.startswith("__")
-        )
-        Conversation.intro = (
-            AwesomePrompts().get_act(
-                act, raise_not_found=True, default=None, case_insensitive=True
-            )
-            if act
-            else intro or Conversation.intro
-        )
-        self.conversation = Conversation(
-            is_conversation, self.max_tokens_to_sample, filepath, update_file
-        )
-        self.conversation.history_offset = history_offset
-        self.session = httpx.AsyncClient(
-            headers=self.headers,
-            proxies=proxies,
-        )
-
-    async def ask(
-        self,
-        prompt: str,
-        stream: bool = False,
-        raw: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> dict:
-        """Chat with AI asynchronously.
-
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            raw (bool, optional): Stream back raw response as received. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-           dict : {}
-        ```json
-        {
-            "id": "cmpl-c61c1c88de4e4ad3a79134775d17ea0c",
-            "object": "chat.completion.chunk",
-            "created": 1713876886,
-            "model": "Mixtral-8x7B-Instruct-v0.1",
-            "choices": [
-                {
-                    "index": 0,
-                    "delta": {
-                        "role": null,
-                        "content": " Sure, I can help with that. Are you looking for information on how to start coding, or do you need help with a specific coding problem? We can discuss various programming languages like Python, JavaScript, Java, C++, or others. Please provide more details so I can assist you better."
-                        },
-                    "finish_reason": null
-                }
-            ]
-        }
-        ```
-        """
-        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
-        if optimizer:
-            if optimizer in self.__available_optimizers:
-                conversation_prompt = getattr(Optimizers, optimizer)(
-                    conversation_prompt if conversationally else prompt
-                )
-            else:
-                raise Exception(
-                    f"Optimizer is not one of {self.__available_optimizers}"
-                )
-        payload = {
-            "stream": True,
-            "max_tokens": 1280,
-            "top_p": self.top_p,
-            "temperature": self.temperature,
-            "messages": [{"content": conversation_prompt, "role": "user"}],
-            "model": self.model,
-        }
-
-        async def for_stream():
-            async with self.session.stream(
-                "POST", self.chat_endpoint, json=payload, timeout=self.timeout
-            ) as response:
-                if not response.is_success:
-                    raise exceptions.FailedToGenerateResponseError(
-                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase}) - {response.text}"
-                    )
-
-                message_load = ""
-                async for value in response.aiter_lines():
-                    try:
-                        resp = sanitize_stream(value)
-                        incomplete_message = await self.get_message(resp)
-                        if incomplete_message:
-                            message_load += incomplete_message
-                            resp["choices"][0]["delta"]["content"] = message_load
-                            self.last_response.update(resp)
-                            yield value if raw else resp
-                        elif raw:
-                            yield value
-                    except json.decoder.JSONDecodeError:
-                        pass
-
-            self.conversation.update_chat_history(
-                prompt, await self.get_message(self.last_response)
-            )
-
-        async def for_non_stream():
-            async for _ in for_stream():
-                pass
-            return self.last_response
-
-        return for_stream() if stream else await for_non_stream()
-
-    async def chat(
-        self,
-        prompt: str,
-        stream: bool = False,
-        optimizer: str = None,
-        conversationally: bool = False,
-    ) -> str:
-        """Generate response `str` asynchronously.
-        Args:
-            prompt (str): Prompt to be send.
-            stream (bool, optional): Flag for streaming response. Defaults to False.
-            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
-            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
-        Returns:
-            str: Response generated
-        """
-
-        async def for_stream():
-            async_ask = await self.ask(
-                prompt, True, optimizer=optimizer, conversationally=conversationally
-            )
-
-            async for response in async_ask:
-                yield await self.get_message(response)
-
-        async def for_non_stream():
-            return await self.get_message(
-                await self.ask(
-                    prompt,
-                    False,
-                    optimizer=optimizer,
-                    conversationally=conversationally,
-                )
-            )
-
-        return for_stream() if stream else await for_non_stream()
-
-    async def get_message(self, response: dict) -> str:
-        """Retrieves message only from response
-
-        Args:
-            response (dict): Response generated by `self.ask`
-
-        Returns:
-            str: Message extracted
-        """
-        assert isinstance(response, dict), "Response should be of dict data-type only"
-        try:
-            if response["choices"][0].get("delta"):
-                return response["choices"][0]["delta"]["content"]
-            return response["choices"][0]["message"]["content"]
-        except KeyError:
+import time
+import uuid
+from selenium import webdriver
+from selenium.webdriver.chrome.options import Options
+from selenium.webdriver.common.by import By
+from selenium.webdriver.support import expected_conditions as EC
+from selenium.webdriver.support.ui import WebDriverWait
+import click
+import requests
+from requests import get
+from uuid import uuid4
+from re import findall
+from requests.exceptions import RequestException
+from curl_cffi.requests import get, RequestsError
+import g4f
+from random import randint
+from PIL import Image
+import io
+import re
+import json
+import yaml
+from ..AIutel import Optimizers
+from ..AIutel import Conversation
+from ..AIutel import AwesomePrompts, sanitize_stream
+from ..AIbase import  Provider, AsyncProvider
+from Helpingai_T2 import Perplexity
+from webscout import exceptions
+from typing import Any, AsyncGenerator, Dict
+import logging
+import httpx
+
+#-------------------------------------------------------yep.com--------------------------------------------------------   
+class YEPCHAT(Provider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        temperature: float = 0.6,
+        presence_penalty: int = 0,
+        frequency_penalty: int = 0,
+        top_p: float = 0.7,
+        model: str = "Mixtral-8x7B-Instruct-v0.1",
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiates YEPCHAT
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.6.
+            presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
+            frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
+            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.7.
+            model (str, optional): LLM model name. Defaults to "gpt-3.5-turbo".
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.session = requests.Session()
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.model = model
+        self.temperature = temperature
+        self.presence_penalty = presence_penalty
+        self.frequency_penalty = frequency_penalty
+        self.top_p = top_p
+        self.chat_endpoint = "https://api.yep.com/v1/chat/completions"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.headers = {
+            "Accept": "*/*",
+            "Accept-Encoding": "gzip, deflate",
+            "Accept-Language": "en-US,en;q=0.9",
+            "Content-Type": "application/json; charset=utf-8",
+            "Origin": "https://yep.com",
+            "Referer": "https://yep.com/",
+            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        self.session.headers.update(self.headers)
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session.proxies = proxies
+
+    def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+            "id": "cmpl-c61c1c88de4e4ad3a79134775d17ea0c",
+            "object": "chat.completion.chunk",
+            "created": 1713876886,
+            "model": "Mixtral-8x7B-Instruct-v0.1",
+            "choices": [
+                {
+                    "index": 0,
+                    "delta": {
+                        "role": null,
+                        "content": " Sure, I can help with that. Are you looking for information on how to start coding, or do you need help with a specific coding problem? We can discuss various programming languages like Python, JavaScript, Java, C++, or others. Please provide more details so I can assist you better."
+                        },
+                    "finish_reason": null
+                }
+            ]
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+        self.session.headers.update(self.headers)
+        payload = {
+            "stream": True,
+            "max_tokens": 1280,
+            "top_p": self.top_p,
+            "temperature": self.temperature,
+            "messages": [{"content": conversation_prompt, "role": "user"}],
+            "model": self.model,
+        }
+
+        def for_stream():
+            response = self.session.post(
+                self.chat_endpoint, json=payload, stream=True, timeout=self.timeout
+            )
+            if not response.ok:
+                raise exceptions.FailedToGenerateResponseError(
+                    f"Failed to generate response - ({response.status_code}, {response.reason}) - {response.text}"
+                )
+
+            message_load = ""
+            for value in response.iter_lines(
+                decode_unicode=True,
+                delimiter="" if raw else "data:",
+                chunk_size=self.stream_chunk_size,
+            ):
+                try:
+                    resp = json.loads(value)
+                    incomplete_message = self.get_message(resp)
+                    if incomplete_message:
+                        message_load += incomplete_message
+                        resp["choices"][0]["delta"]["content"] = message_load
+                        self.last_response.update(resp)
+                        yield value if raw else resp
+                    elif raw:
+                        yield value
+                except json.decoder.JSONDecodeError:
+                    pass
+            self.conversation.update_chat_history(
+                prompt, self.get_message(self.last_response)
+            )
+
+        def for_non_stream():
+            for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else for_non_stream()
+
+    def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str`
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        def for_stream():
+            for response in self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            ):
+                yield self.get_message(response)
+
+        def for_non_stream():
+            return self.get_message(
+                self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else for_non_stream()
+
+    def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        try:
+            if response["choices"][0].get("delta"):
+                return response["choices"][0]["delta"]["content"]
+            return response["choices"][0]["message"]["content"]
+        except KeyError:
+            return ""
+class AsyncYEPCHAT(AsyncProvider):
+    def __init__(
+        self,
+        is_conversation: bool = True,
+        max_tokens: int = 600,
+        temperature: float = 0.6,
+        presence_penalty: int = 0,
+        frequency_penalty: int = 0,
+        top_p: float = 0.7,
+        model: str = "Mixtral-8x7B-Instruct-v0.1",
+        timeout: int = 30,
+        intro: str = None,
+        filepath: str = None,
+        update_file: bool = True,
+        proxies: dict = {},
+        history_offset: int = 10250,
+        act: str = None,
+    ):
+        """Instantiates YEPCHAT
+
+        Args:
+            is_conversation (bool, optional): Flag for chatting conversationally. Defaults to True.
+            max_tokens (int, optional): Maximum number of tokens to be generated upon completion. Defaults to 600.
+            temperature (float, optional): Charge of the generated text's randomness. Defaults to 0.6.
+            presence_penalty (int, optional): Chances of topic being repeated. Defaults to 0.
+            frequency_penalty (int, optional): Chances of word being repeated. Defaults to 0.
+            top_p (float, optional): Sampling threshold during inference time. Defaults to 0.7.
+            model (str, optional): LLM model name. Defaults to "gpt-3.5-turbo".
+            timeout (int, optional): Http request timeout. Defaults to 30.
+            intro (str, optional): Conversation introductory prompt. Defaults to None.
+            filepath (str, optional): Path to file containing conversation history. Defaults to None.
+            update_file (bool, optional): Add new prompts and responses to the file. Defaults to True.
+            proxies (dict, optional): Http request proxies. Defaults to {}.
+            history_offset (int, optional): Limit conversation history to this number of last texts. Defaults to 10250.
+            act (str|int, optional): Awesome prompt key or index. (Used as intro). Defaults to None.
+        """
+        self.session = requests.Session()
+        self.is_conversation = is_conversation
+        self.max_tokens_to_sample = max_tokens
+        self.model = model
+        self.temperature = temperature
+        self.presence_penalty = presence_penalty
+        self.frequency_penalty = frequency_penalty
+        self.top_p = top_p
+        self.chat_endpoint = "https://api.yep.com/v1/chat/completions"
+        self.stream_chunk_size = 64
+        self.timeout = timeout
+        self.last_response = {}
+        self.headers = {
+            "Accept": "*/*",
+            "Accept-Encoding": "gzip, deflate",
+            "Accept-Language": "en-US,en;q=0.9",
+            "Content-Type": "application/json; charset=utf-8",
+            "Origin": "https://yep.com",
+            "Referer": "https://yep.com/",
+            "User-Agent": "Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/120.0.0.0 Safari/537.36",
+        }
+
+        self.__available_optimizers = (
+            method
+            for method in dir(Optimizers)
+            if callable(getattr(Optimizers, method)) and not method.startswith("__")
+        )
+        Conversation.intro = (
+            AwesomePrompts().get_act(
+                act, raise_not_found=True, default=None, case_insensitive=True
+            )
+            if act
+            else intro or Conversation.intro
+        )
+        self.conversation = Conversation(
+            is_conversation, self.max_tokens_to_sample, filepath, update_file
+        )
+        self.conversation.history_offset = history_offset
+        self.session = httpx.AsyncClient(
+            headers=self.headers,
+            proxies=proxies,
+        )
+
+    async def ask(
+        self,
+        prompt: str,
+        stream: bool = False,
+        raw: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> dict:
+        """Chat with AI asynchronously.
+
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            raw (bool, optional): Stream back raw response as received. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+           dict : {}
+        ```json
+        {
+            "id": "cmpl-c61c1c88de4e4ad3a79134775d17ea0c",
+            "object": "chat.completion.chunk",
+            "created": 1713876886,
+            "model": "Mixtral-8x7B-Instruct-v0.1",
+            "choices": [
+                {
+                    "index": 0,
+                    "delta": {
+                        "role": null,
+                        "content": " Sure, I can help with that. Are you looking for information on how to start coding, or do you need help with a specific coding problem? We can discuss various programming languages like Python, JavaScript, Java, C++, or others. Please provide more details so I can assist you better."
+                        },
+                    "finish_reason": null
+                }
+            ]
+        }
+        ```
+        """
+        conversation_prompt = self.conversation.gen_complete_prompt(prompt)
+        if optimizer:
+            if optimizer in self.__available_optimizers:
+                conversation_prompt = getattr(Optimizers, optimizer)(
+                    conversation_prompt if conversationally else prompt
+                )
+            else:
+                raise Exception(
+                    f"Optimizer is not one of {self.__available_optimizers}"
+                )
+        payload = {
+            "stream": True,
+            "max_tokens": 1280,
+            "top_p": self.top_p,
+            "temperature": self.temperature,
+            "messages": [{"content": conversation_prompt, "role": "user"}],
+            "model": self.model,
+        }
+
+        async def for_stream():
+            async with self.session.stream(
+                "POST", self.chat_endpoint, json=payload, timeout=self.timeout
+            ) as response:
+                if not response.is_success:
+                    raise exceptions.FailedToGenerateResponseError(
+                        f"Failed to generate response - ({response.status_code}, {response.reason_phrase}) - {response.text}"
+                    )
+
+                message_load = ""
+                async for value in response.aiter_lines():
+                    try:
+                        resp = sanitize_stream(value)
+                        incomplete_message = await self.get_message(resp)
+                        if incomplete_message:
+                            message_load += incomplete_message
+                            resp["choices"][0]["delta"]["content"] = message_load
+                            self.last_response.update(resp)
+                            yield value if raw else resp
+                        elif raw:
+                            yield value
+                    except json.decoder.JSONDecodeError:
+                        pass
+
+            self.conversation.update_chat_history(
+                prompt, await self.get_message(self.last_response)
+            )
+
+        async def for_non_stream():
+            async for _ in for_stream():
+                pass
+            return self.last_response
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def chat(
+        self,
+        prompt: str,
+        stream: bool = False,
+        optimizer: str = None,
+        conversationally: bool = False,
+    ) -> str:
+        """Generate response `str` asynchronously.
+        Args:
+            prompt (str): Prompt to be send.
+            stream (bool, optional): Flag for streaming response. Defaults to False.
+            optimizer (str, optional): Prompt optimizer name - `[code, shell_command]`. Defaults to None.
+            conversationally (bool, optional): Chat conversationally when using optimizer. Defaults to False.
+        Returns:
+            str: Response generated
+        """
+
+        async def for_stream():
+            async_ask = await self.ask(
+                prompt, True, optimizer=optimizer, conversationally=conversationally
+            )
+
+            async for response in async_ask:
+                yield await self.get_message(response)
+
+        async def for_non_stream():
+            return await self.get_message(
+                await self.ask(
+                    prompt,
+                    False,
+                    optimizer=optimizer,
+                    conversationally=conversationally,
+                )
+            )
+
+        return for_stream() if stream else await for_non_stream()
+
+    async def get_message(self, response: dict) -> str:
+        """Retrieves message only from response
+
+        Args:
+            response (dict): Response generated by `self.ask`
+
+        Returns:
+            str: Message extracted
+        """
+        assert isinstance(response, dict), "Response should be of dict data-type only"
+        try:
+            if response["choices"][0].get("delta"):
+                return response["choices"][0]["delta"]["content"]
+            return response["choices"][0]["message"]["content"]
+        except KeyError:
             return ""
```

### Comparing `webscout-3.0/webscout/Provider/__init__.py` & `webscout-3.0b0/webscout/Provider/__init__.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-# webscout/providers/__init__.py
-
-from .ThinkAnyAI import ThinkAnyAI
-from .Xjai import Xjai
-from .Llama2 import LLAMA2
-from .Llama2 import AsyncLLAMA2
-from .Cohere import Cohere
-from .Reka import REKA
-from .Groq import GROQ
-from .Groq import AsyncGROQ
-from .Openai import OPENAI
-from .Openai import AsyncOPENAI
-from .Leo import LEO
-from .Leo import AsyncLEO
-from .Koboldai import KOBOLDAI
-from .Koboldai import AsyncKOBOLDAI
-from .OpenGPT import OPENGPT 
-from .OpenGPT import AsyncOPENGPT
-from .Perplexity import PERPLEXITY
-from .Blackboxai import BLACKBOXAI 
-from .Blackboxai import AsyncBLACKBOXAI
-from .Phind import PhindSearch 
-from .Phind import AsyncPhindSearch
-from .Yepchat import YEPCHAT
-from .Yepchat import AsyncYEPCHAT
-from .Youchat import YouChat
-from .Gemini import GEMINI
-from .Berlin4h import Berlin4h
-from .ChatGPTUK import ChatGPTUK
-from .Poe import POE
-from .BasedGPT import BasedGPT
-__all__ = [
-    'ThinkAnyAI',
-    'Xjai',
-    'LLAMA2', 
-    'AsyncLLAMA2',
-    'Cohere',
-    'REKA',
-    'GROQ',
-    'AsyncGROQ',
-    'OPENAI',
-    'AsyncOPENAI',
-    'LEO',
-    'AsyncLEO',
-    'KOBOLDAI',
-    'AsyncKOBOLDAI',
-    'OPENGPT', 
-    'AsyncOPENGPT',
-    'PERPLEXITY',
-    'BLACKBOXAI', 
-    'AsyncBLACKBOXAI',
-    'PhindSearch', 
-    'AsyncPhindSearch',
-    'YEPCHAT',
-    'AsyncYEPCHAT',
-    'YouChat',
-    'GEMINI',
-    'Berlin4h',
-    'ChatGPTUK',
-    'POE',
-    'BasedGPT',
+# webscout/providers/__init__.py
+
+from .ThinkAnyAI import ThinkAnyAI
+from .Xjai import Xjai
+from .Llama2 import LLAMA2
+from .Llama2 import AsyncLLAMA2
+from .Cohere import Cohere
+from .Reka import REKA
+from .Groq import GROQ
+from .Groq import AsyncGROQ
+from .Openai import OPENAI
+from .Openai import AsyncOPENAI
+from .Leo import LEO
+from .Leo import AsyncLEO
+from .Koboldai import KOBOLDAI
+from .Koboldai import AsyncKOBOLDAI
+from .OpenGPT import OPENGPT 
+from .OpenGPT import AsyncOPENGPT
+from .Perplexity import PERPLEXITY
+from .Blackboxai import BLACKBOXAI 
+from .Blackboxai import AsyncBLACKBOXAI
+from .Phind import PhindSearch 
+from .Phind import AsyncPhindSearch
+from .Yepchat import YEPCHAT
+from .Yepchat import AsyncYEPCHAT
+from .Youchat import YouChat
+from .Gemini import GEMINI
+from .Berlin4h import Berlin4h
+from .ChatGPTUK import ChatGPTUK
+from .Poe import POE
+from .BasedGPT import BasedGPT
+__all__ = [
+    'ThinkAnyAI',
+    'Xjai',
+    'LLAMA2', 
+    'AsyncLLAMA2',
+    'Cohere',
+    'REKA',
+    'GROQ',
+    'AsyncGROQ',
+    'OPENAI',
+    'AsyncOPENAI',
+    'LEO',
+    'AsyncLEO',
+    'KOBOLDAI',
+    'AsyncKOBOLDAI',
+    'OPENGPT', 
+    'AsyncOPENGPT',
+    'PERPLEXITY',
+    'BLACKBOXAI', 
+    'AsyncBLACKBOXAI',
+    'PhindSearch', 
+    'AsyncPhindSearch',
+    'YEPCHAT',
+    'AsyncYEPCHAT',
+    'YouChat',
+    'GEMINI',
+    'Berlin4h',
+    'ChatGPTUK',
+    'POE',
+    'BasedGPT',
 ]
```

### Comparing `webscout-3.0/webscout/__init__.py` & `webscout-3.0b0/webscout/__init__.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/async_providers.py` & `webscout-3.0b0/webscout/async_providers.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/cli.py` & `webscout-3.0b0/webscout/cli.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/models.py` & `webscout-3.0b0/webscout/models.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/tempid.py` & `webscout-3.0b0/webscout/tempid.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/transcriber.py` & `webscout-3.0b0/webscout/transcriber.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/utils.py` & `webscout-3.0b0/webscout/utils.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/voice.py` & `webscout-3.0b0/webscout/voice.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/webai.py` & `webscout-3.0b0/webscout/webai.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/webscout_search.py` & `webscout-3.0b0/webscout/webscout_search.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout/webscout_search_async.py` & `webscout-3.0b0/webscout/webscout_search_async.py`

 * *Files identical despite different names*

### Comparing `webscout-3.0/webscout.egg-info/SOURCES.txt` & `webscout-3.0b0/webscout.egg-info/SOURCES.txt`

 * *Files identical despite different names*

